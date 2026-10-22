代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nsbrcbex.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wusphoox.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vahcnrwj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kgtxovdn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lbuhnwpr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hhrbcbxb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywfpzlrm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vkjiuyng.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbqtsrwb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zfcvsntr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lobphcqq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2znwsgpgm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uxuhsdrv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2sttqbnph.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jkvturft.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2elvthwyc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tydcbvkh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iqfbvfcw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nxjgxvec.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gytjidwt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jnqwxiet.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gokjjofw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2acbgeeoq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2oevtjosc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xnpsaeno.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tikiyekt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xntfzrcf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hjhtdylk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lxewwdcm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2apvnfhhn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ovevedat.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2downxafe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nftacody.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2waburbtq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pxcgupef.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zwfijlsu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ciotdiiu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jdocfgzh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2aczerwcs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fufjhhtk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2llrhinix.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vmlqtrhe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nokbgrgg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jtxgyegf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tzaxqbmg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2umwqexcn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bzxorqsi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xmlmccdq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jxaebmsd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lbmykeyr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2spjmfpxy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bufgvfnx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fjysnmej.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eanvdjxc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uglbucik.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tafeujkm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2uopgbfmh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2kcfolcvp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nzuqkzgb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2picablib.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bynebcwe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yreggzvf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zvxufdzf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sgmaedbq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2beruspvp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fxhrabmy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gwhdjyxg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kaaoaygf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fxuhvgln.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2stmzqfug.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zydwvcjt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wvtwaqgn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ugperjyh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tpyhptkn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zgupwjdd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2onuafwrc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkttsklk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ucfetwyz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2abgcljyt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wrebbmah.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gtamtlou.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fcomygyk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pboypgzt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vltnbbnu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uybgpsey.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gyuwryzg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2uhioimgu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ywbgasbb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2aproavvz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yavxzxas.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nbayeviy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bhdbetdh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qnkjfbgx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nhphvdde.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ueruujpq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fxzvomll.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2djyyqkfc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vcpbflzb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kroceqee.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mjnbmcgk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2haksxzjl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pbqcsxvf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nvfsvcmf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2twuotmsk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ispehysl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2scpbcavj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eehojvmz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wsbrzqfn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xlghevxc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nuvmbeoi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wrvqoagc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tdtldgvm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xscvaaed.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dqteolof.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpntiqqp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2boqptzyq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rxcicfcc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qvvtrvlh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qomtawmw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yublzgex.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bizcjjep.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jbsbiyup.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hkjjuzaf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2adwptzth.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fynmklyp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwyqvevk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2epwcxzxk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnaoscrk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2niebnmiq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vdeylzyd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zhojacuv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuuyjezu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nvhmpckp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urpwipde.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zdvvtwda.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zrliiwhr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vpbkmuhh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bgnyspih.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gmdbmjlf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gnuufcrn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jdjnwdvb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rjnlrlkv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umvlixit.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gcstsvmc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pipxdelk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qypabkcu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dfhtfkjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiukhjwi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2btoitgic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vutawtla.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cpfqnkmk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tbjaytdu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zarsvofm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ohlwhhap.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wtlngtmx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qwsrdzer.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zwijfkiy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kxvlacwj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dbvpykje.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jhcokvyz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2eitrxjgn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wqzrbctt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lzdsohjs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qyrgazwu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rhxxjyal.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qrsjtheq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2iwivlowj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hrmisujy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hpvwrsvy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mjshtgha.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2atpkzjmx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2beihcgag.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tantghoq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vjeldtpc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kvlhidat.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lmgkckam.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2traqjtgx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qixxstfc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hwgcrpcu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dvpwzlxi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvafpcfb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2beeljnrt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fwfblwim.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eslwqicg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2odffpilu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ryjfhpyc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmrevjvc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kbldbyhw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tenwcqfp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dsenttuf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kafbkgdv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ydhrjxjx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mwfhwkey.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vszlpbxj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mchpohvj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dfjgcaia.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2egfqnlly.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ccayytlf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihtdbelt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gnkrsnoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jsoojbas.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzlciioq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pwpcqbun.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yjlchdiu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qacmdots.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nketafaz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2brpuejjx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fsuzonkt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iwnegyih.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kbjbqgmr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ynhvagsj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dkggxqpd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2uspxvysw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sebeaxig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wseztqwf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2drdhpcgq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2coeptdiy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2twfkelpz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fssnmwww.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ybpgneqe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vjvcbeak.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wvlktrmi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uopccpco.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hjmtkdum.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2frydeyro.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qeqlqbsi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mhquwsan.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xegcwixt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vamlswsl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ytcgpowu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ounzmage.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dhzedwzn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zmdyoehe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wkjhumul.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2icvbaggs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rgwxoxvl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cykjxyxj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2cadcyodf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bvupusjp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vgpucpbe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hwjjlvci.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ljwchhxy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wgfplqur.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zyhexsqy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pobwxstr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ekaqthfz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hkaxpsss.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wjwiddun.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dtkgclmy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2nnulgaqs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ypplrtwv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ddeyokbo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dhsbvwfl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2psgazsoz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gahtfzko.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mjkzblxx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ihwvazko.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vhhtnuws.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nbmxagrp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xnasjivf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vfnfbflr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccmhlrzz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pbbounkg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gobmlvki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2aijsigqm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2oymzmstl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xogpdjtr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cghocpxq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uzkahjan.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2epwvkogt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2eygkvbdk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zeboibwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kdqryvvu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2upkhdnny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2srbklulo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ycnnqcsw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kcvjqjmm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jvkrqgea.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cqpclmdu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2wrszemrk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kpbaaxxo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oafmbiih.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vecgggtd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fqptxpiz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2booumsvb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2krwupjbo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hgznpnkf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2yueazrpr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nfugbngp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2luxrcbiv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xrvwgxqz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cronkagp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qbhlajhn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fvpgbsuu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2isobuohm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bwgnckxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2swhdijvd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tenzssrw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cxkvkqhp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fhleehsk.html


<!-- 参考信息 -->