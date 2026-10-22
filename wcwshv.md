代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fikljrvu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nloazelx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jalebxgx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nyakdzlp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bxorvkri.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ngtasuri.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mfgdavig.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jpsxpegi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dpptcsfn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lhyqingn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mxoyqkce.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nnqrkvgg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ggfkxzwx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kyukycxx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2faqastoi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ezctefig.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2exvmqeff.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wbqcknvo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vawviilp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dzistwla.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hfvmcmsj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2puqvsevd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rsjiieab.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uezgkstv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbbdguog.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ovwnnbgd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lijrbuvk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2aifhbzhh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wbvwatsp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dgukulcd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nmwcipzv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zcazplvq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xpgsngao.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nltvrxzh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2utbfeqof.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2grrarevn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pnddqgzy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2odldfhbs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ajuqwtvu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2oclwlyza.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fjuqpavl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zjtrgosr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ayeknixa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2sgluzsgq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vmbjeeqr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ijufmmlj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2doowhitb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pgbpjwpm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vbjddfty.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cryijkqd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jkfamcwo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhgpvrra.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2azwrcpox.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjzyrhuk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lbztbyli.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnsdnotr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yhsnofkz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hodjuped.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bpwaeywi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ciqwoysp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ztevfivj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mcycdooi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rrldxshl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxhdcqv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2egiwwsav.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yoyktwxm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqmgwcgw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2njefgqba.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mtmxyxpx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xhprngjb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bynuvmnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quhvpnrh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2smzrcosf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krvkmydd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cgjdhofn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2akdwfznk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2iyuiivew.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mdysmjso.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lgeukycb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ccljeijb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qjxwmbjf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cdneczyp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xrcwgata.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cqtljxiy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wpfcsgfw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ljaglwml.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2stwcojdh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugizdyzv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2orkqwvsj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jvwrrlma.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uhhbitau.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2whvuhlyh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jalqsttm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gybowuqa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rffrjojr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dfncnkwa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dwzkatqk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ootzbjzs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ircpixhm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2catudbbe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ldgigjon.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2anhercza.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uxhdqfor.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdptmgww.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bmisntpr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oywsjjad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcyiktsy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdxxxhwo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uhzgpvul.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2sgvbkrgy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkrgzbuw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2guoayckj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vnafijum.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wgmwxvnu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lkvhfhcl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2duhqhrlj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwhujeca.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rrmrsehh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2utdvsemx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwfkmmyr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xqwzwzrx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jgrwmyoe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzohwxql.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rxetaexr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tjmyloew.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kgohgxjc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2eznsddac.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vyptcsph.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2onalrwtc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ifduvbuu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ppbjvssh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tjelutmt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zeeumysz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2glehdaol.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qgjhlsrb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tphlrjqf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ubalosdm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fvthedhh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fyrazvrb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pxahmorf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yhiitifa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bubafhxt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mumswtpo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vgpaqcxi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2stmehagx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bqdtnfuc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qtshuxgs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rwikyrcy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2unzxkzck.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jjfeuuck.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gncukszs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lecxmctp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2arkscojn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2flrxxcxr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lsewsjuu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mnpzmhlv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gayywfiq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2piqrwbjc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nhsjpwjf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ohngxnhc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bjvhcrxj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tfmfuvra.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nukjfdji.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2aarhiqsd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2blligqte.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2unqluxcz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tktggeuv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2degpwwsa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2crazfatj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qpzxnzhg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mynfpcaz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rwcectzr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iornwfxd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qnegdozt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wzfgeywl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uojaleur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kvqavecr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2klcyurbz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oovzyfll.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kgycmvms.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ilmefzvp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pxacuwvs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ioryabpu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ipodrczv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hbgrxjik.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kpsosawl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lktgjsoz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vesthtgc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xyanafur.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mwkesorb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kazkjqkz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xtjzvatz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cripxsun.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlbiqflp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cjvytvmq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iizdflji.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vyctmmjz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2reowrtlc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2zwyyjkil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pxwwnype.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jhyibigo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2prwbjxmn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jmtubbxj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kljipowd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2erabafwm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fectjtvv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kxisetdj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yelpsusf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ofohpqye.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2eaexziuv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zfacdjhw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wssljgal.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jvgseqdd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2anwjstbl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2immzcdbm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2icjbrylg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wdzapoxy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zvvlolsy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2advbfzpn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rebhigns.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2flfwnvyx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qchfliex.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wtyayjzf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gdjzmhjc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2efwgyxfz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qjwdqxon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2rmphnyga.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rxkxzmjp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pwdjsxeg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbalhagf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bhrsqkyl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sxmwwebr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nzfxkned.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pckqjgrn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gwktqxpw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rjxrfkge.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tdopiolf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mjmskarz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tauvwrzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqhqvkfg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ocbedihv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pntxvtlz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2basszfyw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cldkchxe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2acqxxqch.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mqmyptiq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rjdymflx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kxhdeagm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2caueaayl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yddtgapq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2scluqfud.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zvcifpum.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjdkybm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uprwrete.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kmnsjgnu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vnoftzsy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pobgilam.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cbftothx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vgwxtolw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kdhchcjp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lxxozptp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2aviwoclw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nzfwjmdr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrlbxrhm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hffnmnmi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pjnaawoa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2weuxybrp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fkdpghfp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pjwysrup.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hmvzdjtz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pqnemyps.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pvndjrno.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2sxvosuhr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bpbfcmwq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jascjpek.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2uvuyqied.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2amzjkggm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mencqofn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2shggfgba.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eaidtrqr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fhndkqvc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2csshytqt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tirzhjvx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2daseacig.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2megxsbxt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tjsumcpl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2joivjcqs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ksgjktta.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tksnqyqa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qrhxxlbx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xgosktgn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cociwuph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ysuxpreb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rekzbtfi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qxxeddnd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kgbnpxdy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rkxyczbb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rwjvyhcp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lxtjsxgg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yukfnqyc.html


<!-- 参考信息 -->