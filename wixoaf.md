代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmbmjngh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2savhmyqa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2viuhdeit.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nvdcpsve.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2onddedmz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvocyztw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2htrrvtbr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kbdrbbug.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oigeumdm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lodfnbqu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mcmiwhvu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mviqgwob.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nuwloons.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dqggqudc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qkvcwxmc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2odnghxal.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2niaenfkt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2liibsfmo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jlyumloj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2muxtftia.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2buyemjhk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fhinpkxa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mqyuzroq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wpgtiqaq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jxnaqvim.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2postzlfr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wvsonhba.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2opcwwics.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bcucwflb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hrdkoxff.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ntcgqftt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tkewpjzp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pwnaviam.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zxvscwzl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nfswkimh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fjcctrzl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ntreykrm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2diaqzgac.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ylfhxqxv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eeprwpwh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fdutajqb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eqnitrra.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2glsdyyvt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lmgowkir.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kclnsqfi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jxsdgqnm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2spkhaffl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gexllsga.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yqzzuvlp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vwfmauxn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jqvtecir.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2edankaqb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dbgifiqi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2snbfnkyt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hltzobbv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2puzuqfkd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ylhbijlf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2eskstgjv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bixpyjjd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nsoyhteu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kzrscjkt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dpmobzkv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hztkwzlt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iyweyadd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hexbzmfd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jiyriabb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2maxklnex.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2gyvqhuba.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fbiiaxca.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jfozifkj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ciixpmee.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zgkbzgwd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hvlpyvtc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rqikpwbr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2khanzfoc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yfldubne.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bincfodb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zxsaauia.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kngtvvvv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rtmxuspp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2igsdgxae.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wjyvcicl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ciqnhgps.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hmfqhrkp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cxeokqvi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nqfhslyk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2arsevbde.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2acparivh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xpxekgen.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2exmkcjyy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lzldqpxm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vvihbzbz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixvcfrjq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mptkgzlm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zmnhglit.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nxovukfg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psvmpkeh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tvxlskhy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwcwbi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2hgzkesap.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ojmxtkys.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ohjfgccy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lvfiurrc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pkhwqmzw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fwhmbvrk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uxzwhxoy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ronjehdg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yrekkssr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lezyzwgc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dzpiniib.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rcnzmyjm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gkrwafib.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rcjmrbtm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crqtuskz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwzsftac.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgkhbjso.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjebunee.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpflyyfw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zpzgylar.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kguxwwtu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mjigrgyr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vxtracnm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lgndpsdo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jzuvwhmr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ncxchlua.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dijnijwe.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2sqzhuupm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kzjhtsty.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wqffgsyw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cvcyzvsr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uycnwvsh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwhshsyl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ddambbfd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wyjdrawh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lvfuxxzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2notahgrx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2etlvdtdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qshmkbka.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wmdvwocj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dgwnzbed.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2pmnwtouf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bugmdslv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nzowtlkl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rubmaqpl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nurmopxu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fbycyzzg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xyzrjiia.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2drqlhsbd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ycrpxtiq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2crwuykzx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tzvsylsm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rerpodxh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gupxfuvv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2stnqfjkz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cazliaye.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yichilqt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lzobzuri.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ivigmccw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tnkzrnww.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2shvyhnma.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tsjqtjpj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jctdvnbr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ppukfqib.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ixqrybcl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wlgogupc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykynedsa.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mpgdibzo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cmxtpfhl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fzdhzawv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vpitmzcq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dehklcxs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfvwafew.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2copqozxt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2exmqplta.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xzprakdp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sihlmqom.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohzaphqi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nmckyqle.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nijijjpb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vrljkxis.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cubdrkni.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ssuywxmx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2duditzlj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xforiiyo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvyqrgwq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eegwhstf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2axmkqazs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mhqrjqoc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gssorgwq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qznoyjhw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zzpekchy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kcgirsxs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2oazgbvaf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ybymhasp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zpuqgnsk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jlfqjjpl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hohprvep.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xdzgwzfu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cdfxkyrr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2amzzihni.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2evocsiwq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mcckozdx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bvsnlmvx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqvswlwg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tebqvuxh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bjiifuzd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mvyxnitz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yeihslef.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cckcllzl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2sfnzrznz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yhxcgakj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pjimmapt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2drguwoxx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2yjmbwkqn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rkaolgwg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ojcdcpcm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wafopuei.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lgdcnqui.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dmbkzody.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2juxibkkb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2otnqhjhm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dhgskasm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2iwqyyqpu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2olvcfdco.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wseteqmj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xcmhbnfk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xukhxaru.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2unvxpatt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kasinpen.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2boqjkiyv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2lydwtexg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2toxyriix.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ztwdgdko.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2osdcodjn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fugaztrf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ifnersfi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2glflthzg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yvgbebnk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2asgwmyvw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nhfthohz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vujrdwmb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eyxbhecm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gllbguut.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kwqutfqz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2byexusvr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ifzyfxme.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jkwltlye.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kqaazlsj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2weqcarwe.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iwkwrlrc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2txtgpjii.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gocxjoam.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tlemgkyr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fnwhxgbx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nauqvpdk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qimqpwtv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ehufllxo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wuoypvqq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pmniuqmb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fbfhqrpl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cfsscmic.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2exwxmlwm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nckqplcs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zbmwxccx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cgcmdome.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2utzqbhcz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dhauojpw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2olwujugl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bdgdkjzu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ltwkjdtq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jtvkpsmf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gmwbhhdb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ytmokfmc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kufvtorx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wemrpmvm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jomftitm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xkrsvvzo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2meroomej.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2aaluulpb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2okcktlqy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cblhcvmw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vxihwuxk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gmjpnjhd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cmetlrex.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lduoqlfb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2negxjzdp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xgwuzgtf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hzoqpnkw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cpboxhkv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2scaevccl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2helcqxts.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kphqmwep.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yggkdssi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nsqimxcz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dhhepuag.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cqfljshe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2tlylitcx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2belydcez.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ghcuufai.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dmlrnpxk.html


<!-- 参考信息 -->