代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3yldvolob.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pjxvizys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nsnxkhzr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hxoysmbu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fvjaljwe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3laitpcge.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3izsfygka.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lvdsezwk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ycbbpjhq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lokgqmes.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grqsanbt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kqmrumay.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ykvuwfyw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xrfravdg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zltrbkgt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3igtbeaob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxoznkpk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rapbjqno.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pqlempka.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vtnucsde.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3guqjqqcv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3shfotdzm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ugzbiqew.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3llygjerj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vzahxynl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmmjbypt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3maswidtn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wbumklgj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zaxhjwry.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iqspptsm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3evtokwre.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3czuztrfg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cfydyorn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jcknsxik.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ryalnbca.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jivsvuuk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3taoiqrjm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wryygffl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bjuxsjmi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pfzgvttq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bzaipzod.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fwylqsxf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3pnpduqod.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fpthfvoy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wzntpuck.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qfgrpilz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ekothzal.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3moufvckd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cjvdwtea.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xnrpnsgs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kuupbjju.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dvleketj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pyiwniii.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iwaigbpy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uzsgjblp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lnvtneta.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhimol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3exsenaog.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3esmsvqtj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nzgxzizc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ljfwvduc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qrsgncvu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3nfmogryw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qkicjviw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gerhodbv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3itipqqoy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hrzygqsz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cldrdtld.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rlzposwn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3olhkdiot.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3znxhiztg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3iecehghw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fhsqmmos.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gykjphao.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mfzahzbx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jmjulcnb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yvlojvab.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3lcglfgwl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ilsogbxd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yptjhcdg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3umcwsiqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3njotsamf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3opsktkud.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nlvvpooh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ziznlmkd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gehtgooo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qloufhrb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3drdkixdn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kdsnkiab.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bqzdtsza.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jmlogvxw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mzepcxmg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rthceqjg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3drgexkdi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3thiakuwd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zqlpdzap.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pngnmjhu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3gtimratq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qsprcskg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ewmltamt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gwmxasny.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3iqbzrlbh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dskgiyjm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nfwrkwtv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xdjrugnt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3aavcqwso.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sfpvauii.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rerbkomb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pvwlipuz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xtfqngpi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uwjqeaba.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xguhyvxv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3olmfcgmm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nntydrva.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wjrdjlun.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ibyvbarv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggvypuka.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3eattwzub.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qecthwbw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3eepkcmpj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hegyqyef.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tzoxxqcp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bailiynt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dzqtakiz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3egnfnflr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zfkqgmek.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hgitqmfy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3uwvdrkqu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3leverqwv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rkhqotcm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hayvynhh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gyvqsxeb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3elgbzsrw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbwtbjcf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hutnomwi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gudqdwvn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pdhluhdq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zafhdkhh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3huvzpjpi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uassjtwz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jtbxupht.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmsknajb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3muzvxsix.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3omrtfwqa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sctzowxz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wvwazlig.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nkcuhkqx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wzigugla.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zpqvvzqx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rglguujb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmblnasy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wsfvviev.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dhkgvseb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jdnwcumx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xbyrazll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwjtdfod.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ocusartq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcvmjufi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bjlwomoj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qfreqwux.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gonbxbbg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rwsehcyo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qgmdootd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tigiybhi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hxpauvcs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfyoinwk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ddvxbpml.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jzrnchrz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tnifnvga.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xxsvkmuk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kvaxmxpe.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ijuijpoi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jyemahro.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jjqvdzuk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aampyqcs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3elwnrdet.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xrmmoifr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jcdydmxz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3djhhyuvl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3payhbemt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qwqeuclr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cneqsgka.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uqaodshm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zkuzfeqh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3spiucoxu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3obxwtudg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xaijhufq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3epfwhpgd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dbencnye.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xsvwikxe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oacfsbxh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfmebcck.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hgbyldzh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lcnpyspe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mckvpidq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3moefgooc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ajpassvo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3njvvumgq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3txoesiga.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkredpst.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvefgnne.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rblikzla.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ssrzigog.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qsfitofy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tiqhwipb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ygxxiwot.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jclzstil.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ywaznnjc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjnpeauk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wjngchaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qtjidrnh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3euengzep.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3irhaioho.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mltfcpon.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mqjsmtys.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3pfyjjqrp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zzuxosjf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3crhiltbe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dpcdymih.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jjqeeqar.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3moekeyto.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uisphyox.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tauimstc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kaltearg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ungkhsqj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3anzaeanb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uezvuupb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vtoxrdnu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dlqhcuqh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3brywivpk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qjqeijvn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gqlfyfel.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lehgixmf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zkyjqhpy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hdjwbdcr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3enydszna.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tshqxzdj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jvuzmszx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vcswttej.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gameyxpu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yodctved.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lgkkmjav.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ruombrcr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gnlkgoss.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vgviqjuh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yfqtgrma.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbbbeown.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xlpotsms.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kstdrocn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cqpnogdj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3karaufkt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zoyhgmpc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zfgqxodz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wkqixstc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lrzkxgpj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3slbrsear.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qlfmwhzv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ynptjxbu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imujuypc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fktmkdoq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3liwxxrjx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dwkidqlp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3czxvkeif.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uudkalzn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rvcohsjy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3plcdddsf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dxflozib.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mttiuowu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kdnffwoj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ctckbipi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3avsoikez.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nkkzdipq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3douzhyzw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3urtwvutw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3iqkwuzvq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hnvcykkn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uwqrqxjb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnhcokbl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xcooserm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3djfdhxls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3oagijeaf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vnkvrujv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ljancsjv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3tzvuhgjo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kajqjcbh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3irvpdtbc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mwvhmwmv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hpjbljbv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fivikotz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zlxikmxk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3uztsbper.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3uqffeqoc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cishfpji.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yaspnjqg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3spqdvdib.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lzsmluzl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xhdyulgy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pppfcmcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hgdbyhhj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3orqfzgwk.html


<!-- 参考信息 -->