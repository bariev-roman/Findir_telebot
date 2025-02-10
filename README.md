# Findir_telebot
"""Configuration settings for the Telegram bot"""
import os
from typing import List, Final

# Bot configuration
BOT_TOKEN: Final[str] = "7679353189:AAFDdDLjTPcWY5a2SFeHJ6-P5ZiDKMlBZ3A"  # Замените на ваш токен
ADMIN_IDS: Final[List[int]] = [177966998]  # Замените на ваш ID

# Google Sheets configuration
SPREADSHEET_ID: Final[str] = "1Xv8JzPP5gMhdnXcGXO8CDGBLnrQFWr89xyHOqN9kHNo/edit?gid=0#gid=0"  # ID вашей таблицы
GOOGLE_CREDS = {
    "type": "service_account",
    # Замените на ваши учетные данные Google Service Account
    "project_id": "telegram-fd-hse",
    "private_key_id": "a938f55794ebbf6ca66de7516b4366b1ee5b79ac",
    "private_key": "-----BEGIN PRIVATE KEY-----\nMIIEvQIBADANBgkqhkiG9w0BAQEFAASCBKcwggSjAgEAAoIBAQDKuMWWg/OkGwGV\nujlz/bqbejBN8m3JfAhGiC0JRPvhD+szwmyTpo4Xh+SS7Qv1Gtocfz53UEg58WoT\nG/20IJdB8DpVM3BMQTv12nttgxKG+GWKDIi7hWs7DMfET4ZZS8oJ6eol5rWdO1KK\nLb8riZcrSZyWDf52pBCrknRxVC7JilJ7Z0WCqx4/rBqIRpy8KwIA4zLIjUpD5wLR\nsWc40P3cY80a2mLqX6rfJVn590wVCaktPAoN1AQwFY+q0lYETxJY7AQBAdl2WqYk\n04BLL2BvUgHlg+TGArnCtmFnn4z27yXkD20Upz/N5uWEQAtG8m85NJbk4qtXq4/g\n+I6397yBAgMBAAECggEAA4VYhy/1Ahdm/GT+3PUd8dfaMWxhvENfeGwijhvo3QSU\nAvLgRGM66g016thbog7slVyfZt6Z1onLHBhbHG8JeX903+h0DZr/cdpw1NrXLklv\nqAlmMY2UanLjIFV6QaBHmsr5gl2Cr3+phBVd0eGCouGVKuUE06YvVO+G/rXl1yG8\nOBJRH/JmjVmpd4pOHPYpkOUJUi53kcCPDIgzpj6Pm4gXKKR4W66CmM2/jmswPIi6\nm44jNX96EDlyLVl4uWdhFn6A9oR9tsUbf2yh/s4my54P43LvSRLW0Ae0/4K9LRnP\nyvFzZ55IOi7V7Uvwrx1dU9aUNta8dZaRMzv/cVdOcQKBgQDtHwsPr/RjtrIJSHpg\nhov1pu2hqgDPw1sGhq0a7bEVyc4vY8W3hOwxQHIci3PpKm8h6Pxjz5xuafPhgluT\nHoU4+44I4FFD0mRvCOv1mO9SEcPsWFyBg9mb7PcgpfPtqDeUpYb+fKK+rfYiOGIQ\n+EQSoVXWEYzJfBiDkE2H9MnR6QKBgQDa3JrqQFmeFY0yi8+vzsboIOwg5euAW0vD\nXwiHyxr97IfanMs8w6kNe0/rPzpQJJTC6lfhQCSt2ZV5IEcQhLfNXFWc4xNhAoTb\nu8iim0bWPzmEmLhX9HvLmtEu09WjR4XUqLC5eOHY5wZiq1BKeWcF5wCIngsz0cj1\n+0V/WT+e2QKBgA2TQWbcg/lRdE/jvl3YVhryO5iNyw4Z+RQekbqA8Sp2Kz+7To57\nJaqMLfxEX5Zxv3sJg6mTMTmBB11ZwTRjAu2IOVF4xi5D1UwmDpw47TqdmcHmLSWd\nDtBGeL99wMFSaBwyfdAEAq03+GdtIvAlxn/qjKd8ybqfSCgAEvA9q3BBAoGAHJik\neSUNUJV6THduHIeE/8GFeMrx2WSUYqOhJrUIAtOL8Kl5+KeMCCHrkE5DnUMaWNlr\nwBe0cy6x1BC+mE7vARsmaIhW+N7uYxOHJI/rUoUSS9v0gjGEl1bULC0rhdkLiHy+\nEo3T3JZbBDtkE0cHigLj0/XqesvXWSSKsRgFMwkCgYEAvqOyy96E4HUKtpLpk22Z\nyqz5LphEF/tGznTw4xNZFlmINHJ+b82OlVpgxYBUBRa16PbuoURzxoXklOrxjvAO\nPOkKaGmKY7SfImm6kaEDZctTcYUjv00TfZOhQ012tAqUXR2vX4CqunIRsp00LoVW\n5jdnRqubIudN7rmnCBAf6dI=\n-----END PRIVATE KEY-----\n",
    "client_email": "telegram-fd-hse@telegram-fd-hse.iam.gserviceaccount.com",
  "client_id": "100477145381415401381",
  "auth_uri": "https://accounts.google.com/o/oauth2/auth",
  "token_uri": "https://oauth2.googleapis.com/token",
  "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
  "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/telegram-fd-hse%40telegram-fd-hse.iam.gserviceaccount.com",
  "universe_domain": "googleapis.com"
}

# States for conversation handler
MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL, NEWS_AUDIENCE, NEWS_FORMAT, \
NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE, NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT, \
FAQ_MENU, FEEDBACK_TEXT = range(14)

# Sheet names
SHEET_NEWS: Final[str] = "Новости"
SHEET_FAQ: Final[str] = "FAQ"
SHEET_FEEDBACK: Final[str] = "Обратная связь"

# Sticker pack URL
STICKER_PACK_URL: Final[str] = "https://t.me/addstickers/finance_crow"

"""Configuration settings for the Telegram bot"""
import os
from typing import List, Final

# Bot configuration
BOT_TOKEN: Final[str] = "7679353189:AAFDdDLjTPcWY5a2SFeHJ6-P5ZiDKMlBZ3A"  # Получите у @BotFather
ADMIN_IDS: Final[List[int]] = [177966998]  # Укажите ID администраторов

