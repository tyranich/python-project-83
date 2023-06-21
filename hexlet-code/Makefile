dev:
	poetry run flask --app hexlet_code/page_analyzer/app run

PORT ?= 8000
start:
	poetry run gunicorn -w 5 -b 0.0.0.0:$(PORT) hexlet_code:app

build:
	poetry build

publish:
	poetry publish --dry-run --username ' ' --password ' '

package-inst:
	python3 -m pip install --force-reinstall --user dist/*.whl