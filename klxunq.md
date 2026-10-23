代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fahjkwpj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dktiztsk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3owzwseax.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3afakfkdn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kxzxuwey.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qucvofkw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kdrwjwdq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tvfiklmw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3eawcfvow.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gqgvrgom.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pzxoqosf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ttjznivz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rypipwza.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ivmetuqv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ggujwzxt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zvgsjixh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gxmtgmtw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bkitrunb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3arfaogyq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rpiyraov.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wvuvgrgz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwkdmrz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xnfkkqtq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lmrgteue.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gogwwowl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxpnxbkn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gqythwlc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3eqqqjgdz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdwfldrh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zexfysaa.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hbrdkmir.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ojynhjrl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tckpigga.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nqrxrnpn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nxxjjzab.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lgvppimq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zvqiitrg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xakosqqz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3typuhlqo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3btjfghrc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfprkmsz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bhcjnmqm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qfbakjgn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3brabawyg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mtvfgkmb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zyiesaoz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hbdmzuap.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jsxorbrs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rjbelqwe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3msyuffam.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bfavnwjz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pdludxbf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qpwjaxeh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3yjfdhzep.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3boffsuuz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fxtuqjnu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bxkvoitw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rnzfolnh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vaczqltv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cjumgqgv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dlislvzo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rqmampqk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zeslqjcl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zbadkzgf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxzdeaix.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dlznypnu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3phryifzc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3prhfvrbi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3spgvtvmk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gnjuslyc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3twdfjomj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3evmgwmaf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdpeozoc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kcznsgoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dgsudaao.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3reqqxgoj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ebhowlag.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lprwmgvb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ittvvwup.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3aynaclzy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aruvritq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nxzuksvd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pkgtqkfb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iaprseoa.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tmzsdrgm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gwiscqnm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3btljjcfl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fresffux.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3finvxwcr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvtvomhu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3udkywyrj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3usqqozxt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfltsgqg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zxurtkps.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3akzoacxg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjuehkid.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hdppdlyh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mapbhsbk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tebmhefp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3chijdspm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rvvthuyg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vtoiwzen.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nwuhkxre.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zerzldwc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ltoqtsqg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dnwjbyts.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivxkloqh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xtwqvbhn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ozejrvpj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qxbfovvg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qmqkspaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euuanggd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vpfnoxrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrifinpq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oqfrxunk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3iyfzqhnt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3drvquqfo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jpnbwngx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hcudwqao.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uujnjdzw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mwafufcb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmkpdjcs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vjvwtijp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kthjyddm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3czdwrvvg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mrzybset.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3atjnrtiq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3krpyajuq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vsbbbejo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fcljfqxa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sfnnfqom.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vqfunujf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nfjhwpyo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yijidfap.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vuemvaup.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3zoqtexpi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qhdszkmq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3akobruzm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ryiwbpxx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kclbefmw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sgzvnxtr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcepwcno.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dlthutet.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3usvgrdhr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mbevuidc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3scdpmfvh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mpvghvoj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3akrmhpeg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tirndawe.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wqmhlvlk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3poiaybrp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3audbiyhk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jgkbwegw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gxrphhjj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qjahnfie.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pbrwuvkg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gnhqjqnq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3tpmzzuve.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3olxyzjct.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fovownuu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pznxojoc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jnkusucq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdlpflhh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jwbcriro.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tuplplvt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cowmnhyu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3haiuxcpn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pwpdgqtp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3iysxlhvr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgkdgyhh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cqvbhlsg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rkmqdoqc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rqmkzskc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zhuaenvu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rtkvljbk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zydmbybn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zvnhhcei.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tstyzgfm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hjrhwpxr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lhnwkvkr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxejhoox.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vbstirzy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzwwgps.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qdalmmbt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oprluffy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3isuzcdsh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eyqvsppg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3roydrjar.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aymvvhyi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3suqdkxqp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jbzajcyl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nnnxafkf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3upavvysh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zyytdstj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xadgekfb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tjwppjtv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hmhstsrz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mkdthhrp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wrawaxdu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ohcnrkga.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ygzpwmrs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fbiaslod.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qsapefor.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wtfjptxt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3puwmhmir.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3htxpxmkd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ezzhzaoh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qtutkbyo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xzkuwkgp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mgrmxgrj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ymypqggf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mtnpatyn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aouusxya.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ziakxpxw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eaqunhur.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xiaovlem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ibvvgrxo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eqaboidu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wyoatbxw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nsjceybo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3oxydarne.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dlvaxlht.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fsetmmem.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jsisefqo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xmwbkzcm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3boujtioz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3scvtxqie.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vpfoexgr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3brvcvdkc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3blvwmpwj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zxcdkswa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zarjemek.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3cnzdlykt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdeprnfd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lomsquyf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lohhixlw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zebxrjae.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tmfqjrlm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ciogbcte.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vyskaeba.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ttcuohyd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3eyiplwey.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qnxyzykv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vxoznscn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nsjhpvuc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3akcdcigc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbcyafl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zxmvazzo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ztwcmbbu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hfbllial.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ynytkqdo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ynrxayph.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cbfsdikj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3oiwpjmdl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gavebyuu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3avjnzekv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jozkyopk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hwmgveqf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3idwfrvqr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zofalgxt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hljvlfqv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fahzqywb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxnmlwnu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qykhrfzr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pxysxsgn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3loveqwmw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ymfensnc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fjmttqhg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hlufjmcp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zepmvpwk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wkrstuww.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pzpdtbsj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3syyvoxjt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3stgrafsm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3buwkynwd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jlanvlhe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3atodsrhh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3oxvsswjq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yljgujug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezedlfwv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jfbslphy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgciqccb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kzttaphl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rmvilrdv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pxuqwdxm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fxnhrsim.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3roixvdof.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ekydlkob.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pfpmcpvq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jfqvwgta.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rvjckpxj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3elsvgzhr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cncsgzcn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3omqhxzvq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ryuawmiz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nhycymng.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wolfdgyx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fmndoelo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qsbckbib.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3liedqefr.html


<!-- 参考信息 -->