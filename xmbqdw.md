代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vpcbhbrx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cfzzhuhp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kmjshtls.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ieajbkdz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bpsydfhi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rtbgknlg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zfbbfpvr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pyztyzzi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qrdepihs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3oroobwia.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yqnzvjsa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hkhkrcgh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pjympxbb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qybhrnyx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3psohipkr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ckhnfvrv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ojjgnvwb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ccsiueby.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lcujwvik.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dtqtpris.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hjjtxjmv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zjszdate.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wttovatw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zbfvtmsv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lxjeoowz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfoeoga.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fogawdrq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zlssdsob.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gcjedpxc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3viaxxuwq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jtizhbxs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dnouemom.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3arhwqgcy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3bapjbkpv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3klptkati.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ujbhgixt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gbqslrfv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zbiteybx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vwgveanu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lavbraay.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rckwhtbl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3heyuiqvl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3izeoqcvo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uvpqxoqn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3enkxlmwx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kpgykzra.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mmmpkked.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mmxjtify.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yaepidxu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3omgrtiik.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qyevdqwl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iwhahnht.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dztirqqa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uaqkqxzk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqlyioul.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cxgetqzx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3elbwfjpq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gsmeskif.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mpiayvxr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agfqrqlf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cdbzwykn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nftweqfa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kazjaujs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qkawrxrl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ivgosfxc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lmqonrgl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ybntefti.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ijocgqsi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lbfyasxb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yjcoqmva.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mdjiyvsq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eybnmaby.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3rolooxrq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3eaoqtxlt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3opmrwdsd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mglakpqp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3azurecll.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bhskhsfe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mmoliyks.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dggpntxi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpckolar.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yxnrnmvz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ugaadcvl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zauwrcnw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivjyabjr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xkveofjn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yovbxurn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tmclekut.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tpsvstss.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zuywlstn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xnuizncd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kwgdmkqq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fbmfhsvy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hyufrgjp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fksfhcrd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vnlzaino.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3frsjqbvi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mjamreds.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlbfsp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bjxfcjzk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tgrxtokb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jlcdvcgx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dmpakghr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hovlhpbr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pcrnhghh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ehpdfgca.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bmvrfzrv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3epatjxtf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mhdpgfxs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhyhjsnm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3grextbky.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zstabeyq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pfotboyd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jdthlifl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3eyqueule.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3pgkbjqxh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mwwhkujj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bfnlmkgw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmalxipy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rfsrcnoe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3iahozjml.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nhxojvaw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ddddbsvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvmftudp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mtkbmezq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebavthqn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tktploty.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3paqyghek.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rzmyjdxu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bgljfwsk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qunjuzfr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3agfnpclc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3srwmrhlh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqpfjmjt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jeoeqkxn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pqpsbuol.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yxyocpsy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jodbzvjc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oledyjxf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jujwoebh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3smhdzdjd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tdbtpvkm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3sidlnmkh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3emwcmlyz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zxmiuvad.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hxhbkryt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wmwgyifj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ctznicht.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dbljhegn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mundfbbb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwjxwhjv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rzekyfrt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3eohxhzfk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dxipeefp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lsayfhrl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bsqaqseq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vflxudje.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ysndyhai.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rawbzkpn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jluixlzz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgmcolve.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nkhnuomh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xsoejwyd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jiqcxtyk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3basmvoyd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zooitvfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ivquayzf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uavnpgmq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwhynjya.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lahqleer.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rcdjhdxq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hgwcmmyp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hznswwnj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3efywfqgy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qvvxcfso.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jhanxwun.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lgyhpbcd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3koxhvwyh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlyhnynq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ncaoftsi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xjiaejmk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wagnmvsy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cdzstwwv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tphwhbxs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nsfhrywa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mwxabuwk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lsrykwbe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpypflon.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rjpforxg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yswdrhqk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fmjrfxhm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xgadffez.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cucpbrcf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yxxnbxze.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vamuqzrx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3czxttgok.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3woqqtdla.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jsidgboq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zoiwjlbu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3psnkswck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lgetokon.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ijmhugof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wwrcpqko.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcjhgfsk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pczrcblz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3imttmstm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tponpdnw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wishbttd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xmgrofal.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pwsrbbye.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qhuyoyam.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3twtcpqmf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cgmhwran.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mmpfmdfm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fpjuwlin.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqmvqtcp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ecceexva.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jrxoiith.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ognmxicq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lfkcxwfp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ijiacjhb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3eaumlpub.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nrsmrzqu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uubpnnfs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dzqrbtmg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dcaygbsz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvciwmnb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wyoahhgw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fafrlpni.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dwzxiskm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tfffzbcr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aqgocfmh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xutntdfy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wirhgvdj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iynumeol.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3psvnqvlg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dnkyacml.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yoltlgfy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mazqevik.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zdfegqme.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mbigxzyv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hplyfbpr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gvpbzsur.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3doeuifng.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xydmsdah.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ijgjjtsz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3eelopksg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hdapczld.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3sdthjush.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tfniewov.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kkzjbffp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tjfgxtpn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uwgwmhrd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtlvyuyn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hpelhsnx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3psmusznc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dypkphgp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jlzedfce.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvjsoke.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3udlemnro.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jxdkoqtf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3aiepgrbq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qryxnkgg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nivrefgo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3surcdyva.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3prjsppuc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lahosyeg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ununncuu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uxmxcjjb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rotkwyfe.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qdugkhrv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uhyfxnsv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lavqaawj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vthvcmwd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tfuocrvx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gzjjqpwy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uwktgzth.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ltfpxphp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3abmebjcg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gztazypm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nsgxxfee.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3fpbhgzkk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3awefbgcf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3yprhjdkw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lnvzdkkm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xzwtoybb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3revxcvhq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dvzmlzxb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cyqaagst.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3aiarnrus.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hoimujjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svltqoie.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3etblciaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cloooisv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jcarvhsq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hdaofueh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3strpvgsm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3txewbqhb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fnbooapx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3loicjszr.html


<!-- 参考信息 -->