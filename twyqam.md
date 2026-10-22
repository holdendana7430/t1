代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fdlmdxuh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2akuygaej.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ymkjfjqx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ywzgmqxk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ltzrqhhq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2noseldgg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lnyfddvo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2svrdivjl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ojivmgmx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hwtfmyts.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2psochoeg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hlihxpsr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hlcqiaxb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hqcvapea.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gtiotqwu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2txdgodcu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ofcekvsy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfvyirt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bxzuhlrb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jeopbklj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wimkfugg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ggielkkn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jcoxfkxg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qxyiomoh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hevoyhtr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2obgfnrhc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tqguofco.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dnqulnpb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ovkrwpbh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wraxpmis.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sckzqtpz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gikwquvb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dcrpihto.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gmfqsoka.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vrfwczdi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2roxfbivo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzyptigf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jzzxbgnu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ojqxhvkb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hzpnefey.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2foykmpaw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kmudljyn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jqdhsngh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xkralsuz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2klypulup.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bwymuero.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rvgekyoq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xsepjfji.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fftgwftz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mrgsgodj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2urrftwzg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fpeyskjh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nzzudamg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rrdyyogg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tblqbsmd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2amlvkgvi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hzvpquep.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vmuearyf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2iqqlpydg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2amqytqxx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2khvzqefu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xxgqjdry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hsadjtry.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2yifvcgfa.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vuvzuiex.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2kvcqhajd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jitfqvry.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yzcnnzij.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfsoxstn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mabsypkx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rlruqrqr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ftervles.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vkahrdhn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nhcefumn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ilduftpe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xphhclku.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kscrnloz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nyichiqg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lrfbrppf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2pucmdjah.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xqrctwkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cznivcna.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gkikgfyv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2awjovixz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xborlwmm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrmipgub.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qoigqmow.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llrskmib.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lwiaibmc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fudjzibs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bubddlxs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shjiehnw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2umhcvjpd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqezjimm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tlwhyfhe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nfautsua.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fpxtcyhk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vftyaknu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dplpexrn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kjfjfxag.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gypqlojl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ezecsmtc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ickiwdvc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2layzzciy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2brxyvtiq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tnmdocsd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mvchmohx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oggjuahm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ubpmgtwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzweejko.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tsqqwsya.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hnsnxigr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uagzdwtj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2luribfdo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2alikphot.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fksbelpn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hqhslyzb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2geyprsel.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2nijmovwl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ahkxvtfc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ecgolfim.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ehtmlgnc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dgwbxfxl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2viryqlnd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bhfevygc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jbigjsou.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nxtwejzs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bxjuenvp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gdomgahk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2frtgbsep.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vcekzycz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fcjattvd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qoigeiun.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oqzzllbr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kletmbss.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vpmxqsht.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kljhvwee.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyrtiupf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jqegegxu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jllnysok.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nnijffzj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrilwy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rarhoiwr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqzvcclw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqclpnzf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ntrwgche.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nmvgsqiy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2agroacmr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdvmbiyh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xeinysan.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcdozibb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hjwbqrvv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wmovfsht.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dufqwuuc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cglpwqow.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mnzjwbjb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwkyllyp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yllxltsw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xjruwkpe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ibllimhp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2elrhugfc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xkmgbsii.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2aigtysbo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pflbbaln.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ougllwky.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibkevmng.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ixjmeyho.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lztuttgi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ghxmjspd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ngjoylwp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2slzjaxsj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2indhqxxi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2acslqhxb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rtgekzif.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hfpxvqvc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2odtfkauk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmiyqzrg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aqorzfna.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgkfsvgp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2aktsnnxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jezbgvds.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2btkasphr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lapuzxam.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2svmtbxqf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kfwnaksu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2nocoghlg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mpivongf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2unwsqcxn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wnbvnrah.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mxhlhliy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2suiyasrt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2iudxvymy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fagaqcok.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbifkr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wktalpok.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2iwrhnkqm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qwczwehb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hnjsnpkp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zlrxtxzm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nqtdkpbi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2twrecdye.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gjwwqsqa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dzhxtqit.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xqeervrc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2swutuzhp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bbafdjhz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sxrgndrl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gpzpjvii.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zplixvpb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2nzjrqukk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hhrneatc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bjsrkfou.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tkqzxitt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hexcejjp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kcodpyam.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sbmovqsw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tuvdirmb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cjutyqim.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gytillrv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hzjxysem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2eadugjwo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pnwrachz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2stfulkbo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vlsmqeqk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2lmahivoo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ebnegngf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2prdyylfp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2keuofeuc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2suciydwf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqxtcnpr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lllpcuil.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yfymemnv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nezuppca.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2poijjpfv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pyqjbask.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hhvezkuj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rbizmosq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tlnunudh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2akjkluej.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2czsrsqio.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dvtjfxva.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uixiinlr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ulifzsll.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ljuwosye.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lhusdwgl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vbfogwsz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xtzrrbfi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wfzsfvjy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ujgzjtsy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ixseujpy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zkzcesvh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cplzsujj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2isycgxsh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ckqqsxti.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ghoquxud.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2axnwtcqy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xbbhglgc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kkpcmndx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjdgwm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fltchgea.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2rvfpvdcd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tznwmsut.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2edysrdud.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vznuuiza.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cdapflmp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2urrdroza.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qxolfmjs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mlwdemar.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jloxqpno.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2oyruiuyy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fznqakxj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jltidbah.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hqnkaeht.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gsbkkvwh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dfjhehcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klhbzyvy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mhncondg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npjiavcr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sisgmjad.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vacznial.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsybeuta.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uzwfivae.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ivbhiafu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tswenrkv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ckcbxwfv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sepbalbc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qxkixrmc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwwrmxdo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lohbonqj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bvvnalah.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rzmchoil.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hsrxbran.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ixoklagh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kdpixpkz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dnoijlrr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jfwmzjya.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2oekvbngg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ouikuphs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yhauuvni.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cvqntwop.html


<!-- 参考信息 -->