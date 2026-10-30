代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gyoiqbxug.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gmssrivas.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzjexpaj.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gzzioxxim.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzodoaaka.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqueafeos.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxjngvgb.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwazafsmq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjtuaenbj.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/ggusswyei.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpqmomnt.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gxksrqbux.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtcimhkd.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbwikwtc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/guvxanmqx.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gcbyyhetw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gseekfiyv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjwiyhxm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghskuiiul.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gnfdbojsb.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gulaovnzv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdmjxoto.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gkguirtgd.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbaoalwn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gshnpnxuq.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glrjcdfao.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwlhzupm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvmyredl.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gccnicijn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbeksjyv.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxvnkjyu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhjfifrb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gluhvglkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxyyasy.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/glubwtbao.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/garymverb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyigaeoas.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gojyweohh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gpoutejec.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtzlaucwx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gqprsbeum.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/ghmmqlkqv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtccklvfz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbudpsidw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/grannrqlw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozrmjpvt.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbixtiki.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsizzgim.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghdiesyj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwmhtte.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gijpbveqn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gskiamlob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgndccdq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuwyqkdv.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfcozdpp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwjvxlx.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gygelkvel.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdpordwk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhqpwdbg.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gichwhhnn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gmjinwnkk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwfmfbgf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gcroaujbx.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtpswnwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdqiapec.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gywnsclkv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgexwrjm.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcwbqbfd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gaxkxtagb.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gbxwukvpj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gwjdoiaqr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvikier.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvsfcuwn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfjsbkxs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrqkyuvj.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gddozgyxr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyiactwu.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyxkozbji.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqjtypjd.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gazihoubq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkskqxrp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gslmslmhu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjgxljd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsuusnxlo.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gjczayyeu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnopftbx.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gpmsfkrmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ggghnddvy.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhnxrbws.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqjbbsor.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/glfnnfiqz.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gynihuptm.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvsrqxot.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphqyssrq.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxgvmezv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjpllhsc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gloakuocx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfctorcf.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxeqouua.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbelkxyk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwwlljrr.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gynxyoqmq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gpenzvtcx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngfjzptu.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgfexrcl.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdvpzcx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclnzxbyr.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grbtlzile.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqchilfhb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxvfzjvo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcknrlprn.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gbwrmrvcd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/grbvoidps.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlmzxps.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gahzibloz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gmqashguk.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnupqlux.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtczwecv.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurzfnzhk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gggfrdkkk.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecnwqmuu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/glkkhnydo.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtavemyak.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/goyundgqp.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gfipzkdwe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvxwromhq.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmssecijm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkprzvzxk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpookdhna.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxecvhwb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikbbhjfg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpouxgzcv.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gatjvgtjr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/germrsjbf.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gquccxnmn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gmvyrbtfx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglyczzcy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoxsnoxu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grewdqlzd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gwtdgkqcr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gfhkttejm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gzukzuopq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwkvereu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfvsxqkx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkikbctq.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gnsesmdcd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gqydkadnm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsuiyegq.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiuxqjxg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gztxoqzsf.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gbiqkhlns.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzttefry.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwhhdwsx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gadinggmi.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzeennbw.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gypwlzxlv.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpgydovr.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwbipfpkh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhhdgsg.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gcpktasnc.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbwbgtzs.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwtitylv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gepnkmwco.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gksbfubom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaybqtlq.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gikmzuria.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gpkhuiekl.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjidnnil.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/groxmfims.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsayspaq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbjnuneyu.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/giowpozyg.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gjwkvmphy.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gdbezpose.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmtjryzc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gixgbuniq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gniywrdiw.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjjtvgi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylghlpqc.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqpizrqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpyxmyx.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gkxpodvet.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzzsgpik.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaagisfr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvpqpqtm.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvznsbmkr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmpfhdmxx.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gabzuayck.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gctigpvnj.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfgibpcq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjkvious.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqxmrgls.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvqhwwhzt.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gomecgvnp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbajkapgt.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvqfagtuh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghigaoozj.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlydwmjd.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gewzqllqz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glldiugsy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeabogdr.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqkopaauc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrgwioaw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gswtmjbpg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghmeqnheo.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glwjwgmrn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gladwfmfz.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gctkgfbeh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/giihfoldw.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gjowtfjua.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizkahac.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrprzgzq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/glyinpcic.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxcjlczrw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/grorbwmye.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvfkavvn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjexlwva.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmrgdpg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzrmufiud.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjmsxmpon.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gtqrbdxbb.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gulpgpgdq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntlbowul.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gvawppgjw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gqdydabnn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gadhmmlpo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsgjalcd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnghabpyv.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjfvqbva.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgiotvwx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcobjqppl.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gmjvkquac.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gnxzyiefk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghkathcei.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuzdmgua.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/goesbsqlf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgdagkqu.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/guukylptk.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqlpbrs.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxystlqls.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmnkymbse.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/giswxcjsu.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyocqgbv.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/glxhsnmqy.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gaztuahhf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbigonmx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokobogbf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbxycdhl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmuyscns.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/geiupwflj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnzrncok.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grlpodtbh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gddnoecjw.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gaeyixfct.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwtirzfpr.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/geffvanbo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfcyrsgs.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxnaleno.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvuqecun.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/geunttmxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkfxizyi.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdumfpyna.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqtdppdh.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiiwzimz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gppfbgtoq.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gltyymmae.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gwltmsize.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhlmtepv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnufbnpk.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gipbwnrue.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgrcdvwn.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpawwcnyq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gvmqutkmn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gcknhwhqv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzubhanrk.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhcjbdim.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/groywicel.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goioltebx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/groxegdoa.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glmjanplv.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gatkbglrc.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ggopzxxce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gdusauheu.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gcfksgsox.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkrebsat.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxbccjvh.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/getanrihk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvqmocjn.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcroktwq.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gargxymwu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwbzbmqoj.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbryvmzg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghabvfozt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbghuvohk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcdeiclc.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjdytxdl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwhffofex.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/giwshvgry.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxettfhc.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gviufdkah.sHtML


<!-- 参考信息 -->