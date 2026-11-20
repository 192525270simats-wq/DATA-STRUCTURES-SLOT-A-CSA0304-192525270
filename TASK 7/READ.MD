Trie *root = node();

for (int i = 0; i < 6; i++) {
    insert(root, contacts[i]);
}

const char *typed[] = {"a", "an", "anu", "b", "z", ""};

for (int i = 0; i < 6; i++) {
    printf("%s:%d ", typed[i],
           count_prefix(root, typed[i]));
}

printf("\n");

destroy(root);

return 0;
}
