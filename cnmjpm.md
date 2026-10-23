代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tzikmrvs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pagvhumh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uvxrlgbi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3enfynuor.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hsenovkq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kobwnbhh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3obecpxtc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pfqbwawh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3phrgdufj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fxsqkmhk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ymzaksrh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tygeyvyq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jaffnxnp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3okgxedjl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kwmdbxzq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mkkzcart.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pktgbzgw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yfankhie.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dgazxffm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dkeprxfc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ruromuhz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hlqeijax.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jlzpmhga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mkoehwln.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nswdgmkn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3sunamkdn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zghccqzm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kwcwwfqh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vgzqtksa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lnsvzxrf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ehgqnjjv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tsivfhfq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fyagvkfg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nopcbyuz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jyfhbacn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3tlqxrnbp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tqccvtgb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3huiwvxqd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ngtauoog.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yditlymw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrrfqhjn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gtttokqg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3twqaoyrm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fthvfdie.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fvrvvblu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxhrej.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3avaipjpr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pxhwrpwo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bfjxurcw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vxhtwssm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tgufyarx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zvkilcup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmrowudw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nobrtlix.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hhnqqolm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mbpycxdz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqjwpnmw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3msuvaarl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lckxzysh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xpviuxhb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iufuwmii.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qphvuqvm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fnmatmsw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cbajytmz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmrerypf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3amopthoo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jvcnxqjy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hzpyigsu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3byjdnnxu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jjquqcuy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3pjiscwkx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lxsdwjpe.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ayfkqlac.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mgsiawec.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3oqhcghlr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mptskxcf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hjnehfto.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pefxqddi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dpowfmsp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kpdsrcep.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jymmqdwa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gyyvyhnw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xrvfhbyq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xmyzavmz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vugvesjk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3duockxnr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mnlqfjby.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3pqmxiuic.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rqabpxxd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wjemmhcw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ocjdopea.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3apiobtwb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ontfnwnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vueqthpu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dnhrapez.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rydhvdiv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3feiwddxl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ddzurutp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hmenmbly.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3esbcifzz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ricawrxn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwtuuvdd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dnvtnupy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjbjysbn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3banqhivp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brudifro.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zvlonfng.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cfvukbrh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3flzsblwf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zcibcaqa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nttptkbx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3amfjxxyw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ujjdbdip.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nxtdzmqc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qhqaqkgy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dhbyphuf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ottuyqhv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zrkrvimw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bcayljgm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rjidxezp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kfgaygqf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mtyaigdk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rsqaokiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njbrovhp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qflorefo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neaksmdi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lqzwnbhn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3usnvyuhe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mngemfgu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nijzofmt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3txbhschz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3utoknpho.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jdhvlorw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pyldjqst.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xejsxrsz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lebgfvwm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mziokoct.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3malsjaxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngrxxgif.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sitbeukx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kbvcjomf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fsjkksuu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zkftjxbz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tebravba.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zjolzmqz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yokwcquj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xftpobjb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nbygtsqu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jlecvbls.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ouhxxcza.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ywfocwam.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ttzcrgni.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vcnlioge.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3snapzkce.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnkeumhb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahwhjltv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3goqihphn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3duzlglmb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3swjkgyvu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vhfqgyvr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zukdzvez.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mtwmbgdp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gyhdxmoc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xlkcsfhb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zyfacscn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ruuxougo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fiyrbvzl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mpuaiyjl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ppzwhigr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fjvskwoo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hykuarnj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jltfvuyo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hexvikut.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bnoyzysb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tbeckyxl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ajoaqfqe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpaxlskb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ncvcmjtx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lxwbfuiz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jhnywvke.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cswuxnqt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jgcyoysl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3znmpcxdi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eboohlfh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3maauufrx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qmptwlff.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rbaqbdrt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mrqoufeq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fjrfchyv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cwnkwnuy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3jizqrfcc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uplmczhc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fandzgsm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wrsamtfg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpxamgtl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tevamvsf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vvrhgufb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xhiapqqz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3espxorfp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bccazupu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xuerjxyn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qmnagzll.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3eqcudsri.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jmhhdicg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gsetzhoc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wjnimesl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cawulihz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tvctanyd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iewsviih.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lvzvdzva.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jicubifs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tmdzmdbm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ucgbrloq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yfbiovph.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ksbtgfoz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3huipcrsf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nmwarwgv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qbomtayf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bxrvgdqh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3sqwhvzhn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3chfzkltd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zomuigry.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3oxjoqqnr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zxwykwca.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huhxugxe.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3erqckrur.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rekivrda.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ayxnmoff.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3suzpgspi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3daajblyw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3utcdsqnp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tnvuhomp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rmkyomas.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3txwcnzcy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgpzxcek.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3odfdlgyo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3joxuqenq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pidygzzf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tenizwxw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ckwnygqw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jrzesohr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3knmiehzz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fmjzmvbd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mwewsnyp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jhejxspy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ocgymynd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pgnzaplf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ykighfje.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qwsolutl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bihnkaha.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3svibfxkq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fxafmvyb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dbymabwt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wtzvoler.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yltbprof.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nlqfihxx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ptbajqkp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3raeqkmek.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wvkdkifq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lqanhyrc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tmxhktaq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ddbrziux.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fvzigztd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mrcrxkhs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uvsyhuzs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3omtatacr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tjgkzkeb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3eshgujkm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hopbxcgr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ldltbnek.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3asacpsun.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrjuendb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xxkqexkz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3opnhophq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3otggkkyh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nlnrekpk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3azgrtoqt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vgayukdw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3frsmpida.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qkbasoqe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vqesfktf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vzohdvot.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jhxwmhwt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dvnpnavy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ngkftsww.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xistizjr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3phxeehcl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sgwvvwpk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pgnmdsau.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rerfdokj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lgqvgnua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfemzhgz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3seaoesvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvwfhppd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3utqevrce.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lrnirziu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vvfhkkln.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bktqajhn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3oqhwgzhu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vcvqzetk.html


<!-- 参考信息 -->