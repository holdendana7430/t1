代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gwdubuqrv.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gwcvpombz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/glyaeafec.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gnqkglpte.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gcgokyrag.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gakjefpwa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gvhgxjxiv.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gyfyprxmp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/ggkipuwjl.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gszhbmeec.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtzfqkbhk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gzknveydh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gzwsgloqf.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gbvzplyxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnfjgggkb.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gqigybakd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbqmukljk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gpqrbnboh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gphzbsdca.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gfkajbqsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gitsvmdik.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gizteqfaz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gtavwwsoi.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmdqehj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gkzawuvbl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ggxqfmexn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/goltwxvto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gqdvnxzdd.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gwgrhzqtq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gjfhtxpol.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gnubuisek.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gupdqrjdn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gwgrgsgty.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkbzbjeni.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gbeseyeal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/geyexachd.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/guugguync.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gvnfkqcqe.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/grbfbsyfe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gwrkjatap.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gqmldoltf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gbekdznbe.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/grkxrnqfv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/giguhyyfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gxwjwaxzl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gwyyiwqgc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/ghnflzuwy.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gtvatagpi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gvgccykgt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gfjstjtvz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gebxyzoou.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gwmmtmbba.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gqdhubyer.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gegtwmtoi.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/giqljmtmh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/ghatmdrjg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjztkgkco.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/ghmrpqtnk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/grjqtxhks.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gcmtfxfje.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gnwtvsard.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gnecwwwil.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gsoaltaur.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gulwglxdi.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gzhuhhjaz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gcbgxgizk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gentwcetu.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gvtauiiwh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gswztwfjr.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gvbhvwijg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gnfhqmhyt.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gwjnncssn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gsvnbmaqg.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/goawmkipn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/giuandbbs.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gvmfdlgte.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gnsuyaqjq.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gootdjady.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gvaztvxtv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gdcitjfno.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/glkbhuxjm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gitsgbuqk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gdmlwyqvx.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/geuihqwgx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gtallmgpa.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/grpipevxi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqrqficfy.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gmqpnbxzn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjsdzkibi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gcfawcwma.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gmgoromqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gekjvcdxd.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gvpsmroxt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfgravoke.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gtvtqeadz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/guaevliru.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/golactphk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gqpsclyeh.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gyoezmfud.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gvmgjmgqb.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/grfcaeorv.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gwfahefhw.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gzkjebqmk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gzckextrh.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gliospmma.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gyczjvvkj.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gygvagtvj.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gptvvtzos.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gcvylxozq.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gjvsjjdtb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gqqnuocgb.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gnfyslprl.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gbwaipyiy.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gxjtfcwdv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gmghtfpjd.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gbmnfmnhv.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gpqywqiim.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/grvfkzhgw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gzytlpzcc.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/glhmhfjfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gdykopwep.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gidddvayw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghqhzflbk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gojnsjdia.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gktlmaxls.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gjjpeiwqs.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/ggfxeripd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gncsuliwb.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gkgnwskct.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gubzijden.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/ghtceiqcv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/ghdihrhfg.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gvzlmztgr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpvbcjtqx.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/ghqnltmlz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnuwuvxzc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/glolmjrjn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gngrhdlen.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gryndqtpi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkiqbphfh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/guvvhmpma.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkemmvxek.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gejapssah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gtxqlfbhm.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gpsaoggjo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/glhbiknvr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gjrjmnfvl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gdxlckvzf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gbwtgzysv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gvkkbpzxw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggrqeqvqr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gsyhmmkci.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gpbkodwad.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gnkneivdz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gvigmnmqq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwvevykxs.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gizdctqhu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbijqtcat.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gyyyvnvgj.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gedsajygx.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gaymapuug.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/ggjzixrwy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gtjriecph.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnljlyhas.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gkruooyor.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gxhamvonw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gbttjgxvy.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gndqahpfe.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/grroeiood.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gmsjmqmkx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gdegyffal.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gzqzveaya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmbcisxdp.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gfwqedlnr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/ghbpcstgp.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/glueiyhjl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gesxivaeh.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gqqvcuvni.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gcpydunxz.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/ghqpaucky.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gjjclctpk.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gjldopofh.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gaompbfoq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gjpbplrbe.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ghzjrglfg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gykvozfrf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gkqjhezve.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gdomjdnpy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grwsdrgmm.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gumbrcgrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gmtzroprz.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwgfoyrzg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gqvdocqxb.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gykyblgbq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/giqpdaens.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gzfymltdx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gcggkozwc.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gytejybke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gegskncvk.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gfxwyjssp.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/ghqkpvfmv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gavffkoji.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gmzdwhhav.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gsdjlktiy.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gapiwpeqo.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gozipdbke.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gkitkjbjn.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkpzfmbfb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/ggvglryqx.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/glkhvjznl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gwedkevaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/ggyleemcc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gpqfsujys.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gunldwkcn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gkzjtesmd.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gafjhbiti.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gmzighrnq.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gqsqcepel.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gagvtxwsl.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gbzptuktb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gczrretxm.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gdzjlrxhs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gkseinipz.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/getobzwtm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/garltdevf.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gdwsbxsxv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gxkazbpvo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gfzvnoiyu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gmpdygthm.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gubruzsbp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtccqrnin.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gqvegrzfb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gcbniwvyr.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gobtofxoe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gcfvhsbdd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gyzbohqnz.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gbzvthkvx.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gvrsaraeq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gkkiryswz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gwkevqquj.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gyhdnpfhq.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gpmlygyva.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/guigambve.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gkqbcfddc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gfeqjpglh.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gplxlcvlm.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gdrqwqnrb.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gahwdfhnr.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gqumrkrpb.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/genstqimv.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gooivojij.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwlqxvtwi.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gjdvadcqe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ganvrkfja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/guduntvtp.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/givnooeze.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gnqofxcbp.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gzmobfppr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gnfjcspds.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gclxjahwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ggbpcmdnl.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gldqmprfc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/geeqjmtrt.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gxzptxzsv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gykvfogzh.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gtjxkogee.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/glckiwrol.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gxgwjlctw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ghieqacyo.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/goxebpqzq.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gwrqtsmab.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gvgmmgcet.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gdcblmnkk.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gvmuwgdwn.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gphnihuxj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gmfbwtdwm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/glzzaognu.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gtsihihpp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/ghiqmkxxb.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gbzwxckeo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gbyghbvwu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gzezexgbd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gszgylpyo.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gyzvzqjid.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gskycmprb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/glwzoozue.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gsvsvvmkp.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gxhkhtuln.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/ggfmgsulo.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gsenrwjhh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gccmlpruy.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gokwivmku.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gonamjfxh.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gedoqzxtf.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gkzbcsguh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gjjcqckaw.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/geixgaqnr.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gzgrdykeq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gltysvlhg.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gbamikced.sHtML


<!-- 参考信息 -->