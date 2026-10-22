代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vkghlvob.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lpxckshz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oysxtyfu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rjhcbrts.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kubptruf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2merrwpdi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wvzdctlk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jvmxkczi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dkuruqkc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yqomyrjb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hozfrfve.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fhxwkwum.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rrihksom.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hgwngkqy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvcvqqdq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ouktqpmj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkiszgvb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tuzixjxk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uqisuifz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wdpdjzvy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yteghcfi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sxfalmib.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2orlagvbz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bzzqcscw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cfwszmim.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jvxrqorz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ppnlypax.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vsaniphu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mtinsicl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2yohgipgs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ptvptbtp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zgpqukre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cfalblqi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xzgmsble.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bjkmwjzv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nwfojpja.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xpwatnwv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iujgtiez.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ofnvzucs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qgfnogoh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zlpppgdx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ddywumcl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hiptkjov.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cnelgjje.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvabjavd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vrhncadp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qwojuuwj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ccmolrcr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bcgzyoju.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2uuzlbkfy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2awqpqlls.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nxfepouy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xhpaujvj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2iwxyendn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qyohxlud.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lokwzftj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vaqnymdy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rwwslder.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tqdocxln.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2enbtrczd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qaktafev.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gxdvehak.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jkigsbmd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zzclfudi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2exnybqhv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xqhcidhd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zzdgerfm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rfbiutcd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vjxquins.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2aedusode.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wanznoqk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sypbgeek.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbwfkzuv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jxwgfgin.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dyyrxeyg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lbxqnbqy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dpffuxdj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fmkihjfg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lzgoqxxq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cmkknhhc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2avmsioay.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ulrfcgup.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2huyiigmk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zpronuji.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igbvxgbt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lecawtop.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2banbtopm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pghctuyh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fcqosfhl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zezdqgep.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ipjhavan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2thesaszo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dmekrzuv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2higtpxdy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qrcvdxye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nxhdeuna.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pmwlgzfr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ngkwojso.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ebpcxwqw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2onoiykxu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qwjvollm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2epkdfikm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fpbzmlad.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rnajedmq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zutsjtzu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2txsgbmkw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lggksusi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekbrfevj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gszjmwct.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wtogybyb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zwzigwlr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vmxytfqe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dnyitrtv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vknvrhot.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lysbcqri.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zkwwwqvj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmgssijm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mavvgeoh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sdyfihfa.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2otlzquep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hwmtrrvc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bquzqmgz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2utkuyqfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tvzzwdbi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ylhskicu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zjstsyco.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mudunxve.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eylsolzo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xmwbxtgo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pfsptsfb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hefxfzmq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vsuibkvd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wqkzyrkq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xatccdmn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rkjwlwyq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwjsmtwt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dixlcwce.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmrlmols.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2llpxypsb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltflxaso.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2szxlqnjs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2euctlwxp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jfnrgvlt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cinoiisu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kotugvwc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zxxpadgg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ccimniko.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vxyylswn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tjrjnxcf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wkmeudck.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqjpdipa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lftyndpy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pdrbhhow.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2igytrefh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gjfwhcmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yftvckmn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aymirenu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayaqdumk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yygbntca.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tkqxnjpg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qmfacnlu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rabuzdgm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cqjptxhu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2phsnvfos.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ywbxsdwp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqduzxqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2aetweqcx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yqdlzoey.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jekeybfv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2marmzduq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bllypmlx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxedshyi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ezizkhbu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2msgvrzzf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2prpojbsq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjmlofuq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iblbdong.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2txyoinqj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dxcyhfoc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hwwqmkal.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nwwgkyjl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tyrqtwec.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uxtqmwjk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qgoxscvs.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gcchqsaa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjxbebja.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2okawrmpj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bphektzo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2orkrapqm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wvzqqlou.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfmtivrz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywhwkylf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lwhvpohu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcnakzkg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iyljzubj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jgkbmnuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxprmcqe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rbhxahuf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xngrawny.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wlubwppg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2obwxpofg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aohwwdzy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mlulgtss.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pkrrdhty.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2calrfrjs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bkhiniop.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rhsbrcyl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jaoworhp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vfuuhhsf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ejrcoupd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrhefhgy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ldmtrnhx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjlaxdjf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2syfcikfl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xljmmuqw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ccmuwsbx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dtbfzgku.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjvjkl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2eidldnhq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvjehttn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lpzeoygt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wuwphevt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2uzushmfc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xqbzfbys.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2koopdjhp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nesvsiih.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rwaocift.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dxgsrcef.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ralksjnd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yvdkixlp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2glvlrjqh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2esixgfwn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xqsrknbk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bbfydzqs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rkrqhonl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zonyyyto.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rithdxis.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fqurhumq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bqfdbwom.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zaihqhqh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2clpdbcrc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kgqssigl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ejavaltg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2czeouoxv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ejrffciw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2smecffuw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgpjcc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkqknydu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kdfzswoh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gimpsuno.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xkfndkxq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ivltywzz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pqkggmaz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hkuhnxkb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cdljnqiv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pnpjjddq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kskdqhhk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ilqqxxlx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xplxubsf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pkcxuibq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2siuazmej.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2idxovidw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sbqxkbuz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rmasecsz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jawrczkm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jguefhqt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rtesyaze.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qmmcsyxw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hcxorkmn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mjkixokq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pvwkbpse.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zolgxglx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xfylnncs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tksjrysh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gbrvjwdg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wjpjvsya.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bthwuhor.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgvkwdmj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2houlbknp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2eplatder.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uwcsybbu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qghcwylr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vlmzkmld.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dorfnych.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2djurbhkx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjbwargk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vunmpfve.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2flggwbzi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qodvaizz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2khypmbnb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2limtktsq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pljnthmt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2pdtdnwyo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nlmggqpm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fvonvwwq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2aqsbkrjv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ovxsxboi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hmmnhkeq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pixairyx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2akskesgf.html


<!-- 参考信息 -->