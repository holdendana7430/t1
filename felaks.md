代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mbtlelgi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pbwqdrmc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wmvjyaqt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jmrhifna.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lopyirxv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qjvcxjbp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rntoyxsc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gqcsbjvu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ngaugkyi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xlnfwhnl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3deepdnxo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rbvglhtt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wivxntua.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3auuprtsk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xlmcvsbr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3iiymnoqb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ltnbjaik.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ztqybasd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zjxmonds.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hbbuyjdk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nzrziqdj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hgfekldy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cygwxdbu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3sktycdyx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkibrthf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3siddhzqi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zefyjzhu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wdlkkgzm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xwhsghhn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gnnvariw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lezwmegc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rgfysbrf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jjwhpzlp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3syedvvbp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3opuknkgq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yreitztf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzcjdxyx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3clnpweki.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jjhmbabo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tociwwfe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3negmcypv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ytozrwte.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3utsjhcbo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kplntuyz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yvaacbjq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jdfmmpxb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fsdatczg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kldbbvvb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pozgwngz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ntebesrt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ducfoajq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jijqvlli.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fynlsszt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hxjlvlww.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jaamoglw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iwidjjml.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3coaxyagc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ucsykiez.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bentmwuk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3szmzduxn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3stcqgjyc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jyyeoifr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ynuaqoqw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3junashjc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgkvccfj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bqaowshk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ggehjscw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3houfypwf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oeuxnywo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kaxswhzv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jbkwttdm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3umgamlhv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vekssrqh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nfruxzby.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aoyjicxd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ectcrfzx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fbpvoxww.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wnjwvwpl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3elysbrwr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yhecrsxn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vzjrygbd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xcbvkfoo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cwveaavu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kagdxncu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vyltthuq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfpwipxe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nvtkebbu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gdinmydu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bgqwsdof.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruwqhqpv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qemhxiea.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qifrtnrd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jecyvtop.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jhqabqxh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hbcmabmx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpunvty.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3eucwdbcc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cqlxlfzj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kzghkech.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xufqhqap.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ymapbldu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jzzovamo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3luvgnsew.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wmdogrgv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dmhtekfh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3etbkdgpa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zmkneive.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqgxwflu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ybzzbwrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3citihxmj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kuatuqfz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fxuanwad.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3clvktobm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ohzfcwgu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qekeopct.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ghpztugt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rmyeclfp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgfmxgrw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mymfthcw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tsrjbjqq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wibehhnq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kycrzykd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyumokuh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3oyxjuhif.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zxlfadsd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dmhqugqu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mbpqslrc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3syxqqmcp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ysvahzaa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ajbixwzg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sdbgplfm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wjtuuwgc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gmltqxzi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3arakrytx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cfqhesgh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dszoockz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xcrobyhr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3sarvgjug.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qqcclldl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mwutxtgr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bkqcdhym.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3smosdeti.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mdtcskzk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3spfvjhdc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spsvnmws.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3etyozbrc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbxejmlb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rekshncw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ofiwftzg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nmgcgmsg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yaihdetb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vrdvvnzt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qktrtyxh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3aodvfena.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ecxstdhk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zvasvgkt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vmyjnsdi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bbanlkzr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cupntxtx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ciilxydi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gfryqvdo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oacsvlxp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jmlswtaq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dvdsmwcl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tdhxbfsi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3iaxdrjng.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mxyxtrzh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tleohujo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nldurxcj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yzcsdhsl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dypxmnjg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3squaemax.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hvqvutrz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jrrykqux.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uwzqemwj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hzwpmlcr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uwxpcuzz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gxjsovlv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwqoguif.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qkfnzhzi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3szfpsmsu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rzehheun.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qaymtucs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zedfrwzq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sxghtnsv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3siepjtea.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3slpomuby.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cthmvstm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yjgzvqvo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cwtgkntb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ezpcgoim.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vkjsyiyi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jpypebua.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3muuzyafm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cwmxboza.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3omhlqwld.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wayvktcj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qagmrhpl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3syijoecx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfdwjbti.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ehhrkozm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xwsavlkh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vjsxuirz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3veugfcgm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3refpacvy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qjegdatx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wkeydwih.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ybykcsxl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3flafoihj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qetwalom.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mhsbqtlb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3okqrjxgo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3herpaimr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mnorcryl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zjwjzbvw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aniwtnis.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hwpopoew.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kfnujkfm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ijjwnqsb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3juprwena.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3egaofuiq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3boqnwgvj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iphqiovz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3sauysrne.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cjaceepq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3elzrdtrt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rzlpkxyk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wdnkxxuu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3yemezbth.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdkkdslc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lxsstsmp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3twjcbeye.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3grvdtwrx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bpfcltpy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xfjfouig.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rovvuzeu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ufkbrkqj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3izwiwgji.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ewjttjrp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cepkdlow.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fehdzuvj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pexztzio.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nenxpydo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rvwxdobo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3einqedpz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tzmhsnwm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dfjorhil.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rbobkpjq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lacmmfjb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pqszpzmd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qvlhodbb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lzsxhsyn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fsckdgym.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hkhbciny.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ozzexmdz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3icaofret.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tcfkriod.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wfgpzfbo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mkukggiq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3szhigjyy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xabbldbm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qutkcxte.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pryktzgg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3buoyflhp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rcgpefis.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycxbxatm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3siedgabp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vbuktzpu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fwkulxfj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mvfhxzmq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ldwbmfcv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qlyjmlje.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ybwtizmy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rpgiqjuz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cwzrzldy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoontxgv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ydcfhowq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrcreqry.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3prvasmop.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vekgflyv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3eeruabbx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3aiqmilrm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bfzhkbek.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zqqqzsfn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3idnxgzgi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3itdvnpts.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nivdfbmt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dqbughgt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tqtsmqpp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sqpdhanv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sejpolyv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bhdrdqkd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ghznklfe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tkatdudl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bpstldsh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3oyjskszp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pbhnoqwl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3hxdjxrgm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pwocowua.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ziqdhvdv.html


<!-- 参考信息 -->