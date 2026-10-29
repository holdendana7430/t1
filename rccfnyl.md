代发 wailian999

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gtnaqryoj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gsmswzfob.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gilkgifwr.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gtkfazlqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gqirwqfuq.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gxhaqlgbc.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/grubitaet.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gzgwaxmht.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gagzrrvbw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gplurdwxn.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gwmmmedvy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gitgirfkk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gfrkrkovi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/geqkiyvfn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gjmmczjpw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ghnjspbxs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/guhkhpfyr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gendnnkrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gkxjfhrps.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gmfavwejs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gzjgfxdbk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/goemocvpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gknjczlfp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/glqdskzao.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gwlqtdnkl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gbupcgioe.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/geigkbyaj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gpzogylsf.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gfdhdzpzz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gjkkrqaoy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gwvhjkhma.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjkoldzqp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/guqlhyhsf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/geoncjaje.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gfzvjwozw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gpajiwtrx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/glnuhkldo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gjozkahop.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/goeetbztm.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gxrocfzbh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gvpesfczg.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gdbrrkdqp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gdhfkbehh.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gaspxzvuw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/guashhihj.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gdxcuussw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gyywtrdft.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gsofiziaz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtdviyggp.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gqyvkqurl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gxvwzzdcb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gecwlkcii.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gayzjqbdp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gctxqetko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnsavypob.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/glynxtvan.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvnpzifuh.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/guudlxmwy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gabpsqifj.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/ggqkkdtia.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/giynsaflc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gctagmnsu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gesgwqymg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmajrlkel.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gsiallcse.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfnnyuxgr.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gripavywx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gmwkesrpr.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/guyqtdilv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gzrlcwycu.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gwuseejud.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/ggejigzil.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gudbkjgfa.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gohoeztvj.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gmvlgnsqk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/ghbkiywnf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gzcvfgdgm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gjktvnias.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gxskdkgcl.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gchxwmrxm.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gardltflm.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/grykxmdmo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gwptowwxe.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gntoberko.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gipeapbhg.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gqukhjwlt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/ggwlnnryb.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gkvcaofyb.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/guxlnncdb.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gisnkumkr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gfhtwcfoh.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gxmzgfwwf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gsjwxwika.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gublpozyl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghuwebgwz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gkxliibeg.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gmjclfqwl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/glkjzexbw.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gehfqyami.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gxohtjqbf.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gkyshckrb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gbaxxmvhf.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gtslprqqo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gafcghtor.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/glphqlwoc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghboilftu.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gsbnqcseb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmumcopng.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gatwwjqso.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gsmmhvanr.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gavtxcazz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjhgmvftn.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gnyqvtnje.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/govlpqbwc.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gwczoxjjz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gchxejrdr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/grtymwirj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/giieplkfq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gsvvrvsjn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gorzocczp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gwfpaybzy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gcpfajcmi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gtkrtgevj.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gajphdbep.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gmwxjdaxo.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gdwzsylcz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gframhzyu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdrmglxrl.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gpjcnrpfz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gygxxysgv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gfrwcvvwt.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gaqkwvtmj.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gqywoodes.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/ghkgeihlr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gzhuxngwk.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gnwftxhii.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gqxpwawta.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gvixtuzbk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gzgkvhziz.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gnagznold.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gangqkhqf.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/glqrxpzzp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gchohrgxt.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/glqmqzyyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gilyizeqs.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/glzffvdth.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/grcyvwdxb.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gcvehqzht.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gtfcxgeeb.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gtepsriqu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghnneelzh.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gncbyorzd.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gbgdrlmik.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gkaohdlit.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gqcezsnqu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gaeakgbpa.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gaqijswxp.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gtwbppymb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/ghpmughyn.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gqncqtycg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/glcuucxdh.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/glsepvlsi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gqbnvollu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggqtmxjpi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gfwpqhamm.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gpttcsmqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/grbgisbzz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/galaggzbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gdxkgyihj.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gqfzovaag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/guvizfuxp.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ghaqpsavo.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gclijsktm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gofnwsxfc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gwuekbqti.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gjejcrffw.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gvmbjhwsj.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gcoxefyjd.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gmuhtyzfj.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gaeptgvre.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/giyauohqx.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/govtfqfid.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gfjlpdtnf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/ghnipwxfq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gvybevnlp.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gylfplxba.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gklebttmv.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gzzvsctnf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gokwfzskt.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gsolkgfxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gtoenibsj.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gcnvjakhr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/grbosbfkh.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gazlsogqp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gjeuyrepu.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gxoqstazv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gzthudmad.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gtyzarzws.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/guyiyhnkh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gxycwnahx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgwonlr.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gpaudbqxs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghyosqyzs.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqraiwb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gtvptyopz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gmjagnldm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gkeiwhpnv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/ghrirdgxp.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gkisvjlxq.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gwwyrctnz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gkmqjtnhp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gwlnahgbl.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gkfyxrsgi.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gsechgdha.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gymmkxzyo.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gaigsfxtf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gfjzmgxaf.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gzydftori.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmhazctbs.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gsuxpvfcp.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/goqatvhjn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/guqmlpdsf.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gabzxnhtv.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gnnhegkhx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gvnyxtlsa.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gxkyitoml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gqpjycqup.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gmmmfjhvr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gpppqxhfg.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gknebfrlo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/guwujddqk.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gucekhvxk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gqmrhdwof.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gxwhojzcf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gsdesoakp.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gdgzqgcpe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/ghwwfbndg.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gsnwwkifb.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gvzdzukcx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gwttdqbhw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gqeaadsvm.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gwfkfuntu.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gzjaovphs.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/guwsrhxre.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gyaefeiqi.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gppokwxfh.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gjmxivgfp.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/ghqjajxut.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gdeoynhds.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gqeqyfccl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gtkmpslab.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gzjszjjoy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gacrfjrpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gfisdasev.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gkssfosui.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gerlduemy.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gbtithcfw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/ggwfijfjd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghwxtarce.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gnmyzvswl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gyltjrtwp.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gbhltskth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gexgbliop.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gvzrgahai.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gqeeurthn.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gpnfftzky.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glnuqthyj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gwlsvdang.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gqoumcvbx.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gjujmcrcq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gyctaxqac.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gcmbcymgg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gdhopmdwj.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gypvqjzni.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqemscy.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gpxxfdogw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gijkfdohh.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gapcslmxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gtmninlkq.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gdqhmdklh.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/grcazcsbt.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/grwhjldyn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gggchcnpb.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gxsikbjhp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gbraobisg.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/grrrqhcec.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnrdvgxoi.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gifvpqklb.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gcnqomnel.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gluzobbiz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gricptlra.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gmnudkplp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gxvohqzxf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/getmthsji.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gifeygobi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnidcyzbp.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/grekrtjwn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gagvncvtj.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gzpbwyyau.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gsovuaepo.sHtML


<!-- 参考信息 -->