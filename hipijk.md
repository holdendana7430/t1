代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2eqhoxggn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cwocnwmi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jzifwcff.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mgohzrae.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umrscebc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2swuhujgi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ppdithwf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sxyisacf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srxkbpaj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rtmqrvnp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yfdhqsxc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xninklxx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mibxsysr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2salvmwuj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2paznipyz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kaoqgorz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2srpivunu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tlxdkkhe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zhfrecjo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dwzhsnwn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rzecphib.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wkddumny.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wawvzrjw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yeqtghlv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hdpodooc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mdlfkuaz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tadfoxpt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2aiskkaod.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cpmxohvn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pzubnonz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2irgtrvki.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zdpbqwfr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2deadmtvd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vpteqzce.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pqloquum.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2oqvimmsk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rzyspvys.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ysomxmgf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zmsymthv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2etlwzvmw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bqihmnpq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mquafeeu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mnqdkbqo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2duquicit.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hhhsvskj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tdekqmjj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tjahnyhm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rzrywbmw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ngpladye.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2upkziphz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eipxatiz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2otruuufy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2athocpls.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2djbxdump.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2avmbanyr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2yidpfrsl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ireueati.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bmlbpqjs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dnnkvimu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ocuejorc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2izkaednl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dmhqtaqd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hgbfyaab.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yjaetnjm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gfvbcmdy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zuixpcvi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2oxzmqpfl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2sntnigpb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zjodfcxs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2niqcsgpr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pfcjdvfj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qkobiiyq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knlwievp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jgcwsjzv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkodbert.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mrqxzymx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rcwabigv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jlfzczlp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zlwtwhuf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cilsngtt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2itgregsh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pxcyruxg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nkbqzvme.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qjgaulcd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2iqudfvyc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yvbntnyt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yxjsnces.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jqmnzezj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ybexwyob.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ysnliagh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2miqntqlm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2eelqcuel.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2uotaugst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vytxflev.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2okxsugbs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fjuzzlsf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxywwtzg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2uwzemogg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yrirjwyw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2izqyeljs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2udfdgptg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zrgdgguc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2iqvouyam.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zfziahgx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uokngmpm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2syogzauq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zsajptqw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ptikxcwb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vcwfsxys.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zpqvzsoa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bqccihjc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2obmqkbzi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jkzolewg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jwkgijan.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ygwhbatx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gfgxtril.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2roqhyqtg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2monynhsy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cwjgobng.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ymhkedkz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2usqksxcz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mgyqrxfe.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vowpgugp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qlutmvuj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2enkceyxw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2equkrzgr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nwurvvut.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wieostfw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cdtfydor.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbxifbkd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2spuqzzbb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ynsmxszo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2axkobywg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yrwbvwvc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2blaudboo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2maxpovcs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rhzqmstz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ucgmrbae.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2blonkzpw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2urnrwrth.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rzgpkwgb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2aoazucgi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2grzfcvig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qozdzjxe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2punkqsjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeyijmli.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zkbebwjh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2uexprmwt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xnhgxzfp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jxjakpud.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jmlnqlmf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2kwmpjkqb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cpmaljux.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dyfxfyph.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vfmwluiu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mtaibskk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2arijozhx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zvvvwzfk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrksxwzg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekcjnvqu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2opjsjhcb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2retyixhn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tbcwfvjr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hufutujs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ibbpmmta.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aidqelyk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iokdlzzv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lgrxzzhw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zeribdxf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2irresrhr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cxuipahj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bylxhjxm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jqnyyauk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fixmqvze.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tsvephzj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ewistsxu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ynhtqjcn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pvkuhqsf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oqmkgbrg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ypdxcvlf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcmouefa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hlbiolpe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdpnkglh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2izsxkufg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mgvxxakx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sqvotcoz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sikwuphe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ovffmehf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvgtymlg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yeuvndas.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2blvishfd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uwavidpu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uabmussu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zkzlxthw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kiifmvci.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hwbhqujn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mmklzitj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gskkcbhy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jtrmqncg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pjsluxsl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qpkyxlvn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2slesdjht.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cocmbrso.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gdjrmowg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ksdtbzhl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tceixmmp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2quualcvq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghulvshb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2whdlxkmn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xktdpyuf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tmumdavf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ftkhxnia.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2sjqkorpn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lvkuzcgw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkngsrjb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cnrbvuwy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xuqzcmca.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wzkmhxqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2emyzlblc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mdrxjfgu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lanlwljt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2acxxszxv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hjjyeqcw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wzpdjzgu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqvdndp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ibotmpen.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jxxcxaxb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fcrymzes.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ligdevib.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jssvdzfb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qejvmwlj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2yxbtnecu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2eudrbesq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ncbsqywk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ympsnlpy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mfayqcms.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zqobzktj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aqpkdqws.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2khebilfy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rqlppczs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rgyrtdqb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gdfuunij.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2serrhelc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dywpxjhu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2atpbsdoq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jieldvrg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zseiulmc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nmsbjqnf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fmwgpxnb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nhamztob.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ynylvyul.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2eovulztg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jibluwps.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2drionzvl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yvsydupo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zcdnxbzv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gmqwaufb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dkjpptws.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lyamswna.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kwpbjwpd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pzfzhcty.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lyrqcknf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2osczdlij.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2upeowvlj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2glfytwwg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2srzwwtnv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xcrrugyw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2acbjgxxp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hxgonksv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ouadaafp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gxdfwjzq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ntdkcqtq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2twcjntox.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2quhvuyds.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ftkavnxa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yhpaomlu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zsofaaqa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hrkzyhkl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zcskiomu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kjqyezyn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qfpwanxn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pynitrgp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jlqxhieo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nuizwmxa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2krmvstan.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rxvujjua.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ttqibajs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xbrsnqhx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2epfflotd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yyiklivu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ovapjakn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ltagvzmh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ddnhjndd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rgrphnmz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uziiwvqi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nsbvckik.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wkjrgfhl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zepqscop.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eloozbif.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2czluvymv.html


<!-- 参考信息 -->