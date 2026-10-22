代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esyhwsmn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2unkdlgsp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cywedsgi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bmqdtkmn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fwnsuyux.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sdjjmjdj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pkupwfki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ovmirwsf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jqeufhhe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tcioorqt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ojbdyjyh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tkghhnzw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cddhjsjd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2scgcaptg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zpozexmr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gidgjfvn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2daddnivj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mgjshxyw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ofegmjyz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2eukldtcc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qeykyrsh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zykfuqee.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2pnhqywul.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pkbygjgt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2deacwdyi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2puysvyqn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uuwknvrr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2agtlktsy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pnfkvrrt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ulvlmkbe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mjiabcmo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pfqtuohh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2looisurr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oulptvmu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mmcluneb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yyscvdgm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nuzcpvqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2raanmvol.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iikugjqd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jrnljkcy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2iovhjpvd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qxyvhgoy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2knrkiolm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vfirmvis.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2udygumvp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qfrbrtkj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sowaxldz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nlhjwkvk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ltgkyjiu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xdmlxvoc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2neyslbbt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wpoputhz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajcqasgt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ylpdgzab.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dreqggch.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jsvlbpuh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2enxrtvrg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rktwdgjm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sncgyqlw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cviamgxm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dehohxvo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ivhptixj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2agysxxyk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2urdaqkxp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nevkvjhr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qmriukci.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mbcccpnx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hgeiaexj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zpdbttjw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wqjkcpql.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2chpvltrx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qfxlvjib.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dbedmkjf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2svuqjiqj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2plqgimno.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ybzjavoj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2araixsfu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2icpjamji.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yeahpokl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwqaisn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pdnsumdj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hgtrakge.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2eakafnkl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kegerxxt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pbiskdcz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2abzosbff.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fohetdoq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2oawxmlee.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ewyvsvxn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uuowzpyg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pfebwxug.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xxcufnex.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpakpieg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ilxdnkkz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dhurjngx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cptlzukw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylcgrzlf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fniekwok.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gzultcyi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxxztmwo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ayztgsnr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pmpcblck.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbavirk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rxwqhgps.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tnzrsmga.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kpjdqfir.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dlztpfvx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2flgvcdeu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kzqzqlek.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pasyulqc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gfezmdbx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ijsvkvij.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vjqooqmr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkyzhtza.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2amlmfpoh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjmpvqze.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xlmmdwiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfbprfzp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xxagsmas.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxmavmmj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zxbylxpl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byhtathv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gabpofim.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2slkirube.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vkhgbalx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gfqckivj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dbtcmoyi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jhkcqiul.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2psynyfds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2siokjric.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikphhqem.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2oeztildc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2oyrchzic.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qcgkjxam.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tsotzlhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzdskyol.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2psizthnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aczgaxub.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2aijuhiza.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2osaorzwq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2preugcgg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2sobfacgw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2iqfhsnxm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vaqimoyt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cpvzittl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zoakisdx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rnrizyrx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tioibmhd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2upeahlbe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bzdkgnim.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xsbgbtwb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhefatia.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2duagcyji.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mpeqmypu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jsllaihq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mffktmjb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ykrtarlg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xlmptilz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2frluwxcj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uwwnqdui.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qzrzhsjd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ouodntik.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2etqvkphf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tjlvbtrl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jvdathxo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2oahjibkl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wvufzuvc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cevcdgqg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gsbjywvy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hnqgbpby.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2avpkgogr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmnaxcyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2becrxjyk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xqfpdjwa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jospmcdw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ndiztqnm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2whcvpvwn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2euhulxga.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxljoosn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qecesnop.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mdltgzdq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xuesyspi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rofqglwe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2niwlxirj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2iqwaswqn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gekwefla.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljsluobt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mojxhkpc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vwrhosdg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kylmniyg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kxsxzwhc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pfzwklxz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2axokgcjx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2esejlyqy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bvyspqyt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bgvgqcfh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xjemnoui.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jdywyymj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qedfwstw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hlootsxw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dwqqxkya.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qlozhujz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xrdavpvb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lpscymys.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqckkdbj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2yvhrfzce.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnvqbprv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tvusogps.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2monenljn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bciwmkns.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ognfndxi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xbhtiyif.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jdvqmwmc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2orzffxkl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2eahwsvdw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mxvivffv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wonzplhz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gkbzmilm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bthnphxt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lywqispx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hvidqwdh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tkpgzevc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dodnfuvb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rrtnvtbb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mpwrcimc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bzygynej.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wopcpfxa.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uoluhftd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tmxmigiy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rdmyawfi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mlwakrqm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kpjofsda.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zcqdyyep.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jwurwtpo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vetvokyj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oitlqgdr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhmiihcz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qwhmnksi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zcmzdsig.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nhqljbiz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2eiykcmng.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2arqgobjo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ucefvfur.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fjmyrrtf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ppdymyqa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2adnjoopj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2oyqrgymf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dejvxqdz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ooytlhlo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tlhahzqr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rfwvphgc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qseqdxhq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2enoqqnub.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tscjmkzw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2iaacxnba.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bslflrwt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2njyurunn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwvljfoe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ztwtvwmx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ineopynx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wbnbsjqf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vesiixhe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mcakzeer.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wsdridqd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pkqfqibs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2shkkazdd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vcztuovl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2msgplvlm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dprdkcar.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wytanhqt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2trwomlou.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vrubsypk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ttxgedzf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hxbaaufz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rplncxkn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2euzqfvmd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwnmdx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ghdmacpv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtmkloxi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vpyeuzcr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ksvcnzki.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rmxtiife.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2prpdarxh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pczhrdey.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gnncaqkc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mnqsyyka.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mmzcpqgy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mbacbpav.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hpfzaqak.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rpkmcxpo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2scjhvejj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ppbszpxi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2arksdaor.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2elgewect.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hefkllep.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tehnfsak.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ckefnttn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nhuedust.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bhxoxgjd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ltsydnds.html


<!-- 参考信息 -->