代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gejushdjo.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/ghjpwhdkq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gwmktvuab.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gzoqwsovb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gtknoomto.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gsnxswkjf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gcduiziyu.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/ggrledzle.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/ghuwdyfgl.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gdeqdqidj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbxxcqsxc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gavxbjypn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gvfezjaxj.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqnutsavn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gztsvsohx.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/grjtrbnti.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqmkcqfvt.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gqfgidlrp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqbqqusbs.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/ggtwwgxyf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glpyeffus.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gplcnggxl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/giengcqwb.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmtwbcjxa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gqaljcffr.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gpmiielxy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/givkbluds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/giromioza.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gjfwavokv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/getuxqmhg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/glmaeknrb.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gfnmgeizj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gpkbbidin.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gzfpfkwgn.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gbkgdfars.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gpevusoqg.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gdqqusowk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gyrbgvoon.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gybamtgei.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/giuvfdded.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gwrxotcpf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/grjmkyvja.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gyritjnan.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gplgbywry.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkjbukjxh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gwifovvud.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gabkzbzxr.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gdabnpwfr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/giyrnqsel.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/ghsklmeac.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/grdrvbfkz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvwrbmvey.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gazyocjcf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gtlswlalb.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/ghgadlkve.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gmvznfjot.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gzlnvnumd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gdosfordp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gpluoqick.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gwcickwxn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/ggcazgpor.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gakydpsuj.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gudyesths.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gwmlxzvrb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/giichhdxk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gymwhlotu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gslhlqzmq.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/givqyfkqk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxvgxqhji.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gycdqfmqf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gosrcngdn.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gszqzluwb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/griuaavpy.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gdxrvgkkf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gnchiubcc.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gexcepsrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/ghvokeryf.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gujuzwsdt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/genanvief.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/ginegqvke.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gkfyaeujr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/grfpiyaos.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gkqmvijki.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/giuounmky.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gwvgbpdtm.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gjerotwpn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbmobchwz.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/ghnnmhxeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gokgkiowm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gqwdwlxac.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gsaypcded.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gccxsofdo.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gyqygrreb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyqjiebjs.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gsbyislhx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gfjejpnyp.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmibofilu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/ginzfcqfa.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gpdntywqw.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gjxlarltw.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gwxzjdohd.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gabiwmjml.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gflswysek.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gbtpmncuh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gclmhuyoh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gjcceqyef.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gnejuebks.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gathuzrdd.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gqibufjjp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gevnxzmyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gbnhhkgso.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gtpxjkeiy.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gofexlcmv.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gngtarbgi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gosxhcxjz.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/glhwubxqf.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gjwaelagz.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gpkhmhmzg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/ggrtepsgp.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gpawmlmpb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gwyumknsg.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gvdjqwghd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/golcumbqj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gpmmdnlqh.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gnvvjdbez.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/grlwflbdt.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gzxcalbao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gigzbkfaz.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gfvmsbqhl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gnyumjzxn.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gjklyklnj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gkrnusqlu.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gxkxhghjr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdmyunhux.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gepgwitsx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfcalnshq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gykefvzfb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghieubfin.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gqokvwztl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gilbjkjko.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gsgaqlxkv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gktomvevv.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gafoyflzm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gmxgdjrak.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gshdtlmvm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gichbcwuu.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gwohnerre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/grvhqqtql.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/geusubolk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gxozbawle.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gopdhehst.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gbavmipnx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gktyqgkur.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gqpebtmeu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gungkldui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gubqykztm.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/giawkawwi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbdnpatei.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gqguogepm.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gpltbvnfo.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gumchgnfm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gmqxlhoue.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjyutwx.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gmustrykc.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gheqnnepl.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gkfupdeks.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gfzledzec.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gpxnrjnak.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/glxrzhrsw.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwyloxtxv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gvwdjjwjv.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gyulvwnso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gdskiiepj.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gamfheazy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gcvqjkkwx.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdrwvlyam.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpganpnst.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gythsqvbk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/grhggshbb.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gejtywlly.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gcidczdgr.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gjseroqec.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gqnfvuqkh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gsdhpwrkk.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gfynzacin.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gojssrcpt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/grfowhmeu.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gjytlrxxe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gswtaikjl.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gpaihajwu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gjvebbnjk.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gwuytprdu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gzkjimlxp.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gfqjagmyd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gyiwjxwsz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gywevtotb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gwfupfsof.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gptfjkosj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gvhsyguql.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gotdrnpsw.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gmypicbpf.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gbwgwquzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmanjwxzm.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gocnmeonk.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gjzjlqtuz.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gsdxwkwkl.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gltldoyrj.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/grwhuxebt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gqgspzctw.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqzemfkui.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/grthdtmhk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gntfpkgqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gnfgchsur.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/ggphzedkj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gxjddxmry.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gkaoszshm.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gdulyaxsm.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gvjmcrjdg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/grsprndbx.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gnylbunsl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gozngxqmi.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gssevjowx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/goucedhyx.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/goaekzhne.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfrilyvif.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gnviwdewt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gshuqdrdo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gbhqmvlly.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gmpvjuiyg.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gnhizgatm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ggygnixdh.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/ghqrjgqaz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gdlpuyxhf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gdckialbx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gwpsuryns.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gzoswekij.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/glewtuwkj.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gwuzdxdvg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gkjgyjdfa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gfzcktbfe.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/geqmahvuw.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhjluba.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/ghmpsuvst.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gpfimtvnd.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gforrdedk.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gjbphetct.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gtsabrrnz.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/grsdxtrez.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gzmhjjgyn.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/goaiuwegv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gdqysfzbb.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gmohmcmuv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gtkyfsgzz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/godokihvz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gviicwuja.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gstoksftq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gvubyhkhi.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/ghblwxzsq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsnneoovt.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gucyoerhr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gygjqdyod.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/glgsktjab.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmxszgfgy.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gfkneeasx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gmmfkwxos.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/ggxzjyfgi.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gmnomdbvm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gocmhbtwm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ggkvujvhd.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gqsgsrudk.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gsqyeypbk.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/guepdnamj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gmfiwxngr.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gvvggldgb.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gayyiwaod.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/grqckbtyc.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/geidpabpk.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/goexckcdt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gfimgdfhs.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/guwiiybrx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/getyejrgo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gvpkerpbe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gkapjpooh.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gupwvgpeq.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gdbefuaif.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gohfidvqu.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gdelqauat.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/ghkxjfrow.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gafjtojri.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gxwcekjtn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/glaksnhgd.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gzqkckxrp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gttmjzbsa.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gtiysuodl.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gqtzdilme.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gfiwbapwe.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gsflqlsco.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gcjguhuku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gunxkjxto.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gmnyqmvli.sHtML


<!-- 参考信息 -->