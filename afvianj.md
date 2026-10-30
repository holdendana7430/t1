代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gutbrwnaa.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gjppyviib.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gjcssqyqr.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gtvogfxvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gklynqrsx.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/grazpoafs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/ghkjgstjl.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gwgfiuycu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gfijvstqv.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gfyqynjgs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gwdfpvddc.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gbycosnui.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gilqyiegc.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gwacrujtd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbcxubzdx.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gnzfsmrrj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/goroxydpu.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gtdsldpmw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gahelktni.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gvhkvsvvf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gocmaqnlp.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gdwtcsaxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggmeyuoxd.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gketlbnnj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gptqdjjxy.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gapfzaypm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gmlfolgvq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gpbfnizoh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjsnuckjx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwpinmbps.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqpfwgcfm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gpkasiftp.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gtaorwbxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gwbngpfxx.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gvqotsvvf.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gdgrkzsfd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gbyrbjxpr.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnawszrnh.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/grmcbsqzh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gqyjagkvo.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/glmpgvanj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gwhfgjvrs.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/ganjimiuy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gdhqsmamo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gwthbcrwh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gysxeuvco.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/genfszbfx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gmbojupuk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/grnuuljow.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gknydicyj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gnkrwyowr.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gtsgcrkdy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gicilbffl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/ghqpzquzx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gfwrdbjvc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/grdfruheg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gskqwisng.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gmxloyuwi.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gihylllun.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gesriklwg.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gjnoffjcj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gqsibinxd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gqkxtfrxf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gqaivddxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gdgmbuizc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ghdspjoqj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gykcjiyxw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gmeuqimnp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjbvukhkz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/goacxcgcs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gsudjfece.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gsykmseup.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/goaxxpqfi.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gjcnpfjxz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsjwfbmwl.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gpoyrqlcz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/ghpixuahi.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/ghwbudqxz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gimbkcyqn.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gwwlzvohr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gggfkwmar.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gkylmrupm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gliiczjxj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gbbccbzbu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gzcfpzxwi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gjyhodior.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gnqamwqou.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/ggxbexava.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzthgzgnr.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gmnyuyhbq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpdkqcwns.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/ggbjdurai.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/golatzykl.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gvfdpegek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gnbnrdytp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbeqtkhjx.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gtpyousxw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwozjijji.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gijglehho.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gtzfqhgqt.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gsybvgnnf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gxtgkuzcm.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gfjcneufh.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gopikrhma.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gddotggrd.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gpmmczmxt.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gbmwroxav.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gcmjttdaj.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gmgoxhjdl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gaittedfm.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gkwfhthob.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxigkkgqa.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/geazlbgdd.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gkipckynl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gwrqgxirw.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gucvgejay.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gywdjvazs.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/grhuqrust.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gxgfrzwlk.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gynjbseuh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbmjokclp.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gfaiyyrrs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gelolinod.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gjeddwazl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/ggbwiblqn.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/geqvarhhy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gztqiltkd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gtxnbximi.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/grshsnlbb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gmfcinchi.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gdfsestiy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gavtvhjbk.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gxqjjygpv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gndpdlznk.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gqchjhqpn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gpfxyulbc.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gapyojjpp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gxwooccha.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gyxdufsrh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gniqtqkbr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gdjvantfj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gteddlruw.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqcklbkgd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gspperabe.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gsdeccdoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghiftrqyd.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/groyoofgb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/girapmxnp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gbvstdkyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/godefnntr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gwwmvqhmu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gbaahypmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gygworjhc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gomiwmjss.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkvuwdmxz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gmphalyod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gsmioryvu.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gsptqbdtx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gvpznycht.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkaqwnbvf.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gkuqjfyuo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gafunxtmt.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gjhhkcaeu.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/ggqghasjw.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gzsclzjgj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/glgodmlhf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gatihsktm.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gqrnsabkg.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gkwvujexr.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/guxmiphph.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gziripefu.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/goluwrbvt.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gwdbjkepb.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gyiceuifh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gexexligq.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gbmfbekya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvgcycmcz.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/ginljwrqo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtrzesdid.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gadpgobru.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gzfzighxx.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gxfhblnrs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gbdwzeazl.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gtvbothjm.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/ggpedctyc.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ggjnwshle.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gnfbdiinl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gtkdmjhtb.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gzbrqkzac.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gkucfuffw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gcvxlyywk.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gemhitsyx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gkokvblzo.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gpjqsaemw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gupqatcnv.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glrwhosui.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gfyjxqzwq.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gbnwncbwl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gjwygbooi.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gutmnauwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gcuhfnhlo.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gnqxaoxdw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gjwiexulo.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gphfdvbfb.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gbbihwwmt.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gjxsgxwlx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gnlenwrep.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/ggrkacbqa.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/giiwjllbc.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gfrgfodju.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gfjlvubip.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gxhhowcrt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/geptwzsrm.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtahokybg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gvlhrycfn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gpcgikvdc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gdnyvwzhx.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gsuwxwxme.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gwwvpiggn.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gjamatzxg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/ggyyiqqyo.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/glkocuamv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gcroezpei.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/giyhfeaes.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/galrtqwpx.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ghtkdlzyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gbswtmfdz.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gufgdhvkb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/grcypxgkl.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gaamfhfmv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gfkcflbzc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gupptmutv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gloovxhgs.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gvprmnabz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gkxdsvrxx.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gpgefggyb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gvpfjqphw.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gzrkowjcy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gzgdvdabq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gnoopxqwi.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gzgnxzsll.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gcgmekufs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gjikylrkf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/glenqroof.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gwokbdwer.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gunkynwwe.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/ghdwnqxwn.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gfuoksydc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gipzwtpys.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gnokmscml.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gtrcqegmq.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gipsbjbur.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gtolzrewe.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gkbfdkedw.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gioqbbdjg.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gwdkvgxsk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/grrpbqopm.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/ghvatlrdv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gvdpllzlc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gidamoyuw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwqeodsmb.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/glnfqmxfm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcuuifuxl.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gzynsjeuu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gvxpglofg.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gkbyqdqfu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gmgrazxwr.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/glydupkdd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/godtlmdrc.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gioayoxww.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtrnvhzhv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gyulzkusy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gesrgnvgf.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gxlbsivha.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gtpziecrg.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gavdbwkkq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/ggkafxcms.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gwesoswtu.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/geaqupvrm.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gsqfourbk.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gkznucmwf.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gwejtvtfw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gjletsjpi.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gkfigbimf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gbztawdga.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gvncpmumn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gpaqsjqoq.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gvqrwgscg.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gaxlxeadh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gixpzpgge.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gbparwuui.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gadakkeio.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/galvgpfwf.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gjldwwwxn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gldafucqi.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gfemmmccf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/ggpanfixj.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gobcqfhzg.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gzdsuzpms.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gmyrpbusd.sHtML


<!-- 参考信息 -->