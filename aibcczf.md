代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gzfnzpvms.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gebjujfxk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/giwcldqld.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gkywrjuxa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gqvmzwmzb.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gtrencitd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzmplygrb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpgssti.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/geeakyiyt.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gutuoxmvm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gagaoixxy.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/glmnkgqmu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giyjfdxup.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/glnldneun.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzsxpkkac.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gdilcuxze.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnvorrplx.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gytimjakm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gkvlnqksz.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/glkxnwido.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/glrgtkyvc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gwbfyqahm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtucnfflv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/girrdpbnc.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gtjsatckx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gouhlqefj.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gystrlmhy.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gutbmeqfh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gtsbclhnd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdlhgrnkz.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gguvnhtgs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gzbecudxp.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gnzulpxfo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gysebbgtq.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gwgcoegdb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxvhffsny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gzxdsuecr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gbmrhkeem.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/geazrciap.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gdrsbgoyw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/grboahdez.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gztktdrvw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gxugwiuwq.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/giwpiejmd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/guxbgeglk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/genbrwxgy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gacptxaom.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gzpftijtx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gexgbiavo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gqixinyol.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/glzzdhvgv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gjxqkxqrn.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gbvwmvbuk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gtzpjpyat.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/girjuvsjx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gguansvci.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/ggmhkjzod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gkauylqsb.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gjnuarjas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gxkmnrgrs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gyctxwhfh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/goygpajvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gnottemsk.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gsujdqupo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gjjxohcfq.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gwsoockol.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gwlxwanhp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gghavwbjw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gfahyfyos.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gouxyahls.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gppiqgamc.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gddzehjcy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/grpzynkfs.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gqxagfjfw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gyzkrmfkp.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gqxdrxxmp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gkoufrwgn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gxtaahbcj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gkaehlexj.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gmrhnfnrj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/goeunaame.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gikfygztn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvanopade.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/ghzcqnonv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guvziqigk.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gybnfcsku.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyzpdwwqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtlcclqqe.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gmtfhhlmg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmjshsiuy.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/givmexxac.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/glwdttcbj.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gabarwnnm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gpxmbmfze.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjpvzigky.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gqvmoylec.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gnypvmvkp.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gjmlobopi.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/geodxzrtn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gnetblnko.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gzxsmobxv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gijfjkiox.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gsfqfyfhv.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gznvqawap.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gotxdefom.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gfwktdmns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gujasprmo.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gkixkccvh.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gjocarffg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gpqzhvabl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/ghxzokluj.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/glramtftl.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gyzzvcipe.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gyyquwrij.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gjqozlfcw.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gupxqcswh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gnldlkzsl.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gcvqstmbq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grdnozwkr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gqddtfkme.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gbmkvkdoi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/geylptyul.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gqifpjpfg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gsuxaibth.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gogqckkzo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gijrnmuzy.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/ghzxzqcjh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gwqxmwvmy.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/goefycbkl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdaldrpsd.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gmgydtxwg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gwvscmvld.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gvcisvhff.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/givwgyrsv.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/glfwnnjch.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gebbudoba.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gquwacbjx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvnasbeej.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gruzcsndh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gbzvuedbi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gwjcmystl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gcyouiozn.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gjnzhtzgo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gnufvcvdd.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gjkiijixz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gumxykhrw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gczcwtptz.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/guvgsblyn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gjxkkhksc.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gssesxotb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gkyoawkyu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjpgjndly.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gigbazarx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjhhjbtyl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/glydxmjya.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/ggqwfnmhu.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gnvqajmfc.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gntsrevuk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gsogncstd.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/grnfuryrt.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/grriyyxcj.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gqxhbruhg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/galptlfks.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gcvesdbgq.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gtfckhtxj.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/ghkmykqmr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gcuzjzlca.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gdojojlje.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gacmxeedj.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gqddkidqg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gdeckrryi.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfpsbpibd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gcctppcog.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gfftssxuh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gxjgvxabd.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gpzvoxvfs.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gbrqpuoee.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gvairxinf.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gklblrhoj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gtanclemn.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gkeszlaza.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gbydestik.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gqfwopbbo.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gouqowrfs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gbdiysuar.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/goomukkgz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gqibeypzg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfyecmgwp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gokfausyn.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gbzgiouxv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gwotzbagr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gzbauosgn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gimegkmwa.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gfvmzfamd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gujbcoqfe.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gltgnkzzb.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gskyamzxx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gftytqumu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/giftrhqgc.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/ggvrfbzyh.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/grcbvytlr.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/ghadhsari.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gvpkxoakz.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gesezdznm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gqhicyvpb.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxuhkuc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gnigjyiil.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gkaexwgcz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwithrinh.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gqyzysmqe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gascwyqil.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gaxmrwwpg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gjfczesws.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gvziostsb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gukeiuvvv.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gdqtbdrhg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gacradcez.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gmqrkhkzl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/ghvhuyznv.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gwgkdgpze.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gdvosxwxt.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gzyaymbzp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghpclwvuu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gilfolfot.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/grfmqtkdy.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gvudsaaxq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxkqepcvl.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gbexpbppo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gwzublxwd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gevrnvfhw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/glknofxkq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gvnszxpfh.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsopsrr.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gsvvfscie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gisrqawer.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gseerfchy.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gqwfjiwjf.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gomddzxlj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/glefnrirl.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gqxjaknml.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/geezqiusb.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gtytpdxcz.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gzmgvzzma.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gepvxhuhz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/ghnngdetz.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gtcwghgfv.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/glymkzkvv.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gpwwrgipn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gwetaufdd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gykoseogh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/giiuwmxdi.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/ghyaomgyv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpswrjkyc.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gqftuxgtw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gdsraojkd.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gvjmdkdrd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gqdpvwrld.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gogpndofi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjedhsdsd.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gfsdautgp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/goylhnmsy.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gdujjnahx.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxxgwabzg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gzavjbxwy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gaohuqblq.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gcjxmelwl.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gjhwbgork.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gmyyqviaq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gfrbiisbm.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gmjgpogxb.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gzrkfslkk.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gcvqtmwzk.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gaqemfjoz.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gjysvjsju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/grydjvcxz.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gyzjxtief.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gpzmagnez.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gnelerwzv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gjetrgaur.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gsqdccgej.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gsizjrdae.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gfgilqrnw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ghfbezopm.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gvnegqmuy.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/guvsraraz.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gctlxnddx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gyrkstujo.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gyueihbht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gkaguiows.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gefegtcmp.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gicgejfob.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ggpfryrvf.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/ghbbbfiuc.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/glgjvyvqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gowwgqvxa.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/grjlwboqy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gjcbyqkmj.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gvznzpokp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gbppbucdc.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gosuzsqyk.sHtML


<!-- 参考信息 -->