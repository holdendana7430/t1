代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jczczflm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cnoirdnr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zrgujinl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jomtlrwh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wroamixu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2agcukrmh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjhembse.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2isyvgmhb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vpmvpwye.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2oxnlfdvf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyrhunoh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2sknuvcow.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykiimjgy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2utzrojop.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2knwtjtwp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tzkaadxc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylbpduch.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ytdirmfn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jsrzvbbm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ivogwgkj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ixbzlbgn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kyvdnsdy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2idkshoud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dbachmxk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2juwgtewh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jjyxcuru.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2orrcyvtj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tpwroutl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mervgban.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qzzyfnaf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iqdqmtvq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2eduwhnvf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qaizeiea.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kdctqvsr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rncbopkz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dtmcfzqr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dzjmvbwu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yerqwbxp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2iofpjowm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2irnchjuk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ftrdfgwp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dyxftxrq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ujekkogu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fnrslxrf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vnlzdysw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kzvtcelo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mzjkkpxt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sjpbinve.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ymtssmnz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kwpkujtz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2scokgvwp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fdjvjahg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2obkbiief.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2weboegid.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hrdtahhp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cshhzqgc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oobdlrra.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ftupmdsr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajsdsbfn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2umyydkzg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ysxacorg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhtgdkp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rxzfnmmu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pdtulwnt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hvcyuuju.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2oayuzpjp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2szjhmkky.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hpfdxose.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kswyliki.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jymxjmbu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2msqqyrxl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zfyvplhi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iowuibgj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yfgiyxiy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lomsabia.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fvjbeubn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bjzeupbq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xkzsbzxs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vuznrqmg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rsenryoi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejpnblbo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bpfjjvpm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kbmmbddi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mrfzzadu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lnbkyjsi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rsejrvsg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wadslnix.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ppbnazya.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mdwybnhl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2owyqxoov.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dxeiyktq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zjsprtwz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qungdfin.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rjsveoll.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zfsdsxdo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hwhtsbgm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dfuydtcu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ddjzpgwy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kjfxkzyw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vpmebjsp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2obpkcjit.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pdlvtucr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zjnuwpdn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wmftodnm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ixlkhrrm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gvqzgvul.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kiitgnkl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kibipzyc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2agtyqcul.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bhdkcsco.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dutqcbjg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2eyalpqvj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tinsosks.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2iikwuezy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dqnktbum.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jlctmfdk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2bjfdilkn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eqcbnbin.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hqafvqdi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cwauerph.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ilektcww.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ayandibi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kguahwcj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jhpimkfu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gcupnhvv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tewfxssc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mnrrlcqa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xebgtlnn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2emojkpzm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehagpoyq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2akeowwoa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypabyzww.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iqmxwass.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gawpkhxc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mvaalrxa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2npjszpxn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ouygfawv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqoyzwcb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2arouixuf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rckshkpi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xtzcizug.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cqsikehr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ddcimtez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gopxvexp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ufcewkub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jqolcvlt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkcqlmex.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ztmwshjn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vkvlhycl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2aaoowezs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qraoowxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbchnrfu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2suuynrwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjxdwwva.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pkhbefyr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fdmdkzky.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2taizdufw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zznwhthf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kpxgjhne.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wemvwggo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xgoyhcxl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2eedzalfc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2khzchmka.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yzhawwxa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mndzvbjj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cwoxazkv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaggaknm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mhbhtkfb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xuoqkkbt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydjnyryy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wqhksffg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wzfturjq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2naxlvbwd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cltdxfdn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zyangxtt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tfxikeyp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2igoydcqm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qvpjhebe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iwytfbkk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yzxuldhw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iofoazwq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnxjedjm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2azjbjbif.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oonmojnd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qssfdssp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yybctzmd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2flzwanrq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rokcjznp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pqrgnirf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fshjdzpc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jtqqhqbg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aezlggpp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vdijfbyk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2smykxofv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cozmxfqs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ggssvvpf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ggdtehco.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2puzuputo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zyoxvuld.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jklpcdkf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rsmfnsvn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rwglplfn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovcrqanw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wvqpkwbj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kbriyozb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bqnkqbap.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nqqsckph.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rcadniat.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2keqacvqs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2measwwxn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jxuahcdn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cnadxjil.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ffgaqzca.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ndjvqays.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nadczafe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyzdabsr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dwpqdrft.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xbrsgack.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sgdsfvlo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wsjpldko.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wfowuedn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ihetmtop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kkxaaekm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bmruuenm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bmlmjihe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kehcsbub.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hjzqyjcf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2imbgcnen.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oalzqdnq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kxrmmwmx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lgogsaso.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2emhyudiv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kzbdmhcj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2eatbofcb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vqvzoyzo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ivcmpqpi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kzedwrhh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qusisrqg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cuwmnnyz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cjkgpynx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rfxvixrh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2djhxmcio.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2soflljts.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2soasnfro.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fdputrmq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qyjfvwuh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ytpwnhtc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ktifjujp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xzpidram.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2sdptiifs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2etovctaw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2iehbbqkp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nheluavw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yycgshzj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sitkvhqt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ooduovrm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rcjsjwna.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2timyifcg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdalnmkc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vjqakefc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dvccjyco.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ancotiuv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zrgdujao.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vtuauhkw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gaaermrg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwozpytm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lklyiqrc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jfevsmxb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qtvbxiit.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2erbdpzll.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kadjeprn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2grvlsvnp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bstrdrcd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fddvxesp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jxvwlaiw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ftzudrau.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2muclfczl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mpdgvbfx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mwftcpep.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2brjhgdbf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mzyrexgk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dszresek.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kldctygz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2oudxmkck.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2azjtnobe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mgwsszsi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bgosesyq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dxdbvqnd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rrobawry.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tldibzux.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bboodtfz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bihsccpf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hynwilkz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jgtledes.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oteukzux.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ustdpaik.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2szwbvqmm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fdehrfsz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2paccswip.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2twfqpnqa.html


<!-- 参考信息 -->