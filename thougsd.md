代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gchojoyng.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmppuqo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsjbdnia.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/guerxrixd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwtazvyc.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzatpjpnk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnuymefnu.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcscmrvws.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/griseseza.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gbpgloxoi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guiickdlk.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmttyweat.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowtjybef.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gtmlvdklf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gkzcxtlhq.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxkxgafl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsvxmxzz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtegwzav.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqahgtxj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gkjspjinn.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/grvqaqtta.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gryovnmnw.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gkxbtbkdm.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gkswjjfyx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gkjegqqgs.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrrsraqp.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkkvccr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwftsprgz.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkbvacfv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwwbrhzc.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesrldtig.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphbmnrix.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gmizewbch.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucuqwomm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiyasord.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/glremzcyl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gowfzfihe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqbyvqcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhpelutt.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlkgeqmh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/geqvipfzg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/grjntpnim.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmowhcedd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjmlbjzga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gbyvjtcky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqkxejvaz.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/geqplaibd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govztfcxg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsiajfsl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gahktxkzh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpbqnqkl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gaaiiqtlq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkfmwjoao.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gmdvglhyq.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwknbgjq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnvrjtrf.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyafuhno.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gprrapjof.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/grhgjxosh.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwpcupfm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxyagkho.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjuwngam.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gwmphwwhf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyzmlauj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoogfmwf.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gcxzbrbwy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmbsrerg.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gquyhrtgy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gcakaphnj.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gmhevgosh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjxlisbz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gdvtvwipp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakasvnru.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gkbdqlomv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvahusbfl.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/galuufdbb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcmdwxqq.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkskmevi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbpoasrs.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmfxrgx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gawmrqork.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gpzyohtnx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gozsxhavj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gvlmvlsyt.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gvvpksljl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezupwtlx.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtbuihtx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/giujaerbq.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggpzkhnwz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvnzoebx.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzhrhjgq.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gufahhasu.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbmqnfwo.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyayvrqne.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhvzcsh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnbfequy.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztpyohod.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gflcoywtd.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gakhlyogc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqjpuocg.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/glwywnyqf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqsdtaxh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznnqonzx.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gtluzrrdj.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwpwoedxk.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gsuuuzjhc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxfvqzbs.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfctwjto.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfgzfvhda.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gmmbziofb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gycdbbnor.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsltloxu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzqpnkko.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwoozkgu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/grapgrfka.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gbeewkyvm.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtlztrcp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gjbowblng.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gisktarrb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gdcliyvol.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gcepbhjzb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxyicgy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzqjvtzq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gshefxune.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrnthgzi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gccopajnp.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcfckfjt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhryaij.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsooykkz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwojffdxu.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gawkuelnr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giotqqwps.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gluohowqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcswtihgv.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/givrxvyoj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnfhwwle.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gtalxouaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gstducuru.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunhxpjpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmthfhnqf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gzmfduhxs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gxouxgoyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwwalukih.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaeqcbdz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjazlnghk.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gvkohuesv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggevdgafp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcbuifmie.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/glahhlusc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkupalapj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvoellzu.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gvgtslelm.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlkkppls.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gxkzahquw.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gyirmipyk.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/goktgitsh.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guomzotdt.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbrvbzco.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ggseneuex.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gdghlodzz.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggybioszx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzruotqp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhtchdld.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhbaupda.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvwubtsq.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbawvsrrw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbonxxotz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkprdubia.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gimpeyhri.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmqdtlze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtwynsom.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvyqjaof.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gphcdofjd.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gudwxrprt.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwabcdcoa.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhiibtzf.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/girhfnlph.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfcyiqdl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gemofhved.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gemxyvdrb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyefsuua.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxtngzz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gobfyiyzm.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxhjbdqgk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gecerzjzw.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhkgjdsy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfgjtoyk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmlednhu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcstdkror.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gacabrcyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwbmobl.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjkuwlkv.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlfibad.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gnvotvcyi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gatmccxlt.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfurcvjbw.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrwutizy.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gvgyerjkl.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwskvriy.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gghhwjxrw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gliqhsnis.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwbjspih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcfqjugxf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gunrunblc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfykspqh.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggetpsgcv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwosbbix.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gyfeewtwm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gavdjikeb.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gorovwptt.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/glvdgphnh.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrezimyh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmsikmxfq.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggczwqxkx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gimfjtjtu.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gppaygqdl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbpprljfv.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkixcijdx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gorjfkguq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxreuktfp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/glnibxpyw.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpimupkyq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ghixckvpa.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnbiakkt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbgaddak.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzdrnrfet.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/geztgpfuw.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grbmggsla.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzpztwyj.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkyozgri.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbrvreub.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcmxbffv.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ghyaqldsn.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncwomqws.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldmxlame.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gogmzjqad.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gldfqytde.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gzigbfhfg.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnnqwiqka.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsdpygxni.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gqlmmptfj.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gnsrukabd.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkstgplo.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gyyvcpuey.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gojjwdzey.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/ghjfktykc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxnunsvn.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/glqixfcge.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyrjlmenv.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gisanbfys.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlitkkea.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslwgkthy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsywmvdgz.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gnsjpmyop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhjxctpr.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gepaqmrvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/guicfslyb.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gztvtmhxa.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gocivqcdl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmtjkxpe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwrlnkng.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gemjadand.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztinbcyb.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gblvlrwyr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlybmre.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkggbizzl.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gfyzgcnuj.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gfdezttyj.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gdckzxihr.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpegfmtsn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gvxzcxbaf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqtklkxv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwcnsuta.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatpureri.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfuftitg.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghosgtaoc.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/ghcgtlkxp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxhaqpdn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/glyokkplr.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/genaflsjk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmscfdmq.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gxvuuwfsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gllfhopjy.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtteggzax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuhjesqs.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzybiupwl.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqzbcelfv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyruicoit.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gwbngtmvf.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxioglltu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlryrlfa.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmaqpybd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/geblraukl.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeyszjss.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gleluuldr.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gokuplori.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvodsmcu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkrlmfcp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmcwdupjh.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmhgovjk.sHtML


<!-- 参考信息 -->