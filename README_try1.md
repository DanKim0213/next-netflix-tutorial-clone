# README - What I learned

## SWR - Stale while revalidate

```js
useSWR(key, fetcher, {
  revalidateIfStale: false,
  revalidateOnFocus: false,
  revalidateOnReconnect: false,
});

// equivalent to
useSWRImmutable(key, fetcher);
```

## HTTP status code

400 Bad Request

405 Method Not Allowed

500 Internal Server Error

422 Unprocessable Content (WebDAV)

## JSX element vs React.FC

```ts
interface AccountMenuProps {
  visible?: boolean;
}

// const AccountMenu: FC<AccountMenuProps>
const AccountMenu: React.FC<AccountMenuProps> = ({ visible }) => {
  return <div></div>;
};

// function AccountMenu2({ visible }: AccountMenuProps): JSX.Element
function AccountMenu2({ visible }: AccountMenuProps) {
  return <div></div>;
}
```

## Font

Font size is dependant on personal taste while font weight is used to highlight content by giving contrast.
