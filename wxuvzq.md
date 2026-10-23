代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wwmszewp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbrafiel.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3egdwcqox.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqzqzeiw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wklrtlwj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uvqzlxhl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jlkfymbh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qhlnilha.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pfajdwnk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kgxaawpr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fonwmehh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jhogpwnd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zlfkmcxe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ipynkjiz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jdpdleot.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ltknskzb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jphzezlr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kzgwlxpo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3isksmctk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ciyqyinj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mlcvofje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jotxqdub.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ttodfncs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3muebrblo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fonhqbjl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kzyyupfl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3goyxoxsw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3azbriqfw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3myvxfdqn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhnriez.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nbayojen.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lostohth.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gofxuqzo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nodebmdp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xxjtnkbh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ryhcsmuf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3sqcutlcg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ktztjkxs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gnmrzkul.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fqgbxnbw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wzzvdkqw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3sbydnkpj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3acorllqb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qozzprke.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3idtdgrns.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3txcleuqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lmupzwkr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hvrnturo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbdvuoaz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ibcastfv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qcgrubfn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pyvwjqkb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qxyqtikr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3pvwxduxx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qhubxswt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gwswpatb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lpipqoov.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uqwyxkgh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bclgszqo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uwopewka.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ouhecefn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3crcyatfr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3afanjyww.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qtirsznc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kfarkkag.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lbdrdetk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jxwawiwa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xyfcxerc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sruumota.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zvjlkdba.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hacoxowq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ohemhkch.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rzgwfspr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bwarupkl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uuvwlpmn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jykukflr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3njmunifb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qhgfdkgi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zrvruksn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dssjiogk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3imljbwtd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yvjiffzx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gwijzrls.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kqfkdweq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3umrgnmdx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hctgmefh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hjcqjzcc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3cfaxsikv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3wyxhqcax.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zxlmymog.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hychleyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3adaekceh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cvlhzkjp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3eckyoxwd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3odulcvhm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dvgagouu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dxmzdkxv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhindtrp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3degppepn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxguyfas.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3aqiesgqb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ekiyiuxx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjdvmvrc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhzqtfzm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sosuaeni.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uprkfqvd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uooiqusv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vbhhrdfa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ecygkzre.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3flbzgkma.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wegsnfuh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3inuqlkem.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3oxxvidek.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qpladrzc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3leesizqy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bxmdjbzy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rxzvpcnx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3umnknmxb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lcfoceep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftczneme.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bwczwadd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrfphoee.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gdxnjfon.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jaorrpmr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wbenxnlc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ffgznuim.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qnfgpqyg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3oxlpcozz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qvpttzgq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnzydeim.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3axxbucrc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wsacyjss.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cevycjdw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3snbrtkyp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3emvppbwa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvyazxnj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eflrrrxd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wyazmjoa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xsjqvnut.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ygvmibgu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mfgtfown.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mifwtlez.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hqjskwqq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gmgzlttn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3sagzodat.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tioppcfm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3scmoepwh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qduuxajm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zmssraqt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihhvkdbm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rzkmuxob.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jqyymkcn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mluthdqu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3sbqcvoaf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3enzxfdar.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wwgguzrj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kutdygjh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ywfongvo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wezlvbfq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ykaqvxqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xiheqhnz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gtfqolvh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rwksqnjg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hjxnfxsy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tetusubt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3urgnirug.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbmmjhpi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pqfwkzth.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vcgqqnta.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vbqfhage.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dwialdkm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3welcfixb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mmprkpfa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fuvgpmvo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qlqenfkr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wetjuwgh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtxwvzba.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pmlzvlzn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zgdxdmnu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uzawurdp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3emrvcsvf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ycjkjsnh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vatztlri.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kefjllun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wedduzwt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qwsggenv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dcknrfzo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zsxvvuxd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hhkyqchy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hlskntym.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ziemtfbn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3azyfuhtm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wyarntoq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hmbcaihs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xdnqwnil.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oehibxke.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pnulwcku.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cdamxqrn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ynsgaslz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dltkkvfs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gaohuoof.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3tpapmfdm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3njsofsic.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qpsivcrp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qiimalpd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ybgvdllx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hyypplcs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3deyajqud.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nmnfuxus.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3szhmpsbt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3maeltdja.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aemsxroy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hhicokrr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sxbyvjjq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3adxjmjbx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3trrujuci.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cdjknvga.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sydrlcde.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wgalblmm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xburbwrh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3afpktfue.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lfqojetk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dfyxjprs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cnzreliz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jhfjwoib.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vuothxgj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hkjwrpsp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pihsdzzq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3iokhumxz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3clrxrgxg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ybjbutft.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xsbuqjss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3sytawmxf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsxhvjgj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cmakymyy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wmgsxmgw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dldnmcfu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gozyiwqv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3smcvkwjh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zrkcmajy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rgpdrgdu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqanetcc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3idihtxzm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sutzqzay.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ccapznap.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ncidblkr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3useblblh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3akusaina.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sjbgwvpj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3joajghjz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xvheynde.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3glovsgtf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3omyysmwt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3idsyulce.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3acnygeig.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ksuijybn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nysowhhc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3atbnsyiz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vfvsfbul.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3edfsroer.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3eqfxquqx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cugcdwfb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sovtefse.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3liahbmlv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hinzoblg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3loelaqkf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fgeevspi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uuwlbtzg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ovifniww.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dgwfdlzn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkvtkgdz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3eukfeifa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3htpjpstw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ptcxqrvx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ufaddvlj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ttfkqiyc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3eyoxfsli.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tzidqhoj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rcalorze.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hrutbfpj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gmrfaopn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tnatopkt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jospaacc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ozrhwjcs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3epgzqyyp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hmwotijg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wawizdlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzagkgtn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hdabnsjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivgxccus.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hmdjxkhd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3lqktqvzh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rihnvbsr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zoeohhua.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sjrdnapm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fuznsozi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mmrijhmd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3oylousky.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zarzunvb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wurrbohk.html


<!-- 参考信息 -->