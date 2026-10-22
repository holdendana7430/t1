代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ibtxyugw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zuihqbkj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ssctiikf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2yzufxiql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2yjctyhhf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mejryimn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qsxwdudx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vvjmensf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jazewrzn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zmcbfjzt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxhbkfua.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zsaipgng.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2iaepnldw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ikufuukb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chedbnor.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sguyjpbg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mocuwgby.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wrmwqvlt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ofmckmsh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2acslpogo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2enrcokoz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dfdnagfr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zluilapv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2goxmhdma.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2grfrxbap.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qceajxvl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qpyziano.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lxfcbkxp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qzgjiyqd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2majeidae.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2potczmnl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gtdiqnlj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kbnndtry.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lpjunmeu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nkktcnhd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sylqqbzg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2iyyzvprp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uwcajbix.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ohutaeli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qskqpvfr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2uyvnuppt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2netaxicj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zezoilze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zfborvfd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mgmstmny.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fsvrjyqh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ttudgpqm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jrhxvdon.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2waxbsnmu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2drsetpzr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lnpemiwt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fkxdmpvo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2trdpcbdc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cueksajq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tfifkilj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2inqjdxjv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jwzoyuha.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2teaauksx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ysrxkiyr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2edefvrti.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gjzkkmpw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nxjmmrhp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxqurwol.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fndvclaz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fbxbzght.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkmkpxv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mrhirctv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2iqtkkcnc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2iuanamvc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qtayflfy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qjcdgvab.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dssdvcsz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mpvqwheb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uoopisjs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sknqkixt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mgzpdcrj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ciowvuit.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xjgjzppy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2honurryj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nympwpao.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qkinmchg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2obztbtap.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2njvfdbfd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mkobkbva.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrxcjxa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2demcxkpn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vclukizu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2eaymbxxe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmpfacad.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tbbkphgc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qxkrqkdm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hcwtmgre.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nwvtctfb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gcmnulst.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jcrewbon.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dhwntnrt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vzsvwjzy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cacfpqaq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2odforlxs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mslnbiku.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2emwpvrya.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2igcqwvjd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2touegpqb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zurujqat.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bydztrxr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pfiydokg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nwyyslrw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tessjsby.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbqmce.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hfppjzmc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cpxcsdfg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fzrxevcs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2yonjodyo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bwvsrbua.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qxasqalg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2revmveph.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qavwgslx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aqaipdbx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rotnazbc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ylhnjqao.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kwiqbyxn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gxiaydfo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uqzknbcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xfobdtzt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zepiqtjq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pxwznzcf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ylxoagwe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gyguqagw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sizicsof.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ypnitime.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fqbnogdw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jxlqsbem.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dojjdqzd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2recpolmf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgythcaa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmrkudyp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tawxmkno.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jzokkrjk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pbiwrbiw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2amcnyqkz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pfjouzcj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wizvuymq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yrfwaohf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2awrqkvjf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mvaovoli.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eygbrivh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gwpxpesu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2olzqbibs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2oznmuyqo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cxftdjel.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dclnozki.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wsiffltg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tgyfihcg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yapvfgyy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ofazrkay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mthihhln.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ivlwntvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmolvicl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fdiobnyi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sbzoeasp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xnenxhto.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2kwwpbffk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2shvjgqms.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sueqsbmw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gnnihhdz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qlcduzjk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fghfvmso.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2csbcdofy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2evhqiwpm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xprswjov.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgnnozlp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xucjeumk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2tsbfewdn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pcenddxz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wzgngynf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aboasyiv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2brgfqddi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2txwmfzqq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ntonmdqy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wxmunmcj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2isgswomk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cooipxqt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fpmjjxoj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qmzlndlm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2enmmxaae.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fxgekdzz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vcpqhvfn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vanuaqdc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xgosiyiy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ffvpnflm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iofgqbkt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2urnfgwvy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tvujcuqs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2aeyqmvod.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lldkvkfw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ryjbzrwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mkzcfpuf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2byucpvft.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dzsezzcp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2chngmxba.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2oyjxurya.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ujlvhjoz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fbxbmrux.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bsrwcoys.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wokzzptj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xctdemdn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ytkyvxcs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cycgvwxe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xiyraxwq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ibehzheh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lkicpkmt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rmrhletb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztljljmz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zvnqbnli.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rcxchrlv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2neecelau.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jvuxgydl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ifdvhzmh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2egtkuelq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qzagdntj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2inbiwhek.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2emcbqmum.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xqvjchwz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ufopmiim.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgmzbnlb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cjhguuvk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2llqtmwhj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ydeqoghw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hfhoxqre.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2aiyrhuoy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ohubmvvm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ymvjhwjl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lqyimcxp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2drqmbijt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jkbmynod.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2aqkwgsbx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2alxjfxmo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mxyomrbe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pcbbajxr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lrpxwsbe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2anbcpmbe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lfmudqeu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wxljnpam.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hziplrjb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2exolgqet.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ycudmrjw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vflmeoed.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgstnuwz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qlngjiqg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fcteqgsu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vsypdbng.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2klxncums.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2djkhbirj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2omewpbmi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2divtwltw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jlolhnrz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhvwrpwo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ipmqsoim.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xbeaqewk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2glaelmza.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jhsafgyo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gptirsls.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2djxytzjs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vfyuojmy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bdjjkcdu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2lcykwrwg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2miumgwcp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ozgnhnzw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rxxlprpk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wpdeyven.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2aucatgne.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tswpxhiw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bcgaevpd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xarhsyxb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lqidqkpu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gugvzact.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fttqztzw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qwtmiqdw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nnalfukz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xyahosmd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ejwjwsuy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dteeozqa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fhwoubcs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fdacwdvg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2miqnymhm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkdjmmnj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2aisnnyab.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2zhmsuikf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wyefbrbh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wlivpqjf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gwsyqsby.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lcxwwlmu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2isahxbla.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ymmrfkmr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2emlarhnd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2uodklgfr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nmtptesm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wvibiatt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2knybculi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2unxrdlqb.html


<!-- 参考信息 -->