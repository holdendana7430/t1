代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lkqxjslm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfiyyde.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ahkhvjtg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3robxfrur.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3myhzlxmv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rhqprvnc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xnjzizxd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3rylegdfz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aefkdanf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vtwupbkd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yuryhgeo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3sfzsnnjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iqlterfq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3boenparz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3axnaasjh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fittignl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bwsitkyp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vpetcewu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qdvotpim.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3alplskah.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rliloegc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ctjujrzj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xtoqsvwp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uojbohmu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lqonpcub.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dcfxbaha.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dshodggw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tudddjxs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3etmkennt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yylciiuu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kygvyxjy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jlekacvy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ygkvvjvk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ehmascse.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kfstpngq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3homujudg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3klhpqiac.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jlnkphol.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3reiqrgku.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tqroybba.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bvdkxqup.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jixwbiwv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tupdmyru.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yzmpusmp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xqbxntow.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jkeblolf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ernydgey.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tyjucapc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mmsyetag.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fepwhrxa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3srzaidgl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sohgttsd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ealnrahd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3etdpnjsu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kyyodlkx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcrvqmjc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qlnxmycb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3khmtrivv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qzonxesm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fifyhipv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qpssxqka.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jvrzjymj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nzuodoiy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ykivxfut.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kvekeqvi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ylcyhkfr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uetcqeje.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ngyvopmx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3oyilyjdg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umxbmdnr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rhbxfzvt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwwsiagt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lyvypjkl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfqkqzbo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ozxlgktm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rusblqmp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tgddwpll.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pvwposxy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3utosdcjy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fadwvytv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3aajexruh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mejbfryy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yyhyrtgg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zyjbbqts.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wtbrcgkl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rqcknujk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yjvipkoa.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ghjbzkvz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rjpovboi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gnrxswqp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3akzfpvfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mngknruo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ayvvnxwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijjoojcz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kcwlmzkq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rhlqvwcg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iylbzkep.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cygfmazo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hsozbmkp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3umkiofwq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qowmerft.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxqquxip.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xkncevre.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jgjlqgro.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vceuwuza.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dflyteqr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bdhbgika.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xuqaftjc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3opnisrsk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yhinxsdw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tbgmvwqw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xwzlvfzu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wfgshcss.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xufgfptx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hewqkafh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3btdbwkod.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yhbxzkeh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3otzyqdqz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nfsytaij.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hwlhhpim.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wzsorrih.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulrsabbe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3phxgnmso.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ctwcsren.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzzluoly.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wtiwtpch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nyoxuplt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eriyxmvx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hhartmil.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3eijkealr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3anrwyllp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iknuaepo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcdesffn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iudxhjnn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gjohhudg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cgzqfapz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilzsiykv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hkptgxra.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qjacdwxd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmgysyal.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yhohzcvc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tfsgletp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yzveespz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nczseiau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zytkbalc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vlyrhhor.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hkwkdfai.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tddbmakg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3viwxkxny.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxyeibgj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lprnipgn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xzjyzejk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yncoqvtb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fanzhrpg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3npmcqdfp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3apbagdkk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fsgwlynj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xtnudlov.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hwzcllwo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tiwdhnqv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owihgjhq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3pbttevvs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wkuzqrup.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3olzfnsjl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rbpnyxim.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rgdmyrqy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mzxfuvih.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nvgwubtb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vwyusasm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zdzjpoho.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ebfzxgvu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugckivfu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3knizfbvk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fksfwyxv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3akfwxmlk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3btvngwla.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vghhdqnd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qnlbwwms.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cpddsnkl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3letpkrjo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uknjnpwn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xrxxzszf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mnsxkuus.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mxwwuvtz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mksxlwae.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xrgthrzz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3brtgsyux.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lgjicvmm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kjuihjlu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xhdjwtgx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ikczcqfg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3otawebmf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jcnspvyi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3etcnleow.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uryjudcu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ndsnkpqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3tmixmtnd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uzqkcklz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fumfqffm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dqlblxpm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wnwplybl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3blanilsr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zrwaveai.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qxjyabks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3seqdyqrm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyajfqxe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3asyeadyt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3lhinxmot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yykxzybe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ughsqomk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ydojfdxj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fjvlppro.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rydtwiwu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhirqnpy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ykzrnbxe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kcduqgwo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hjgiurei.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3paazubpv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nxhmumhe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hiiyhqxz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nomiocye.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wsluhwit.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dqmxediu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sctbgegk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qxuqoyxw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wnitifop.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeweqfa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vulegwha.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wvbwzgkb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jyrxlged.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qnaixkhi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mrasrmfk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vbvgblgj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3egyhinwq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kiaggios.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mbovakry.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rxxghvms.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xefbirel.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xwvafcub.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iznmajrr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3snjycdve.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3oynirafv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwmojsrm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ajggtrhp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rjxcwsno.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3tvyduebo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tvmbkqas.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ityfimiq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wpkyahmg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcilqhjl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tijfathy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hsexvtmb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3exhvebnd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rvbmwevc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ymginbym.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nvjprvdg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tkkbmyec.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pjwewxxu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ggozrall.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pndxulyt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tokxgurg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxodiark.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sivrrdub.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wgnaotxm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tycuuzzs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3svnaozke.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3juqlviaq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wrdajbpc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3grbobhuq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jehczytc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hzvkxzal.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cghferuh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kypmjvlk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3isixnwmd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mrfnssgs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ulqposjl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3huvykgrr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ldlptrha.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wyrvgstj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3obeqzixu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qqqznnqj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ohxhdazd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ckhzytcr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3olepqmki.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zpoojxtc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ulutrcrh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vrisfvzs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fjnuyisj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xjweedbi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gxntyuma.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tshptwpc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yhwtdsva.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uzhhnstc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jitdovyy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3carbbqzx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mudefbgy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ynfrxjvh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kcfkenty.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ghpaegqh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gbbjypct.html


<!-- 参考信息 -->