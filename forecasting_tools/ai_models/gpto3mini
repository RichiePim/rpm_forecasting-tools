import logging
from typing import Final

from forecasting_tools.ai_models.model_archetypes.openai_text_model import (
    OpenAiTextToTextModel,
)

logger = logging.getLogger(__name__)

class O3Mini(OpenAiTextToTextModel):
    # See OpenAI Limit on the account dashboard for the most up-to-date limits.
    MODEL_NAME: Final[str] = "o3-mini"
    REQUESTS_PER_PERIOD_LIMIT: Final[int] = 10_000      # Example value; update if needed.
    REQUEST_PERIOD_IN_SECONDS: Final[int] = 30
    TIMEOUT_TIME: Final[int] = 30                        # Slightly lower timeout for faster responses.
    TOKENS_PER_PERIOD_LIMIT: Final[int] = 1_000_000     # Example value; check current API limits.
    TOKEN_PERIOD_IN_SECONDS: Final[int] = 30
