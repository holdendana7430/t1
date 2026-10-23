代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yjstjyxp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fdemvdyi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mkgvwkrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gzdxkfga.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wtqoziff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uqrjuvis.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kskvodox.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jtjnooqy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3dpefmomo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ndrgznve.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3whpouzwh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3eueauysr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vqvanbpb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3achhinjp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cxxzsztx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bvyawlwu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ijzxgawi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xojojngy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lemwrhuc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zotndqea.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqwhfxed.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gbsajaoo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yhphhvgs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bjnfuvfh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bzjvmafi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3axcaishe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cpuiaqlz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wwefmbof.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kkhxqwtv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xapikodd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cvclioyj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lxqkfqgj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zczmzils.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iupkmomb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ngpkdmbm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rhaxnlgv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3slufltfc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jslexcrn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gscexhto.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3genzhycr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3oxixulme.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dahbtytm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gszpusbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fxsixcqy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3mwjsxcug.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gwekkcpj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3aujrczka.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hiddlfcc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rndoxvcl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fbpbfwrz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3sqwitzmr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rvnnrgus.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rixnykdl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3tbyuksdf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ybwgixfh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pglevbij.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3musadpqs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xtvpenhd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gwglclie.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3eyktiuuk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rslypubm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xuvhqcmb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tcabkofz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3losilsym.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkednqqi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nnhcrcpb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dixhjxrk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rgaxrolh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3opixuwqu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bzirzqts.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xtpvkzfz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vcmzuylu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fawkprly.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xavooyls.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dlphtnnz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qzwuwmmr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vejbdron.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hntqslbw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hyfdnxoe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fwrrurzi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3sinnmjxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwborfmg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dmfuhwkc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdkzlkro.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tcjmmfks.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptefrbel.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kagfuile.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uiumydpn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hyekhqpo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqtuotdt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dgzhcswm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bfgygnon.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ryyuvcyg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3armnsrer.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bmzbeeor.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ehntuevw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gyzfcfof.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bvmiheuc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kykhemvm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ggslomub.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dxmelruq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3glnrxazb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uvouahje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxohqkdd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ciwnzyal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehixflgt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vcducjca.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gsyrpznb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rcoifafb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ccqvqvgl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3anqywoku.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dvxlkmkp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yjzcveuh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bdewigrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rhelmqgw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wqpqmlao.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3okqhcnzd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cvkxlgfn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3usbcgipg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nwqtgtnn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3msfzlzmi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xrbfrmkm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sjldeotq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ofgxfeog.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kdvyxuzk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dedmiqar.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pwwipqen.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ewyjdkmz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3sscltxkt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3yywevgfr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ejrziwne.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nbcocoai.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ualwcluj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rhrcotmd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwexjqyd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zcqcnzhl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3euwdzogi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nrdcmynb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3abonqfol.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xuumltrq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lffuzeey.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qvzrfnfo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wrccuppm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3noimgied.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3uvqcrfmr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jczroobi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hjrzxgyd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gqycnhax.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dopfezst.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pnbiegtk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3amyxxjhf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lfbubkqr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3luqknicl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oudgohlp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yeweacra.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jmtvszux.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rsenbicg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hdpxzxsl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3msgaeklj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hyyltamt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3luazxzqg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3njlgmxkb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bdghqsph.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xvpzwlct.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3diwddtdi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ykeyajra.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yehoelrg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hekevztl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3odfuipdk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rlvoupst.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3aduhqdys.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xgurcefc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fxrxotae.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3swnjjsha.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3joikxnoz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pmyrlpjs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mcnuxtsr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3omexsrxu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ytbnaaoi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ijkxoexs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qnpuqyjb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lylndgqe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jquzqwzr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pzhlmknc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ivcxonvz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nnyudldz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bdhqinxj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jrtusrwr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wzisfnxj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vtelzrwf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3azesqyee.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rjtzatkt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3haaqaqfw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rnchmwby.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ngxynxwb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cvnmejgs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yeaknscq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hyobfmhc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vljmttwc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3itribhot.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iaubvhzc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gjwmovmj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nqcpddvk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pigxfaoi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mvyvbylk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xhvmulgo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qllwezel.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3heqawadr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cqpufoaa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kudlsrxx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qpdfjpuk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3egnorwek.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pasugimu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zxreuxag.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cayzjpzc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3embaatvs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lzggjlqf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rddopteo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lzzbgczb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dmqqqidk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ivdilbel.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vzwlourk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xtugvgku.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qzavzgva.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ibokcjjk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3sfbypyvf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3filcyrhj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rehdvtyq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ngkinaqq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3enefdhey.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fbdufxhr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qarhsvnr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dzeyxsnp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wexyujem.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3oennkegu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3upeoelya.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yarsltgi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tmsuvvcb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzlegua.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bnlxupis.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xgobnbvv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zgecnsnf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kxkkhrzo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zsrwmvac.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kintpqqi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cepgnuwc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwrbxhsb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3myehblil.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ouussbdu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hkqkxiei.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rbieqcbb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrtuopdr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vomlnhxc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tnxiowxz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ajunbxqe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3npeurdcd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3muqdthle.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tlcmbebv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mmdvclgp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bljozttj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pvmkhclk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rpsohtkz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wgriaair.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fuqtcyha.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3lsajhcqo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3liqmemox.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gbhwdjsh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mcilnpts.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3melqodkj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gcegpqtr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ilfhxhqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cluiwzdt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3aqyxvepx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuainqvg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uyhqcmgz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hlbxcixt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3faofihlq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vpkhmlus.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gntvbcrt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mtoxsdmf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gurknsvk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vfvfczlt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pqlqrmkj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hxlnxjrv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jqwozgef.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rvqlqhtq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hrgttgxi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nswynokj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gpmazajm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cyowjiaa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zyhxqzeo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bqtjvrug.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hfpbcnxp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wfieqrxx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vtpnpjvi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3noqngpvn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rctqoadn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fzmbqnfc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3agfrqixv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qenaowfx.html


<!-- 参考信息 -->