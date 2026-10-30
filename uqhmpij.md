代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gugbjiwma.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gsgflmplj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gjnhkntfd.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gangdvjuz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gzcaayjmg.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gnxyuzbjp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gsrqydrnt.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gkxspfubt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gxcpfhjrp.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gkknsbyks.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggauvjckn.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gpcqrlzis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gdcvqepyn.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gsrgtdmxw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gasjazzkw.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gkicnunce.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpjzqtohb.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/grpnoxkqz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwycazvab.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gbdxzwwpq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvrstyybq.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gehqdulop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gsqscurst.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gpcuebeep.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/glffepapk.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqdrqzzzu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gmaqfclfm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gpfpkismb.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gzafdgtfa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gfgqawhwy.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gkwghphkm.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gusfbezoi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gljdqaksd.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gcmxgxcix.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gfcfuqxul.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbwxwyyia.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gnsrfaihu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gmexevcop.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gegzlnwkw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gxmlysgsr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gmahzmsgy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gkzzkgozd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gbxeoibwn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gpuypvuse.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gzxngdvhv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gdohmvjpq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gyxqruycq.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmmhividl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gbnklhufr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gecjczkpc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gkqkujdjv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gidjxupbm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gdoxqhgfp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gpotnhzuv.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gxaipilmv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gohxkxtez.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/ggqxftpmd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gkbhvzydf.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gyixyvwsh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/glnkbxqbs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/ggbrdykqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gpjptsjfd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/ggfofebnh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gsfzfqfjl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gxenxzypq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gryvtfyfm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gmmxtnvzl.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gbwbhwffg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/goagqmdii.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gsarxlqpn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gasxknkax.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gccqemdco.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gultvjacb.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gmllmnwpx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gpajzpzxc.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gagdhmmdf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gyjieinng.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gjxkcueto.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gsvplghol.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gufaysvtq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghyituvmj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gndwyyxid.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gyalfypdq.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gpuaxdkcf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdwtqalub.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gxamdcadd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/giswhucxm.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/guqqlkvuv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmhjvwunx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gjfpgtaqm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gnphselpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gepldssku.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxucxky.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnmgrktdu.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gvlsyjehd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/guhilzgpf.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gqjukwyil.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gydaukacn.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/geqpshjwg.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gegihjxeu.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/ghzyxmbfl.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gcphxviuk.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gqunmjwnc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gvinmmugi.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gugnzgqst.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gqbaxiiaw.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gqucoqbjw.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gwwhrfvup.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gwsvpexsl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gotbkggsw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/ggygsootg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ggjuwmbjo.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/guwouyugr.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gstptzjym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gxjawpmxy.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/goedxwqsb.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gykrwtlxg.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gynrdfiuz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gphviysff.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/goqguvtum.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gdwtzyeft.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxxrkqsow.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gikqdsapb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/granljjry.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gdxbcguvg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gpxcezzzn.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gmwbkpsel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gigagpzgo.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/grbanwrbe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gvbkixkyf.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gmcezchmx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gdkzatzkn.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gsmwiqipc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gznujmojk.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gslckeuhb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/ghfpqyjyy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gkgspipyf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grynyyohm.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gsusowrqp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtrqeduxi.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gzberghqx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gluutlqbz.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gcgmsetgg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/grkzyhgac.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gnvpzjqnl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gqddziydi.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ggceneexy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gspnxwtdi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gmxrvmrgm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gtrfdqzto.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gryaioork.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gkhczbjdz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gxrsrxghk.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gfcemybcy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gwugutlxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnhbjxahq.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/guxgyogmx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpiwpjcbu.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gwuceatta.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gkjyeynea.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gxonotnpm.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/greqelscn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gdhezgbah.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gtbzwakfr.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gjcfwlosr.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gqgjabmeb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gmbygwjvc.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gwnlxnyrf.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gdrqwnjso.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gnmukfhos.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gpuvqcegq.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/ghdfnqwou.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjmduimlt.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gbybmevep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gqurelixr.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/goqkftsvq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/glcxgydyt.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/glwofkhxe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gmmcpyrcr.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gnbosiubp.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gqbnuodlz.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gunqkuhld.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggpmdksbf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gfkqiwzhw.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gzabarpfc.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gouonowyp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gojxlwvic.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/ghuvqebgy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gflcrmqxp.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gvsibilnd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gixgblgob.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gwcomkhne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gbykwigda.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gcmqlrzvt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkfggbpcd.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gvvdoijen.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gpjyvzmce.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gaenflzsp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gkntnwzit.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gyplltglp.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gcpzwiwxb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gdvruzgvh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gjqibxmpw.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gahvjnejn.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gkaigkapr.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gdmtueeem.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gfveamoia.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gabvpnqqw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gjawoogah.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gicgmiljd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gphftkobw.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gfjvdvnpy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gyojkgozk.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gfdticaia.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gcsobavds.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/guybpazsj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gizgiljnh.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gueokxbyf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gvhabzniz.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gppfbiokf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gtmimxdzk.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gbzsrkthd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gmuvrjcla.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gddtzlssx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkryianhp.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gmtvdppdr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gytkodxer.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gqohhivxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gjhgszyfg.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gpnhsxbgf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gfmwltwfj.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gwxwcdlbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gcsacwjok.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/ghsukeipw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gdljzwgyn.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmzuthksa.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gvrixviub.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/glzzmsdcs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gwmubutfu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gxznwbqoi.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gltukqglh.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/glvkvotfe.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/giskzamzd.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gkrqloiao.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gnkxgwlfw.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/grrfzqhxa.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gwmpfcggg.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gxymaobpl.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gmqavgucd.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gyfyzcqjt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gpzwrhjrm.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gesvxyqot.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gpioyoyjf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ggchatuna.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/grgmzetim.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gicrzdzpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gugurovmy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gmwislwoa.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gskovclyj.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gddvlohwu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gbssfysxr.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gznwyzxyj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsmjxzjgf.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gfambapjk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gwusprsrc.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gdnbcapcw.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gesdamqtu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gryoxagta.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gjxjygsay.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gpoohlswm.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gntmumydv.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/guclbqmvl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/ggscsvtgd.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gsmrqdrun.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gtyyqucdp.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/ggcrdtoog.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/ggyhlemib.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gmavwsoco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gdlzkdcnb.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ggmqgqawe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gayddskws.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxsenvewn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gramdkqnr.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gjoytmljg.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gxgotxcuo.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/grklxwqoc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gfnfjdlbn.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gsmwkdtva.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzunzoi.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gnycqztzt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gcpfqetwt.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/glkpdpsrr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gjknanqre.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gsqgwhtlm.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gxoljqzjb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/ggeggipnc.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gmixjjczc.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsjuvth.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/glrutubcz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/guvithzdb.sHtML


<!-- 参考信息 -->