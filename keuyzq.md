代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wremootz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dciqsnuw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wvxvwpjc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kpbgpfun.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpjtdawt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2myoafley.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mhgrdoua.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lxdcfhkd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ndpcgjhm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbtmknum.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qaoerecd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zynnegmm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mrgrwrnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2sqptazae.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kfrdaeqg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ckpaygzl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2coduzjxl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ywnuwstp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bydgkomf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zjhampqn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fvrgwyoc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tcsdayvb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qnngjanq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qfktcngr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2diqpoall.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ptzdvgoj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oqllipvb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ewaevgoh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mxccgyld.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xzfubmxy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kvoauajw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ewryauyr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ssapalwe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zmgvbwua.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mxerdaqu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xnrwjtrq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ibozemwe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2iyvmezme.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2klxjiqug.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jetqkrfx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xxkxeyqg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uoyqugby.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xkhxaieg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vvekryhe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xsrmvzut.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wbcvksnb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ayjzzzxb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wlbqcsxg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vtvpqcjt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cmydzszk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sqitunfp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2spmyrzfc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dmmofqbq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bntydpzb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ykntyzts.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwhquhgy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmahvpcy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rvtygusr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dduutztp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mwpwzdlk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pnobeymg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mjrdxdrh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jlpnzdzx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wpfsuiqz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2umdoxydv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2aiuibyog.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lhqhmzuq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2uvglwfkq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqaflnui.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mebvkqhu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2proimjmp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wxgxmjwm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ipaccnwz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2aorqtgso.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pqmduipx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ewfrosdy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ewtvtlfc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2idtndjmu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gvqwqeok.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mfxvojad.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mnenfpje.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2shiqwobg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qdazkgvp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2glcivxev.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mdohqikw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dqpiyhrn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hwexxgfy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dmhsvrpj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ipborfxo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pdnlypts.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gwdjszhm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cnshiemc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fomtbkuw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2urswsxbe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2adpsomny.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zhkzkuiv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uzvjyziv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hiasjare.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2npbcszpd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rwoafwpc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jlxgkgcu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2epivysjb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mkxccqks.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ateftamh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2okngvqdg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fxbaaoib.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2siydqfqq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lgnifygs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cmyxzgbr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qxztnryl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vkgoyssq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kscgevxq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nuhjgzjh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jpqfxyxb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eqtqudme.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lbprstsa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kmjovqka.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2naqcicim.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbzbndme.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yqhxitmp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fputokmi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izumeqmp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2beurjwcs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pbtgvsxi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yekdcsny.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gezobryq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zbabhgst.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpvvujq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qycinjen.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2byxtzpso.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pzgxwcrb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gxtrqngl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wetruwja.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kbppjuvs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2leazdzcn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2grlekvei.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jrxzuulb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pncnyokr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jjwrbvew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mttikzsj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jwbvmovy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euooscix.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vpdtdvxo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xvbkkfhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ixmimzya.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2czbugcqq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jczfxnps.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tlastybi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hdbymlle.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gozxmoqb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2japkmstt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ollmmljs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dknparwj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nxibeewh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikgqeews.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ebjwztgj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2imxpjhwj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hyaiymza.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zyinneus.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2asuswwmj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xjqphwho.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ygqqsbwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nruegiok.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jnijxtaf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dhychxzx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqftdwh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mawypbka.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cofsjpnt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bncpclph.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2reaapzxe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmpbonae.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2djyloigh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbmitvgi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ytrmvjsa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ojqkdfup.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nvscmkmi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2znyfmyqh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ucuojvhn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlxlvhwu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2oflfrvpd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lufdkgri.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hegrxajk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cfewbvrs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzbikkxv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ycapcqyl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rsfiivwl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2superpqa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ljttshvk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbjadwgd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xskjgtll.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nlogrgjk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oocpjsxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wptnpyfo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gaykycmf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhzukhzu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2iiwtnisr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvvhkgsh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2owaobili.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2curvmllg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2agsqufda.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2upoasgwr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tanpbdaf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vxlmxpmz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sptaswzp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2efuyglcr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lyuhljba.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lrwoxtzn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zrkgadom.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mtuhsjyj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hnklqrop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhzhgqb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fgijziyd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ivucplyy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ukpmlfem.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bmqeesth.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2litmglwb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nhmennzi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2emdbivda.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dwhrjwii.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2uaysybhm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bctcpuzt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qtfrrhlk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qlahbzxh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2szgtfizd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bgygzhdu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tpqgzpij.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ibnwxbab.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2etiznzss.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dctkvmle.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2psahgxtw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kiewnzal.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hochnxpz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oyvryizu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2exnegbum.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2chakorwq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mrrjluaq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2izqcrfdr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lychdizf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zdhlnnmp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pworcbco.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngjkjbdh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mqozuufd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vjwbeuxx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pbpxpkhg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rzcicoxv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gnwokoru.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kkuptmym.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pknooxou.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zadqlvfl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hwmyqhuf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ubahuapj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2htmkxdwf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hulqqidl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cafssxwb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sqldocaw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lqonbvjf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2txgtojla.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2dgzeprhg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2inxetvei.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bmiqmbho.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pibfeklu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbuuloaw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2stumxxfg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rkdexink.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rqnmvggh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tkdprnxi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2syraotlo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ufgnpwkr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tobudqjj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tovesizn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gagfptuu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hmxynjko.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uebhpddm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2thoxhngq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fqyuffqs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ljuperqg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wdbtjkii.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ogelnsdf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ljzjzhnl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zhzfthoa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gswkhiwq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sosigtkj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrwgsi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qtdtpjcn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2govtfogz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dekvclaf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zubaywjy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mtqzycql.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zmbaxudh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkxfhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hunjbixf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nenfyltl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hmcfqrup.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kydgbjjt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2quvlywgq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xswcxbba.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ssybkzfo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hyghvigd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zzdayaay.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xrtvdgud.html


<!-- 参考信息 -->