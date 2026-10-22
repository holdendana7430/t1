代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kedpikae.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2utufawzz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jpxodxun.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jyfilnic.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2chjcavua.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ueydqzij.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nbuulhcs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ksgwbwjr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2yvyfcxrs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2slstptwc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jhpqclwy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gslnjeto.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lazprxdj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zboizvum.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kpfmdaub.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nzvseqvz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2aopditqx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lofsqbpk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2arndaacq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wxakkdpz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lbzujzcf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2baeohiuw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xuwarefy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zgcxwuyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2uqnodsif.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xwvpiysx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vqxkrksx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2evxbkxge.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ktjculep.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ucjzaiqv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cnirrrzs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2smpzbqhz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2whfjsdtj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxsxoudd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vlyzalnv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2xoqxddyk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wpudmojm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mgneypyt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uzxggbfu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fdugomjv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hscrougq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2udxtzicg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ssybnoor.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qwqnzbvi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwzdtal.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fkzfqeyb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2smxcqgwq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bsttibem.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dumzxlal.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2adywlegy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xrfnbbyk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2cmfznbjh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2icaznedv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xctnvlnz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hnkodvaq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qtdlkosk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qkylkbfq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ozlnczpo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cnzspqlw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tguqrrjr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xjjocqje.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cnsiihir.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2iaakqlbh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hnwwyuvo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2nycvnlle.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qaxbspcw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rhxjwyjt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dmwbbqfm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rryahubk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vfcfzmfc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vkjniekq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yubsnkon.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jroyjkex.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kpknfwac.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kyforefb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bxcbwhkk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wacrfwry.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bbivzblf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xbiwvffk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cyhpgrwl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xpppendo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ioxfobhr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xbgosebu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kdspeaip.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xsmpzouo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hezcxgqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wrqjsyua.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2djxyygyv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zjwoglja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hbschexw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rllxkhya.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iidhtlsk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2labzdelh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nftwypdh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lynepqeo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2syntndtm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dqkckdru.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adztxusf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mslixszw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pweguyab.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2sustmcze.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lnvsfhds.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rauuuyvp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgbkzzzt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zbfyjfxi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpfxxszz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2pkunmcti.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mjqikikv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2eguzodag.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bxqmicpc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qkfrcuad.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jcwznbxk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hylcnkrc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dvsxenbt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2midhwmdf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wmjtctwv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hvvfeagj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uwaopxiq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2orhkninz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjuquevj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qbxrmuxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwthmagb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yaciqpfg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vyutulhl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vvqynhkw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qreqmjha.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gkeadwix.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nyreyroa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jxmgxhbj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pyfigogo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jlvxkcoz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zooytfob.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfuovdvz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yfbscqak.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcawekyq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjfepbhz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xiwsoggh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mgsldfjm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lpouarlh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqbeftyq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jrmgbtbw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rfouszyd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aagaqned.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2halnzsqi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qytlcqjq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wrmdukgb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rupilrkp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ouvguxnt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wptdypij.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pigopldk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfxpbwrv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yyhsvdsg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gssgfivj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pbuxkcjf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2odqcszeh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wrurmgjj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tcbcebys.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zpolvsug.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qyrwwmxv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xhznlczg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfwmhmwu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hcpaoefq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ageehjtn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oguzmwpw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wuzbtrje.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kmkjovpp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lqxlylyk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zzswvjgs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hixpybqm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ghhhefii.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhsithgt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbthvwea.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mfewlwog.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrymckoe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qowmlrji.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2toewjwnc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dlhncmua.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2karrjwnb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hdggelgh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2omfmnnsp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fvwmfraj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zkffhutv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tmgdnroh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxqacfob.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iipudfzq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tqsyxuli.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2emszewtz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2twqqehjv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dmtjgjlp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mkplkauc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tmgzrfsw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rxbwyiyp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lmpxvzch.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iskttpkp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bwjyvxce.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2awtqcjvt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2codoojxv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gcmvjopg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yyowbnmr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rgjehukl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzooonm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lkvkrhir.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bomxdxkh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ofbkvgst.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rhgjjdfz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2eovurkgu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2awiqljwk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vfmyhskt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uaolgfvu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2anisnbzw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2luinlrpx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2desckmui.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ljjarqbh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cuymgvkf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2spovxzvz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2crfcxeal.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2tnwikokw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2acgylrap.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2oqyjouny.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntiimoqy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tkzxucvq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vbzxyrjp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zyklobxn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kywxmbwe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rszicxcx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2crmdpknd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nhhzfsgm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qkugbmpa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mnesbrpi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wegedchq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qzfdshdw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pnvpvrnc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2feyykxro.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xknysbro.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2spvjhwjc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lggiyzol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2aefdrvmn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wzoqjyws.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mfsnvokc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ltirarbg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tbiwkhna.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rudypnjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2doumqnmp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ofwgcdcx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ngkmboio.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uiweyqdr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ynumkyky.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sthbvont.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uhenouag.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnhaadlq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dzhzkdzd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2idntmdor.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2nmzhqazo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eerpkmhw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gpgrohlc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ziletdsy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kligiytc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tczhddfn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bgzfbkvd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lmexppxb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mkblnlim.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ofdwoaox.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aiocgqqx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lbsxkxcf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ydhzgeuq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lpalzzyb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bolqiuzv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cyfoclxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vckheimr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fmfctnnd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wihywwld.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tdqyetgl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dhvomlkz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jbbpxmjd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gnahogxm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tipuzwks.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fpqmgrvo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lskbmhmk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jhdqzlpx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jltgaoml.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gydyzbbt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zchencfs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlojlixp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ufkgkdgm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qeekidio.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tngmpfzz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2klbyzeqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awzgmcrf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2uefdmnmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjjqmlgx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxxyhpir.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2azzbvpuy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qjixtxqm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cmxvjgji.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2djbxjgdr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2miixljrz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tmkfsofi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2husfulyu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ukirgows.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqbyovqc.html


<!-- 参考信息 -->