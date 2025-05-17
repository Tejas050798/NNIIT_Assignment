# Smart Flashcard Backend

This is a backend API for a smart flashcard system. Users can add flashcards with questions and answers, and the backend automatically detects the subject based on keywords.

## Features

- Add flashcards (subject is inferred)
- Retrieve flashcards from mixed subjects
- Organized by student

## How It Works

- Subject detection uses keyword matching
- Flashcards are stored in memory (no DB used)

## Endpoints

### POST `/flashcard`

Add a new flashcard.

```json
{
  "student_id": "stu001",
  "question": "What is Newton's Second Law?",
  "answer": "Force equals mass times acceleration"
}
