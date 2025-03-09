# Contributing to Solana DCA Monitor

We love your input! We want to make contributing to Solana DCA Monitor as easy and transparent as possible, whether it's:

- Reporting a bug
- Discussing the current state of the code
- Submitting a fix
- Proposing new features
- Becoming a maintainer

## Development Process

We use GitHub to host code, to track issues and feature requests, as well as accept pull requests.

### Pull Requests

1. Fork the repo and create your branch from `main`.
2. If you've added code that should be tested, add tests.
3. If you've changed APIs, update the documentation.
4. Ensure the test suite passes.
5. Make sure your code lints.
6. Issue that pull request!

### Technical Requirements

- **Backend**: Python 3.12+, FastAPI framework
- **Frontend**: Next.js 14+, Tailwind CSS, shadcn/ui components
- **Infrastructure**: Azure-based deployment

## Code Standards

### Python

- Use [Black](https://github.com/psf/black) for code formatting
- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide
- Type hints are required for all function parameters and return values
- Tests are required for all new features

```python
# Good example
def calculate_transaction_fee(tx_size: int, priority: str = "normal") -> float:
    """
    Calculate the transaction fee based on size and priority.
    
    Args:
        tx_size: Size of transaction in bytes
        priority: Transaction priority (normal, high, max)
        
    Returns:
        Fee in SOL
    """
    # Implementation
    pass
```

### TypeScript/JavaScript

- Use ESLint with our provided config
- Use Prettier for formatting
- Follow functional component patterns for React
- Use React hooks effectively

```tsx
// Good example
const TransactionItem: React.FC<TransactionProps> = ({ transaction }) => {
  const { value, timestamp, type } = transaction;
  
  return (
    <div className="p-4 rounded-lg border border-gray-200">
      <h3 className="font-semibold">{type}</h3>
      <p>{formatSOL(value)} SOL</p>
      <p className="text-gray-500">{formatDate(timestamp)}</p>
    </div>
  );
};
```

## Commit Messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Limit the first line to 72 characters or less
- Reference issues and pull requests liberally after the first line

## License

By contributing, you agree that your contributions will be licensed under the project's MIT License.