# Google Sheets configuration
SPREADSHEET_ID: Final[str] = "1Xv8JzPP5gMhdnXcGXO8CDGBLnrQFWr89xyHOqN9kHNo/edit?gid=0#gid=0"  # ID вашей таблицы
GOOGLE_CREDS = {
    "type": "service_account",
    # Замените на ваши учетные данные Google Service Account
    "project_id": "telegram-fd-hse",
    "private_key_id": "a938f55794ebbf6ca66de7516b4366b1ee5b79ac",
    "private_key": "-----BEGIN PRIVATE KEY-----\nMIIEvQIBADANBgkqhkiG9w0BAQEFAASCBKcwggSjAgEAAoIBAQDKuMWWg/OkGwGV\nujlz/bqbejBN8m3JfAhGiC0JRPvhD+szwmyTpo4Xh+SS7Qv1Gtocfz53UEg58WoT\nG/20IJdB8DpVM3BMQTv12nttgxKG+GWKDIi7hWs7DMfET4ZZS8oJ6eol5rWdO1KK\nLb8riZcrSZyWDf52pBCrknRxVC7JilJ7Z0WCqx4/rBqIRpy8KwIA4zLIjUpD5wLR\nsWc40P3cY80a2mLqX6rfJVn590wVCaktPAoN1AQwFY+q0lYETxJY7AQBAdl2WqYk\n04BLL2BvUgHlg+TGArnCtmFnn4z27yXkD20Upz/N5uWEQAtG8m85NJbk4qtXq4/g\n+I6397yBAgMBAAECggEAA4VYhy/1Ahdm/GT+3PUd8dfaMWxhvENfeGwijhvo3QSU\nAvLgRGM66g016thbog7slVyfZt6Z1onLHBhbHG8JeX903+h0DZr/cdpw1NrXLklv\nqAlmMY2UanLjIFV6QaBHmsr5gl2Cr3+phBVd0eGCouGVKuUE06YvVO+G/rXl1yG8\nOBJRH/JmjVmpd4pOHPYpkOUJUi53kcCPDIgzpj6Pm4gXKKR4W66CmM2/jmswPIi6\nm44jNX96EDlyLVl4uWdhFn6A9oR9tsUbf2yh/s4my54P43LvSRLW0Ae0/4K9LRnP\nyvFzZ55IOi7V7Uvwrx1dU9aUNta8dZaRMzv/cVdOcQKBgQDtHwsPr/RjtrIJSHpg\nhov1pu2hqgDPw1sGhq0a7bEVyc4vY8W3hOwxQHIci3PpKm8h6Pxjz5xuafPhgluT\nHoU4+44I4FFD0mRvCOv1mO9SEcPsWFyBg9mb7PcgpfPtqDeUpYb+fKK+rfYiOGIQ\n+EQSoVXWEYzJfBiDkE2H9MnR6QKBgQDa3JrqQFmeFY0yi8+vzsboIOwg5euAW0vD\nXwiHyxr97IfanMs8w6kNe0/rPzpQJJTC6lfhQCSt2ZV5IEcQhLfNXFWc4xNhAoTb\nu8iim0bWPzmEmLhX9HvLmtEu09WjR4XUqLC5eOHY5wZiq1BKeWcF5wCIngsz0cj1\n+0V/WT+e2QKBgA2TQWbcg/lRdE/jvl3YVhryO5iNyw4Z+RQekbqA8Sp2Kz+7To57\nJaqMLfxEX5Zxv3sJg6mTMTmBB11ZwTRjAu2IOVF4xi5D1UwmDpw47TqdmcHmLSWd\nDtBGeL99wMFSaBwyfdAEAq03+GdtIvAlxn/qjKd8ybqfSCgAEvA9q3BBAoGAHJik\neSUNUJV6THduHIeE/8GFeMrx2WSUYqOhJrUIAtOL8Kl5+KeMCCHrkE5DnUMaWNlr\nwBe0cy6x1BC+mE7vARsmaIhW+N7uYxOHJI/rUoUSS9v0gjGEl1bULC0rhdkLiHy+\nEo3T3JZbBDtkE0cHigLj0/XqesvXWSSKsRgFMwkCgYEAvqOyy96E4HUKtpLpk22Z\nyqz5LphEF/tGznTw4xNZFlmINHJ+b82OlVpgxYBUBRa16PbuoURzxoXklOrxjvAO\nPOkKaGmKY7SfImm6kaEDZctTcYUjv00TfZOhQ012tAqUXR2vX4CqunIRsp00LoVW\n5jdnRqubIudN7rmnCBAf6dI=\n-----END PRIVATE KEY-----\n",
    "client_email": "telegram-fd-hse@telegram-fd-hse.iam.gserviceaccount.com",
  "client_id": "100477145381415401381",
  "auth_uri": "https://accounts.google.com/o/oauth2/auth",
  "token_uri": "https://oauth2.googleapis.com/token",
  "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
  "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/telegram-fd-hse%40telegram-fd-hse.iam.gserviceaccount.com",
  "universe_domain": "googleapis.com"
}

# States for conversation handler
MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL, NEWS_AUDIENCE, NEWS_FORMAT, \
NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE, NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT, \
FAQ_MENU, FEEDBACK_TEXT = range(14)

# Sheet names
SHEET_NEWS: Final[str] = "Новости"
SHEET_FAQ: Final[str] = "FAQ"
SHEET_FEEDBACK: Final[str] = "Обратная связь"

# Sticker pack URL
STICKER_PACK_URL: Final[str] = "https://t.me/addstickers/finance_crow"

"""
Telegram Bot для Финансовой Дирекции НИУ ВШЭ
Часть 1: Конфигурация (config.py)
"""
import os
from typing import List, Final

# Bot configuration
BOT_TOKEN: Final[str] = "7679353189:AAFDdDLjTPcWY5a2SFeHJ6-P5ZiDKMlBZ3A"  # Получите у @BotFather
ADMIN_IDS: Final[List[int]] = [177966998]  # Укажите ID администраторов

