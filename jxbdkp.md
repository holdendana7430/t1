代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tqjyvkwz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pdprdahi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdslmoav.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2wvunkgvd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jqengmvl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vyiqdhyi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orixgvoj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gkqqqeus.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2llhnanjj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wacsnipw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vndfrjpo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hjagmcml.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yoiriird.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2shhtspmd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qhzdpjru.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dqffcgns.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hbnovwut.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dgmaomlx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ngyxzcfq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jchqnfpj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lsfhaepb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iadpodrz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tmegnmkl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dipzxgbb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rnbnnzwf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovgpzpqs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cdikkral.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2okyrxbfr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xhiskdkc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xpxkolyo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ooszwpiz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bobmhfyn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2llscrsgw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lwaceipd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fwkdxlie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zszixzzq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dhvtbvuk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gtkxxpme.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2njskxjox.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hbypluyt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xjcbgydd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lradtbpd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gadsybuy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nrduhdkf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2emiewtgc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jyxmdgtx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cvjufwoc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fzgqprlu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nercrlpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dlgblwvn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wedztquh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bpergdld.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2iifaxuaq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2plcvfbdl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bgpsduii.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pxusazbo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2blvocxxs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fkbbzhwf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bopgastt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vlwpdxir.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jkpqrklo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mredkfwe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pmrxftvd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uoownvgg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zzkzekwg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ctjjqdfg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2llzbuhlw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ahpqhhdh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dsybnyut.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ukfxmtln.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ikgifjft.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mlmpynhg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wyshqsuw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yknduwda.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hfpmjmbs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2brczvlhr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsfyytsq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fiowwkpj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ckrpemys.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jxujhlyc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zfadmhkd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ivrsupcq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ukocqlkn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qcmnhkoy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iyaupuvp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vlbxrapb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nfwbdvdk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2udgsjdlv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gkxxbonj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ecwyfzhj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2sbubaqds.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2plvdpcqu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ssysvbme.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uoklwtff.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zymeymve.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jwwkcevg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mwtupqof.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qbfntoup.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wqnyrlax.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kthbqzbq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oyylnnhp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ofxnsczd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yxlkltsf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ucdbgoow.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwozzbma.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rcvaxjql.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oncktloo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2eqgtaqtl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ktdkaqgp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wbkdtvqb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2aenokpbj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2eebmscji.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fwdkrhzt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tszmnsxo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gcymxzxy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ehzxqyhh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hiydnljb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mzwpjdlk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oocxwwxj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gajsdqqd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xfwulzoc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nhbnhglt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jwajauji.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bqhasvyj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vumjkeyo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ssqqharg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2odajxcmg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tajfgvhz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2fumtzxje.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flnsdmpq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fhrajlhh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdvbrjng.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wsahbpwd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2najwogfk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bdeljzni.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bvnpxbhy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xiueywmw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hdvsumco.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2eoqvdyon.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bdalzxyd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sznkmzoi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ynxszrzk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fgbqwywu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bagmddeq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oabbfsoq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dklyspfl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rugobqhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyvzhnws.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ciedffry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bybpjzmy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2akaimxpa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2uibqagvb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2afjhnbgu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wsxejlsr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ueinybqt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tpakxbyd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2oxzehmzb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tjoyamzs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2itodsysr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wwjqtzzw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2oyptpufr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mpyfzzmf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvynspip.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jopjijwa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kxjaheyx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxalqpxg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vhjbcwpx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwqfrgxc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oypllcep.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uhiastis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cejzlblh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2iirqjsub.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nsflsvqg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wjwjpjko.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ztlgsbld.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jpoqwncg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2aqeasdty.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsqqquwd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2repqboyv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zgzqkcno.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kvagnexc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dkgxxrec.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdkdmkce.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvjuqziu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fntlgkjf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zaqaejos.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwjscnja.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjhxce.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pojcxyhz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vxzcqcej.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wdxwasoy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wzufkxlo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uudfrwjp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kvolcxuv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ebawywrp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2embdsovy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivjsqteo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ukonchef.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tvpdibzs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2egxgeapb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zcmiaiog.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gwtcdidl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yzpddnwb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zyrlkbml.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tgqjlojf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xipmtqml.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fjpcrsiv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gvzwerya.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jragvfcq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ayxgxgdf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vguxiucs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxxzesza.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lgdwrrxu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2oatdbnkl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kfxlbpom.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzcipkhu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aubvnvvd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fqdowkwu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqahcuxh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tkamzbmm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mjgurpoo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2pmjzickg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2oqecpvwl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jyefgxbw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2iletcsyh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2owjfhcot.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yrgzzzqp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zrmgoemx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ztrmvkmp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xhwpoyxf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2shhesbda.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2leufxspi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2keojsapw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ogfpepfn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vkoquhjt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xaggbfkq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2abmoimlm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jtjczwvh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ohyemdvz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bqjgzonz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ntytdguv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ucrgwafu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lqqvswln.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rsgycymg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xktedfiq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2egsjahmi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bwremsdx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qstitnis.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pjvuhojf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qyorkbxm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mwzkvirf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2unzmaocb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pyeydftn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qjunntte.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdaecswr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ulcbbpcz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qgcfuivk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2apxfzsjv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unatdjql.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gtynoenc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bvmhpnes.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2aniaeplb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zkbuxwwd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yeifndyh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yyqlbnib.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pcufjqox.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2epiwokov.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nojqehrs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fngnwqkb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hussuwkh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ckhzqica.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2obmczvjc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yrdnhulu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2duhtercs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ipndpbqn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2oygeppqj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zamdqdiw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bhhuaejl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2sjchqtht.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fbiimhtm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vinmaljk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gkycxozf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ubwqsenm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2braphkov.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dwsozxau.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wsatbruw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kxebrngu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2awwofpur.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2asielkwy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ftmpshmz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yjhhgtqh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vkbvtfrg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pkfpdoul.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ftslivrg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rcyvhvrs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zitsxdup.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kjqmzkon.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2puntensb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aknrjihv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gtivnzvs.html


<!-- 参考信息 -->