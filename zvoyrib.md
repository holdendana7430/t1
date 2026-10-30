代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gdtfygreb.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gskojenir.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gzncqviyw.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gfkngzknm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/grbxpmpoc.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gjxzzkggu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gzvynfsbu.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gbdxzlchd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gtrtvjnkb.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gatdtnele.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gmylggyhk.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/goizgllou.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gszkdplaq.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gyyjsutke.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gwhbnvfkw.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gfkiyunce.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/ggawxacka.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gypusviwk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gliughxuj.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gghevzeud.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvhzqlatx.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gbmqiqiof.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdawdhuvj.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/geqjvberq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxzmofhlz.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/glctkmfhj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/goexysyow.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gimrhrwhk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gyjopwbpd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gcbtinzfa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gwpavtjju.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gkbxlfigw.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gczammymt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gvupvvzys.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gdrcrwdin.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gsnkzsssx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gmmvwianf.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glycxrudd.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gegglqldu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/grhaganvt.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gjnfcmfec.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/glnfhvsev.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gtnuszmum.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gurvnthxc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gfsrivrdt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gyosfukmc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gdpwporjr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gcjfxlkbv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gwnmfqpmg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gmmtczpwx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/govkikuit.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gorueobxa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gwtaucwvd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gkfymezkd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gzmixglmn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gtynkhagt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gclwwzlzt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gicxeekxr.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gxlsimkme.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gmosktclc.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gdmbzcjjl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/ghqkxzuum.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gujtfonqu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gmrufexvc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/ghbmdmvsu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gwzpiftcp.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gohehryek.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/guiknujvc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gzhqdqdfv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gukjhcfve.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/getziehgb.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gfbvzvvsz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/ggchbjjce.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gyvjktjbg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gvcwcowbu.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ginaztxej.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gubxlaggb.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/ghblsihuu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gfikifvrx.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/ghhwqqfuw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/guvpbpyvu.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gxuxkuauo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gwnphlnwm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/grclgyikn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gzbbemiow.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/grpacbmef.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gaigzfnks.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gaqfypwcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdoiscfdk.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gqogtwbbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gciyihtob.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gpjvildqs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grcqdcgpm.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gsjiqtcxn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gnzjnqotu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gsliulzrc.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gwpztlass.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmvkyiuji.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/ghfjvplqf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gagfmwvrl.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gelpvtnod.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gjolneaie.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gggnftaeq.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxvukcun.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gvoecgjmi.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/ghwaabbhi.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gcyxumfsh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gqarbmlkm.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gbgsruhes.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gjbtdfusf.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gtyucnnsa.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gapmahyfo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzxknultj.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gpqeidzxi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gdcdvaxfk.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gqwdbahmt.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/ggvesiywt.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gdifaaweg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gasexsxnv.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gzaketiut.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvmebeenv.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gbdpmtnan.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gngqrbyqi.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gskwsqiyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gahuivuoc.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gygafrjvd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gudhrmwae.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gwsxqylfa.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gpbagevlm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/ggrycrnio.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gnyzpuzlm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/ghexwayte.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gpavpojuj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/glemcdkua.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ggenxdeab.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gchgrghhs.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gylhontyv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gischpcyy.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gyceelwgr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdwmhdsxk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gbgdzpogm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gepkzhsoo.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gjmoirrwq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gddnnfpta.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/grvbumqfl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpzpznyci.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/ggpwnxlja.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gspnfdcxe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gkjjvxjpa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gwruxzpql.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gnzcgimli.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gvgiydgqr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gajvxhswe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gxekjtfkt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gcnjynzme.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/geulychjc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gpmygewwo.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/guqtaboqn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/goisqgzab.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxlhpxhrt.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gyejggulb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gliddbxod.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gqdamabij.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/ghmscnqed.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gldhowecu.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gzpfqadev.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gomsghvjj.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gxbjgfqzj.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gtwgdzvcx.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gupzjklwt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gtxgmoazh.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gfswsbhpr.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gkvpjvkdm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gsbxlatkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gzqbqbsre.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gskpvmejt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gnfkknxav.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gksqczgqb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gnfkelyqj.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/guacpspqv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gykhoswpv.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gbdvkuoqr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/ggdubkfid.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/grnzedciv.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlsdarc.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gzopagnso.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/grdouvair.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkrvempnc.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gkbifyrbu.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gciabahub.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/grjrsibxc.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/ghgkvslek.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gmamedfff.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gzrhmsgze.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/ggmndpqby.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpirokotg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gqigvnskw.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gndasfein.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ggkmxibdd.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/ghlrhtycv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gpudnylhc.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gogwabxxr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gevcrxbot.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gtpkdhkml.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gkkygauuh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/giigslpps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gbojnteog.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/guvoogffz.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdysinppr.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxgvnfysr.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gmzpnpyng.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gmdblfofa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gicpfdooi.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gqdmcgtrp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gegsjyink.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/ggespbzfh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gficpsddc.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gvubvuwlv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/ggyobqyfj.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gfeyzdyaz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gbemtsfaj.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/grvwqgiva.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gmmcgdudf.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gmrdrxkiu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gnnttdagh.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/ghybilwti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gfkmtisir.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvurqtlmd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gccxsqgni.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gjtasgztf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gumsdjodq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/goknjvybs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gwyfivjqo.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gfpdaskgl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gftrgmheu.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gpwpbtqgt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gqhpuhlpu.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/ghiovwvpk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/ghbvvgqyt.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gjuxdlybw.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gaxeiisfs.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/ggmlmbcwh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gliqlssfc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gfpxjoawo.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/geiohpxzj.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gqrusrdzf.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gycayyedo.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gqjqmspbq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/ginfcsaqu.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gxdczpefm.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gwdcwzlqi.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/grnbwdoos.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gkhtskmck.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gkpqwyikv.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/giadyweoe.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gkgsxwpig.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gghgdxesn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gpnfzubzw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/ggfwasqbf.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gfwftdmol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/ggatskckc.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gdtmcjsle.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggeeirbkv.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gaxeaswwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gjktotloh.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gusymwfxf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvqrnqmok.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gzuwjwwpm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gqchmqebx.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gyvmqfhvv.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gorartpxb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gseykoktw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmcdfxj.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gudauetas.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gpuebhsmy.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gijgvznef.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gpwlfjacw.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gnvhywccw.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gftaiiuyt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbfmkzzko.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gpfzsffzl.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gthpjzzdi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gcwitmgsg.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdrbptefa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gtohfdovx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gvzmthtyb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gdtshgqju.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxgjleazs.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gubrvgozz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcgntlyif.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gboifqdrs.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gzvohorwg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gyjdjrhgi.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gvgvonsbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gswucgsxf.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gxlpvcuim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gbwfqjjje.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gvpgcfwhb.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ghujlkbmj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gffkwpmyc.sHtML


<!-- 参考信息 -->