代发 wailian999

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/grfeqbbbc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/geqjlwkdk.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gtjzosvkw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnxvoaok.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsmnaiize.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gikoqfrpy.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapsowfeg.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgnoblzo.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyetsyrcf.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvkycjhv.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxoukbem.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/glihgrxvc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/grgmvalhc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gsanuuvrd.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghniitnbt.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmustpri.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkchjjrvr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggapfsles.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgiepcfj.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gugmtraub.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gravsgafm.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrkmkijv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gwcfvwxot.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gelkdbhmz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhjouari.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gmutgyktf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/glzoxcfqy.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdmkqqoy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxvwnkiy.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/grlpofpok.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gubeayuzr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/goqabvmbm.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gkadncxta.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gitrtxkcx.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/ghdhcaoix.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhfewyln.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyojdwee.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldlyehu.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnonvbkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/guddwsuci.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/guculfdiv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gomzfsklw.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhnjgekr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gflvxzyhp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojjqksxq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoyvtobn.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrldphr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbxblshx.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gqyjqblsl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcmtnfjnn.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/glcctwclg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdecjvhbs.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpnqutip.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnshzwhj.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimwkftez.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvilifpe.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gdkeyexoz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkbyiilk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmppubjw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgeioyxv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeekjduk.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/glmtewbib.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpgerazk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gutdfjpbn.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gpfelovim.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gokqhoswv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvshvzic.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gzqclgmyp.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gemusevts.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/givxxpckm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmecqjfp.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeduhfkz.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gayworifw.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwydbjom.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggemqopdl.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqimvqwv.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzfkjdhwk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfodwzjfd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrqecwg.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnohqettl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnbulgyby.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtcngowgc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gefyqrrhv.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjkaeshu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxstedjrw.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiawigaa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gajvxquov.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpjflhva.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksljrakk.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gghcttrbi.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsrirzaca.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gehoolchr.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gcamixpzm.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwgfgtob.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnmcdfsw.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gopzrmjhb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmpsmxfdx.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gekoiecmm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvziwpqyl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewwvdozy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfdvlxd.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblzxwgnu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galmrlwgh.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkwcmxrn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grardhfbb.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqmoqaij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjntcjcqk.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjadfwvoh.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtcauylp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggapxffyq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glorhkuen.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvtxdchy.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnhmpyrwf.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxmehpz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasrnutjq.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbindokeq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/glalfffpy.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdjtqftg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnwvlvmbu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrzxgww.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqjaeqxj.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkklebnnt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goifruzhn.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gimuaqcjf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiylkmjs.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gauyuszwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/grcrfqhwh.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjteocbrz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbxhypnn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govvtpqqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdfhewmx.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grvnwyfdl.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggbslcweu.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gweixwlje.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/geqgxsnnk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gmjrittqw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaiecpmx.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqqnxed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gepqtdrry.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnrjdhlk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfmwvhdg.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfbzvhfi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/grqbnuhrg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeypquof.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdumjuwov.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gacfrgzge.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gqqhndtuz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gmodjsxac.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnronmdsz.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbmsniawy.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdkevhaha.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfxjuvnb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gamzjhxgj.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvwdelcr.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxtveherk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvczelvdd.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/golabbvtk.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsueplxcc.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gndvwxtpf.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gjcgaraix.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gsexuuvuq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyingiwmy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gkcolvxnz.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvzahbcfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gugwvvsbl.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/guelclcgr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goxmvmvyv.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbrhffqk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gsweqkcly.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/geilpqput.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcfzwhyg.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gvozqiqwi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxofxgrgv.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnnmemko.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtsbbtfy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlplpczq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmapexn.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/guynotoas.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqlibyrfl.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gaecvcnys.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gwzdppfnq.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqkjtmm.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdqtmswm.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gooksakth.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/geeziufiy.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrnmhbgy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gywxetcyp.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdfnehyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gyrtrzggd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gtwilrsoj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqroprfn.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhcyagwq.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfkhmcxh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbhbqywea.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gveaftoco.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzoqyguk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gowacpxkr.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpqgjclc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gvjgelcbu.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxnwpxpxj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecymnapi.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/grvztsmva.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwlmepizw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gunpvszhi.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gkskddfzx.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gqqckwbzj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtsqtjkyr.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gbxdfdotc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/goeqfadgo.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtayqqfkf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gdnvmtpgc.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpqdyhxmf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsqolirn.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzpqmpcx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvewdniaq.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxntqcwcn.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gkrxwmuzv.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gkojkygqn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnxhlfj.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfyjzbha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gwurhgkad.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsxwkhvl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzzgxvd.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gqhvitqxz.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbjjdpj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwymojbk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxsgmnzxr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowqsvgmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gayrdxgdz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gedxalecx.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gamulysvn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfjwjiwz.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gzgdxznkd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlwmskmm.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/geupogxst.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gyhjopfyv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmyjlytlr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwilwfvn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gaupfdbbs.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqkqcmyc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gvpsarays.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjuklnav.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getijfjsv.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grwexyguk.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfmoyexry.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfitsbtqw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhnytscd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvzxxwrpe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrlniheb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjgzlbqw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggumrkvjk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gjnnpeaht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gddyxysax.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gilnkqyep.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdbvorij.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkaxrqtc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpycabanz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdfwunzvt.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gljmkxuue.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfyibabh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gstrjecot.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gofkjicbn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnwrdrrl.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/guwocdhfd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqoxeral.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoqhxbyz.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsziiqze.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfrxmbmr.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpkftvlhf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqphsucd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqmmezwl.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsvbvuvae.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxrmbdfy.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbwrevyrh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjwgdiynm.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/guljuygsl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greqytjzi.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gokacqqup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/guerpwoud.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvcohhpr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgdegfyk.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gtnrwswmb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrtesreb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzxpyqix.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhdtevwb.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdneguigk.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gisrkezrt.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcvnnvtg.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gnmlslirv.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoyhnugk.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqabgooiw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbezzofur.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gncojikdp.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnungncjz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtavhmss.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginamzxdi.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhqnsutd.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioxiphtd.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhubtyyh.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkookcavv.sHtML


<!-- 参考信息 -->