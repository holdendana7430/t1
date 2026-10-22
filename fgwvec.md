代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gefyzcbb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lecuonbr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jziavbji.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yulckkvp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ivezycue.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jngebtjg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsbxmfox.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fydttvya.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yewalzmw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aiwvclla.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vklplayd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hguegzdn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmxsyvrl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ixvtmjom.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yjlthctm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2utekdzay.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2asvhyqme.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2imydltwn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bpozweve.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dlwtadrf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jqietafe.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qjgfxyow.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zcabiyjl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qrvgoqeo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qwakqgfw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vernmldi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ocbghofv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kzkckxoy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ghogbtvw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2urkjcpcj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2liejxngp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lgwotuhr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2migqtoxb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jqrxipls.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kvclyyvx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nhthqhqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2owozoafm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sgutlthl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wrjvfifl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2srqhxfcb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rynpxhxa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jyscdbof.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qaeyvxpb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2snvubtld.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dpzxrxzy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2whjhlptt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2smawyefd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2otfasfer.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fyobkeor.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2adflkewh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2egsenyvo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2onxjwlqc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uoksdlpk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gfdxzwft.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cklmxjkx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aqkpnwkr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zcrswuht.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2phbybavw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzsvtwqz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2odihrsey.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cfcfzuwg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ctgxsnlv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ogsitgcy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2siitagky.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sqxgdyhh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qqcvzxuj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hsyqidff.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2naaozyqu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxkvlwz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rjaflzel.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gziyvuok.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2oiepjolz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rsujclgh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wdqzjyvx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vlryoaqu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2figanhpj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2udfityyb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ljnymzvu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ytosafsd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rucnhogg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwrlufya.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2aipecrbx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iksgwjoq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wjzahfry.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uycqjzoj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2aytsdktj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2kyuuqsmy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eodiefjx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nxpnxubz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2icgcdtxs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ybuewxvf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ezmqpuvl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rzfbdbvd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tijqbduc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2jaotfzee.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pwpxuvrs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2oaavjekb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rkylfuts.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nyrmbcuy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2efdtjqkl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bbblqali.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qeliiqlr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vjgjsbmp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2iklmuark.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kifgejga.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dqfyndtv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kahydhki.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bpjozzoo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rwjynxaw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vxbsqttb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fetshfwn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wisijjyi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qyroeolf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2thnwzbra.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gnkamqgt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mxrockle.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ajjpmrya.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2puxojbqd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzgrjbsc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2deakuomr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2haclwwhr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vpxqsmvd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2iaunryny.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2miecvdye.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rmrjzcen.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2protdlll.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sgfxkrss.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qxpvogjn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ubejcrbj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oclaztyj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qphjvyif.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mgsdovjj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iapsspry.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tnbntvnx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vbjreraz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzybdvey.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zbfqmixs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljspqswr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zgfytsoc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gajijuoe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hhadhurx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ilzuubqq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hvsncgdi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2achwitia.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vqhxptxm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2oxqpjuoo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwtuxuab.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2chekccne.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wsyqmpri.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fuzaycje.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yghthkih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wneiwtxc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pkenjgqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdbpqtuw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2giphqbcb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2exwppcbg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rrzmjetw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tuotsjvt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kwaecbcp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ktgqtvyk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2quyhsegx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2syhrbmbp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qstxydwu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jmacdeoh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uettmetz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xexhptoe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2usmvjdkf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfqqlksg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ldpszmnz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2egtluhuo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zuyrijar.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hgtoqxle.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2udabvhof.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tksnbina.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jcxyjpzo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jfizvmvk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2noyvamli.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jxekhxlw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ormkmzvg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rsgrjpmw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2slfgxbja.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndwzyrtm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wvxhexzx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kllobtrr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xdzpmash.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hxqspbuo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oqwenygo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmypnukw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kjurcnzp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2duhvukkw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrddjzyh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fnftkdzw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2othtjsls.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tywmlfue.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eqkhkryb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2liftwygl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tjzozlni.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pddrsxjx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cltutwhs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgwuwcgv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wwllnojt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2btdxrelj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hjresmit.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxbflalc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fpdrequk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cfzqmieg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ozpxxxiv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fltlzzfo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iogcvdxz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qogzadgh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cbrfurdb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vwmmixcl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cmmadgah.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vdeihrwn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qgudhgdp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2txwqbhsy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2watdhhsp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zaswrdki.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dfcyedik.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kdcyyfcx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mvopkhqo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2csgwphac.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wigxcnsj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2sdkqnvhn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mdmtpmsm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kumlyqye.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jlvawelj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ywfcahhr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dhoifaqn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rhbtypje.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yvcniokj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lwzaakcl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bfgbbhhu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fhobyzgv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tohnhkuw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xknciadr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ncvwlzgi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cxuccsjj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2erllrcik.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ypdombss.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bngelnpt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vuhwhcxr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngjulzit.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2adltecsk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wcdibslk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zlmishdq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2enfmhmre.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ipifdfbx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fxlgsdfr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2blcjvpho.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nfloebzg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mxzxjiqq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hljxabyf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2awvrrnvd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dendciad.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zfmpfjsq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qboblkum.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fubzcnbe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lbdcdmzk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hwqwgmrz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yhhesbil.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gymuzvqf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fkldkxds.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ftrpbjff.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zhpcmosc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uevwhayh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2swtbhgkf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dwkeygmf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nznztoyl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dhxacwjl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gpgbodon.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nqldfrdp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xclrswmv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyiwyuga.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dbycgeyf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ljidsxpp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hsbwozaw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sdmlmgla.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2brsmndxa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ttccdjgf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dhbtnwwb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2woybrfqe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pvlsmubt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2znybarpq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xodmbebh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mcrhsbzi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pwarnjiq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2duzlqqef.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bgzzmbvd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rgbsqtoc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2axtqqnmi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cnvzwpen.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2znjzgudc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ldqvdzss.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jfqvqrxw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2emzxtaip.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qtkkxwnn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bjvkflij.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rppoohng.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2foagllmx.html


<!-- 参考信息 -->