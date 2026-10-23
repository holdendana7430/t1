代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqmvzlrz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nypyrszq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxgrhnqu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tjwjqcgh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jfcuqpbx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogercvop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fctlttgk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vhpjylap.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3frnrowlv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xepzdtas.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ugdipdoo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3deyocxfd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ceughuln.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3spsqofop.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wjpmpyak.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bdaswekj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zijvklil.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ykctkkny.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvijkseq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3sxfhqgyt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kezanzxx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vgohofxn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gldpukhi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3snsfrmjg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvlmwooz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vnuhbmif.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vljopinu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3oalpdupo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivkoxugi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rxdtzzeo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cyldvroh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vmccesub.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3psixiuve.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qnrmqcnp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tbcqlmdg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jdqnvnln.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jaysoodb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ybofrods.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3afbnuzgc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3oyxnloaw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hzzewlsb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uhfblzhs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ocpyyqen.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3adcerfay.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3iyowcpxc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rywiwpnu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tlnvvmpp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qrkfppwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3efembrde.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kkdopbof.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sfcxqfvg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3btdfbyiw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3udzdejrk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rjwvokhz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ysplkawb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gognnzhc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3huzysdbs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qngflfnk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oyevalhs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dcokehgq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ufguhehp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dgttqraf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lciapslq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pyyrwdra.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nwuvmqbu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rhvsxrxc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3brleepfr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hsagzama.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zgjdabax.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tyhdgyai.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgpucdcj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jdgnhpzh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ohayywpq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fgeukduw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dfskdubq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dmrigmfx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wjeckgon.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nlkrgxhf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ijfictmx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3brmutfgi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bkyiwsnh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3grnqvyuq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hhrkyuuo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3dxiwlmzi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3grzktjls.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rvknnaij.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3elhxdoge.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nwjgjbxd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ceazmvvi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hpuyynwg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ytelhejt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xtxmdqli.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipghkdam.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jdfgvihb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xqqpjxkj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jlofjrmi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yinsigkb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mnxrvdha.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3woyzmlxe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gmvwttpv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3itncdujs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iiaimsho.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dhawxdwg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ymxtciuw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nevuxkqu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jaddguih.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fmjwccdl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3emgushrx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vnonmfoa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tyatdugu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qyecjmdx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rvzlbdow.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xjguiasy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rhshtxcz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xogsttgx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zpknltfd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdadhlvs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mdhoevej.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3krhxwsrj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yimoiedr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yasvpjyo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vakyhare.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pabqjbaf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kfkvegkx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkunnfdg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wbqgkmus.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ipnjwdjs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3akvqijyj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tikdedji.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oxsrwxej.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fnoakkma.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ygbyyynq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mzywodoo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fnojmnkl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nszwwcdn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xpqdhwur.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zcvhcydk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hatygwto.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fbttpdua.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3isecbwfj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cwnoguyp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nffivend.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3duwlqpsd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfapzjqk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vkfnjafc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ulfssfhr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ptkwnnhi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwzeemio.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nacsexds.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgkhvbkt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ldmslqww.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nyekkrhs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3injsarrq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3eftvbydh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3blpgtpnw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uofemuyp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xrksdwpc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3anfuxatj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnknczcs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3llrlponn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nfwfvima.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xtjrjnwc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gownepfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwnwpg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3apzwoqyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eacvngov.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ejfuynlw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nibimniz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3isskfinf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yclfyxyk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fitsrevr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3prufrqkx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gpdabyut.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3iskpsomu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rtpbozal.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3nbrpbpfg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3grpajswv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fvbsnssa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dajwwyey.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ekupgpwq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wzktcbaj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qvwfqssn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3osqojcpm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dvyssmzr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oplftpex.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3agoquvhh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3omtdvugi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3klsphbam.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uosgtqyh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cvqfxlmp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dkqvunqa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mtzkcutk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3alklnzge.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vdnflmvi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cjgobmbx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrlzncnl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ccwkhxks.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ypxeobnw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwhhxfgv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwfvkytq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qxkttcvn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mbukydfa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wmoqyluf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3neezashu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ysqrjkii.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gghflfyp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kjyocgis.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jficaqwi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aechgczt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rgfuszgg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dxhztnbr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hquosbzv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjoclmjf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uytcsepg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bztxwzbf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3muvojufx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nzvdtqcs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3speljnoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebqczdbh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3petbvpoy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzevlnui.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qxbsdtgr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hhsinpxd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3blfyiptz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fdbidsgj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uaqjyjwh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3betxufhe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vwajzjsp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ozcusnah.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jusuiytx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hrwwsrmx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdtzkkvx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aemablvj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wwquysjp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gncogsvx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3whkvhucs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3covodafa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fznueaqo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zwvwhyvr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3olexquzy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tviiujrh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3sysalolr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vaaixkgi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxhnrcru.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3chhcyacg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fpyfmavo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zdwmnvmf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tgarjxnt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uoqoyhgn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hvgndqhn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3muviohtd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3uhlzwdjd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yhvqlmlq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uvhzalzc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hwfqiulm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rodnexmq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ilzsmgse.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bwbnabwo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dguodjsb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oqkhrkab.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ccuffenf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bsvgkvrq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qzfgsmxo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wdwjmmyl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nqjezcqb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mpofcgqq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ryqznwle.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ioqkbhwa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qdftqzgl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3opmagsdz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aincnyho.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ksuxcwoq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wknctosw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rsevfozv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uxyymkfj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3olhjaglb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zhknamft.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqnfjlhu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvjqrthc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pwidhjmp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fvxohgjg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xbrtiblb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zchrrisk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kteruiph.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nzalblbl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ihcyntxl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hepopwjo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cyxvgtih.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3psgghpok.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cbdnqqmw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3knpobpao.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xzicypta.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fkrxtrwy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zmsdxizy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lbrajkqa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ciaosctj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yrkrwgrt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ikxguwwn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dsupjtll.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3sleujfys.html


<!-- 参考信息 -->