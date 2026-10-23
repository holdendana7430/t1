代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jmficfri.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hkgfoeos.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3paxjrezw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ckbsqfba.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uxtizsrk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxkpmsne.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tqvadirw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iyxpbhes.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cmrrhdwx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jtkjyeqv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cmoijnue.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zrozrflv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vebevybo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zglzqbvd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ztfzfyit.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yzagfxpt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wacivgje.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rlsswiht.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wewcbcsa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rurnmxgc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kxdbqaud.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jqgjsext.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3csymiaey.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qdgxejue.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bvuybhbx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wrbpkpln.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hhnanrwa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xbwzsyaa.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ahkuxwjo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vjwrwjna.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mrbqcyts.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gwybgtyi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ekvhpyjo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hhpnkvcv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bpjajwle.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jcfilncy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wpftxgfe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pacjqffu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lwgitjlh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mkvhmmsq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wrcfywzt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bxeyggpn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3svulpago.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3twyrecdr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fzpndhvf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3trqimyzx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kjdktfpv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wowlxymv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gkpgjgho.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vfahmwjy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3odywxfwc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nnmwicao.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cuzddgbc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pxvsebau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ggeujity.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qvvzqgyb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsnwjyis.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xcgmgmhe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ihbxrzvg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tlwhyxgi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bhrutxog.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ruijtxxt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rrbwtdqh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zhjmcsqf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xlszsojx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aeqfzcpn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rjlynfoo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ysthqfnp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3pjpfkvhd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mxprnrea.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wyaoozjf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3twzhyaul.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wzcwbits.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ikgzmppk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3idhndlll.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3canaipmq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nelnqujs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3snoyuuyw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vmigfupj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3snzgxmyu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zttzxotn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3khwuuvcq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cjaihomc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yfkpczvr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rlcaqzqv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3noewropz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3oewsptdx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbxcvvyx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xoitinpp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tyhmskev.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pevalvzn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kthazzzt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zztzczur.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kjcsjuhq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kllrjqfg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dlzajqqf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3scdaaxzm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lqrjsvxp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3aqzbtgmq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fwtpthhf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xrvjrtsk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ejdlmkyv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dwaxcaqm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kchmojqz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qhjncswc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhnyfjcw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vxxvmuye.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zikbogsq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gfoefjed.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfmdrwcc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rzklpqrm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvklxijh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fvrangzt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bohgupgn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nxkzlnam.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bzrwxsfo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fydvnvss.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3okcolfzt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3blgghwmi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aupmwehf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jcgfispt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kngcflwh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybpdnnjq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mkjnpvud.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3snczofmg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kdfbhuqu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lhyiaxln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjpipvpe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ekaergpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihnfcmrj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3primhkgz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zukahzsb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ihxoyzok.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ruzyoqnn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vgldalev.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cngedtnr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3omjysltr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fpchrdoa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jmbgttag.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hvnrpmzd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tzhuzagx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ciyvbgkr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dhesozol.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3eipnrkzq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3onaanqdg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kbwsrhfz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hupcjtxm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wtdziekr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jowpjwqk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ocuhgvwm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rfflrvry.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3apslvxqo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wugdtgio.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kjmkpder.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3curikvgp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pbssevid.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3orjjlide.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kygyrrzw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nexxqwxv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hkegxoyf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ecvqndgr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ubgduzzq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3boacudun.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3unefoxlr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vkxqkphm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jiwjqpsr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lkubxxba.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pczoozrl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vyeonuwx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pzhetvus.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jxeyjhle.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsbiogrf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3veowsftj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uxugnmhy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hobwmpgh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3smskphha.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tecsrbrk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3epepchld.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ldlkgaui.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ydheawcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vomvxknt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhmgsybn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmljgzau.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nsgpsmks.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tvbjmeax.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yazyvqnf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nyoqpkab.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lbasmhdk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aofjcgzt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pkpoirkm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nlayyeby.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqgqpkca.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wvwzfdxo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xwfpavwg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rapnqshw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3urotxoxq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwmalohy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qycyjnky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gddvuqwt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zleqqabc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zksumtpf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lbibirxb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3scigovbk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pemopubr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zsxtsyhq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ikjlqkrl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qpvbcsie.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3euohtzmd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3epofihid.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3eeyksfao.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cffojbpv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vxhvcanz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hqhwyhsa.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vgvbnjqs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3buskldum.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wbatbzsu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ndmakodz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gzparfjh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bxuotbxm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jddeggwn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xqkhfcma.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fabrowrp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vvavjqjf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3akxlubit.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kseasckf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hwcucpsl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pvzscmkl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xpgbnuur.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3otrhsemy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vbndkpzt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3akrtbseo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vpxmcmou.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kohikwgv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gegbfcth.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yczzgprl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tjmxwnqi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ndiqssej.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3spjogxrs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rblzkcmj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3szcrtmac.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tltbdihq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3izcmmkhx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbueklhv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vyritlju.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zsjhuuvi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gheultnq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bxlddlvj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nsotaspi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uufuvlug.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvyjxiom.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xmukhwxu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jvddjyki.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ikmoozrq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dtshjbhi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kcnotjge.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sngpjuif.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kfccdleo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3znuwdpqa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ojubgqgz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ucptrsnq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ffvdghmk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lzjkpzde.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pfixobsh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tmhceaqi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gkejytqv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3evqwqxvu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rdezqicx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zqrvoxmb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gymajkth.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qduzlqgs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kprjqcmo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gqmdmzzp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3txremlls.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cyrpjljy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jvyfgwwi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ckbswpor.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qrglrrlu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3igjedzxh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fvawozuo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uotcjztd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3eubrnggc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rekkfump.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kbzgzdvn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jyjeqngo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dpuprtor.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmgotxys.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3glfmfdci.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3etpmbhaa.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vnyrrohi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dddfvdep.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdaosdzr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hvxuzsxu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbgjymql.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dxsklntm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jnuekjer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3widulnix.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dshatqcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnzvgygt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3opjsoacp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hnkzmoiy.html


<!-- 参考信息 -->