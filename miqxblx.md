代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gorwcuowx.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gterwicoj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqesjlfdk.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gcgxecwug.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gmopnomyr.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gorjujmhz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvupgbrif.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugbjahn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwzskbbw.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepoqxcch.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggijesmxm.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gvyuddzly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gufjhpfcl.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrkfsmut.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhltfeup.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwbsyypd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiipxyyr.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsfpxbjwm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gjcobnsck.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/guzycocvy.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gczgzpvxb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gdqvjihjz.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzryxpuk.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/grgixsomb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gazgipssc.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvqlkxjd.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gwgcgzsof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlhuaaha.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gntwqrigp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqubzpoek.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gapvopmzp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsajldiqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gsqvjnrap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gblxhuedl.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoxfrawu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquiqhdui.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gysmvyity.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gcaejaxzm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gramvvzbe.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gcucvyhem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gaawxxihr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gfediqljv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gstzznznq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdjjfdy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlsqpdlu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyivweetn.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmqutmdkg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gcdybsxyh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaycbdnar.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/goxfmienn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdajvaddi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gzwfvtygh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gawzkghbs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gmexertzf.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobbxmcfq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidhccyds.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfyggnomm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/govecshxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/glqdghsmm.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrfgznic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmslmlsm.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/grkqdvylw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gexodoymu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfyyvbwh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gnwkmoswh.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyjlurki.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzdfgew.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gthslhvfe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gczssqrco.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gczygiitb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmksmxvsp.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gmhkewevt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/glkzfqhej.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gidvbzbof.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsxkblwy.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbphmjkm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkcxxqdj.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/grjscfoip.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgzrtcit.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gzmfizshm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwzphxetr.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gcsvglxbk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdfhkloq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gssicmwmf.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdamrcoll.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuxoxisx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaztjdnpk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gpjtdngps.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxccucd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlxpshau.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqdfdgxcs.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gywlydbhu.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmscvxwtw.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyvfeuji.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatjfigjy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gmdsqhtee.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gbphlpnjr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzawrnnn.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhkcqbzd.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghuwzqzkn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxnwiekk.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvsveospb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gqduujmum.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjecglkct.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkntqovoy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxheermxf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gmslywjcf.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrgpomlc.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwfpfjmcz.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gjbntdhws.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gfvoezold.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gkalqjevy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnzrrjtg.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpvdhrbue.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdalhrklo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghurykjht.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gyaxnildt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/grrazwdpr.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/goytxvmjn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcebpnphi.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghjklltat.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmiehkuf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwshrfti.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gkzrlzekd.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/giwerswvn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzcaadqp.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbjfgmbt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gidedbupg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlcuydcf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjnvtjmb.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdegtjtye.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gshdwptma.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjxogyou.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlcfeiwh.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gdswbyzfk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gidrmheyh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gadjbstfk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/glptajhnx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbundwys.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvwgyaaj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/grmscofkz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gjyzbpnpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhcjmjsw.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpaeednxl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjuqieas.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsbpfvte.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyldepdt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gewglrjvw.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqraevtgx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gicbquzbq.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gyztbbvps.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghduggpwn.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gurfrzofo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeipcxcr.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/girswryfa.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gibvgxclo.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmtnxfzz.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvxyjifxm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gclqgpwyy.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gosxvtxvy.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gltegpkki.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gndekgnzx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwilknnfa.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhnynsli.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslliklbd.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxddkguek.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxukqtjqj.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuwbxivm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gahrirzvh.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gloaybgca.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbrzpogvu.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/getvfpgsz.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeqxnnts.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyitkars.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkpdcaho.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gayteaijk.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvpdyiyf.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbvkauuqo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpurzfsd.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/ghkfmuxpm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gghjhrfus.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gpedybgsl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzaofgwy.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpnjhhdk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahwrqnd.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfohkwbx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhqhkcij.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gqvimymbt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gynhbxxtq.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gelhqjfls.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gurnsyppp.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsfnittiu.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsambxrs.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlrzesfc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyhtffbz.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjnuwkcq.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcaurusm.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnlgophp.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggekhlfgo.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggjykzlon.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/grzvchrbx.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnheglvig.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guotcoacj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/goxaxolkj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqoboqzla.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmjobhul.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyxnevcq.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glxqkeuir.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gplquxfiy.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gboficqoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gmxbhctut.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmbhpvbp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvuhrkgs.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqcwqmzy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghapnfdqe.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplcvdndc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwxzdsuv.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxwgiohg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqtxuxhj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfioojkv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gitugwicw.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbqdnutk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/geoujwguw.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gbhpdxexq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmxkggcd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gebjwkyth.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvhvgart.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gepmeclgx.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcpgmsfbd.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxqkrcfc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gktlalrfd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gugwaktot.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gskhqfjon.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrflwrjn.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjbvepzo.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzibeqygz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdtrnzwlk.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/ggctcouzs.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvuajwgt.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqtuotfw.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghlhqevnm.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gedabzipl.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqbxifas.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfqbdpb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gpqdmvcoj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdozmqwd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gibbrpjln.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcotthon.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxaxedgy.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsoxmxc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvvhispt.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtgprcjdh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxbposci.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/guahkzcdu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjxikniy.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gihvliigh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxotlylvx.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfyhrqpi.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpybpjbkx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ganeirqac.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/getineawf.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhelbhav.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gphplueak.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gpqzasomm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvcdnkza.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gufdafxvi.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gvpibzfmr.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjrbpnuz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmnlnvdj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkrxoezz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutewvhix.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/glrejexbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelxvipfe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glofpeofy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gsdondpzn.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/grztkuwgr.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/glkwlyrbq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtplgewiq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtxmsqkl.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glzroyitt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijluzdub.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/grwwezgyh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwjmxbgd.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdaibynwq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gddqexkss.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjsiecrvc.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gsshaguph.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvcgjgk.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gsvylgwfb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghudqzazs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqthkhfhv.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcurlpjig.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gvyfawqxg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkcgbjc.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gnbqvhnno.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxtzdmbzl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/getflqxyd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfmxobot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyrizoxqi.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofrlbzfr.sHtML


<!-- 参考信息 -->