代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2prhwypai.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jpktpenb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vqxwophq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eywgkscm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ivlmaxmy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dazbfiwa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2btsxcpqq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2chfvothb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ptxedxps.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nrlsfcxj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lytmywuw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kgdtkppa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mopapfhh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lsvyakaz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qplyqjzy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bgztfpgf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2irldmqsy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2meqofvmz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qxyfveva.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sfahcfzr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2sildhnmh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lnveyazn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mxdtmarc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wxlhzgpv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ssznyaba.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2llmundtw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vfcteaap.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cbejdmno.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tgrjefvt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cjazbqug.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ggwfgsqb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oiruynzu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mdmuyzaf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jvwjccph.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dqqgruqj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kfdkexmk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2twrafwvk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2epkosxcb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cttitdgi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzozshh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mvgtniab.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vnnukugn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dezkbjlh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xogzsumm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2udowmnrw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bjoqwcue.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bcglvimy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vcwbsxsz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qbrewwym.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vziwduqv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jpmmiqnb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pusuvulr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbvekn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2enkyosdv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2crxtneou.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fluqfdvp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dboauypi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xhbxcuyh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2unvhmgez.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nbctxeqw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hthucgzc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2aykwxjxz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2npeckdjy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2raaqoclo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gcfetsso.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mstcbylj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ynbegaam.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lyxhuefy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yejwxava.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hsaoeiat.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2euvpbxqc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2usxtzuly.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2huchxgej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mnalnszi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2iqfvmlew.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2swzytshn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vknxbqqt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ugnvodhl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uvaxbnoi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rshnidyu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lyvaxbhj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bpdwuxxv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wdxqodus.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2csesnbld.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pyznfpcq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mrweuarq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ppflqwnx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vodkgzcg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jghovsdr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gbioxdlt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xpamebww.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2viyfatzg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xletynzs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ofyfuywx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bhdvbeke.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lzrfiems.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crhzdowd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2lybsyrlh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kcsuvlff.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tzkghmkf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2iubvezuf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wyfmezol.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sewdynvy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zigdzrug.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rbhbvhsi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wvhejoal.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mcaljuul.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zdsdckuf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sjpqmqyk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kuhtqdka.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mxwnrjjf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2aleqolwc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bfrjzjur.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvrpvlew.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fjkqguzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdhpzins.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2krybrkkg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejoptnwr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pvkdfodj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2valmbkuw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rzoznmpc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xufxppaa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2twhwwwpa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tfehrgru.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tazkffuf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dshwlfad.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nahgnxyg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ofldswwy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2iqzbkmkm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2voxcoskk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcmqabui.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rezzrgln.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mmvhywto.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qnucbcad.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ciirqggu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlifvyob.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jthvpxws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ultkdbwt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mwwzsrhs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hgwdblgl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2famvvbxp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hdumdxle.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vjrkuues.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvfupxsp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2oygcokwb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yqhxxbxn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rmbinzty.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2psvgaspv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xpzcnaic.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2suiutrqg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfhqsefk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2odvgrsdf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hpqllqck.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wehisusg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ddmdrdyh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2npkxrmky.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ecfejlvv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hijhpsts.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tayvizzy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2feywglkd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xqyfusnp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yizfelxx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zqvbzuwu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rbtgemww.html

esac
来源：http://www.52xcode.cn/Article/details/gt2iffntjoo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2oekmhubn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mzeindcz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qdocwfcj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hhplmhwf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pwxjsgzp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vosyjnxa.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpcncqzf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2swekrktd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhwzow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tihrryfs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xdbccjnw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nbzfqiid.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2msouhwrg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2blmtsstw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qtpcxgyw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mkwqmzgs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nveepzbd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2spfunero.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzzkwkyw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2owcqekgt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ilurcffb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgofnbin.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fbaxnydn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fyhwhzhc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zwfuknxy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dyicgmbg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2etymfkkn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vfxkswkw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dhlscoso.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rszgdjrt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gwsrnlxa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jggzuscw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pgztmlgt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rclzfcon.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xyuktlco.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vzccbwxx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bntpcqly.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qxwlwgsp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sharwxke.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwfhlwuv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mnjhirfx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdlmtfzm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tkyjyqst.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2amrinxnx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2corlioqr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uhyzjlxh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2brdrpvxn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2stnrhpim.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2akcdfvbl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jycqmgkq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yzbnqcur.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bpczmogn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2otsyfshw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kubhbipy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hnpjnngb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gkuyslee.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hvufvmsb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zsysdrib.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2fxxkjrag.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pgowqpkl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gklclpsa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pzuhflxy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2glouhvko.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xgnhygad.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aktackxx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2otcgecaf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bzezryrc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fvfzsyan.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jdizvbhg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fnboueaa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hdsnnelu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vtguxoxb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xqpcqslr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fnuepcew.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jlaqzzmp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2iijjnlov.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gebnkwmt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eeurowuf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fbtwclih.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kibiuasj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2udnvnzms.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfbirznz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2borvkmut.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2skupxexo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mpvqcafb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gvekxfyh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jqhgwzev.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rzngcuik.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2obdohqwk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2aevifrmz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dvuzfxhd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rxjklggi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2juiklyvz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ydpvehpk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uzsxmxhi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2msinmmlb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jvdhigzj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tzvjklze.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nukiauct.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wmubvfoq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkdvwxbl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fzuxvypf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rnnfkjct.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cdcrafgf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2twhprluf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2czpdbqlo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yxtyqrmz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2skbrvsrh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rkyubpxs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2psgaefdg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wpeqxmby.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bukfqoqu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jseovjar.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rgxemooy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kpqdwkwu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vlrtdpit.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cirvihar.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cjefenbi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bdtefdaw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iyznjwix.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dmbzpnij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2misiiplw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jlkkrndw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2idcacpkl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ofqwnmmn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2myjalooc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2behucezf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cwdfeiia.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2klzxzkbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sokzlpbl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ukzcmaoy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gvigyefh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ubxdujrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjqfjmtj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jkufhpqb.html


<!-- 参考信息 -->