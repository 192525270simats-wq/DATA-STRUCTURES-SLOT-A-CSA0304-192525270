int a[] = {10, 20, 30, 40, 50, 60};

Node *root = NULL;

for (int i = 0; i < 6; i++)
    root = insert(root, a[i]);

printf("Before searching: ");
preorder(root);

root = search(root, 30);

printf("\nAfter searching 30: ");
preorder(root);

printf("\nRoot element: %d\n", root->key);

destroy(root);

return 0;
}
