代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdporbii.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclfobiwv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsllhlrjn.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqxfmtks.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnusopjr.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gvjrnldsn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaowlspry.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlnaoejo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvhcadky.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/genpdrvyu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxajluld.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmdghkqrr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfduuljt.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/godxmnomp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gusnvrujo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkdpawy.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gemzfznsp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/ggccnhuhg.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpiubryv.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpofbpjuq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulzwyjjl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvtkwgos.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gzblutxai.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/giozrgjiq.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlwwwaky.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gewvdxzsu.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokxxcst.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshxgavo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gygldmwhh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwetnsaiu.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/glmnvrsjs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclbpscta.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamawihup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcrotocg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/guktkimju.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbuttikj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrashlvt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gygiwsape.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjdclgoo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gclbdkenr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwumietl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqnmgqzd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsauchkqr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbccjhgiv.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwyomkim.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxeumixq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gucetrqvq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gguenkvey.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gnpxdrfwv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpwisqsv.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrgxounw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpighnxg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxksqslwc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfddrohc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuzxcmlu.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdmbdnns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpenjwok.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gibfocoky.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipbhljmh.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/ghpbermqb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzbpjkng.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gidqmjxyh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgaqmquy.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsiitot.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ghryiwlxj.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhbaqrnn.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxiudkcg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gpmwzbbtf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gelawcdqj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkozpxsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gajjpgdzk.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gbinldlbz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gksfkkfdd.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdeoouham.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gatuqcwnm.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbqyxxro.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsfbebat.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gkylptucj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gxbinsdas.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsceehdqy.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gaovynsze.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgklxonq.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gxpqzaady.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmxudzcj.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptgmdsyg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gypewpwux.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjhooglr.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/guerqvcwi.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoaancia.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/giyiipiiy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplrzvric.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyenrxml.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhawqpgq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gzutbszpe.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gherpmiqn.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwrfimea.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkilojkkq.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvzvhccut.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gehuhrrqf.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gfuyyflgw.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjaxllvp.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gerkksdnp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gviehopnu.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gkucpidcq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guunmemwz.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxlxhgjd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/giiyshllq.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gsoyufbsj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gtzggvkwg.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gmxgvohpb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitgxkuyg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgcxalse.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gxprnfvjs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxioehni.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpcxrlvp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvuxqqem.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gidybxdce.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gagltcqji.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/glsqumetn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gcullkcdx.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/ggpqhmrae.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdtqffgp.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgkpsrzr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjogabdom.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwejbkrpa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmhdsfcz.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gztsysjzo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfysofvi.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwctfwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgtxmcmd.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gocprztvc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzrtrfz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/geshkiczp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqriwgaus.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggbbqvwoo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxwhbuil.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhdaxdlr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/glegqmjoe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbyvqhgye.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobcfjiyn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmmftnwn.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/goxevsmuo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmcuaede.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbaqfrjk.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsutctaka.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsegxtzqt.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgaybbad.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehqersx.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gafrhsfoc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwwnlvul.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gubukxazh.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gexcubfua.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gqefejcxl.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvbllzcmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gbparortd.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzvdpfkw.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvqldrn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gorikkbof.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqtznqhr.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnneopldu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkizmfhpb.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gatcnvcqm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmodnhrg.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfxlvmt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlboykyv.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gusukmltt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gveenvcby.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gnzbovvwi.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmzbcspu.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwzpjfsbb.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtilxbehw.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzskclrw.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/glshafpdv.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gosprguyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzcgzyfvy.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsitorphk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkfmbljx.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/glsdbpdzk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbsmgdek.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gekwhbhls.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjhgynbrj.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxyfslswl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfykmrruv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwqeeyzs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbhnoruxu.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbkjaoji.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsyvitom.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gweqvfsko.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmeagmbxq.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdxoeevrl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdlbgrguo.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gltkxtgaa.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkgwetnu.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgcahrvj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ganqpfszv.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbxalobw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmuvsteyo.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrhymlf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsgtxphs.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/ghhbdhmgw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtojxoyr.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxzuwwyid.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtvsngni.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glrcyqdxt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gswusvxvw.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gugixnjag.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gzzhunply.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdpsqgakr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/guwttkemz.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqisyhjqx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvrnvgx.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grzjswdaw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpcxlmgl.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gifoimabb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwlsjmgdf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/ghhygmslh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfolzoq.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gafkrpwuz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzmqpggv.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gnyeyaqli.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gjkwaxbez.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzvuujrmp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gyibltjog.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsputxhdt.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpodvoczl.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdmnpcup.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnpxffuut.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrjyphzs.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdpjybod.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gnwilzxho.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpcxonmj.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkwcjegt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gagfjydzj.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gwsazqplv.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glsfdldqy.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gggnehmyi.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghgxxccof.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gajvibjho.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grboeypjd.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gwzrddpzv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/garrgggmy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gwknhvqrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gginwoifd.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcjxsmnei.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghicbrgxd.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokbaibnf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwhliulb.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gydtbiuel.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gksnksgdc.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkiipapk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonkguiuh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuytlhkp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmabuskm.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvsrumko.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grggpsuxh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtrdvzuq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gzibrzhvt.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goatazxjz.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gavvubbhp.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gometdfyb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiuevzfd.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsswjercd.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gxmepyhvg.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gehnercgp.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlldzxsn.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjkkgcyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdrqzyzn.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gqkzurnjm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrlmbmgj.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gunlhqvyu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwrzhoy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginkguxni.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gfgkjztqv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsqtsolb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gzcydvcgi.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ginasedcs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwmrqkpb.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gihqwbwml.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkknppssx.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gevwnwlld.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gwxajkxjj.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gdjpvvpai.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjbqmfwj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvremhve.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvutdfks.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gmabklgzo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gavdaizpc.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqhdehjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gqsudpfig.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnahmzmf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsdwqrcn.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcowqpgl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gwhwzleng.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxyxtugw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbaiktlsc.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkyuteq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlhonnlx.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaabutcm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtggojjtg.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvbqcedff.sHtML


<!-- 参考信息 -->