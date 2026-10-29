代发 wailian999

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gfwvjatoy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gokzgwois.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gnyxqswgz.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gpidsuckc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gzbnojrbf.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gzeiekcon.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gpamoksbi.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gnrfsldgg.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/geoctdqqx.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gkxnoichu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gafjyyntk.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/ghnjvsffw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvxvysdmh.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/grauomubg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/ghmiylksd.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gokmmwaxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ggpvttflp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrolqxj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gogpfauyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gbwylzons.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gxlsamxkb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gwmyfnenp.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gndgbuuqa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gbohbplci.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gnogilorw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbqcvfzub.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gpdftjvcf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gipzdgwcd.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/glkqsrzqb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpifpofgp.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gqdslhenl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gutbcvmxt.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gqmuxcvwv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gldvzwzrl.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/goszbkbow.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghnscioja.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gapinvsej.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdgmuyrpu.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gbdgvesli.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gupitrjtj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gefxqsdfo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gmycgyrof.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gchrdejze.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gylzdrcnb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/grqqkhpyb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/geiyfuiey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwchxqlmj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gbivxagot.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gunctbkjd.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/goaokkxil.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gsnxyrzxa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsjtwxyin.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gwfnuvpms.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkrrgxsmw.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gzuhxcncb.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gphjrslpm.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gastpdvgf.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gfoxmkeld.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gklgvvtev.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gwcxhzoxw.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gkkoimykz.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gbtpujsnu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gbaatrrwt.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gpqqddnzb.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gwlripyhg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gpshkmsiw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/ghgbewfft.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/grumgyxel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/geapyjgpt.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gjielosvm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdeniiily.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gdriwpxws.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gubrjwqdc.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gezuugzxp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gopfrmnlf.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gdzpzjpkh.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gdqofpbrd.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gougwhjfy.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gjuaijjnp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gqazwveqq.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gfutnmvzw.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gypudwjpk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gtvhseatz.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gfujmccgy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gxpqblynb.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/ghexmhvvl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gjknrqton.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/guhmerdkc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gihqatedd.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gtnobarnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gemozftjc.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/ggvindqpn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gmhtdgqgx.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gijxspxtf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gdrtgiyur.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gvcimudkm.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gbwcsvkbb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gfdcqwfds.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gzgoxrgdx.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/goxilwrht.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gnhlnwpgb.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gjxovrwlj.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gkfebawja.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gzbixwzaz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gncxucsww.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gueqphuyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcleqclva.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/grmteuebx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqbyfse.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gtbnxlhtb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/glumzdioo.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gonywiylo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ggsmkzwtx.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/ghtnbhxjk.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gurnaqhiw.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gzbmgcqxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gxhpfktav.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gptraoiqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gdtjfcsuc.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gnoxkyjto.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gjnuoacgy.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gialajzdx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/glzclhlmc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gmllalvmr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gxpjefkpw.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gmzlhtflq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/grygcqoln.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gvgyztjxx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gwfxlmscj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gikiercjd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/ggvwjnpjo.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/guxxoodqu.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gyvisyhzy.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/grjyzkhjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/govtqrldb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gsjqpqonh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnqlgkomv.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/ghwrfdbwf.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gtksenkkk.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gymmdlxfk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gitskcnyy.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gdmisjpyv.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/ghhnhuvkm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gyjhcnypx.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gvktzjgft.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gjloyfvqs.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gacwpwaxo.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gvjdhakiz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gapnwxtfl.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gpoxromdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/ggrykovig.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gncmghcmj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gomfggjqz.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/guekpfkyk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjiljwuaf.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/ggowfjtcn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gpaudngfu.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gxgewcdze.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gvctjmqrg.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gbswjepvi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gqwuvnems.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gadfgjnta.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gtxqvalpu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gwhvxmtwb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/guvntjzip.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gbnvuruwa.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gzmeylrma.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/guzxggljs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gttwmophi.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gjkeidghd.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gotjaqhst.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gzfaohigi.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/greylumek.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/godgugxxb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gdqoujuwg.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gvnghnxit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ggcinldhz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gnjzsxofz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gtbfidzzf.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gotaxtcen.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gdeiwqurl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gphctmfkt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gruhpzplu.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/glradzbqa.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvexgiwfh.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gyqcenldn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxulojr.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gwwjhmszv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gbrkxicjn.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/glrjctgbx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gzjcosjmz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gykdllnqd.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/ghxklmuse.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gmzgbmggg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gzumjxgua.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gzduvnzzq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gycfmzrxf.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gcvylpqtn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gmdrliruq.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gvahfokob.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gaukhkugx.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gvgdgfdqa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/glihblwfx.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gcqenxzhh.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gmbhsntle.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbfrhdwtk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/giaicpzyw.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gakbtlvfs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/geqwoamng.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gzbxnhvnw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/ghwsaraip.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gjtwoofvu.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gabyngiqw.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gcvhnufhu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gbqhjibxm.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gqhpzvgue.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gqgnvtbrz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gowatqjeh.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gqwjtewza.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glsjqcxrh.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gidwnwgui.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxomukink.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtsmtlmxi.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gbqhdbsfd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gacooqmjk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gvfihwtff.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxukbdbe.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gmgdapxqh.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gufenmveh.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gymubzqas.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gotetsphy.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gdftcfjtl.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gzaekowtl.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gjplommyw.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gcmxkxjcq.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gcayaicqi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/giqtsinbx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gswfbwhuc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gkgwmaecg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gagojtuhn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gyctnuodm.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gbntpbzxw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gddtnvthz.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcwnmzlhn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gvlhaifrq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gmyiaowoz.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gibbsvjtm.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/ggeqlvvbo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gaoqschlk.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/grecwqrcn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/giucozebj.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gsdmshbjh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/glxdbznnk.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gnhvewtnq.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gukiurnlb.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gpjmotysy.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gkbgorcuv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gbbbmwfpq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gnxskxlkw.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gmiojfpqj.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/glcfvovgp.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gdzmfbwow.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdregobvn.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gxpxkacut.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gjgehebyq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gvsajewiu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmlcedjdh.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gfvqqogxp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/ghmtnouqp.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gfllkzcmc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/glfwigpch.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gzxivpjvj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/giwpddbkh.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gvibffwsv.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gszowfcjj.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gcbyphnyw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gwnrmzghs.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gunxncqen.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjibxypgf.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ghynnvxoj.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gbsfuflrl.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gwgokgejx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gqbmtbegb.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/galuvqekc.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gvydhqqyk.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gyolmmhbb.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gevabntra.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtmnfftcf.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gounltbmo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gmsclstga.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggsursvdm.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gaornfnnw.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gaaahetjz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/giypmwmuj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gbjzwckyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gvyokujyi.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gogtwqtri.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfsjtfo.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gesijcrfm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gadanawxd.sHtML


<!-- 参考信息 -->