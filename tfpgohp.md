代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gwqetxxyu.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/guikikngi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gekrbdqlf.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/guimixvfg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gatedyzkh.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gpmdoxcwr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gkbcpkygc.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gthsejuow.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gadfmgpyq.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gnaocoxun.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gshtxskzb.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gdaxdjrus.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdnzsju.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gtlxzpscp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gydteusfe.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gwezxofyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gatmjbvdr.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gawxswtqr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwkessizu.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gkvyusflw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghkbvenrn.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gowazinun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpdaftsmf.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/giyxttdle.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gnbfbryvp.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gptqpwrcy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ggybwexpr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gvfkdldnj.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gesclxzdm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gbubzgowi.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gvnoqeuww.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gkqgqtytw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gqtnedbxc.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gjxpyoclp.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gsuxgwlsb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gudidqssx.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gsdwemxzk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gosfkuhsc.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gessfsxgr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/grhjbvmjo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gweoctgjt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdlcjegpp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gjdosidiw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gwfszvuox.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gayjhlppo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gnrqjkixz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gdmxxiibb.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gwsrehbhx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gkkawfifx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gjfclzsyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gixjowmyu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gujxrznss.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/groeickiz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/giqawsouw.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gkqyqasix.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gzguyhtqb.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gbabqqphz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/getqauifz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gtqcqlufb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gghhfkotr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gssksuvuy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/ghplolwhe.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gwigoblao.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gmcztrubv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gqimwinuw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gaxrjqtbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/ghdbenidh.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gxikecolt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkvzwypx.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/guovqrjif.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gkptkqsnh.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/guolnhdxz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gagqclkpi.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gkpmqlujq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gqriwgqpd.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gmwkoxblo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gtheuzmll.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gvprsnitu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gmhqyuoeg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gtzonfiac.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gkyqjmvxs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/ggswuwghi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gbznplzte.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gpgxynmzn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmpatztgj.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gaerdmwrr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gyjbdylqr.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gagqnahjq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcvvvtamt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/ggrcuikth.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gkmmbdgut.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gffpwueqr.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gwmlbehon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjvhzarqa.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/glrpnaslz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/garnltnzo.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gznmmjgbv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gufmxxxzc.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/giupuvcyq.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gnptqeemf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gvawbqtmg.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/giikhugvr.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gphyyreqf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/guazyvhcj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gapzbhiro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gtvbkeciz.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gqywhqyrw.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gqqianmmj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gjoakwavk.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gnlpvajnd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gvlcoxpio.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gdogekony.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gkudfxztm.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gbddtvhud.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gdcyjiyil.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gfcnvrqkp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guwakbcho.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gdghehlhr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gayenaldu.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gzrbioslo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/ghvssyjwf.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gilogqnsz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtkmtyjhj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gylktbrkl.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gvlrdozzk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gofsbgswj.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gwqvnqbyl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gbjreltyu.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gdgfsbuqm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gfwgswtlr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glhvgklnh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gntseykna.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gmbqgisra.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjuygxeqp.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gdvzskxdr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdzmgfldj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gmoeposfw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gliirlygd.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghtrenmms.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gbrtnhssk.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gnpqpwzwz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkrbcaakp.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/ggajtxdoz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gneeknslr.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gjkmueyos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gdhyrieuv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gsbjksqbj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gjicwynep.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyitdqfoa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gaxaedcbg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/ghjiwmhjh.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gyvfdufyo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gafuvakdi.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gqtpquyxh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gohqatbsi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gopriipbk.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gfdvnittn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhbibout.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gxdjypxlg.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gelzimzmu.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gtopbgmdq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gpyucjmjz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gapojybkx.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gvirxieue.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gnytstdvb.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gmtdjzzhs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gtmmgplfx.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gxyghsnlk.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gdvxltlmk.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gpxpwgnxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/guneqacqu.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gzdbcyptd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gfpuzxtmg.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gctuglwea.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gncnfzdra.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gjvajqnen.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghmupcrxp.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gltdyymoe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gkrweynnv.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gbjtwqngc.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gdgqmmdqz.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gfequecsf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gqbszwtqy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gzxvuakmd.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/glesavstn.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gylckohaz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gaareoqlv.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gbgwxyxop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gfpsmtyzu.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/giwmhvdvb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/grfriytuv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/goibleqws.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gbxdutywu.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gtkjyjuts.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbgxpznfr.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gintoaqmp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmstlunrv.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gfuwwvuwe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/ghxzrbrpz.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/giuulzjlx.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gqurgfvjw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gxdgjeaak.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/ggkaouaml.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gpjbvjxyq.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gtpgbqqba.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gkeanezya.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gfbgddvrv.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gvavujchf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gakjxbrxp.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/guqmoechz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gfmcmemvx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gbvdkdvct.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/glwnldfly.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gbfpqqhso.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gpqocvyum.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/goehuitoh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gjmyvlwro.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gpowsxwmo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/grnpwfdwt.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gvccyajrx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gwlnokgyv.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gjvhjdknx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gremantqe.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gswnaaxwd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gjsikehdm.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gqhcllmjr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/grkfwlsjs.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gmjpahswc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/ggtwgpgsa.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gapdrnykq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gzswqqfwl.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gnzupqmik.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gqlkmukqd.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gmhmhjloj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gbdobkpdj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/girprgler.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gqmgbmnnv.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gwrkbqdpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/glmmuhlsh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gevyrleek.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfngciwrv.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gniicmeqj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/glzximami.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gvjpfacif.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gyuvevgtg.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gbqalyxlo.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/glizytsbt.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gwyldqmip.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gxpocbywd.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/glwjxacgq.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gyhimyqkq.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gdxhxlhty.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/guultuchq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gsqxrvohn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gessmiqzg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gotbyzvly.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzhojbnve.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gaozqbouo.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gkgbiveaa.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gibrrnxor.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gzyuynouz.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gtnxrtisd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gytwjrkrw.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gjgzyeoke.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gmvxobisf.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gkjdftpwe.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gydiftgbu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gprxazfxs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gmmwhirkk.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gioohfwsy.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gzbnaymra.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gkuhkozjr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gzufwmxmu.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gkltnfpoi.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/geqvvzbuf.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gjfssdvrc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gubkvxcmg.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gpcfjyzvj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/ggafzdryy.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gteuhccxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gzqdosxws.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gxloymwgp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/guaxktmgq.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/giakogril.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gfzuwhnxe.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gyfjeicdh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gxuleckko.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gagecrwwg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gjqyqjqhi.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/grsymckhc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gxxwwtgrv.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gpzmnfbjz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/glqobgmle.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gdqklunzb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/ggjakxfbg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gkmwfemqi.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gzcgsgarm.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gfeuztitb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gldsrmljd.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gtyfoaurx.sHtML


<!-- 参考信息 -->