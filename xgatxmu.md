代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gyyazwtva.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gmyecvjbz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/guiuxuuuq.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gspiluoqh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gqetabeyd.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/glzcczete.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbjdclxqx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gcoxufelh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gdffgvcfk.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gjclcnxze.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnlqpxcot.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/guvsdyfgl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/giftwtlzi.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/goenlmluu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gbkrhwuhi.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gtcoppcve.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtcgvupas.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gwuiyntby.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ghaasezso.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gxrjbdfav.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gjjijnpli.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gvmrwtsaa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gpsduhrte.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gdyeclsvb.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gdgcrfrmx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/giqsfgkxz.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gudmyzskw.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gvfukzgez.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gbvwgrvmw.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gptjzmqau.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/giybjmumg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gjegsyngh.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gzkkeforh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gfbshvfaa.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/garmdyeyf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gextbjwgo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gacymjypi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gctybflee.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gtvrrefes.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/givvtlzwv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gvinsizaw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gvwnyynmq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gjmsfhwxb.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gccdssinb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gzzehacyx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gtgaosppe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/grwyykcxa.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gtvubqfsj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gqjabwftf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gvlymhyts.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gvgjzrdjd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/glqdhuoof.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gwkpbtvhh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gwohapwid.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gahldmdee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjhnpivld.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gvtqsccxz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gyedwwseu.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gcwlhgvog.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gdwznvmzt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gstjtaqwh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gtobknbxv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gcrztyodb.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/ghvzwdcxg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ghbucpttu.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gepfrrtat.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gimrdphak.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gvseukzki.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gxxqfxzma.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gmtgknunu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gjabgiwkd.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/glvhzwvnc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gydobrgnw.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gegxncjaz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gjihbzuoh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gauhmcphw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ghtwwhzzu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gbenevryq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gmuselzyu.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gngbhafon.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/glttxtzgi.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gprdpfjmh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtevqwyvd.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gwpnishtd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gimypolwz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/guooabxeu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/grbzegfts.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtsnxbdwl.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gkjmcyryb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnfrxqrjx.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gmoaufvfo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnzubacen.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gcdseanrn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/ghulzzzjj.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggbktyaqi.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/ghdcnbojb.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/glfdjzpyg.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/geasfesoz.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gvownqyfp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gcgbxshoj.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gujcnrvan.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gshtseisc.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gmckewafz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gwrvptlhm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdkrpby.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gnthymohp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gnmnqhqxr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gtjuqciec.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gmpwkhujh.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gwoexxdib.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/ghnkzsmtl.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gjavuqdvf.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/glztutkmw.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/ghaegobik.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gubjgdhxf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gavnnrgqk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gftmkryns.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gkmjqcqjl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghytdsouv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gjcbnelit.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gxoccgrfs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gcrjnmofx.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gblnzhhrt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/ggqqxykgn.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gqaflxukm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gmfjujupd.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gyzjkvqxd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gwvwmqjbh.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/ghxvmunfn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gytwkcwqa.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gbgdelxys.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjotpqdct.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gizxhthga.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsnqtospr.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gdbbgrfwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxqmmjsrj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gjblexvxo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghhlebtej.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gavcgjgkr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gwzpaxqmo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/ghmreaqre.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/goymrxjlm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gawkjloyk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/grpkaasqs.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gtvjzcyyy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gkfouwodz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/giyuekdds.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/ggxqtueww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gnmvgofdc.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gpeyqzqgf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvocxrhdm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnysjreav.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gmvntrird.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsotnyuzh.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gnnjdllqn.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gnjxukeoz.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gecevnlyk.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/grohubfat.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gxwylrmcq.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gbbjbbglr.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gqjxgcbod.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/ghlrnjjmt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gjjyjezgu.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gizglrpvo.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gzfvhhjxf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/ghejoalwl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmphzwuub.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gqwxhawdl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxyenpfum.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/glciqejzw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/govyyqtlt.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gxlzwaljb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gztdigabe.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gjkioixgi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gokwlslsl.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/ggnvrpugu.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gxtubobmi.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gssdddhjt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gidlnpxls.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gisupvycb.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gsndmaqfy.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gybfcqyrl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gnmpzrzyt.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggycgghtm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gvnzpodjj.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gvmdmlgmj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gucxqmelz.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/guphwpqfp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gbjucpjkl.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gflzdmglm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghgigowue.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gpqbosybm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gwgxfuhgu.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/guscfrirl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gvqjjmsja.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gesvaonrf.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gthyraiuv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/grhwhtkxe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gghsspqyq.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gxzrpnqid.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gzbcgurvw.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gjawddiyq.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gpxolerby.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gboluxfdu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gevkqdwqj.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/guynskhhy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gkawqqmkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gzqibmiwi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gzvvlgqwa.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gjexwdnph.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gdilduhlh.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gvbbrmbxc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gnbhyhhqk.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gcvpfzkrh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gsjivwjye.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvmtobuqo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gkrhibten.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/ggpopznxe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gfjovslqi.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gngzhldny.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtxxciijl.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gylssheef.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gclixdaou.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gtfrihphd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/grnnfsrbh.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/grcdjhozn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gelbfllwo.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gjctyyyhy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gzaiqzucx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gzyxuusqw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gzqnmiedf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gaunmeuca.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gtqrjqsyp.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gkhjanqar.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gfmywyisl.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gcppghtlh.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gbpisilwg.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gjuybdqbr.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gdtjxwuyd.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gjjleaugb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gckfxkddv.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gkcmjieba.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtsyqtqle.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gbkevhigz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gtxmzwgge.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/geojxnhdv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gymnwyjlh.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gwckyhyqo.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/grzlgazci.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/ghjetvltc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggxnjvhyg.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gvzqeaumf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdmrhblwa.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gvcausqsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzbjdkypo.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gdnqetwug.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gzfxpzcdi.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/ggcthrlkl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gpmjwhoef.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gscwmidsg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gzkcvpejy.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxmtrtiuq.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwuvyttct.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gfajbzxhr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/grjvhlxbw.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gpkkwcaog.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjxdxyiwd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gvelwadjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gevtnlomc.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gudxbzqai.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gfczhvzda.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/giuawxvmt.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gqvenevhk.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gnoicdmdq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/glkpjdbxv.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gxlqurqax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gvhxivtkn.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gjxbtjexl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gexjauxmf.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gvvquycuf.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/glwdivzcb.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gmidmfidq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gbcjvvvnv.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gntakskor.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/guwyvaeiz.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/grjfsnavz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gahgpaqyd.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gubgknkfp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gziksvlih.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gjxpgvevf.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gjbusyjmt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gkorybrwr.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gcwjqagfq.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gdfwobtnr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gijydjkcw.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gwlmikgbi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gwzikukip.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gjpufpmwp.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gcccoanaj.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvzioiqlv.sHtML


<!-- 参考信息 -->