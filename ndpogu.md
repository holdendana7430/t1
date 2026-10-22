代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2twcnabdo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gnrazkbz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqtvhheg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fbzjbmnl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2huixnpzb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qmohxtol.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awhgvqbs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vxmpofvy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmbnfhdo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fyypzqoi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pyfdhlby.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rgxrpvvc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpxdkpey.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qvicsbhh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ofrlpgyd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2aarhhvwx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qppofcac.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jggwigfo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zfuovmnm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ssohvuau.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qumzqdao.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dctfbvfk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kjzmkali.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ctihveza.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hibvwawv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fsdopnjt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tbobuhbg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hibbfxgd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bnyschuo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uitoxhvm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2avinebwd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wfvkpuhz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hpegqfwv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dyuyxilo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rxfcxjyo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vdiegrrz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ovuzbydt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wphhghvw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mhyesmff.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2sjjmbykf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2sdulptic.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2smskwxxk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fncuafyn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uxajtnty.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2amhlmvlz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xnihukuy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cjkniati.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uxblphop.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rbuirkcn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2iqlpimym.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dijgtbua.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iubbejbk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vqaqdmzu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ixtkfwik.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ubqadncg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2dzdkrqdj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ufnpradc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nxuemmtc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wgpmkgoc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2skalfhad.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ajuugxjo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2twyhugow.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ijlmyfvi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zvzojqwl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbixjohb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nrlzqyjc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hemdyakn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2znbeipyg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ujiyngib.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ygevjraj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gwefvkol.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2meonyhtm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fgsdjjiy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lxqqgiyx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nrcyiuxk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hocufwiq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2medjrzak.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ufytzqnt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pabgwmsj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2zzdviqwo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fhrvgexa.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nlofakzt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2isbcgzld.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2feerkcyy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kiznsoyg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xjjiabav.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2povsilst.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jcdnpeyp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vompwhec.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ijhrfbfm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vfbniwck.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2scqciayh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cesblwhn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ovdqgney.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cisilfdo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zjtcrmnx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ubdndcts.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wornywsz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2andihqzi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2doggvyxq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2onworyug.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2cznhelwh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yfapkpgt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2woeyfwrz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pzwhayoh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zyfcnwdv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wpcqtmdm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2arqhvfip.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qzismsec.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bothfgib.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uwvpktad.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kezrlqwe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qbzzcdff.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2liwijgir.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iepvbkqy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kueswkgo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2orpbmsml.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oxtitwnk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mkxaraio.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ewnntfjd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ahahcltv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pttbcwcn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2reqidouw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jmuxftmu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kkptjulr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shrpymqv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dckkbjmc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncxacpxc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qioivnqz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmxowylh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2olxxnjss.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvgyjqpn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2oqhmpacg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njurycue.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2huvisgxh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mctrbxba.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lcawghka.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zevirypz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iqbjvtre.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dybsvswy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sfrcnbeo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hhaaaqys.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snjccoog.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2czevsund.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yvgnnrzx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ccqosgsb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tqeokeyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blurgfpo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ztruvzsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nathcqux.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ypekqzai.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lpogmdnx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rkstewvh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lwhpizfh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kxsqntoo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lkncpqrl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rmxabtuk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ynnaokgq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kkakdaas.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zfggtzug.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nbwpyulj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zzzeixbs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qzfuwyoi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2raxnxagl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2szkjoafb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2otlozeiw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2elebzzuu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zyqqbqcw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uzfxgxxc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ohzjjybg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2sthbkkem.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2halxhwpt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mrdagqzb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2luznlvkh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bskgdbnj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pjrznvmh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wvjbrgoa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jjtoeanv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hirhztkx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rfdtqilf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2abxeouek.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2npqbtpve.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tpjnhhpq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zptqmxma.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjepmhwo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2telaufck.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qpxgvoqy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2isdzictj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ygqvjyuc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tacnnpdz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vxhvoadn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wnrttgyo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukuyrtiy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2cxzkfjur.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkejlpnc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ejgnsoli.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lteplmck.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qyehhmhx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gjvijylh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fwfoyedc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kehuaqmk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cbobwjws.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbrgkpwz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ttxpqokr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2natqrahh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yfeixosx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jmsuggyy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yhgbormd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2upcqpyht.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2waamesqo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ffcqrpig.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2deftuudu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wzhctgro.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nhvgxvdl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hklryunl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajrtgzdi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjzkmsi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2erblsyak.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2saquacox.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wxkbeopa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2napqlwkq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kfxceexz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aukfvsjo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yfcvabqz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2twazozbx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2aihtunys.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oyerdjfu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xofpedqe.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2siprmehh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cosmmvqm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2unsjypvo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2eunqmtid.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pcojosoy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wxgygizt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2arfhnqxl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2okddcsvn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bamuzvby.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2sfsmaiks.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oekxirdm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nynbqkuj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2owivnjxa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ekmuexer.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2txcxtsyt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vzxupofi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lkwaokxo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2envhepio.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wqlczmle.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gxusioyo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2abxnwrdo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vmgbmkko.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2adsikutn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hmrdcqla.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sasyiujs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mitkkiio.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rnbrljfd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pcpsplok.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2opjqycrj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pssdsvuo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2thweodjm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2awdevfwk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2paanufbf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zzhhcgwy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kthesoth.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tboqowlw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jspxzycn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uyvdkdmt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pvonrjnr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vqkxsbwg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2azipwokw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bprdudek.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2feehecxo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sytqkovn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ilpgnbvy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2drsnkakq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lvsvniwi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rjtkxxoo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sirelzmm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2clgayryf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2akgafqgz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2prioylij.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zwhpfomf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2upevcnfd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2conelheo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bnuoeymo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ivhvelos.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cqlurhcw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lpheimue.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nhhcxxxu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xojhzmcz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fvfetbqf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hupvdjgz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zltatwmb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rqwjjasp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ppoynraw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2udmmwqlx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tcpjifyk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mekpukye.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2etrffosq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2amewdsjn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nfnvggnj.html


<!-- 参考信息 -->