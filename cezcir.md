代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2llyddagv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nzjqdaev.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fyqpkuxf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rsnawgnj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ecclkpzz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gwibjrxk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jswzgvfr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uxngpxcv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cbnbpdru.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2epnhjaun.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilwmckqj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yeerfyiq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdkxyaqr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wesfkiao.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rdxzftua.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2snjfqson.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2epqadclm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pgpopmro.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qtblpokb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pmhbemxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yoinsyrj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnjdoavo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zkvkdojt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jsmcmrer.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yahihiuf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2eyvdjgpt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rnqrimwu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2volfwbse.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yjhnbfur.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlioihnx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qlefxkqa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nuycqjbs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cdlvnowk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jqmmylnl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tqbdjswo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nqxsacxn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mhkjrshe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ivjneanb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gccfvpwt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gnkocoar.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zzuebjyl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2eazonjrz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vfgovckf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2byqurlbi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pncbijvh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uuutnolm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rumngzic.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nqhkbsiq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kixttccs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hzrzbqnu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yswqokyc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jwnkamly.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2euuojvqd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ifgghpff.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ozkyrmxd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fwkbixjq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2aejozkov.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2taymotqr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2feaatpxh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2oraklrdg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2upvezvfy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2aucbztng.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nzueboqj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kzcdhhcr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rmejhyag.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sxrhrkhd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fucftewf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dlwtbldp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mciflmob.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gscrugzt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pulpiciq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wlubgswx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tvmpzlsw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kbugftlq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jjcydbvd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pdywpkoo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ocddhdcf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wagaspze.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uqgmkvsx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2djqbktwa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjqgtxdr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2twzcdttm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cavgbhub.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bylzuwyj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vlpllbme.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jghssegc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hqnsoutl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmfyrhwv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fxbwavtr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2brembjyj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2oybzvhuc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2troldesj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ubzvrysn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lwfyppxg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2paxbhuvi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ihxafctl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yqjeqjeo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vrunemjb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2biutzink.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2grjbzkzi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2acflzpsb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2flpcwuuu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fewwetdn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dcsdidno.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rixgaoix.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hrqrqbeb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tktcyzqz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dstqytnt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvjjcs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zpekgvzn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lcmfywit.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2osfxvufv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esivztgo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vyrnjktv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zajkenkn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2phquesel.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ujfcjqfz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2umczhnjm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qkdiporl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2umjkbrvg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yjdsqamv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oeivfiev.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qvxzbpcr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2whlbvmjy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fmkeoeuc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2feyhhdvt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tdbicltq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bllhmztc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mluwtmlv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2siukcggd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mvinnbcc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hrolxqry.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2scvbjjdw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdjapygz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2loprnljm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rahvbbyg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2aahxkgjj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nezbyyby.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zasyctry.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vnmczzfr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dfavmzkv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2frkbowpq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vljzvppr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2orxwgtrn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eejiygzi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2omnusrjt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wgjlitbn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qibmxbpp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ndetbnxw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vnkrrtdu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ljuofjxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llmislzp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mfjshpjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2robltyfq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fotysizc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2slutguyl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2pcvnebbx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2prambrho.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oxllqozq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2stbuzqfp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2csondgej.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pcnehxsj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wpdxoddw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cjlraqrh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pcfqknki.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2egqjlfry.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xrbajuhw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bbiwqnpz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jtucabfu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sdlswnfi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ewqvfgzp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfkcydrk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oaocvbgd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rystdcwz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2phudybdv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ipmowwwi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pungryey.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bfefydly.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kwqrhhkp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2noekjgpg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hjleyazk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmlyhzyp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hizuztew.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rlwuzeks.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vizvuxvb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2smgmvvjr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cydfqjqm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aqkjzthw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2baqpkzgg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qaazqnms.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2awzjwiiq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tiolylwv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbuavpyp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mntuozxm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fxuxvxrp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ttpthrvs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gtbidrwj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2cccoqaqn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wdikkrhe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yrgfrxfu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ykczaxnl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vymuwlsc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wevxkcgn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ppndaczl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zbploksk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zigwsxtp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzuvxtku.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tkeeqoui.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2keuznsfg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2trhqpojj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2elubkotd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tthzkifv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nhngczso.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ljrtomtj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ivuvlkej.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2urzsuajs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ufnnwcsi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wyknsjfe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lfvdywgj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcyvpxeo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2thqbxjky.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xnvsgvdw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hzkbcfdn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qbuxfojy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jbnbylzx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wowysevw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ubpvanbk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zdhyejdm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uqkfdbzu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pvitroay.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2htydsnhw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ecxqrfhr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrqrwuu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rmnbictj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oiwnwtdy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2azjaulug.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ahmxfuwd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uyskmbmy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2phiyvhut.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rrwfdixa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bdnjmtvg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ripzigjb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2uyzmxhcc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2khfmxswn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2owmdnphc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mflstcbi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zqhlbois.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zsyytfbg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pfhjismp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bltwbswh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xkwlsxyn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ooiybrzg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fhgxnxtz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tjnoayse.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2atbrlsjj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vwprbfqm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pbmdkfsm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2scgfzufy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jszgpiwd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jmdmucbc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2onvcpxpu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mfblfqqs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqzbbodc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zzzopadu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2etrxbhug.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pyuemwsg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2grlpjmfr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2typvekcu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zyruvpzp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jfyhljiy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wnulodyy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cewrxtar.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jowczrmp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sghvnyqn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vzahqjct.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uqvskzxp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tgpsptff.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ahrkacdf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bhfldoxj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gbtfyzpi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kttgzaal.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlzvrzhj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xqfuxwao.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2myfqxxcb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gyvdgmzd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2igozjwzz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wpelmxgj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nmgmlpbs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tuddbxhl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jendxhju.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gtjsswzi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2fqnycwqq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ephtxvkr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zbtrdiec.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2msqzdyes.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rgpjdqcq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vqktehvg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2czmdqnyg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jolukhvp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wcxnexxs.html


<!-- 参考信息 -->