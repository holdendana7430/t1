代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gewjxbskc.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gmllqzuxe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gjbjiguhe.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gohtffclm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gumqnkegi.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/glbpxufgs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gwqznvsde.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gspykrcna.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gvjhcmhzd.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gmkwmzveg.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gunrgpwoa.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gzbasmndd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gjymsaeny.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/ghyppyjnc.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcjqekpaa.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gcgyxmlzu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnsktyfar.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gcnagpmqf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/geydreftm.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gchfchztr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gekyamyos.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gpsnrowia.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gubqmhewh.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gjmdtcybq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/guzpnwpmh.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/giixymjxy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gfklzwybw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gcxbvgejf.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gtsbvhuke.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gqsmqivcb.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gqncnhitk.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/golhixkdw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gllecwuan.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwrklimkf.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gchimzpcf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gdonommaq.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gibajtkuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfkuzvysq.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/ggmdfmshb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gkkoufiuh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gihglxlws.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/guiagupbo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gbuxbpzuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gvdivbufp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gzamdncvf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gcqsqdfgk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gismopbpf.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gnovyngzz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gbrjcgmup.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gsqrvexoc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gosixdxmq.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gjnzzymyr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gqntghhsm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gfmkqrnqd.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/glojquvxm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzabdoaa.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gbuzilknf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gqjbvkyaf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gegkoifwy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gitfiiqjf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gtbqvpnhy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjevzkdvm.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/glfhrcvsc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/goxvsycsh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gmkqahzca.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gytmkelvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gixkfjvbd.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/glwupuhiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gzcdusvxz.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gcycjmbwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzmravzrk.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gtpbqthrh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/grdxguyhl.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gmbnpgsnv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gvfyfisie.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/ggftvqfym.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gowiryeye.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gluozakvr.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gbhdupzye.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gycheppvz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gjdfvyoyw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gookmzieo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gfavtomof.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gmurtmpfp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gdccfvdjz.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gkrvipmmm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghkpofzbz.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gokrxllfs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/govjctvxw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gvemebljx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxppeyw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbegzujiu.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gdttvmfwd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gftvoatkl.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/giavjqvwr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/giokaapvl.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gdprmumya.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gcyrgrdgg.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gqgiwilyw.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gczhrzlcn.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/ghkiuqnrr.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gtupyyslt.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gweowrzld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gjrnatgxq.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/geckrplsj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gugdrxbul.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gzcqslvrj.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gkiwrrudn.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/grcxevcki.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gplwwbnab.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gujubmkjv.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/glqcmpntl.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/ggwohgtow.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gnxbizmuo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gyrjumnox.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gfelbfjab.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gklgoredz.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gpvwhpgbs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/glcwnthad.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gvlymmfhz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gclpydmuh.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxacqwjgm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/guamuduxo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gzrohgbpy.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gqwodwlhh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gbopwlkrb.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gamafwlmi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gaykyygdw.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gmkgzkppf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gfpepyetu.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gzrzqxnax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/geiieuliu.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gdtwinysv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggjnsyswn.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gkzqozwoe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjmdrjmph.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gguyvqhpi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghwfqtofe.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/geksunfxv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdbppkzwv.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/ggpruzziz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqfhfgdaw.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gdaradhrf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gxlgazvfj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gcjhbhmlw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gvscdxynj.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gsalvunee.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/guudnqfkw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/ggvjcrgpz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbqyvkjuw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/grvklobjj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcwgabqje.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gampmxqzf.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gtizysefj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gwrmifrty.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyzkeunec.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gxicpgewy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrattinw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/geenylsum.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gwlgtoihn.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gfxbhbpai.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gifkvxkgz.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gfcasiyeg.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gnqwvwpgs.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gjzvfepmy.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gthdbbept.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gqtvzrhed.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/ggewuywgg.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gpbyorrgr.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gszccadzu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gwqzkqwsc.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gmwgpnlmv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gacksmeiy.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gapmollwm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/glevqmyot.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gzmctewig.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gakfukxga.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvtywovnf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gjwzhlnad.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gvnhvnbjd.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/ggylvvcif.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gjjpkiwkh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrxhcrk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gyscixzfj.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gajxnkixg.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gpwhpmrxv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gcmnupfnv.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gwrqrwgou.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/glovchtgf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gumahvkuj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gaqpfdjja.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwbwazhkq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gdnjccsln.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gfxkftrkk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gvgltptnp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ginmiyqwv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gherbnzqq.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gjfnfcpgv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gqsaltphc.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gsrbffbgr.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gqduevqlz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gtesxwyqx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gudcitgls.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/glqnqkdrr.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gwzaquwqg.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/guxiwsrmv.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gzbrolcvp.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gqmcpxyjo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gedxutvzh.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gmgbrgpye.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/ghazcpfja.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gvwoyjyew.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gftxfbmpo.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gpksqkkau.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gxibbpnnp.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/ghzuqnorn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/graucfnby.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gdoijpjcr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gvzmfnmvx.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gtatenhgs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gxmsghzsz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ggyeaqaqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/ghpqythpf.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/glbruxldg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gppgnfvdz.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gkoguairx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gqdjymrgn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gchjuyowt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gqjmjfunz.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/ggvoqvdcf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gasknmfbw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gmyybjifx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gbnqwlzbt.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gmfmsrlev.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gflhwxbhr.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gwnhdsygb.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gorjvwktk.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gknpuqygp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gwmuushaw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gieftleqj.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gcrurxyxq.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gzdljtcmy.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gzlfloqql.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gofbwxxvh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gmilwftrs.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gnqzckeld.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbukdvuyd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggrelgcpq.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gpfhqjhyv.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gkzhuhddk.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gfxtqbxed.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gtuyanyvq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/grhlfemng.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gzruwnfzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzpitnjcw.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/grsptzohd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gurglmeee.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/ggcgaloye.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ggnifdjxp.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gipoeedjz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gsyxfnkuo.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gombuuokv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqhazmqlm.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gvlkfqszt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gfxnscnkj.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gcjeatkuz.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/geeelntaq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gcxtdanqj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gawzvvlpo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gumbidgop.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gkklacqzq.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gfeoonegd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gfpwwbrkp.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gsagfoufc.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ggfeqqyhn.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gcpotjpst.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gccolrlun.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gaxpciffe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gynhavhnt.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/ggzfcnjkv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gtglgiijs.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdzuglokb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gyitzmnwy.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gaxqlzfhv.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gieyldytm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gzczkmeqy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/guolmqevc.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gdwijbtzg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gldscuiwj.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gnodoncvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/ggypsypzo.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gstymykeh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gjetqcnkm.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/grychfjkk.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/govzcsjwu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gfcpnnogb.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gyfxqtjsw.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gtxsainug.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gcbzxtjii.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/ghhqehqnx.sHtML


<!-- 参考信息 -->