# Google Sheets configuration
SPREADSHEET_ID: Final[str] = "1Xv8JzPP5gMhdnXcGXO8CDGBLnrQFWr89xyHOqN9kHNo/edit?gid=0#gid=0"  # ID вашей таблицы
GOOGLE_CREDS = {
    "type": "service_account",
    # Замените на ваши учетные данные Google Service Account
    "project_id": "telegram-fd-hse",
    "private_key_id": "a938f55794ebbf6ca66de7516b4366b1ee5b79ac",
    "private_key": "-----BEGIN PRIVATE KEY-----\nMIIEvQIBADANBgkqhkiG9w0BAQEFAASCBKcwggSjAgEAAoIBAQDKuMWWg/OkGwGV\nujlz/bqbejBN8m3JfAhGiC0JRPvhD+szwmyTpo4Xh+SS7Qv1Gtocfz53UEg58WoT\nG/20IJdB8DpVM3BMQTv12nttgxKG+GWKDIi7hWs7DMfET4ZZS8oJ6eol5rWdO1KK\nLb8riZcrSZyWDf52pBCrknRxVC7JilJ7Z0WCqx4/rBqIRpy8KwIA4zLIjUpD5wLR\nsWc40P3cY80a2mLqX6rfJVn590wVCaktPAoN1AQwFY+q0lYETxJY7AQBAdl2WqYk\n04BLL2BvUgHlg+TGArnCtmFnn4z27yXkD20Upz/N5uWEQAtG8m85NJbk4qtXq4/g\n+I6397yBAgMBAAECggEAA4VYhy/1Ahdm/GT+3PUd8dfaMWxhvENfeGwijhvo3QSU\nAvLgRGM66g016thbog7slVyfZt6Z1onLHBhbHG8JeX903+h0DZr/cdpw1NrXLklv\nqAlmMY2UanLjIFV6QaBHmsr5gl2Cr3+phBVd0eGCouGVKuUE06YvVO+G/rXl1yG8\nOBJRH/JmjVmpd4pOHPYpkOUJUi53kcCPDIgzpj6Pm4gXKKR4W66CmM2/jmswPIi6\nm44jNX96EDlyLVl4uWdhFn6A9oR9tsUbf2yh/s4my54P43LvSRLW0Ae0/4K9LRnP\nyvFzZ55IOi7V7Uvwrx1dU9aUNta8dZaRMzv/cVdOcQKBgQDtHwsPr/RjtrIJSHpg\nhov1pu2hqgDPw1sGhq0a7bEVyc4vY8W3hOwxQHIci3PpKm8h6Pxjz5xuafPhgluT\nHoU4+44I4FFD0mRvCOv1mO9SEcPsWFyBg9mb7PcgpfPtqDeUpYb+fKK+rfYiOGIQ\n+EQSoVXWEYzJfBiDkE2H9MnR6QKBgQDa3JrqQFmeFY0yi8+vzsboIOwg5euAW0vD\nXwiHyxr97IfanMs8w6kNe0/rPzpQJJTC6lfhQCSt2ZV5IEcQhLfNXFWc4xNhAoTb\nu8iim0bWPzmEmLhX9HvLmtEu09WjR4XUqLC5eOHY5wZiq1BKeWcF5wCIngsz0cj1\n+0V/WT+e2QKBgA2TQWbcg/lRdE/jvl3YVhryO5iNyw4Z+RQekbqA8Sp2Kz+7To57\nJaqMLfxEX5Zxv3sJg6mTMTmBB11ZwTRjAu2IOVF4xi5D1UwmDpw47TqdmcHmLSWd\nDtBGeL99wMFSaBwyfdAEAq03+GdtIvAlxn/qjKd8ybqfSCgAEvA9q3BBAoGAHJik\neSUNUJV6THduHIeE/8GFeMrx2WSUYqOhJrUIAtOL8Kl5+KeMCCHrkE5DnUMaWNlr\nwBe0cy6x1BC+mE7vARsmaIhW+N7uYxOHJI/rUoUSS9v0gjGEl1bULC0rhdkLiHy+\nEo3T3JZbBDtkE0cHigLj0/XqesvXWSSKsRgFMwkCgYEAvqOyy96E4HUKtpLpk22Z\nyqz5LphEF/tGznTw4xNZFlmINHJ+b82OlVpgxYBUBRa16PbuoURzxoXklOrxjvAO\nPOkKaGmKY7SfImm6kaEDZctTcYUjv00TfZOhQ012tAqUXR2vX4CqunIRsp00LoVW\n5jdnRqubIudN7rmnCBAf6dI=\n-----END PRIVATE KEY-----\n",
    "client_email": "telegram-fd-hse@telegram-fd-hse.iam.gserviceaccount.com",
  "client_id": "100477145381415401381",
  "auth_uri": "https://accounts.google.com/o/oauth2/auth",
  "token_uri": "https://oauth2.googleapis.com/token",
  "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
  "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/telegram-fd-hse%40telegram-fd-hse.iam.gserviceaccount.com",
  "universe_domain": "googleapis.com"
}

# States for conversation handler
(MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL, NEWS_AUDIENCE, NEWS_FORMAT,
 NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE, NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT,
 FAQ_MENU, FEEDBACK_TEXT) = range(14)

# Sheet names
SHEET_NEWS: Final[str] = "Новости"
SHEET_FAQ: Final[str] = "FAQ"
SHEET_FEEDBACK: Final[str] = "Обратная связь"

# Sticker pack URL
STICKER_PACK_URL: Final[str] = "https://t.me/addstickers/finance_crow"

"""Database interface using Google Sheets"""
import logging
from datetime import datetime
from typing import Dict, List, Optional

import gspread
from google.oauth2.service_account import Credentials

from config import GOOGLE_CREDS, SPREADSHEET_ID, SHEET_NEWS, SHEET_FAQ, SHEET_FEEDBACK

logger = logging.getLogger(__name__)

class Database:
    def __init__(self):
        """Initialize database connection"""
        logger.info("Initializing database connection...")
        self.news = []
        self.faq = []
        self.feedback = []
        self.use_sheets = False
        try:
            self.initialize_sheets()
        except Exception as e:
            logger.error(f"Failed to initialize database: {e}")
            logger.info("Using local storage as fallback")

    def initialize_sheets(self):
        """Initialize Google Sheets connection"""
        try:
            logger.info("Attempting to connect to Google Sheets...")
            scope = [
                'https://www.googleapis.com/auth/spreadsheets',
                'https://www.googleapis.com/auth/drive'
            ]

            try:
                credentials = Credentials.from_service_account_info(
                    GOOGLE_CREDS,
                    scopes=scope
                )
                logger.info("Successfully created credentials")
            except Exception as cred_error:
                logger.error(f"Failed to create credentials: {cred_error}")
                raise

            try:
                self.client = gspread.authorize(credentials)
                logger.info("Successfully authorized with gspread")
            except Exception as auth_error:
                logger.error(f"Failed to authorize with gspread: {auth_error}")
                raise

            try:
                self.spreadsheet = self.client.open_by_key(SPREADSHEET_ID)
                logger.info(f"Successfully opened spreadsheet with ID: {SPREADSHEET_ID}")
            except Exception as sheet_error:
                logger.error(f"Failed to open spreadsheet: {sheet_error}")
                raise

            # Initialize worksheets with headers
            logger.info("Initializing worksheets...")
            self._init_worksheet(SHEET_NEWS, [[
                'Подразделение', 'Email', 'Аудитория', 'Формат', 'Заголовок',
                'Текст', 'Дата', 'Медиа', 'ID автора', 'Статус'
            ]])
            self._init_worksheet(SHEET_FAQ, [['Вопрос', 'Ответ', 'Категория']])
            self._init_worksheet(SHEET_FEEDBACK, [[
                'ID пользователя', 'Текст', 'Дата', 'Статус', 'Ответ админа'
            ]])

            self.use_sheets = True
            logger.info("Successfully connected to Google Sheets")

        except Exception as e:
            logger.error(f"Failed to initialize Google Sheets: {str(e)}")
            logger.info("Falling back to local storage")
            self.use_sheets = False
            raise

    def _init_worksheet(self, name: str, headers: List[List[str]]):
        """Initialize worksheet with headers if it doesn't exist"""
        try:
            logger.info(f"Checking worksheet '{name}'...")
            try:
                worksheet = self.spreadsheet.worksheet(name)
                logger.info(f"Worksheet '{name}' already exists")
            except gspread.WorksheetNotFound:
                logger.info(f"Creating new worksheet '{name}'")
                worksheet = self.spreadsheet.add_worksheet(name, 1000, len(headers[0]))
                worksheet.update('A1', headers)
                logger.info(f"Worksheet '{name}' created successfully")
        except Exception as e:
            logger.error(f"Error initializing worksheet '{name}': {str(e)}")
            raise

    def save_news(self, news_data: Dict) -> bool:
        """Save news to database"""
        try:
            if self.use_sheets:
                logger.info(f"Attempting to save news with media: {news_data.get('media', 'No media')}")
                row = [
                    news_data.get('department', ''),
                    news_data.get('email', ''),
                    news_data.get('audience', ''),
                    news_data.get('format', ''),
                    news_data.get('title', ''),
                    news_data.get('text', ''),
                    news_data.get('date', ''),
                    news_data.get('media', ''),
                    str(news_data.get('author_id', '')),
                    'active'
                ]
                worksheet = self.spreadsheet.worksheet(SHEET_NEWS)
                worksheet.append_row(row)
                logger.info(f"Successfully saved news with media URL: {news_data.get('media', 'No media')}")
            else:
                self.news.append(news_data)
                logger.info("News saved to local storage")
            logger.info(f"Successfully saved news from user {news_data.get('author_id')}")
            return True
        except Exception as e:
            logger.error(f"Error saving news: {str(e)}")
            return False

    def get_news(self) -> List[Dict]:
        """Get all active news"""
        try:
            if self.use_sheets:
                records = self.spreadsheet.worksheet(SHEET_NEWS).get_all_records()
                return [r for r in records if r['Статус'] == 'active']
            return self.news
        except Exception as e:
            logger.error(f"Error getting news: {e}")
            return []

    def save_feedback(self, feedback_data: Dict) -> bool:
        """Save feedback to database"""
        try:
            if self.use_sheets:
                row = [
                    str(feedback_data['user_id']),
                    feedback_data['text'],
                    feedback_data['date'],
                    'new',
                    ''  # Empty admin response
                ]
                self.spreadsheet.worksheet(SHEET_FEEDBACK).append_row(row)
            else:
                self.feedback.append(feedback_data)
            logger.info(f"Successfully saved feedback from user {feedback_data['user_id']}")
            return True
        except Exception as e:
            logger.error(f"Error saving feedback: {e}")
            return False

    def get_feedback(self, status: Optional[str] = None) -> List[Dict]:
        """Get feedback entries, optionally filtered by status"""
        try:
            if self.use_sheets:
                records = self.spreadsheet.worksheet(SHEET_FEEDBACK).get_all_records()
                if status:
                    return [r for r in records if r['Статус'] == status]
                return records
            return self.feedback
        except Exception as e:
            logger.error(f"Error getting feedback: {e}")
            return []

    def update_feedback(self, row_number: int, admin_response: str) -> bool:
        """Update feedback with admin response"""
        try:
            if self.use_sheets:
                worksheet = self.spreadsheet.worksheet(SHEET_FEEDBACK)
                worksheet.update_cell(row_number, 4, 'answered')  # Update status
                worksheet.update_cell(row_number, 5, admin_response)  # Update response
                return True
            return False
        except Exception as e:
            logger.error(f"Error updating feedback: {e}")
            return False

    def get_faq(self, category: Optional[str] = None) -> List[Dict]:
        """Get FAQ entries, optionally filtered by category"""
        try:
            if self.use_sheets:
                records = self.spreadsheet.worksheet(SHEET_FAQ).get_all_records()
                if category:
                    return [r for r in records if r['Категория'] == category]
                return records
            return self.faq
        except Exception as e:
            logger.error(f"Error getting FAQ: {e}")
            return []

    def add_faq(self, question: str, answer: str, category: str = 'Общее') -> bool:
        """Add new FAQ entry"""
        try:
            if self.use_sheets:
                self.spreadsheet.worksheet(SHEET_FAQ).append_row([
                    question, answer, category
                ])
            else:
                self.faq.append({
                    'Вопрос': question,
                    'Ответ': answer,
                    'Категория': category
                })
            return True
        except Exception as e:
            logger.error(f"Error adding FAQ: {e}")
            return False

