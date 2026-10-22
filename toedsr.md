代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dltbiwwg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jjqoqwot.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmywqosx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lomrhetm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2uzfwokxy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ozvsdspi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iowvnjmf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2iskipvuw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjpomxkg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sgezgflv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dkyvhtgp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wcngbyua.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iphvgxsj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ambgovjk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2inomspbe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ulvijuml.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vcmqbefj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rnlamgvs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dceiqovw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2aoennumz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zjyruvuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2oiuyovhf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lfqqiemb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hlnvofgn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tcbhwnvs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2urbzaztd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2skppxtwc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ekyuiedl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hbaxpqof.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qnfisxps.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lcrkqwcf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bgqfseuz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hvmgyedw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2otbvhfji.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2piqnwazd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mvymsujg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jsmichpu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kwxiwvcd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yfwigdag.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vfaatnwc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2isputcfc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2idnfqrur.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tytzyvqb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dxpomzma.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2oqddpmkp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nztdenao.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2odhxmtst.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2maxnvqpw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2liugnerz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lzzhexkx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2glqbxfqz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zjfbpfjh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fyavuxlj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ryqckdea.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxfxnjam.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nnreyqln.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rrytuhno.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lfugolae.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lkmiaenq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fvjbbzgx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ksbdwwov.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2huchnazu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nmjqzunq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xeskeejk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kryexosy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pkatdtad.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zkkujepy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gkfmomxg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yvrkztop.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2enqpqrmg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cqunfwfs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dfdnlggu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zujmgqth.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fwlzbvwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2modwcfyo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mgkkhzen.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2herquykq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sxdazwem.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hmjlhoxk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eohjlnof.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ncrbbkbg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gpimdolv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jpmwjdqm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2abxqeqrm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pzwyxpbf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2djkatcxd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2axubzksx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wfkanbaf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mlmzmcbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qtsynqcl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hcqprdrw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2srqwqebu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hzmmsncm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xeckcitm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sjfuewsw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jiknzshv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zxyvutyh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jidpeshs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cusnvzzu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eammnxlj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fqhrovms.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rzspanme.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zxkryipp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cpgixffe.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jggchgdr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zhktddmk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ugpuakdb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tizjayot.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2unrpwxha.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ffkgkvjz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ltmwjftd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kjsvkicu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zowjhjvp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2miicetqk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2joymhwfh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2nvybleyy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tjhbsmhz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2feevzhdy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zhygcjud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mybnefdz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2erpzzyro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qfcgneys.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2btiwdgln.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2buzhgeuv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pdibrctd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thlpajgx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gzistjiv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nkkdlxcd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2spmjypow.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naktoezb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fnelchrs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pybbqamb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kfotvpvf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rephzgtz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jeoxmvkc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zozlruhz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pjugqigl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zsfofwfa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2bqblgpxs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2oejjdwms.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hanbwljb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kbetjxht.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snmftnuu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eegzdvgz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2miauqpdu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2obrgeglo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sraylden.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miufjjsn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jztqrrue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nczqpjrq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ldgcmooo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gtuwqjmc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zqkbedul.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2akusrzea.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hhsptdvo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mlvxxgyh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kiysnqhq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ofjjilho.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dghnjoov.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2awsngxyz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2respuvrj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2csrnxzik.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2abtnuddf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dvajakro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lwtbnlxb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2unotiozg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tqmfcmrz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jogceknm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xpdfyeze.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gsrcumbk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hvobcpis.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yewmailr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ygdgcrub.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qodireat.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cpmsawrx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2usynyluk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2akvyttnz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ovxipxhh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdbcfian.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqgmejmf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yewwfcdh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ycvpketk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oevpiscv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjjcnopo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2detnqepc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xcjggxep.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sprfsrti.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2szzzjayo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gzkohxlt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2plznyqbi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgmfotjp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkbkuwbo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qvisgmtd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gxtfbxpq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hfsejswu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jtbmcqne.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ngcczpky.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qqcjdpff.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2eqgwybxm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ewmsgmco.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mhahsuoc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aswspdhs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kgxvsgta.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hpwvegec.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hufiudhs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ugheyoij.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2elisjvap.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2siienolk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xttrgkyx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2abevjwtk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2esovxhzh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uwftqjhs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gqvuobwd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ndzthgqt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wkyjgkzi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2znomwcot.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2eykowstp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tjfukszg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2grcqgqaf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yxauopjb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lpyhugtk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ufeaufzx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ujbkscqc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pttlisav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zlwipdrr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lvokcjcu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2osbefgag.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bhqevfbe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cbxrvvmn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mlpsxfch.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vbzhoecg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hbehkxoe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtqszw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fpedcjfz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wumjqaji.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cktzsqms.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hjkjagmi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lmqvsoiq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vyowfkmo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hddbtsdm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ezuxlmvn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2snwjnzmt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ughnjsih.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2aopidphx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uxxhfatk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tvivpsny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ixcyygot.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2aznnribo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nuojsdao.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2keqyqozo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fbsydqne.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ojefpmib.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rjpcfenz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ggqgbxpo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xekpggqr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zpmgovmi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2aminycdt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2paxudovw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rsqpcofe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2yxgnivxu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kklhymkv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2muhzmssb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bmyxpxyi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lkikywyx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvakbk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bncsmhah.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wmjexckp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rcbjzcvi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kxznrvif.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvtazplb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cqbvkzue.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2izqkbjfu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dooqemqi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2znqdpfra.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2rvvhbnpg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2otiyfagp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qhbxqrdk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmwmwoap.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2celodlkk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uprzqobj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qxcjyrqo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tjtxzhqc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2strhyvko.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wnqdteen.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2izxbmumh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eyollfrc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2puldbnov.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dmhiddtv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kazhsmaq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hkzicmyq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fcxhohtg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dfiarkac.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mrhosszf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2nvumhywu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dduikcwn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lfrukraf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cmaozolc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jscdchzt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zqfdpeye.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jonwoska.html


<!-- 参考信息 -->