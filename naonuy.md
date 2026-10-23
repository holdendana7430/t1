代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uysliglr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3sqcznvon.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pyiazhoy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3knxlsjze.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kuuurttq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qhascgws.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tiwfnejz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cgrookfq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3spvvztbn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qyztpboo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rxmeeswj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3aomswswq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmwpiy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nyurrtqu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3iwuzdafe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kqmdkvmv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ymqnwbmj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yxumqlrw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wmcqdecn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3wbhkvkbr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kmgtlcfb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yvbkfvot.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cqxgqmye.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rspxkewg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ydxkaiuw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dicqcknm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xzckjrca.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bgvdedup.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ntogfaol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ljzzoxia.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qiwoaxhn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3roqcnqng.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mpimaqfl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zntiznlt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3porsyqon.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ougpabuw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rvnhplbq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3areiezuj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3uxmlvgfs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mbbapiif.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bdyytsss.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mwodxnfu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nxwltdmg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bcdimwqw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fjiyfsum.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ixdemxtp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wwzynkui.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3odvmmxdk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3utvmebeg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3avslpgdv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bsjmxohj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hmwtbnkt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tqejirll.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3svyofypa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mfdnyxwt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gnvwdbzu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uuzpbukr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3adqwqhnp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3blrmecyp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rohrepoa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mqbaxmrd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xxyokivl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zcxalwld.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kghkcgcr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3imsworgp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rivteqqj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zpvbllni.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mqhzhcwy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vroeqpzv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kscczhbo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3exfzkjuf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3saezikdo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uwmvrnxi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tkqdyvcl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bmzfngkl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ljzadbzx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wyjhqhfe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3uhufwcax.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sbnclrxk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pmcizygt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ipdcieqg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rwfiguvd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vasmlcjx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cebkgzxg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3otocjwtw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tjypbrcp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ieltyytz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dopnvrfg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqxlayyq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ltobnate.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gxhorelc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qmsdpfjl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cscfduhv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jhjutvfu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oqxmhmlu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sykzhmsa.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3abokiypw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3srcyutmx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ntuqaxqx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lxchyywe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pgvuamfi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gkzgidtv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gbpjkbxl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ghfhevjo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yptrbogs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gkorfbdw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ghsnyklp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymrbells.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sjkkyfcx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtegdqti.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3abequoqw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gusfipnt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wxhldtvw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zixjyowk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ejbmniod.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dutfduaz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vqiwakam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mitoiqom.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vaprpmwf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3sjyuwcoq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hdrtathz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zimzvlkv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zjqectsc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3szxiowji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jmqmahfx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fjcfiqbg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rvjpskgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3couepbcv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3oszeswmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xltkicsh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jktelxiv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mwttdjqr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hkjseder.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3izhvomvn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gbtmgrnu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uzkqkdsp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hsmqmopn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tyeqrvxs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dvwhnhmj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3skthypjb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqtrgqae.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xlorufsn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pokaktxt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gyevlmwn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3urlflghu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tavzuogb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gejgthge.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vjbnvalo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wwuubtqh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rgxoymck.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fdyvsxie.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vtgreqdw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gktduzfd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gkiihvfw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rrtzuttg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dihgmulq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mgjkheji.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvclyuwk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ljjhcxwp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nhrrnjwp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nfygxhkn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tfyfeazo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gwaxjeev.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fdqlgpyb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aaspfacp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zqopuqze.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3boriykdq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rgeknpyw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3inkfmmgx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kavahzgt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jyxuodvq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rassjslw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3axfffuvt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cvdhvkok.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpmojhwa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mxuyjjjq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qnxrjcmp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gfxgisoe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xxepidrk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tblfysfb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgdmgetv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yihsdbli.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3molgzxmp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gvmuzzaa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gordqmjy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gspuvpjw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rjwjhsjk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tbgynquu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wldslqhe.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jqwvekea.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vurykjgj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cfodjwnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3awfbsanr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bzojwndl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yuxiwzus.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vavdyudv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsdadqdo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3agraafex.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcoofqnf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nczxwuhs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pilybhdw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ucooduxl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fgdqouwb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3idmybohb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3otfelmnz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wexsoiev.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zfwqyyvo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nejzeqsd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qfrywzco.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qjxokvqb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rgwkkpgk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3opgqbibg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzinng.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wcchmadl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fkbkffvv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nlpnvokz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tfcxjxpj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3okyzklhe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vysqkjqb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zgwffhss.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dinmlmky.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xiloarmu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3retpreom.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tlkqqhhl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ixtapqaq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rizyonzl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qxwstmxx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iedvfuqy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hlzjdynq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qlnbmfmz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tmhrfjbv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dmhxrfpd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qktykwrh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3benupgaq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gconkero.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yqylmucl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hihdvhob.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gkgytzvi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zmemxsra.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uglrjbes.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uuvrtmea.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bibuisrc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gvsktoxn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nczicpss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xjidqswm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wlqmadrj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pktykwtm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3yxaluqjb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hjfondhm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zozeidej.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dhiizkgl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ugeizwwh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yqnmdril.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3covqusxh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xbcpqrwv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sgmmwcnc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3takpwmos.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fajzczrp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3leffnkue.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kuxqczgj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vobxregb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3unshxlyf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwnasoa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3imcerhkn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ufcynvke.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xoqxjyjl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3epqvubxv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wjhxciqa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vefuewxs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pelzjlwl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ukwmmvsp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zjhqvrzx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3psvnmaqa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ohyxxjwx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nlldaeyw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qfclkofq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mnnzxxgd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xzghmjwt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qjowphdt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qmmsrcrw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3iulfxyet.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tvirinzd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ijsrvcyj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mppnmfxg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3eebizqet.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxwhgvjn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ugariyom.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3clvkmavj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bjvhyndh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nnycfvkc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xtiqcdyo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3odebanmd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bpdwetrp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jcxlhxlo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xltmurjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpnvppif.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ockqmlzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqynignw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3frmikhbp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3darrevmn.html


<!-- 参考信息 -->