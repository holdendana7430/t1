代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3eswyiykv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3oexnvnyh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ihckfkmx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3leuhzzlu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3mazossmw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zncfsrxq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wqovbhzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xijrdlmr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vdzsoycx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xnlgleej.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jpszfkab.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hxghlckk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fibvbxxe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qtffdbgl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3egvdfmzi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3agehrsys.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xifjlnmq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ndvnbzvs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ojlmwhok.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gbcyqnop.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bdsshyvr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wphqjbwo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dutziyhz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vafduriw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3caefofzj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3etvvnzzo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fjwgkpcc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hojthvpy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cughlxmm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lmdcyhkl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3txdmekbz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nfvtlevc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stkmdpoo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wijqzhxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ldlespvm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kjvhzsnw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3livzohmn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3axpgknbw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xixtddys.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sztrnnhf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jjowyfoz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fozvyvlr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bhedlxye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ptdrvygo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kuhnivqo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mbkxtitt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zcmsulir.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qerlufaq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qmwmxvwc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3aqmowbnl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3sbimkzsu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cuwzvgxx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3aprtydxh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3krlntfja.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kdaklzdb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3slenrnyf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3anjdhxif.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nijafiye.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zsgesami.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gdsicstx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxkkqslw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ykjoclge.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xdmjdeuz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ucggoyup.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkyhmdtc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jbfczcya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dhpuzpwc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sxtmbarc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3npjozpjb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mkihkoyk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vttrnhuj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3onqckdcc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aeezkwxx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kfkshjmb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qezwcyye.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rktdgahw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3eosbnhjy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vqeonmej.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ukhqfhxn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gjollhaw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zjkztecw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xbcdjefd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3stepajmi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rukesogw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3elkafbob.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfbygfsr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nluzfbpj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gmauysro.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3acytjcny.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifvcwara.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nuapgxpd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jlcohiek.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sctybhhc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dfuzwgef.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ripewgiw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3myckkrkk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mwpqtzna.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3scqftrie.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgocpnzj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mgsaewhy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qxjgkuhc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gesuxwel.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vokccadx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elaidobe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ytvgrkdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayrpgoyi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qrlkrfns.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vxsjktvx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wpgzixoq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ownpkcbb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ywocfqnw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zglmjfyf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jyutzrqr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3acvftqws.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dipbniqo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wartgfwu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xuwivlsg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xdncuycn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdeckqqb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rfeifkqj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3yvhkhhpz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3znpcioyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zfrqwkzz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dyrhunvv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3erpsvibo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kklienkt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3yuihazdj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pxntcczs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zosorimi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mbhhfkyp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cfubyrcw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qgolqeib.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3latbfaoc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yiaicoff.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gsptrxoe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bcxtlsfb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtxxhpfx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dehdkdse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qlcfjirq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rdggkmvd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mczlqlcm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tgszhkgj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wygprqvm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wcebcpts.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zqzkytwh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kjmcfqlp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lgdvthza.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qjvqaddb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hymrgajf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zcnbrdyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3npumfoxp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fibgfysn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tatwazoi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rqmtroco.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3izkfcabz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xqrrwiey.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bqxqrbof.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fyxurqhn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jtculvxg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ckkchwjx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvnjmx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nweogxvt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ojxoxjnd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qnflyvtn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3klpkprgn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3shkleqpp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pbrrocwi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3smmkcxff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3otcnjjcu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3iioaxnpf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rygumsds.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dfgomzxh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3npadupwq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qibwdzmy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qicittur.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3snswtdvn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pdgcmvwv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mpfqomai.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pysrunmc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lietymug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vsavgbnv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gembdokv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3exmdqkos.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpaffkow.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzvkjbac.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3tibmriey.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yykvxxsk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3spfrwcpq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lkezpwab.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ijuayvjp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wqpoqkva.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ngskewbz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wnywaotj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hkglxkug.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dnvxuhps.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3eenlmonn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fskoktzb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3okjfstxb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ktkvcwlj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yulzlfyk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uagvnfbc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pmdqxmay.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3womiftxn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wwmwyznt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uhcxernc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3cotwmism.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3osghtxnh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zrbuyenr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kfrrqqpw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uzqizgmy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zwjjtrna.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zaxugtby.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tucatjsf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ifjghviy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fcwrdudv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xqehmicb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dogqcpyz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmpshryu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hdivuahx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xnuuclab.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sbkeppfw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oobtwyam.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bfxzuxkb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kqjlpyql.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hyhfemxm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3iffmeild.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ksezyvnr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3emxnipir.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wlkwmaod.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ndyzusuv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bzqggrbu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3struwtrg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sontusmq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gusisdrj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3efswbmkq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mbdnwehg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pxypnctw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tzpuqqqb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3urcgnqim.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fvgcxzdm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ouwhngpn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3krnkiwwg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ooifpbsb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3grpdnsvu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uqgpucbe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3loubjwna.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xqndythg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3chhzoxay.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fojluvcl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wxczbboi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3avikewfn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mgzzxhbj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ckvbpmtw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xumiqwjd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bypvuxcp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ccefseog.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gydtwwwx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3trmtacoh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hfmuhusc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwjntysw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3duehuwtn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3inuctjbz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3spzxtfcn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lopcwkst.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnmmkq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jjqvqewa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3uspgvltt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3khztuhkl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hrfdozyk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yhfeqewr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ahcioovu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhjoqmxr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nrxzvwlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iysabdgo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skvbgzkp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sjekawwa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3stvebqjw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3brmwosza.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mjionrgl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mqmzvbqb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3yydidsdg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fxssfewe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cgxhezlq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dprkyhij.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fgwijlpx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gixgnoax.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gnjeujbs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wsaitkts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vmzxeiwf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3siwtvury.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3obusmyjl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ydujawml.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3izybeivc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vcaklrkh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xrolqnjw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfjaenjy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vjxtfhpa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lblbzhfo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qbnbqzzd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvajhctk.html


<!-- 参考信息 -->