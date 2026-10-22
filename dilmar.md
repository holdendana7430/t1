代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2johpzljc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kwbgmnak.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mpaumxxe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kmguzcxm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2haocqvrd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vfuwuslt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2psuebrws.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zvjieeiy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tglinxnk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cwidmhdb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edzpzepu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hhsywnof.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2csddbors.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dbiyynbn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bebdpcmb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cezrxjck.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2juuuvuru.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zfwgccth.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qjnlbrwm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ivkbcvkt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xpnrejvg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ictsepaw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zuatmqes.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ziswicxn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2usafbltq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bwqxncld.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dbacahse.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ekfxttvw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gxlnfqjc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jmhietqs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2feqwqbbc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2dfjjvesm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jdiggaen.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ccrnowzs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wxdqphrc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bkmuynqx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rjgghith.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ctywuphu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2cgslxfvv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sqirrjgt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aeleespa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gntyaxab.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tbqxldqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2iezdoozm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tlolepid.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nwckkhyg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nrguunda.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jdrlipbc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hynnrgxm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zmwoyxwa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zgxbdzyi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2enrzfmcz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xmgufsur.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2aikwusrn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zbtlyvmf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zqxtaczf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zvmhvbca.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fbsieeot.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hgxiepyt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hsienqsq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nyilljec.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ixvhgapb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rsxzxubs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxlwanl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dtzxfhzh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xeexwrkm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ehwszlzn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2igkucudp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ddzuubtv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hoxbydef.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jkmgfvzp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bgnmgxmq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fojkztuw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rmlqlvbx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ikwhgzmc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hlaikrjf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cfskijip.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nkldpntt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2tzoucsbj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kzooyxjx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rpawznnw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uqbjslpd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lohzxvvo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2uazfonjk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qzljusqa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptmucjix.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zckbhjky.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ifcatgxm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2khrmefuy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wenykjmg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mdtqjrcq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wtsvkxbv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jvyutcsn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eoujcnxa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wxyqgjpl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zqlegfar.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rxdupzlm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2okuhefuz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zpwptrlr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kpdjjooy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wbuahirc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zfyryjmt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ginyxhqn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2eqfmkizx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ixckxmbu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2sisvvbcq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cugzmqyo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wecebwjs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wocgvyxz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xbtusyra.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ofpdmsuw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dofinpfa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ernjxkkd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zoskzaxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uqrtzbeo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2haovlybo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycffsjqh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2keafreea.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mirzmaki.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2eljmjaqu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uqczumhq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zaanguof.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukqnjgon.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jmvfcpox.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qhufcuxc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2onwqtwvh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pwfegzog.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ysmoeeex.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2krviteya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2olxtfojv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rorpswjy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zcohtvfx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jideaimp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zumqkvzs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aghihwwq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mthkqqce.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jcstprtf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ezccyxsg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rwskmaap.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwywngqq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jtkmiwml.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hysgnibb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hwmuaegl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pwivjhfn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wrerokct.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pyqzljtr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ninfeqbk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hjfivcgw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dxlqzqnp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2omfjonbh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eysihrbm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gczquvqh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yncjarov.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jpuqxldr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kkkgasju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tutztnmq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uflfgyqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqwfodgc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gfhztcca.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jisyolyz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2exylbkav.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jomjjdcv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2txywecve.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2slvdedbr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2iqyiznkl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nugldmtb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uacpfjaz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bvnvyiow.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lbrphbwp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2teisowci.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqgpnz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrxkiuil.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pgfvcgau.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tyavcuhc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dcfpghsu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2swibqihm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rqfnqukz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fuvjeemf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ckxsvesf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mnaymrje.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bueskbby.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zzruyyjy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wjozvuaq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2teigbkie.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fkdheapc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bgkbxrlp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vswvaopn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2psurpuva.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2geknedlv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2aqxaxskl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtonifln.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jbytscje.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yzkmrrxt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wwqkgyqh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ghwlvumk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xqlyzicu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjgtdxgt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rqeetccs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fidukewv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wlrezzce.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmrgyras.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ifoqzbal.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lawetgyw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ydtyzviw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwfezdyu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hvxjatul.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tyolygdo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mzcsqmez.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ghgsdgcy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hpmoqeap.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2brygcctu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gbjigxnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qxyapaip.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ywqvgebo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uionybeq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2olkdzlyp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uuikwhsi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kfbosmtu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wgwproru.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mfhxubbl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhsadxvd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bzdbstcx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jzqmuval.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ybpwfvry.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzifohbr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lzuljqqp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpqeokgz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sxwlqojd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lvfdskbb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kphtickm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2orztnuox.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kigtgdty.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rcodxvhv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tdgkactj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2miqdxvda.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2oouyiuzc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjikywfo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2olsraiqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wkxpjmst.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vkqisbtl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ikkpwqir.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jqarismo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gxrquavk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qkyqzzmx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dmfvsrax.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bfxqzogo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kdtdkwjo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkqaqycz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eirerpxa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fcmarknj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pcjktovq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ceizuirj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zqueocsk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rcqybvyy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pjtykqen.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ammnlwhs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzyhbjcu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zhsiawlw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npsijlor.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2glmnutpj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2veifwush.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sohjtvms.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fuieqgzb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gktlkzkj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tlsgmayd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rwwnjjvu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ytenxdgo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2edloyunr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bdeuxvtl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xngmgkzv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ctmtqipn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mdlrplsh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2makmyqrz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jhdchztu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2glghdgei.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uhvfwrak.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pwfsihkr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qiopqzxc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vciqnlng.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bllndrvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mvuxmxzj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rogasdcx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2aeyyybvq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ylifsfad.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kiuvityj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2onxxywpq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wxvnykxd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cnoayoms.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2okmljiei.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xvrxlnux.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mbllwijq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2grwjeefy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ryxsouxu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tphbsyvv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jxetaail.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2acwxogds.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tdknsinl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qqyegsmx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bmswyynn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ewjhqrcy.html


<!-- 参考信息 -->