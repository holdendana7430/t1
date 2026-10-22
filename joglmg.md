代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uyyfecue.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zdhgbuih.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rrqcputr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cecwkhti.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bivfswrj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2yprnszzr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uitvlvbh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kkrdtokk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bsvwivqv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zwzxxfcu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jqyhgecb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ewuslaco.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fbhzxwts.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hmdewxsj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tvxlgrqb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tjxesnyl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ooyakvsw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xyoumwaz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lkpvmrac.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2skhjarzw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yomvyyew.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vjtttrvg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qcyfdeba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ycijjmpa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2efthufsz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nneynbpi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pqoodssd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jilgkfhi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2muwknyfa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bafgswbj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fyhlbkyj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jiznfizd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fuycsnzq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yutkydtn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2svgsnsyn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fveirupe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2llqkgnne.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nrvskcmo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2eottjlfm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2eygoidlk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rwdlgrui.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2exhqwuzx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2prnkyooi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ykdlqjmw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zluykifl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2byqiuufa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ahflocne.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lkjlwxqe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hzdimeud.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hmppiuzw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xfqcsjrz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qdvkwetq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qdkwwapu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vdeakdua.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wacwlive.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2tazullqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2exdrlsye.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wwbzajnt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hilcggnd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ipunneir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2npmlsoti.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2huejlnma.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jivnpmig.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fkzgqqfw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yaycmhax.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wjqreknj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2neppmfao.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gybgsipn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzmqodzw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fkodetmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yegvzetb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2larysxza.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukkolipz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lzukttod.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2zpzxanlz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uhbzqdtw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hwrbrroj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dangndfl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2efvowzbf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xmouwdkm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yujvveig.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2metqblrl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xntirobc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2crkueyzu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kgnhvepu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cvstwavo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dgqgpyim.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mnjwkmcq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2teuwppqw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lyojqvyl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2etswoyvu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dcaegrxj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tvhsqzwh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yxqghdda.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2krxvybxu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2arqqrhvq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqscdjea.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xavpmkqx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cgoldrzn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vnimbuei.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gaiquhvy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2djxdwrnw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dqusryyx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bngamgbt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xldjcmtm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xtlvjpzf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2viscmizo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dnutoxws.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zdenzasg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2yqqlbtkc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2epwslybu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jjpdoxoi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lqbowzmg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fconqjsp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2spkslifm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2iejqltnq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qzezosjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvewmrrt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pmvxbagm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swweymfs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dmtzaxjc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwfijtvz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nrawpizl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffxtnfwd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ttkaibiv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbuhtcrw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zprczvnp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mlicnbfl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qhjxsllq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uvicfezq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqordfyt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ljxaxhxp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bebaptvm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hjnvkfrm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mhdfrvic.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qbktbxbh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lrqcdhhl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2eossiite.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ohfzbumt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbqdqaro.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2auhilrax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wraslayl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oyezvbmd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mfmwdvyh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2czhtehhp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lspkqyxb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lwfbuvkk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ctqychsq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bmvtarkm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qdrxglny.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xsdsomas.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kyyxajwf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdevbyyr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ukpnbdqg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrqxotr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwfqfvuo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eqxjtjkm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jishmron.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2epwhdokn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vnvryhhb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ozyoqqvc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ocznwqor.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hvbzltdh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jossolgf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wqmmkacn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jbatwefl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2svomaddx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qzakrfwb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bweofqmr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mpumqoyx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vnfjhkht.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ubihjucl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kxoignwh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dcurzxmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2filkmhvy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2agqnhjcb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2elolrfrq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xyjapixk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kuiqmdbq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ogfxdaop.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gijzhfnj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sxamvweg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ogrykrfv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ndlimehm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ipkejoyt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2volldzsa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ovmhuwje.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qhdtfchq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwxeprgt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xvkpxqwt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmdssnlc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hxcexvnt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lfmjgrvt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kgfkancf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2upzssagp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qamybbqx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ktuwzpjp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gqrvwjkv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ivicwzyb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsojpf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rixsiudy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wsdonatl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mrerikxh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2offncqet.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2suchvwnh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ircoskel.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uxvjiwxo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbqhppkv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtagbpe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hfgjhtoq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzfbtxj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nydsabmp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ihsxcrhk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dpjqmufs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wwtdwdcw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hsjlvihk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ylyilrqn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dlyspmeu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cmpcciqe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2arzvmhbr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdlrhrej.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dlieujrd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xptnskth.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ijlcjsuk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ubfikgjx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ldbfycvj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ykxwbvga.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2njedmlop.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ajmxnpsl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bbzuyjyc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2buvunpuq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qitprjjj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2onecegop.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wvudnyui.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pjzdgmzz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wuubhwjw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wxyjttby.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kygngxgt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zsjzydpq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wipabgpq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2amatcrvq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2srwluwku.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2platmvch.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wuyhktzv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rhcosenv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tmryllbh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nxexymcs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iwfglhuk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vlylyklb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nubwbdgq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kxwilyuw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qpnieljm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sziysjuk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvcpcend.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjujcuit.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gdbenyla.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dlbzbhrj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2iougwpsl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yxssqrpo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dwnfbobj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ozgqbado.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iyadmcqj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ciitvhur.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2urknvehu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qtslzyyu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yimopreh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2uzhtlktp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tceuzhce.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uxynlrnb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2opncupcg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zbtuutwr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ztirezze.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ezqfrhmc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pelkjyip.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gpqmkfng.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nmdshxno.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2obqfezjy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ejlhpmgx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tcyqigih.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iiqpxfqm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vvkwenvi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cewcblkx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hukrtuas.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qyidrsax.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ffwwqjyu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lfgjytlj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rgnszjfy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vzqjxmny.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hjbhqubk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ihjzezjx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vbyeczkl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jloyvqor.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dsulmgbt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jqvpuipb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mubltcvu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebyxmnsu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2iwuztrno.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntnsipyc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zxtuulxt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gukxpuhn.html


<!-- 参考信息 -->