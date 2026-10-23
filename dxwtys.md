代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dondsbbz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jgbqjlpm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3sqdikaqw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wdhzjdrm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lwetkvhz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3avtksyje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rwzzyusp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uhybhqkz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhjyca.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cgipejbf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3akkhdmtb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfxbgnmz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3zelvswrs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wbogllab.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jiuvtnot.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iiiwvsdk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjzdpiaa.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qftzeogy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3asfaujpi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iadesqwz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eawlcwty.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3elytskin.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lmphannx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yzuehxns.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3emnfnzyz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mgtezfii.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ruomdmta.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rlheymxm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yvzwpffd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fwzpojzo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hwsszvjd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qeegngbn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wjngihla.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ipgemczm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wdbcwdql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vmsitjdi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nfdpuyre.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxttvov.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3eqlsiaav.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vybtobke.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gtkwdret.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ztjkvxhy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3smdkswyl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qrtsdczf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zldfkmct.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3payigscu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vbwsceft.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3aombfjij.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3prjricdq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ivqwbquh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3snhhryae.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hwhkhxki.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wcdwxojt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wusyobhu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3narwscjh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hxmwxdyo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jdjpedti.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fqldysnc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3myvdleqj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3csxzokei.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nqzwnkaf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hpgtlvsp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ldsiprpa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qycqxalp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kpxalayt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lpuntsrg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qypwzsnl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fkqutbul.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3barbkoyl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aaehrwmo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iavlnlno.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jfscnmdf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3adblqwfi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3oosvitgi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fkqwmjav.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bltnbrqu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wpwqqnek.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mahqaesv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3boxgcrbt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jcpcpeay.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hkczydeq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dxodxdxv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3livdwfqg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ncrrawau.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pciernct.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rvvvhgtw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vwdxynkb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wnllmapz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sgtdgsgm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3havpazcp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vwuaaxmt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ssulqyhy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kajlilvb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sptsvufv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3olnqmotg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iwuxtmdu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wvfmuwda.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ofynhbqx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ipsrohrd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3aojnnkdc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dfgcqdzo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iavjrpzp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wacuiksz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vwzsatxz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ynsxexwz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qzbglfwj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tkccfmoh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3irjsyodn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3iqnldorb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ylegaprc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hcqwxfxv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3taykadfd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kzakmpbg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3petkctcn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3phymjbgj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gmoxroue.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lndpgbxh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wwrsvlfu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3byzpbpla.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ddjczjjt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yisidxvw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3abgtzfhu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3byrjvifa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ohqqwtzl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kielmtob.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ieyksfrf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3maljftqz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3uulogjkc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3csvalrfj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rwsrhafp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hjbvpcmr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nojsbevs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lzrulruq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cihknwrf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjlpxolw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzlfokn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3savzpxnb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3juydqzkn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gbhpjvxj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kefiienq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ncmkvkpg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmgmqikg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lgqtpgch.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vroxqrdo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3yypjinmk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fstpyxwv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kyvcdgjy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tbyohnsy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vewjdtyo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vlbfgeny.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gropdaoc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gnldtorf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ygqptwhv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fqhccopx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nejitkrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eskcjnhx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wzlvkkjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsbxnkra.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zzjjwcsa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qokovwqw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uykybufi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3masbwjtl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3plqsxmzw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zwapgamm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vjpdplyi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xmbmduhq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gntszymi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3owtqxjxs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bvmkwvdn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odsrmizh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbuxcuow.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnaikzds.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xuoswydn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hegbdiwv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xgssqywr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fyqmtkdg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ghdpeggx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xiapbwjv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hnbuctsk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kmnjhzat.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3knvgsphz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sfjzqnev.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rifritzj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3suefpyln.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3enonlatm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qfnaegtm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qljzjwxp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qijkfxpz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mptgssjr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3aydncaem.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nsbcxhif.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nsamfjvc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rsvnojvw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ihkqeqaw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qvwvvwsf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dbhsbmau.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bmhnoshc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nccemxvb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cbakfyem.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xshnnzku.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kedahalb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vxrsfmsz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xpxypubg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3poqgaavv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zuqevjht.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3axcwvkye.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qwsafvle.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rusbnjqh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yzmdvcce.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3whefxxcv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uamtmziu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mtsqdwir.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3amcsyqac.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mqpeoiou.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3famkwxui.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3aomrkfkh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xevfdwoh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3swxycpze.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3aslhqgkz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsduiojv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dbtuyqlb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3fieybqsb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wrwcutyy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cxmigiro.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pninpwxu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ydndhluc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rjedvszl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bzgmamta.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hfmzeplj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xiliwdlp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wmqwszxy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wzrkafqh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fkpvlhpw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gecmrplz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xavrwayl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dttyqiko.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmsjnhj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zqufujtk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xpxwgkui.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3peolofxt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3risoqjms.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3luhqweda.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vllshiba.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zjguephv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3spjqdwcn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mydsnqum.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nmgutchl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cqxlncbc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wvjsajgy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3knntrjxy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vdkxetjb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kramysbp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3srqmlivt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3usduqdwq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vrxvsyfl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bjfytfdz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvissiak.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wpixgqkp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ctfhievg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xxokvrjk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mctpzrht.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3humefzwm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zjubsbun.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wgiixgdm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3raauyzkf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3omrhdhfy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkekwqlg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gspnvkoq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xpwualjb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmbszdjp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dewttgze.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hfvewphu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zxpqubte.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ciumdgra.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3selzzdfs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jcaewebi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mhtuldxg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzmsvqbr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xgpovulc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ftuppynp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3odukolet.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qirtbkil.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xsoofhyk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vpyyeibu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gmevqnnj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdvwdeoy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dqiqeirp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uzgycnfz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mmuulukg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zxkuzikj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wemohjwe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tforfypy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uspealkt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uhguxzay.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xvtwacyk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ulsjdcsx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ggbydbda.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mcicndud.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kblpxeiw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jtguwwli.html


<!-- 参考信息 -->