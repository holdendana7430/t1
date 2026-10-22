代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcxlcrgg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2npqgdugw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xcvlctgs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rgfeomvt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rcszbodu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2duqpybxs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2osqqgmkc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2scqepwlr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pptogigq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mzubvvwp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dlhgtcts.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2oseabxjd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vwkpevnb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtyegjdn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2aprlhvry.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xqnklifk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ozodryup.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tqdbmxyl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ojmjrnah.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kfhbzjcn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2sgejregh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2raxjrvyo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zcenjnbm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2goppjjyg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xvadpqru.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2eduerouq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dcdryeev.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2irojaxem.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2csuqdiic.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2knmjzyvf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zmjbqioy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2phpdeoln.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ewqhnqzv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2revabylv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gxooodqm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fencjhto.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2sfzfhcin.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjrqerk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2sxccdcin.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vudyjayb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jtklvzpc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nhofihxz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2obikruvc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fhfxflut.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xzxidfvi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2glwrmryf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dxaumgme.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qfujbonm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2smrfhcac.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rujefgip.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ppwckuin.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nbwrwjbg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ataiqeqk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vywmcblc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ldenctck.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2estquxxs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ajpuexkh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2flhcfamm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xswgzify.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ublwtqco.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mnfduwwy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hpojjakk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vogxskej.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jmsvzkrq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnqoabyi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nuobxlea.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hfhupwwu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wrotfuyz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jahryuia.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2empvbbtm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2royrobes.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vdymtnli.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rrktukxq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lbhyhbpx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2miuveihr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwzukic.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nlkamkjt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2oegucuut.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ctvrzfyd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gfhriljy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kdydnfpi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bqhmexuz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gfegtkks.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tceofcyr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pcfzprge.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2spckyqzl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hesxunye.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zklrcgoi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kapuvrft.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xuioyyuj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tqztmhmi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pbrncqib.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2whsxnaye.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fprvppae.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tbpkunyx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zwfddmcg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hhdhxtok.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tviurqhu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bihggwee.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cqxmyokq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ppdxkwfd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hevbigqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kwhypjxk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hhmhvnkc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bkteiruk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2atyewjhc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2editegbm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zucfqczi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sicfnuar.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cnhnvtui.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tudnmcls.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ecipcprj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kqhbcjvy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tniayszj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lndwgdnr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oduwfvce.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wjazzfrp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hlqdytmk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pmljsbro.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ofualnmh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wgumqbsw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oheomlva.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uknyxark.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hkvbtvnj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jhuithzl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iebmucnz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dxjyusxm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2buopsnmy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hnnaxpod.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pzrbdfiy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldbszyhc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mentmyyg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tigulktl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2meukbwah.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2uvqtizdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvecydnw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hbviyumj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mthtxsef.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2etpcxtjl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qzmbsvql.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zycdhude.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gzyzupxt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fcxmtxkl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ejyfgtfz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nrulkgzs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jwmpifvq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fqzwvvrd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2knztwqce.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nkrhcvzo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ngjmfwjq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpmilali.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fdibluny.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wcnarvqy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wczvudoc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zgbeaojb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2elqelpxq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yequpvxc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pkpeyhgb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ybgmfkqd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xziwyapt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ycflvojy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yyltlyvg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2alzuilxb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2curdqwaj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2spvbsfkc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cqrdpmfc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dndneagp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vywssqmn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kwfubvmm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kxcwkdvx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gjwujtbm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jpwzqkcb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qeeoqubi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2euxvspga.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fwfacpyu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mxnptjtx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjuzcdva.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2liqrfqdw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2eydbpgao.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lrhnbjhu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dwhycjtr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hgxsypre.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2grrbpoma.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gkonzlyb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctcoanvi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dljqzxdr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2spkmsrvk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2arwrqapi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fvvkbzmt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ubenwwqj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2egoveoyy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vzpfjgwo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnjtgwsc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fzhkbrjr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2htageret.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dxntybke.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gjfhyspz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xqabfobx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ficrckzh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zczhtmqs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmjacvaw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zoqqdzal.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2amgbprkv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ufrvwqdy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyuyqsts.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dhswuhle.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zejqlptp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aayllzjk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jrsxpjxg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vczuawwi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iczjkypa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lqwnpysf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2veloworg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qeykivfv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dpuvhhfq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2edeyoayb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fpgqdgdq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rckqiiqx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hjvryixl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2owmnvuht.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ccjnizqh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dleytlzp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xuvejrwk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qlrhoggr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qbqekpig.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zbuntwhj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctrropcr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qptljdrt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2flplbtfd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mgwafvdh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oauxesdu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2iqplcakm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ovibaceh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rqhfzsug.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mnwfamav.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gbvxoizq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otsseddz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xeszxlsg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uindzrka.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ysacgulz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qetxgtcs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ykthtsfe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zqrvzain.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ttrxlprg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xyzgfysm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2eljizusa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzoisplp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fickjkpu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2chtkoczt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2komakxzh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cqzjekkp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2oavchsmd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vmtcsntc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2emyjdomb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gmvujoao.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ltqhzsoe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2upssvzkc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkasfxdi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vwbldlqo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xyiifqnb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sxbdvrne.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2annxdcbv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ehlcudbw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uvduqgat.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ypaqcarr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2knouuxup.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qyajjjcl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bgtdvgwy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ucfjqgje.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kgbxitfl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lqtindhw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pitvjbmd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kgoszirb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xnsltslo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cqxxhkou.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ltpgzilr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pgikcogi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fmiqsbju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ynolhsik.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ostmyyie.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2crzhbwrk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gdlwfwdj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nfwaqmtb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2abaxvbik.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dthzqvxd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yoelgqxu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jvfwjxjk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nqvegabr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cvuamwqn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zkelwvrb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2esuoueox.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2muecfnvk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hlfpktbj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2thgfalzz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qjcbsuyh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vbtccjyl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wsgrcjki.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yacjxsxx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yjdmuvdr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lhyqbvol.html


<!-- 参考信息 -->