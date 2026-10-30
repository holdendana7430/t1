代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaqgfxoa.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqhwrtoc.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gevzmhifb.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgyvsgkz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gyatpnvrt.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gtxapsbef.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsngwxcb.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeqerupn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpncxqbf.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gavmwbzrz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyivajjjj.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfscqglaa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhudoymt.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gsoihowul.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmhdnjjb.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwyzeiav.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfckxeyg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpsptgmq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmltybax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gjyzdhpbm.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedjkatxz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gpugalsxu.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gzcbkumph.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/giawclmkf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gilerqqqh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyqzrjts.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gqsaupuka.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdoqsojl.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gkiwhffdo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gesdmcdez.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcwvxurc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlvlhkxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcycevwow.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghezxqiho.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqhgpmoa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshfixctb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gppmkytgx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvanzcxs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmzpcdfx.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gurdcpjfi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnflbnlll.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gifwbzreh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgnpwkxj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gaqkduown.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/giajebrpk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gmfjqaurz.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdpieqec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gxlfajvdg.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwrsdkyts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gogmqagkw.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpvtwapvm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdwnxqwg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqwklsev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdwzhmvk.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoxnbbjw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsnrfitr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxkvjgf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkptymtc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/grfzmcnbn.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goidyjgyb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjpskyrw.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeocctqn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvianylz.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gneeenmib.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxovsotpx.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/guheynpbd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyounnzfn.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgsgcjxi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gkppivecd.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbdpnle.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqolthk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhuceygw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkljnrou.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvfofgxn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gsdidhpvj.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjbgfapb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdzcfwmb.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gskfzcpiz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjgwsfex.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxhowuio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnokkfbhe.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/glsyzxcqj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnlvkpdd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/giymhaxhh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhqnyfn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghagnrihp.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnobenoc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrfhwkwo.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfowgxbpc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gafexnvrh.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gkzqcsdao.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gagriwrqx.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwditis.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxlzyla.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmwsfdmn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gkffhmkib.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/giqyjruie.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/glzijnnjn.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfatfqxzu.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkxpaett.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzlewkcf.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gfomgulzf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gvglntujj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrnvcsws.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvyfirzq.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gnilkvwqq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkfccqek.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvoaqpfe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grgqyvpya.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gzqoadqvc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfigascrt.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnajeatx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzndmdaf.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/glwighpoz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogdreenj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjxoajyx.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcgossie.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gifjhixxx.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gciyzbzuc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/grewwiqab.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpyspoogi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpejdcee.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gobpnzykq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gublcuhej.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/ghafdmiti.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgnqtjir.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmqqcknie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gshiyozfv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gywgtwenp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gipfeafmx.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gunpskzxe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpcrzhqta.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjalbljq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gddknfdjw.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuaoimzj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnbbojug.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnnjyiht.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpktqemf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjxnyyfu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhlyatlu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gdzdyrjin.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gfptutiuf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrcvmsp.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpxjsefnu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gmengxxfb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghafkepm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/guudpktjy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glrftpzlz.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbnnxpmw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdhhrburg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqykaxhk.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gjzfptzde.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/giiwbrlbx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxgmitiy.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlpwtouc.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gucrtvets.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gxzpogxik.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyueipxn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/grnuxmlgy.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfafmfma.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzamptugu.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gookdsvge.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhjgnmop.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrgwcsfe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbabmtrld.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggburbayb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gysrblwcx.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gowdgiifp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhlrsmag.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuqwpgyw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjnpijsw.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gqtypgdkj.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/glgznrfnj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvlkgyzr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givuckabk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gdymsiqpu.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrkidujy.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghicijaiz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfgpzxwwa.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/glampwqxd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpopipoi.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtavavdw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gotazuqgm.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gusjufsus.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gngpuwoze.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/giqyjrvem.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grmqxlrzt.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnezvpmll.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsghyaprr.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvknoah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grjbwqcyd.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjzroalp.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnckdsnf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrxixszr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzmfzxboh.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/glxiglkhr.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glwjzuufi.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/grmvsxetr.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glxmxrkhz.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvqjiquw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpiatnnn.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gffrvhcvz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggeovxqan.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gldafcwkj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/grzfaztmx.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbcslxmt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdiiprft.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/geralvuob.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gujilgwez.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtumqgczu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmsjnat.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbjetnwae.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnxyfixz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrjkbic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gkuluopri.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjgpqicrl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gydrpuqzy.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfwalcd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gppkrxcjt.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjqnducoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/giqllquqs.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/grquxyapx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcoyubiq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuoolpey.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuzjrxio.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcrzqpwjq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/giusdtxgb.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/glawhqjry.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gclpdcszp.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvgdpfuu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhcctqom.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebpuheg.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gshgyhuzh.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gsdgfmsor.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/ggchcycph.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxxuhjni.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gfzoeroxf.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaijgjgm.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvyixpp.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtzcdxdu.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/glweffbog.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gucjtdnhf.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqaidxee.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gihmsmnsg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gmtglsiwk.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gapfylljh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhuwjvve.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtudvjab.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giaxxhfol.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxnugbelx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxeneqiz.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvvzymtg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/grpevimzl.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoecmmge.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtguwsyrn.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwzjcccs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gvxoedgfl.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfgaojdb.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gordriysb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gkirgtkim.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gewjbgout.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdanxtrjf.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdbauvy.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gfrnzqunv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gsntlnuax.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ggahstrre.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gzqvcyodv.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/geanodqro.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgrgsbdh.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgtiihze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ghkpjmuab.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gotzwhhkp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtscoznro.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkyidxkc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpbteuqqq.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkfawffz.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gglynufms.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grkzuzoxe.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/grcaiuocd.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcaoeets.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooyybkgf.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtabjiekq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnqeaseua.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzbufbzus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkcfzfb.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glpeaqhtr.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqnuoqlz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghanzboil.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/glenvnwuu.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gzljuigum.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grphvwbpr.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbjdiiqa.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwhokkdw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gabihwjcf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gighbqolc.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpueftgd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhclyfkd.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gnryydiuo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ginldolxd.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gipgwetyf.sHtML


<!-- 参考信息 -->