"""Handlers for the Telegram bot"""
import logging
import re
from datetime import datetime
from typing import Dict, Optional

from telegram import Update, InlineKeyboardMarkup, InlineKeyboardButton
from telegram.ext import ContextTypes

from config import (
    ADMIN_IDS, MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL, NEWS_AUDIENCE,
    NEWS_FORMAT, NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE, NEWS_MEDIA, NEWS_PREVIEW,
    NEWS_EDIT, FAQ_MENU, FEEDBACK_TEXT, STICKER_PACK_URL
)
from utils import get_user_info, is_admin, validate_text

logger = logging.getLogger(__name__)

# Keyboards
main_keyboard = [
    [InlineKeyboardButton("📰 Добавить новость", callback_data='news')],
    [InlineKeyboardButton("❓ Задать вопрос", callback_data='faq')],
    [InlineKeyboardButton("📝 Оставить отзыв", callback_data='feedback')]
]

back_keyboard = [[InlineKeyboardButton('🔙 Главное меню', callback_data='back')]]

def format_faq(entry: Dict) -> str:
    """Format FAQ entry for display"""
    return f"❓ Вопрос: {entry['Вопрос']}\n✍️ Ответ: {entry['Ответ']}\n📂 Категория: {entry['Категория']}"

async def start_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle /start command"""
    try:
        user_info = get_user_info(update)
        logger.info(f"Command /start received from {user_info}")

        welcome_text = (
            "👋 Добро пожаловать в бот Финансовой дирекции НИУ ВШЭ!\n\n"
            "Здесь вы можете:\n"
            "📰 Добавить новость - поделиться важной информацией с коллегами\n"
            "❓ Задать вопрос - получить ответ на часто задаваемые вопросы\n"
            "📝 Оставить отзыв - помочь нам стать лучше\n\n"
            "Выберите нужный раздел:"
        )

        await update.message.reply_text(
            welcome_text, 
            reply_markup=InlineKeyboardMarkup(main_keyboard)
        )
        logger.info("Start command processed successfully")
        return MAIN_MENU
    except Exception as e:
        logger.error(f"Error in start_command: {e}")
        await update.message.reply_text(
            "Произошла ошибка при запуске бота. Пожалуйста, попробуйте еще раз через минуту."
        )
        return MAIN_MENU

async def handle_menu(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle main menu interactions"""
    query = update.callback_query
    await query.answer()
    user_info = get_user_info(update)
    logger.info(f"Menu selection: {query.data} from {user_info}")

    if query.data == 'news':
        if not is_admin(update.effective_user, ADMIN_IDS):
            await query.message.reply_text(
                "⚠️ У вас нет прав для публикации новостей",
                reply_markup=InlineKeyboardMarkup(main_keyboard)
            )
            return MAIN_MENU

        rules_text = (
            "📝 Правила публикации новостей:\n\n"
            "1. Вам предстоит пройти 8 простых шагов:\n"
            "   • Указать подразделение, в котором вы работаете\n"
            "   • Указать email для связи\n"
            "   • Описать целевую аудиторию новости\n"
            "   • Выбрать формат новости\n"
            "   • Написать заголовок\n"
            "   • Добавить текст новости\n"
            "   • Указать желаемую дату публикации\n"
            "   • Добавить медиафайлы (если нужно)\n\n"
            "2. После заполнения всех полей вы сможете:\n"
            "   • Просмотреть новость перед публикацией\n"
            "   • Вернуться к любому шагу для исправления\n"
            "   • Отправить новость на публикацию\n\n"
            "Готовы начать? Нажмите «Далее» 👇"
        )

        keyboard = [
            [InlineKeyboardButton("▶️ Далее", callback_data='start_news')],
            [InlineKeyboardButton("🔙 Назад", callback_data='back')]
        ]

        await query.message.reply_text(rules_text, reply_markup=InlineKeyboardMarkup(keyboard))
        return NEWS_RULES

    elif query.data == 'faq':
        faq_entries = context.bot_data['db'].get_faq()
        if not faq_entries:
            await query.message.reply_text(
                "❓ FAQ пока пуст",
                reply_markup=InlineKeyboardMarkup(main_keyboard)
            )
        else:
            faq_text = "\n\n".join(format_faq(entry) for entry in faq_entries)
            await query.message.reply_text(
                faq_text,
                reply_markup=InlineKeyboardMarkup(main_keyboard)
            )
        return MAIN_MENU

    elif query.data == 'feedback':
        await query.message.reply_text(
            "✍️ Пожалуйста, напишите ваш отзыв или предложение:",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return FEEDBACK_TEXT

    elif query.data == 'back':
        await query.message.reply_text(
            "Выберите раздел:",
            reply_markup=InlineKeyboardMarkup(main_keyboard)
        )
        return MAIN_MENU

    return MAIN_MENU

async def handle_news_rules(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news rules confirmation"""
    query = update.callback_query
    await query.answer()

    if query.data == 'start_news':
        await query.message.reply_text(
            "📋 Укажите подразделение, в котором вы работаете.\n\n"
            "Например:\n"
            "- Финансовая дирекция\n"
            "- Бухгалтерия\n"
            "- Отдел закупок\n"
            "- или любое другое подразделение\n\n"
            "Напишите название вашего подразделения:",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_DEPARTMENT
    elif query.data == 'back':
        await query.message.reply_text(
            "Выберите раздел:",
            reply_markup=InlineKeyboardMarkup(main_keyboard)
        )
        return MAIN_MENU

    rules_text = (
        "📝 Правила публикации новостей:\n\n"
        "1. Вам предстоит пройти 8 простых шагов:\n"
        "   • Указать подразделение, в котором вы работаете\n"
        "   • Указать email для связи\n"
        "   • Описать целевую аудиторию новости\n"
        "   • Выбрать формат новости\n"
        "   • Написать заголовок\n"
        "   • Добавить текст новости\n"
        "   • Указать желаемую дату публикации\n"
        "   • Добавить медиафайлы (если нужно)\n\n"
        "2. После заполнения всех полей вы сможете:\n"
        "   • Просмотреть новость перед публикацией\n"
        "   • Вернуться к любому шагу для исправления\n"
        "   • Отправить новость на публикацию\n\n"
        "Готовы начать? Нажмите «Далее» 👇"
    )

    keyboard = [
        [InlineKeyboardButton("▶️ Далее", callback_data='start_news')],
        [InlineKeyboardButton("🔙 Назад", callback_data='back')]
    ]

    await query.message.reply_text(rules_text, reply_markup=InlineKeyboardMarkup(keyboard))
    return NEWS_RULES

async def handle_news_department(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle department input"""
    if update.callback_query:
        query = update.callback_query
        await query.answer()
        if query.data == 'back':
            await query.message.reply_text(
                "Выберите раздел:",
                reply_markup=InlineKeyboardMarkup(main_keyboard)
            )
            return MAIN_MENU

    if update.message and update.message.text:
        text = update.message.text.strip()
        logger.info(f"Received department text: {text}")

        if 'news_data' not in context.user_data:
            context.user_data['news_data'] = {}
        context.user_data['news_data']['department'] = text

        await update.message.reply_text(
            "📧 Введите ваш рабочий email для связи:\n\n"
            "Например: ivanov@hse.ru",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_EMAIL

    return NEWS_DEPARTMENT

def validate_email(email: str) -> bool:
    """Validate email format"""
    pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
    return bool(re.match(pattern, email))

async def handle_news_email(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle owner email input"""
    if not validate_email(update.message.text):
        await update.message.reply_text(
            "❌ Пожалуйста, введите корректный email",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_EMAIL

    context.user_data['news_data']['email'] = update.message.text

    await update.message.reply_text(
        "👥 Опишите целевую аудиторию новости:\n\n"
        "Например:\n"
        "- Сотрудники\n"
        "- Студенты\n"
        "- Преподаватели\n"
        "- Все категории",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_AUDIENCE

# Продолжение следует...

# Продолжение handlers.py

async def handle_news_audience(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news audience input"""
    if not update.message or not update.message.text:
        return NEWS_AUDIENCE

    context.user_data['news_data']['audience'] = update.message.text

    await update.message.reply_text(
        "📝 Выберите формат новости:\n\n"
        "Например:\n"
        "- Текст\n"
        "- Текст + фото\n"
        "- Текст + видео",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_FORMAT

async def handle_news_format(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news format input"""
    if not update.message or not update.message.text:
        return NEWS_FORMAT

    context.user_data['news_data']['format'] = update.message.text.lower()

    await update.message.reply_text(
        "📌 Введите заголовок новости:\n\n"
        "Например:\n"
        "- Важное обновление в процессе согласования договоров",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_TITLE_TEXT

async def handle_news_title_text(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news title text input"""
    if not update.message or not update.message.text:
        logger.error("No message text received in handle_news_title_text")
        return NEWS_TITLE_TEXT

    error = validate_text(update.message.text, 100)
    if error:
        await update.message.reply_text(
            f"❌ {error}",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_TITLE_TEXT

    context.user_data['news_data']['title'] = update.message.text
    logger.info(f"Title saved: {update.message.text}")

    await update.message.reply_text(
        "📄 Введите текст новости:\n\n"
        "Добавьте подробное описание новости. Можно использовать эмодзи, "
        "форматирование текста и любые другие символы.",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_CONTENT

async def handle_news_content(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news content input"""
    if not update.message or not update.message.text:
        logger.error("No message text received in handle_news_content")
        return NEWS_CONTENT

    error = validate_text(update.message.text)
    if error:
        await update.message.reply_text(
            f"❌ {error}",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_CONTENT

    context.user_data['news_data']['text'] = update.message.text
    logger.info(f"Content saved: {update.message.text[:50]}...")

    await update.message.reply_text(
        "📅 Укажите желаемую дату публикации в любом удобном формате (например, 15 февраля 2025 года):",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_DATE

async def handle_news_date(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news date input"""
    try:
        text = update.message.text.strip()
        # Try different date formats
        parsed_date = None

        # Try DD-MM-YYYY format
        try:
            parsed_date = datetime.strptime(text, '%d-%m-%Y')
        except ValueError:
            pass

        # Try DD.MM.YYYY format
        if not parsed_date:
            try:
                parsed_date = datetime.strptime(text, '%d.%m.%Y')
            except ValueError:
                pass

        # Try YYYY-MM-DD format
        if not parsed_date:
            try:
                parsed_date = datetime.strptime(text, '%Y-%m-%d')
            except ValueError:
                pass

        # Try natural language format (e.g., "15 февраля 2025 года")
        if not parsed_date:
            try:
                # Remove "года" if present
                text = text.replace(' года', '')
                # Map Russian month names to numbers
                months = {
                    'января': '01', 'февраля': '02', 'марта': '03', 'апреля': '04',
                    'мая': '05', 'июня': '06', 'июля': '07', 'августа': '08',
                    'сентября': '09', 'октября': '10', 'ноября': '11', 'декабря': '12'
                }
                for month_name, month_num in months.items():
                    if month_name in text.lower():
                        parts = text.lower().replace(month_name, month_num).split()
                        if len(parts) >= 3:
                            day = parts[0].zfill(2)
                            month = parts[1].zfill(2)
                            year = parts[2]
                            parsed_date = datetime.strptime(f"{day}-{month}-{year}", '%d-%m-%Y')
                            break
            except (ValueError, IndexError):
                pass

        if not parsed_date:
            await update.message.reply_text(
                "❌ Пожалуйста, укажите корректную дату",
                reply_markup=InlineKeyboardMarkup(back_keyboard)
            )
            return NEWS_DATE

        # Store the date in ISO format
        context.user_data['news_data']['date'] = parsed_date.strftime('%Y-%m-%d')

        # Proceed to media step
        media_text = (
            "📸✨ Вы можете загрузить фотографию для новости прямо в этот чат! "
            "Просто отправьте изображение, и оно будет добавлено.\n\n"
            "🎥 Видео и другие медиафайлы (например, документы или презентации) можно прикрепить "
            "только в формате ссылки для скачивания. Если у вас есть важные для новости материалы, "
            "просто отправьте ссылку на них, например:\n\n"
            "https://drive.google.com/file/xxx\n\n"
            "https://disk.yandex.ru/xxx\n\n"
            "Если медиафайлы или другие материалы для новости отсутствуют, напишите: \"Нет\". 😊"
        )

        await update.message.reply_text(
            media_text,
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )

        logger.info("Transitioning to NEWS_MEDIA state")
        return NEWS_MEDIA

    except Exception as e:
        logger.error(f"Error processing date: {e}")
        await update.message.reply_text(
            "❌ Произошла ошибка при обработке даты. Пожалуйста, попробуйте еще раз.",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_DATE

# Продолжение следует...

"""Handlers for FAQ and feedback"""
import logging
from datetime import datetime
from typing import Dict, Optional

from telegram import Update, InlineKeyboardMarkup, InlineKeyboardButton
from telegram.ext import ContextTypes

from config import (
    ADMIN_IDS, MAIN_MENU, FAQ_MENU, FEEDBACK_TEXT
)
from utils import get_user_info, is_admin, validate_text

logger = logging.getLogger(__name__)

async def handle_faq(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle FAQ viewing"""
    query = update.callback_query
    await query.answer()

    faq_entries = context.bot_data['db'].get_faq()
    if not faq_entries:
        await query.message.reply_text(
            "❓ FAQ пока пуст",
            reply_markup=InlineKeyboardMarkup([
                [InlineKeyboardButton("🔙 Назад", callback_data="back")]
            ])
        )
        return MAIN_MENU

    # Group FAQ by category
    faq_by_category = {}
    for entry in faq_entries:
        category = entry['Категория']
        if category not in faq_by_category:
            faq_by_category[category] = []
        faq_by_category[category].append(entry)

    # Format FAQ text by category
    faq_text = ""
    for category, entries in faq_by_category.items():
        faq_text += f"\n📂 {category}:\n\n"
        for entry in entries:
            faq_text += f"❓ {entry['Вопрос']}\n✍️ {entry['Ответ']}\n\n"

    await query.message.reply_text(
        faq_text.strip(),
        reply_markup=InlineKeyboardMarkup([
            [InlineKeyboardButton("🔙 Назад", callback_data="back")]
        ])
    )
    return MAIN_MENU

async def handle_feedback(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle feedback submission"""
    if update.callback_query:
        query = update.callback_query
        await query.answer()
        if query.data == 'back':
            await query.message.reply_text(
                "Выберите раздел:",
                reply_markup=InlineKeyboardMarkup([
                    [InlineKeyboardButton("📰 Добавить новость", callback_data='news')],
                    [InlineKeyboardButton("❓ Задать вопрос", callback_data='faq')],
                    [InlineKeyboardButton("📝 Оставить отзыв", callback_data='feedback')]
                ])
            )
            return MAIN_MENU

    if not update.message or not update.message.text:
        return FEEDBACK_TEXT

    error = validate_text(update.message.text)
    if error:
        await update.message.reply_text(
            f"❌ {error}",
            reply_markup=InlineKeyboardMarkup([
                [InlineKeyboardButton("🔙 Назад", callback_data="back")]
            ])
        )
        return FEEDBACK_TEXT

    feedback_data = {
        'text': update.message.text,
        'date': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
        'user_id': update.effective_user.id,
        'status': 'new'
    }

    if context.bot_data['db'].save_feedback(feedback_data):
        await update.message.reply_text(
            "✅ Спасибо за ваш отзыв! Мы обязательно рассмотрим его.",
            reply_markup=InlineKeyboardMarkup([
                [InlineKeyboardButton("🔙 В главное меню", callback_data="back")]
            ])
        )
    else:
        await update.message.reply_text(
            "❌ Произошла ошибка при сохранении отзыва. Пожалуйста, попробуйте позже.",
            reply_markup=InlineKeyboardMarkup([
                [InlineKeyboardButton("🔙 В главное меню", callback_data="back")]
            ])
        )

    return MAIN_MENU

"""Main bot file"""
import logging
import os
from typing import Dict, Union

from telegram.ext import (
    Application,
    CommandHandler,
    MessageHandler,
    CallbackQueryHandler,
    ConversationHandler,
    filters,
)

from config import (
    BOT_TOKEN, MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL,
    NEWS_AUDIENCE, NEWS_FORMAT, NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE,
    NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT, FAQ_MENU, FEEDBACK_TEXT
)
from database import Database
from handlers import (
    start_command, handle_menu, handle_news_rules, handle_news_department,
    handle_news_email, handle_news_audience, handle_news_format,
    handle_news_title_text, handle_news_content, handle_news_date,
    handle_news_media, show_news_preview, handle_news_confirmation,
    handle_news_edit, handle_feedback
)

# Configure logging
logging.basicConfig(
    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
    level=logging.INFO
)
logger = logging.getLogger(__name__)

def main() -> None:
    """Start the bot"""
    try:
        logger.info("Starting bot initialization...")
        
        # Create application
        application = Application.builder().token(BOT_TOKEN).build()
        logger.info("Application built successfully")

        # Initialize database
        db = Database()
        application.bot_data['db'] = db
        logger.info("Database initialized successfully")

        logger.info("Setting up conversation handler...")
        # Create conversation handler
        conv_handler = ConversationHandler(
            entry_points=[CommandHandler('start', start_command)],
            states={
                MAIN_MENU: [
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_RULES: [
                    CallbackQueryHandler(handle_news_rules)
                ],
                NEWS_DEPARTMENT: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_department),
                    CallbackQueryHandler(handle_news_rules)
                ],
                NEWS_EMAIL: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_email),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_AUDIENCE: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_audience),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_FORMAT: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_format),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_TITLE_TEXT: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_title_text),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_CONTENT: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_content),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_DATE: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_news_date),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_MEDIA: [
                    MessageHandler(
                        (filters.TEXT | filters.PHOTO) & ~filters.COMMAND,
                        handle_news_media
                    ),
                    CallbackQueryHandler(handle_menu)
                ],
                NEWS_PREVIEW: [
                    CallbackQueryHandler(handle_news_confirmation)
                ],
                NEWS_EDIT: [
                    CallbackQueryHandler(handle_news_edit)
                ],
                FAQ_MENU: [
                    CallbackQueryHandler(handle_menu)
                ],
                FEEDBACK_TEXT: [
                    MessageHandler(filters.TEXT & ~filters.COMMAND, handle_feedback),
                    CallbackQueryHandler(handle_menu)
                ],
            },
            fallbacks=[CommandHandler('start', start_command)],
            allow_reentry=True
        )
        logger.info("Conversation handler setup completed")

        # Add handlers
        application.add_handler(conv_handler)
        logger.info("Handlers added successfully")

        # Start polling
        logger.info("Starting bot polling...")
        application.run_polling(allowed_updates=Update.ALL_TYPES)
        logger.info("Bot started successfully")

    except Exception as e:
        logger.error(f"Failed to start bot: {e}")
        raise

if __name__ == '__main__':
    main()

-1+1
6
6
BOT_TOKEN: Final[str] = "YOUR_BOT_TOKEN"  # Получите у @BotFather
7
ADMIN_IDS: Final[List[int]] = [YOUR_ADMIN_ID]  # Укажите ID администраторов
7
ADMIN_IDS: Final[List[int]] = [123456789]  # Укажите ID администраторов
8
8
 
-3+3
25
25
# States for conversation handler
26
MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL, NEWS_AUDIENCE, NEWS_FORMAT, \
27
NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE, NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT, \
28
FAQ_MENU, FEEDBACK_TEXT = range(14)
26
(MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL, NEWS_AUDIENCE, NEWS_FORMAT,
27
NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE, NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT,
28
FAQ_MENU, FEEDBACK_TEXT) = range(14)
29
29
 


"""Handlers for news management"""
import logging
from datetime import datetime
from typing import Dict, Optional

from telegram import Update, InlineKeyboardMarkup, InlineKeyboardButton
from telegram.ext import ContextTypes

from config import (
    ADMIN_IDS, MAIN_MENU, NEWS_RULES, NEWS_DEPARTMENT, NEWS_EMAIL,
    NEWS_AUDIENCE, NEWS_FORMAT, NEWS_TITLE_TEXT, NEWS_CONTENT, NEWS_DATE,
    NEWS_MEDIA, NEWS_PREVIEW, NEWS_EDIT
)
from utils import get_user_info, is_admin, validate_text, format_news

logger = logging.getLogger(__name__)

# Keyboards
back_keyboard = [[InlineKeyboardButton('🔙 Главное меню', callback_data='back')]]

async def handle_news_rules(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news rules confirmation"""
    query = update.callback_query
    await query.answer()

    if query.data == 'start_news':
        await query.message.reply_text(
            "📋 Укажите подразделение, в котором вы работаете.\n\n"
            "Например:\n"
            "- Финансовая дирекция\n"
            "- Бухгалтерия\n"
            "- Отдел закупок\n"
            "- или любое другое подразделение\n\n"
            "Напишите название вашего подразделения:",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_DEPARTMENT
    elif query.data == 'back':
        await query.message.reply_text(
            "Выберите раздел:",
            reply_markup=InlineKeyboardMarkup([
                [InlineKeyboardButton("📰 Добавить новость", callback_data='news')],
                [InlineKeyboardButton("❓ Задать вопрос", callback_data='faq')],
                [InlineKeyboardButton("📝 Оставить отзыв", callback_data='feedback')]
            ])
        )
        return MAIN_MENU

    rules_text = (
        "📝 Правила публикации новостей:\n\n"
        "1. Вам предстоит пройти 8 простых шагов:\n"
        "   • Указать подразделение, в котором вы работаете\n"
        "   • Указать email для связи\n"
        "   • Описать целевую аудиторию новости\n"
        "   • Выбрать формат новости\n"
        "   • Написать заголовок\n"
        "   • Добавить текст новости\n"
        "   • Указать желаемую дату публикации\n"
        "   • Добавить медиафайлы (если нужно)\n\n"
        "2. После заполнения всех полей вы сможете:\n"
        "   • Просмотреть новость перед публикацией\n"
        "   • Вернуться к любому шагу для исправления\n"
        "   • Отправить новость на публикацию\n\n"
        "Готовы начать? Нажмите «Далее» 👇"
    )

    keyboard = [
        [InlineKeyboardButton("▶️ Далее", callback_data='start_news')],
        [InlineKeyboardButton("🔙 Назад", callback_data='back')]
    ]

    await query.message.reply_text(rules_text, reply_markup=InlineKeyboardMarkup(keyboard))
    return NEWS_RULES

async def handle_news_department(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle department input"""
    if update.callback_query:
        query = update.callback_query
        await query.answer()
        if query.data == 'back':
            await query.message.reply_text(
                "Выберите раздел:",
                reply_markup=InlineKeyboardMarkup([
                    [InlineKeyboardButton("📰 Добавить новость", callback_data='news')],
                    [InlineKeyboardButton("❓ Задать вопрос", callback_data='faq')],
                    [InlineKeyboardButton("📝 Оставить отзыв", callback_data='feedback')]
                ])
            )
            return MAIN_MENU

    if update.message and update.message.text:
        text = update.message.text.strip()
        logger.info(f"Received department text: {text}")

        if 'news_data' not in context.user_data:
            context.user_data['news_data'] = {}
        context.user_data['news_data']['department'] = text

        await update.message.reply_text(
            "📧 Введите ваш рабочий email для связи:\n\n"
            "Например: ivanov@hse.ru",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_EMAIL

    return NEWS_DEPARTMENT

async def handle_news_email(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle email input"""
    if not update.message or not update.message.text:
        return NEWS_EMAIL

    email = update.message.text.strip()
    if not validate_email(email):
        await update.message.reply_text(
            "❌ Пожалуйста, введите корректный email",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_EMAIL

    context.user_data['news_data']['email'] = email

    await update.message.reply_text(
        "👥 Опишите целевую аудиторию новости:\n\n"
        "Например:\n"
        "- Сотрудники\n"
        "- Студенты\n"
        "- Преподаватели\n"
        "- Все категории",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_AUDIENCE

async def handle_news_audience(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news audience input"""
    if not update.message or not update.message.text:
        return NEWS_AUDIENCE

    context.user_data['news_data']['audience'] = update.message.text

    await update.message.reply_text(
        "📝 Выберите формат новости:\n\n"
        "Например:\n"
        "- Текст\n"
        "- Текст + фото\n"
        "- Текст + видео",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_FORMAT

async def handle_news_format(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news format input"""
    if not update.message or not update.message.text:
        return NEWS_FORMAT

    context.user_data['news_data']['format'] = update.message.text.lower()

    await update.message.reply_text(
        "📌 Введите заголовок новости:\n\n"
        "Например:\n"
        "- Важное обновление в процессе согласования договоров",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_TITLE_TEXT

async def handle_news_title_text(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news title text input"""
    if not update.message or not update.message.text:
        logger.error("No message text received in handle_news_title_text")
        return NEWS_TITLE_TEXT

    error = validate_text(update.message.text, 100)
    if error:
        await update.message.reply_text(
            f"❌ {error}",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_TITLE_TEXT

    context.user_data['news_data']['title'] = update.message.text
    logger.info(f"Title saved: {update.message.text}")

    await update.message.reply_text(
        "📄 Введите текст новости:\n\n"
        "Добавьте подробное описание новости. Можно использовать эмодзи, "
        "форматирование текста и любые другие символы.",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_CONTENT

async def handle_news_content(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news content input"""
    if not update.message or not update.message.text:
        logger.error("No message text received in handle_news_content")
        return NEWS_CONTENT

    error = validate_text(update.message.text)
    if error:
        await update.message.reply_text(
            f"❌ {error}",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_CONTENT

    context.user_data['news_data']['text'] = update.message.text
    logger.info(f"Content saved: {update.message.text[:50]}...")

    await update.message.reply_text(
        "📅 Укажите желаемую дату публикации в любом удобном формате (например, 15 февраля 2025 года):",
        reply_markup=InlineKeyboardMarkup(back_keyboard)
    )
    return NEWS_DATE

async def handle_news_date(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news date input"""
    try:
        text = update.message.text.strip()
        # Try different date formats
        parsed_date = None

        # Try DD-MM-YYYY format
        try:
            parsed_date = datetime.strptime(text, '%d-%m-%Y')
        except ValueError:
            pass

        # Try DD.MM.YYYY format
        if not parsed_date:
            try:
                parsed_date = datetime.strptime(text, '%d.%m.%Y')
            except ValueError:
                pass

        # Try YYYY-MM-DD format
        if not parsed_date:
            try:
                parsed_date = datetime.strptime(text, '%Y-%m-%d')
            except ValueError:
                pass

        # Try natural language format (e.g., "15 февраля 2025 года")
        if not parsed_date:
            try:
                # Remove "года" if present
                text = text.replace(' года', '')
                # Map Russian month names to numbers
                months = {
                    'января': '01', 'февраля': '02', 'марта': '03', 'апреля': '04',
                    'мая': '05', 'июня': '06', 'июля': '07', 'августа': '08',
                    'сентября': '09', 'октября': '10', 'ноября': '11', 'декабря': '12'
                }
                for month_name, month_num in months.items():
                    if month_name in text.lower():
                        parts = text.lower().replace(month_name, month_num).split()
                        if len(parts) >= 3:
                            day = parts[0].zfill(2)
                            month = parts[1].zfill(2)
                            year = parts[2]
                            parsed_date = datetime.strptime(f"{day}-{month}-{year}", '%d-%m-%Y')
                            break
            except (ValueError, IndexError):
                pass

        if not parsed_date:
            await update.message.reply_text(
                "❌ Пожалуйста, укажите корректную дату",
                reply_markup=InlineKeyboardMarkup(back_keyboard)
            )
            return NEWS_DATE

        # Store the date in ISO format
        context.user_data['news_data']['date'] = parsed_date.strftime('%Y-%m-%d')

        # Proceed to media step
        media_text = (
            "📸✨ Вы можете загрузить фотографию для новости прямо в этот чат! "
            "Просто отправьте изображение, и оно будет добавлено.\n\n"
            "🎥 Видео и другие медиафайлы (например, документы или презентации) можно прикрепить "
            "только в формате ссылки для скачивания. Если у вас есть важные для новости материалы, "
            "просто отправьте ссылку на них, например:\n\n"
            "https://drive.google.com/file/xxx\n\n"
            "https://disk.yandex.ru/xxx\n\n"
            "Если медиафайлы или другие материалы для новости отсутствуют, напишите: \"Нет\". 😊"
        )

        await update.message.reply_text(
            media_text,
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )

        logger.info("Transitioning to NEWS_MEDIA state")
        return NEWS_MEDIA

    except Exception as e:
        logger.error(f"Error processing date: {e}")
        await update.message.reply_text(
            "❌ Произошла ошибка при обработке даты. Пожалуйста, попробуйте еще раз.",
            reply_markup=InlineKeyboardMarkup(back_keyboard)
        )
        return NEWS_DATE

+1"""Handlers for media and news preview"""
import logging
from typing import Optional, Dict

from telegram import Update, InlineKeyboardMarkup, InlineKeyboardButton
from telegram.ext import ContextTypes

from config import (
    MAIN_MENU, NEWS_PREVIEW, NEWS_MEDIA, NEWS_EDIT
)
from utils import format_news, get_message_text

logger = logging.getLogger(__name__)

async def handle_news_media(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news media input"""
    try:
        if update.message.photo:
            # Get the largest photo size
            photo = update.message.photo[-1]
            file_id = photo.file_id
            context.user_data['news_data']['media'] = file_id
            logger.info(f"Saved photo with file_id: {file_id}")
        else:
            text = get_message_text(update.message)
            if text.lower() != "нет":
                context.user_data['news_data']['media'] = text
            else:
                context.user_data['news_data']['media'] = ""
            logger.info(f"Saved media text: {text}")

        # Show preview
        news_data = context.user_data['news_data']
        preview_text = (
            "📋 Предпросмотр новости:\n\n"
            f"{format_news(news_data)}\n\n"
            "Всё верно? Выберите действие:"
        )

        keyboard = [
            [InlineKeyboardButton("✅ Опубликовать", callback_data="publish")],
            [
                InlineKeyboardButton("📝 Изменить", callback_data="edit"),
                InlineKeyboardButton("❌ Отменить", callback_data="cancel")
            ]
        ]

        if update.message.photo:
            await update.message.reply_photo(
                photo=file_id,
                caption=preview_text,
                reply_markup=InlineKeyboardMarkup(keyboard)
            )
        else:
            await update.message.reply_text(
                preview_text,
                reply_markup=InlineKeyboardMarkup(keyboard)
            )

        return NEWS_PREVIEW

    except Exception as e:
        logger.error(f"Error handling media: {e}")
        await update.message.reply_text(
            "❌ Произошла ошибка при обработке медиафайла. Пожалуйста, попробуйте еще раз.",
            reply_markup=InlineKeyboardMarkup([[
                InlineKeyboardButton("🔙 Главное меню", callback_data="back")
            ]])
        )
        return NEWS_MEDIA

async def handle_news_confirmation(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
    """Handle news preview confirmation"""
    query = update.callback_query
    await query.answer()

    if query.data == "publish":
        news_data = context.user_data['news_data']
        news_data['author_id'] = update.effective_user.id

        if context.bot_data['db'].save_news(news_data):
            await query.message.reply_text(
                "✅ Новость успешно опубликована!",
                reply_markup=InlineKeyboardMarkup([[
                    InlineKeyboardButton("🔙 Главное меню", callback_data="back")
                ]])
            )
            logger.info(f"News published by user {update.effective_user.id}")
        else:
            await query.message.reply_text(
                "❌ Произошла ошибка при публикации новости. Пожалуйста, попробуйте позже.",
                reply_markup=InlineKeyboardMarkup([[
                    InlineKeyboardButton("🔙 Главное меню", callback_data="back")
                ]])
            )
            logger.error(f"Failed to publish news for user {update.effective_user.id}")
        return MAIN_MENU

    elif query.data == "edit":
        keyboard = [
            [InlineKeyboardButton("👤 Подразделение", callback_data="edit_department")],
            [InlineKeyboardButton("📧 Email", callback_data="edit_email")],
            [InlineKeyboardButton("👥 Аудитория", callback_data="edit_audience")],
            [InlineKeyboardButton("📝 Формат", callback_data="edit_format")],
            [InlineKeyboardButton("📌 Заголовок", callback_data="edit_title")],
            [InlineKeyboardButton("📄 Текст", callback_data="edit_text")],
            [InlineKeyboardButton("📅 Дата", callback_data="edit_date")],
            [InlineKeyboardButton("📸 Медиа", callback_data="edit_media")],
            [InlineKeyboardButton("🔙 Назад", callback_data="back_to_preview")]
        ]
        await query.message.reply_text(
            "Выберите, что хотите изменить:",
            reply_markup=InlineKeyboardMarkup(keyboard)
        )
        return NEWS_EDIT

    elif query.data == "cancel":
        await query.message.reply_text(
            "❌ Публикация новости отменена",
            reply_markup=InlineKeyboardMarkup([[
                InlineKeyboardButton("🔙 Главное меню", callback_data="back")
            ]])
        )
        if 'news_data' in context.user_data:
            del context.user_data['news_data']
        return MAIN_MENU

    return NEWS_PREVIEW


1
1
"""Utility functions for the bot"""
2
import re
2
3
from typing import Dict, Optional, Union
-0+5
34
35
 
36
def validate_email(email: str) -> bool:
37
   """Validate email format"""
38
   pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
39
   return bool(re.match(pattern, email))
40
 
35
41
def get_message_text(message: Message) -> str:

