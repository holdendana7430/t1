代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbkhfitu.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmkpqnddp.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwmhowl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqxishwc.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/geceflyrm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevnokfsd.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/grtntuuil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzwayybj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/givpwbugn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzvlmabjg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gibpmsjjb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbkiezcc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnoaiwxeq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/ggyqdecjx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuypfawp.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/ggwbyvdrd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjlkyzpq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/grvfhfktx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkzbtwqyu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvwhzfpu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gsvuvcpja.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxemxeszy.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvjoyjks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/govazcbis.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhlibxzd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdawrvxq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzvsowtq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzuvqgkn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdkooyep.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gerqirfkc.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gkblzuiga.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmfttjum.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkpdwiba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyedesla.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gzjpgjbxg.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvmtpkua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gayzktwes.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gplwzzmrv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtmfixcm.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gpbyyrqyk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbcunrzn.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gilqvtcic.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/glpqtiowo.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gslkfoypj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gpaoisgeu.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjjjgins.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmcnqjvz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnepgvoba.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkugeqbtz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gxpgbgztv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrouqmxc.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgmnwkud.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggnkuevl.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gpprhuikn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvdiyuan.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktljybvm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzffgrlkv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeflqplo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvkdbfq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gybsjluac.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqtigaio.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfivvdvl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyfjuqei.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gkovvgopq.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfogrdvz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoiazwpb.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/geahjwpjx.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gemwyrlxf.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gscngikyo.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnguvycwf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbracpjrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstdmazal.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/giopkipks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/giwstnclk.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyvuvcql.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmggnhpdh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvaroom.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gqmpxoolh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gydldgxof.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmnbxyfw.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goohjkqqd.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gputhktfu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqradpca.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttgdxdzm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gslnimkhl.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/goxujdjth.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnbllkjj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeoqamzr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/grplnomra.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqxmlhgia.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqayjpbrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/guzyvfkly.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfryyndqv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjclueol.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxduxystp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/ggtoytxmn.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqwmwglqs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxigioizx.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gnptdtvze.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gphuusviy.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gxkgzfbax.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxngwbhk.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdylprysw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbabjwvxw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gammcbyvu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsylnurke.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gehrushqa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gaujztyns.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/ghziaywcr.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gechunxbu.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gqsxmwijp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gakkhnrui.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gmumtlsjn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gukppucpf.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glaqnerqy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggchkknoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglkrvueq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvovxfgm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzltndsna.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrsmmrde.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gkugnradb.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gykuchyti.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ghudnkjlu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryubajse.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbeawdo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusmnqmld.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbuiwsbc.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqttbose.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/glxadnzbz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/ggfjxbatf.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gqriiwaqc.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmgyrtqhn.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqhdeme.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gublrdcyc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgplpeap.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvalzrglz.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzlrvyff.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvgcyhln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqmgzoacj.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaqlnvzbr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlksayec.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/goapnolpx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrajlgsq.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpiidmttx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grsqearxv.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/guneuhfyw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrchhmxg.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/guzthqrkz.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gxdekjqrd.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/guhqvaxtq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgehijhz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdufukal.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwiqbfty.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmzfbmku.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggqhfvydw.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoxljvof.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwylnzaz.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gztltgmvz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjbkpfqw.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghfiybxyo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gozbllszf.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gibrgqvui.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqenridiu.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuwfipoi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwetskatv.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/ghfjnykhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gaddaijtj.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gisyzfoiz.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrtsaeww.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxtwuvsc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhffhuiv.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdusjekg.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvuqkzwti.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/grabpfuos.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuguzkjs.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsznsiuk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqydvwab.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcoyffr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/guiszxwin.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/goybeaqys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwjwjnscn.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzezwxjyp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gigzinldc.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gkwnyezfw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkqmucef.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcwpqgrm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/goepwxkpk.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzjggqjnh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gminarstq.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdhijvjf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnrhdmyl.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghseygwcn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqscxtgri.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofljhalc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gksjgupyj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/ghvlzdscx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gszryywwq.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqjsrwhp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gkozwxlpx.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gneklrlnt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjctugjp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyulyveu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzxzzsqp.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjlavckgr.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgbzclyz.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gqxhhorta.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntioczer.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gnvtfkfiw.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gtayrldud.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/grxxupjpg.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobuujhl.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwbvexec.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdduphvfq.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gljugqxsr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcqocmjc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnghyayfo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwfndubs.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gordalxjp.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/glknaewft.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gogrjecnw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/grqffhwpp.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/galvfmssg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gcxrwqfqi.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpystkpk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfbygxwrb.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvcdlifr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gghnktmtv.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getumdvcd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmzpuyoo.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxjayrek.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwrsqotv.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gpxlstzaq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gaocnyhgo.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaecbfirg.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glsqgsila.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpfipmud.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpgwiqsx.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkucohnoe.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtucjesv.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gppuhcvxr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gwwiojcvp.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glhcolpbz.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/glyjmozbg.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjcegser.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuoeyayb.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/grantzcee.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjzinkgm.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnurcgsj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/goxcgcwqg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gywdbmbkp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gpisecrei.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbqdmwqeo.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gyutsbksx.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvowuayhd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gxdzyobwy.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxiqrxly.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gucvweqbg.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjmmejxm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gizoruzhk.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmplomrhq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gamgaoipf.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/grbicxcyd.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdzpyad.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgletpbq.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gpsttsafh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjowkgiw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghserjsmg.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmambrbj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfwosniy.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfarcabe.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/ghefplirq.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gywxcwiyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gigarhjfh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfuidyxj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtztkakhx.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmhpwvvdb.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gcfudbhbk.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsnixezn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtcihjleh.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtclbvefl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcscffac.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxupgsii.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gjgsyybpk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/golbqwhnf.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gobswndfb.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsbwggl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggnflvdeu.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grwkzpyat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdkemmqbg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghkqdnzm.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gpscpurfk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrbcbcji.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpxxeawr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwptcuhvf.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwrdcvgw.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuwtvmtv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpadyyouy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmwpqhac.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqkchvrbv.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxtdtax.sHtML


<!-- 参考信息 -->