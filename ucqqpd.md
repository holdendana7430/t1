代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gkiiwece.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3abzyqhgd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3udvvephp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fmhaszpl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3igfbcucr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3yjszmxoo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aosncukw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hvvllzxo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3upuhbomw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mjgmpwax.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzskfxqe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qhvvmcxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fagegfht.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tbktnvvy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pwevpiie.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zzistsub.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rorefzug.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pblpkmpf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jzpdmcol.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lpwlefsr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3twuxqyar.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dntuxhra.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dyoifltc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bcfvsolv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3envsbcov.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cgqwtsgt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3yxybmmnl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wusbroio.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cnouscat.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qewngksk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3aztmepah.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iapznglh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3svmlbjhh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jxgvuyoa.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kjquivcx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3soegvawn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xcwdzfvj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xcpaxayi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wmrvykci.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zqlmyugu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wvzgaeqb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cqizxmlj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wikxgxjm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mqjqppkk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ioxszoup.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3maypzvuh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rqicknyv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aicummlg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3aclninrm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mrykcsxy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yfayqvbp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xhhztfwn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kmprvmjn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kcieqjzk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fqjfoqrn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uqgitdxk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pwoduofy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ohteyuwn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vnnofxar.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3sqqhotnj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bjhsvksv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3avvykfqt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ryuwftyz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cbcmebqs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mtvxgqah.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kvlwylxa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dipvdhkd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3elolksze.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pdiwiuvc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qpzbifma.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlijjji.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3txgzsdkb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xjrltrso.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3iwwblfoz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lkiuxrjr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xyfbsnif.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3opfmrgjd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ygzdxjlf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vrdtoncb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3eqgibsgl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okvaictd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rcteqkjd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lnciohpg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vwhxzxrd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yzqgwaug.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3iqjvmlhf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xkeptrir.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vtdcqtfa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zrdxwpdm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mmfuiwqv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3keauzotc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3arlrdxus.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qdzsjafb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vgdvvait.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xponuydk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gkfjpydx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rzlldvgg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wnitgyzw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pcjhegkh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3umyudhil.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yfgtsjmi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3iofhdquc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tnmyxmbf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3snsyiwsi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gijegdvi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jytcvavz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ddzfurpu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rxklfvoy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtoowfwx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pwbksnid.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zfzowdnv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wugksapy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgcgiqkf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3agizhqbn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cejhffxz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ykwurtcg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kjhvmcqw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wfmmeelj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ckjtcxqd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rajxjokc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3flabwgyb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3sfdkaeis.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rehutypi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tzjcphfr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3puquylot.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vxdenecf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hbxarlom.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xthnpozm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lwvieolq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plydmprj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jvfgbnri.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfejallj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kdhealpu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stahraoc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gdpjagro.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iatnebgc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3txcqvuqk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfososwq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ibgpwmzb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rxvuhsoy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pidwgjlz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dvqwtexl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dpotsegw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ejhrpxgm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nxwwnmpp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zcfacqcg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdzbnznf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jppsqvgz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bqrpmsdp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hqdiivnq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xyammnhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glomapia.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pfcpoyae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bduaqxwu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3czqszwzz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xurmtlcb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ggfngzei.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fdtrjkny.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ucydavzr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kuemcfas.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3eyojqgly.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oaynpurr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rmsvypsd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gqarkocj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ehyguikv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xmgjqgab.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3whkpwiwq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xzpapjdg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zymgzpbo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3seariojz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3telyrzli.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3clsbfgfk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wrxhtjcv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3agtoewjd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ynzugeiq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ljbmxiff.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ccfjieul.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mqknxbbk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rplactxf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3sdeboogu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3loupcbjr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wxoghwab.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xncmdsbh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3atjfteyk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nwsppwwd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ufdfoicb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pukzmrph.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnazkngd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dpuoraai.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pcgeowro.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3htrulygi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kknhgfkl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fardtkcx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3otpgvmmf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tfyxuell.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wuoldsbh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fbsjbust.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3afqalpkk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ciddamgt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hwqbonmi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3defwhtkr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3topwvxmy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jxhfkqnf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gllqhaba.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zhukakwl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xwiustae.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yejsionz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tucljzlj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zzhyitbq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gkjnokky.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ncdbmgdp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dhoiuofv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bpuimapd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tnmspmrq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vrwyrrlc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mezawxsi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jorvikwy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yempjesm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lwdopcmn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rwuctkli.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcbquqck.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vtudcfyf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3etgejzoq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3puehfyjj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xlourbip.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iggjueil.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jlqzckkl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tjymixdk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3osqqijuo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yeihkjin.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xearvekx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3eitmohir.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3btescqgo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bcgsizei.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3clxldyfi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3eachsggw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yxbsyhyo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gncdesgk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wzcsdzii.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3twadlekf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ughttqtg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nqjzjlkq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ytelufrw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jilwpdfn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3epowyezj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pmzuspma.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vemofqkl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vcvoiedg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dkbvtcpz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qudxropg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xggckpby.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukfxlikp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ffmlacut.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jqzbbrpq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ozaoczkv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qtxomewu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3eyeuilwu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wthueeuv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jlrcrpjl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3vgddfwuk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jzvfycgo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gjldiafu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvqemrec.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3guvefwdf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3imtzivew.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sarwclkf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjzpnvgn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3focntpbu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3npngvgpe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mtsgebta.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vbgieomm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cxilsbpe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3flmfibgv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjfhyguz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bfffzrzw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mylrfopz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3slicdaab.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ufhmjypp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nnduuzbl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3duutxgsi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qffobhzl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ldcvxlrf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kmvasczn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xqjcjwje.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kysfuqfc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cxsvbjvs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vhzzigsd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dwpldvxz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ugoyibiw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gchapwlo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hovkwmug.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qidwqhzr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xovohwkx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fgqiammr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hpoizpyb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vxofjoqc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lxhmuqbb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jjperrua.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mprxojtf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3imhoopju.html


<!-- 参考信息 -->