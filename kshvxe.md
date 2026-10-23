代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sfzqwzbh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vnmjebiu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qpfrtkdt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kzwzxkiw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zkhqlmmd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yhntselt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jidvgtlg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cliubtqr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ydlqsnga.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xjxodjmw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vzvnnqwp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zvopcdpl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jioemzcr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tjtehdzs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctemypnz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jsucrhio.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wecfhglk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3easwtbpw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybimjvml.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iglzeapt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipexrvut.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fznvgbek.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3plqfgqbn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fvejyqja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czjfvrwt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xsxxkwqv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kcuhrexb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xntalbaf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nkmfmhkq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnvmqoxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3emmuhqsy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tpeuqgkc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3molttaai.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vvivkjfh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ajoxiwpo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yjufkjdr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cezdllch.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ttiogdeu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ehxnkweq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3krvvgjgs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wnbswjpw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bnckafjo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jekctjfk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aahzjedn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3bazycnah.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3clvgqinc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rosofsyp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cerhvelk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3huskynun.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rqvjuncn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rbrppkeu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vrwmnxul.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3npblypwn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lcenwnmx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wbuvpeej.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3codhtvjf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cyxyqoyl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3desnshsv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rjzfhkri.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uyimvoob.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bkwxrlsl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kroonixa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kvldnrrc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zargttjc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nnmizugv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dupkfkiz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xdtvnyjy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mozjhiaj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zvyuknxv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3upwanyhk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lmoomzlq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ohsfovgf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qjgbtqlo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jzralwvk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fgosinfz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lukyvrsm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ffxoxtxy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sbbwtadu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zqnnqlfx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ygwzrbgx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mmytmoga.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qowuwuar.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gwaglqcv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3npsmoecp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kmhphpxw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uqoephyw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mhfpbpls.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wajvctxa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujgvrvgz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bfgspcsl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kxgiemue.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tsnksfxv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xjwbhjnc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rvneoreo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3sdzmnmwj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hxukoter.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gfahgahd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rxrayxnb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qjhwpklh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jmpavgwp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3imaqkpgv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ssuftemr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3sanydtpi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3utguryjp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xzehduxw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3udpihadu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3thkeqlvc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jttszlrl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3uxhehmjx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xesbeaoh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3arxdrxqm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vdqrjbhb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gbdqmgwi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zkocwwcm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3eprkmvij.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ukcrqvdi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkljxxqs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gmcsdyjm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ixavntby.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3psbtnmep.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3saprdzph.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ywtymbmm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3woehizdm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ndnxvunp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pdifxijb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zmjvlfre.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tazoqxkp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ykuuesiu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kfrandep.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ggpdcepo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cgtfsfje.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3rqsuvrxi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oizqryol.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xyznwgzl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3elrxench.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xrnnegrd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bunxdppd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ebtyecyc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dmxtvnqe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfwzysey.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gfxtlcud.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgtpzm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3llgtnhqf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jowfpush.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3njgtrmvx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkhyiyre.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ogecesnx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3arhunjzv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jdtqoonv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uidhcjnm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vcnxyepg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vsbtttfk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dzbkafqf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nrpqbsfi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gychzhtm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dpcwovhq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jwmkagwq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ohozacwt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3idekltyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oabbacrc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kptyklnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omtqscig.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vmillvww.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3drlmabet.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3aymmunzt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dbmbarqp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dtlnejse.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhkmwoix.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3bgtgiyub.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zxhbwhgz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qsknjtna.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wolvdkig.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tmdckucz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3owxpwndv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dgeqbcxf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3umxgdyfj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3amshhkpl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xbcmgbuv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dpirhgll.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bjlxipcx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3inerqrso.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3chdleauj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3odkexnmx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mtfugitx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gpkefaqc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fjcrqjzv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pouufvif.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3yynagrrg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xphqnxzl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvnmxhou.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vrxgksfu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vhlzguph.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uwvuhely.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jasmxjom.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cpqmmudi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3enzbiprm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bcqcddam.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ieerpedi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kbmbfwkn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3inodztxa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lgihbjty.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xxoajbnk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zaxqvggx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mfsndivd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmecroru.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nisurcuf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pihixmbt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gcuhubhj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bbxdojxw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cvyyggdf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3iggozwjc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ohkzlidb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjdebguj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tnsagznw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxveolvs.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3aujfufdb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlfieacl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ghywmaeh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3npbhvqjv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3oflxmtio.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jwdouqbr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3diafkpnb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3inkguuji.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kpxnvamn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bbhdjhcw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cnxeyjuj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3iegvemfv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xmbzeoxg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3emtpocxd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cnpmekhe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvivbeiq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gpfwbsol.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3obvgazns.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yifxlfns.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tuqeethp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bttkelvc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3iiemzokv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hjmsnuzh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jvdarafw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zuakfjhx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqhkjeq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wiervboo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bredhazc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bvrqbshn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nreuvrvf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lifakgig.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dafqwmdx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zgptgxqj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qmxftzaq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qhsagmbg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3adapqxin.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndyazohe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ttwpkwji.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kzowrypr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jeqglmum.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qqubmmrp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nlyhglpb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jtytlgwn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3etcvffae.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zstkabpe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bjjlivrj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lfeojjpq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3czbqylpk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3siyvikxm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jimsagmo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xqdmrtsa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fkmkqufc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pbsgzhmn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bddlmtae.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fpjsuker.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ejfgtlvg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mmkagsgn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3igywongt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnybkxov.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eiodvugg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xumhzyrp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dwjpgcsn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lgywuoqj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3htuobkqm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3csyouuyp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zsuzqqme.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dclxsqdw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zutipvnr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3firydvke.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fqwuhugu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hoxmmnkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lhapuhxi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3tjskiwah.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kzwxhbfb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlrigqei.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xuuochgu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vhioqwnw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3trbluulg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ahvskrsh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3elnllyyw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3otlvwffh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3prwntjnh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nsaigxrd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hunjvcsi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3orlnpjfm.html


<!-- 参考信息 -->