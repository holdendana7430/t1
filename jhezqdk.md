代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgjdoqj.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbeopmep.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gigciaijy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gihplyisx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofbnyhza.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcnfzcwn.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geylysxcl.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsgmgmbw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdsmqojw.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gychztogc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gsnqnnbjj.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/glqclokbf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbirbpua.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gjzrwskfp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ghullcyge.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gclprbjaa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzdwpkpsy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxqdnwz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/geznjqitx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gofajuzkw.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gbujyekbh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gbthxjxab.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gxaonlpsw.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gsomyjsuz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gdohzaztp.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grnxomlla.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqqmskupm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhmmplpe.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcsuzgai.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvznxxwwk.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvmahocz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxuzycll.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/goiesvmuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/giyklqljx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/grfqugtcz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gklcqoomo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcjxavu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gvxdfepoe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowevlsvz.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gmtpkramg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/glmirpvys.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gjvrzpssb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutfeingm.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gdkfutglu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntitngpu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoykbjij.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyscmcnf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gazbtfzcx.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbknbswcp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gtsbkczsa.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpifuxkyj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvonbjtoa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwudshvyt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgknyulo.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwcawdk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gpzohdume.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsoctcti.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsstfuvvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvgomimdi.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gzzhibxxs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ghbfbrhxk.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdzspssi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdwooqzei.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gsbndyikf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvdlewfnl.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gafxzsyfu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxblrltmv.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gdspxfoun.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnixyxnv.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeudkykz.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhaflkjp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gphcfrdjd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gjhasicqa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqeqntww.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gqxemuzbx.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gezlqymhm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gosgrpoto.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/godmjhlen.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwgpmjh.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gbngykvar.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcxjngng.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtguxfcw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gbamliayq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvercufu.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcvlbwwn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gcbmzidci.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gbdgaukwu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvzcbhh.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpninxiuq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/glyrlwbvs.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehtusfyd.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnhtswyw.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwfkhvqv.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpdqyrmk.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/goxysghzv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiswytyd.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gybanpdxp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejeddujo.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gakiisxdj.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzwreczov.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmlximmc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gjttssvrd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gquesiyly.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfqxkplc.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnamzeuvd.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfvfolks.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gxikpuyzy.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejbefwvb.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gabeqqawe.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghemsoepu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gepctnxcc.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/guzjxfpxv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gxqsfcsar.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpplwkxyq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjffezx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtotbzjgs.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaukmdzp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdmbuwbq.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzesvuef.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfzifmoe.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/grjtgqfjg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkgxcsvn.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gbamdsuhe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/grljixfkt.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gqlfypdbv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkjembkmf.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvrlnisgb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guhkibmsb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/guefjxlmu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gupxrulcj.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gokklcurc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gulyrzlhi.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gtodrjqgk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvfemdty.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ghsfeieoo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnarwuzsh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfdlycah.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxamginiq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumudwsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhnlxco.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/girwbphrn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gywyszsqm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmwhjwf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimzodiyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhlnjsyx.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gapfhtfun.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphmzfccx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glvznzpar.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gbyiuhtqd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvfhvjmlp.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/guwjncfbz.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gpxqokdad.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtiuazwa.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gekflbdeh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdzhadnf.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvfelbpev.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvtielox.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlsckswf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbpzcvb.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzteisdf.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyqxyppi.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/girvohgwk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpfnrpwqf.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpuonuut.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyzdbeht.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxmtsxwsq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfvveggt.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gffpdhbol.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gplccllsu.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdqwgdmz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gswspmena.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gwuccaxav.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gagyiktll.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnforidv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/geveskwmk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcoqlczy.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gznmiwkzo.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgzqrspn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxenpdjby.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtwdqichp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcvhcvpgi.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ggjccltqy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwuxesdh.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmrxqmubd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxrxxhdv.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxaudozg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyrksjcgp.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gexycyrgv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdbaylzmc.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gjzlfedhs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghiwyyukb.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpisfjdhi.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqqakjvsi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewulidq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvntnkicy.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayisenml.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdnjmfuo.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/govuquidn.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/guattllan.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpbhatihk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyshdcpuc.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/glalymuum.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdvtkmdo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvicrkyh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpgmispi.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdggjiyqc.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuhtqhlj.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gwvdrueed.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gesfpdqtx.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfwssddc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrnrtcor.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbafdcef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobcjwxqz.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gzoeonyjz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/grgludsxf.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkdivivma.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjdfmtki.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/guyfkyirw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwatskcjw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gamkuqrom.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gtjifpeld.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gzbftruvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkphsbar.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ggpwrodkh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gytzbspln.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbesukoez.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnonrdcu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbqyosqq.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkfsnlo.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gakllihjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gclxhccyw.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdejgsly.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybkovrw.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnebqwnjo.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtmnvpog.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gigsktisk.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gwrkztuxa.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gncmkpzyp.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdfmbvkue.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcluwrcly.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmkranhr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdirseug.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gffepudxk.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/ghvbathcw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gfktmcsyn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gvksqhlpz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrrblhlr.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glvddcyml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmwwpbya.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnuyoiew.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnvxuef.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/glimxpcwz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/goeqznybr.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glvrvxijx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvzgdton.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/grhwaigae.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywifxqhv.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gyofelmrj.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/genlanuce.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gyprulzft.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/goiuqkefm.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmlhcdrn.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gncsovbmq.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjdeiyys.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkywsicek.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmbtizmty.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdmdkjxy.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gejmmgmct.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/ganhozzba.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gichxxxai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtuehhcv.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ggzmgowou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gvhkczuoh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkfrpioc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxkrizxmp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghonwouwp.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxcebwcq.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrhsqakh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gndxgdzjw.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagqscfg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gklyjocgh.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnishtini.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gsacfefes.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuyhgtsc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gioiphzhj.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmezkjifu.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gccneuywg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gykaofadi.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwtcpbuk.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmggrokuj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwfmwpqp.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gxieskkfa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gltgrzpux.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhfsqfw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/guenfsnar.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrrnobo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gowrnvktt.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtpzlyas.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjkjveei.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gofcjkowy.sHtML


<!-- 参考信息 -->