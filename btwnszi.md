代发 wailian999

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gqnnkndgq.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gyskwxtvd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxudjmk.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gzmntncrx.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gccrmcrhv.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/ghdelmeej.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gaoctimqd.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gxjjungao.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbuucmtuf.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/glzeuhdpn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gwvnzxtks.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gegbprhug.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gfpdsvnjm.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwmvgekha.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwvwdkuii.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gdkjtncyi.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gbdsknxrd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gomqqczdn.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gdaotrnji.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gydrwkwit.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/ggkpdvcjy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gajoajpuu.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gtidejowz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gfaehuuik.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gtncjrbkc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsxaoadge.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gttsvsngj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gctpivtju.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/grwqsvsnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gaarcbpbg.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gwpaktrdj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkubsnhul.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/geyyldcfn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyhznybnw.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gedahrkhy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gfwbveaua.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gguzwuyju.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ghtvgwobl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gijocwqgk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/grilryhhj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gocopztyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/geodjyffi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gloywhhbq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfszgqnny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gfxyrfctf.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/govrdhepa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gtmmfjhft.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpjzofkul.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gthyubedj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavtochce.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gbulapnxn.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gsuekvbfc.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gbibottcd.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gqjdyukwc.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/ghnkubknm.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gnqwhjxbu.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gznultagd.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnzzyrtkg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gnxvfselu.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ggsincuna.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/goznbuhnb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gvqwisobu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gcklmysad.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gcvivtamb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gdekfqncy.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gywpbivyp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/geqxzpoar.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gasaoaspo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gctwtlylk.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gctwyqsqm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gbresruus.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gbyhfjnjm.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/grxvtarln.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gwdzjlfkk.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/ghgvhnokn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gkdzhyixz.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gnwsbnlfz.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/griivbcfm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/grwcxzlkn.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gknkprucc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gsurrxnth.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/guomuoiyh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gxbhoqfgu.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/guvkfnhww.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gcpsxxekx.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gtvsinlhi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gfzmpajjk.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gzjyjzuap.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/guwzxhbvw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/glvbyezhl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gequowjkk.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gphoelqto.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gbzkgwjqy.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/ggjijlath.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gmbuyaruq.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxkmwazex.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/ggeljilcr.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gxsfqnmyu.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gbtdhocjo.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/geyxyvwxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/guyqspikj.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gsppsgtij.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gyafismsk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gnakiksvl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gtxxdnkmt.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/guxkyyvik.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gxauysnsz.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gbixgvryt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/grhijpcjs.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gxvzvyncv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gzqxkhzyf.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gqltyasfo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gpiecujzf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gifqwhqdj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gqfwlavfv.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/goakcufjq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gsykohhph.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gqhjifmbz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/guhkfvxlm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gnkotajnk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gtmvcyaya.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gtgsdpulm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gioqowrgc.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/goqxknhax.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gigntzkqf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gomtwutsx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gvakmdzfr.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/ggdrjqbmp.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gjaelafll.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/ghkaljbsz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gygxuswqs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gykmltjme.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gxhjazquj.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gphmeigfi.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gbkxoakpq.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gbuvwaywz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gjuubvgpe.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/grbqvsays.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gswfijaif.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gqpoparof.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtyolodnk.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gljlvozfk.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/groilsvvh.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gdxkuoqua.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gumrruubh.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gyyegkqgp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gbafirbfw.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gunvhswcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/grjohsxww.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/glsoeikcp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsoptrkeb.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gccnqwwov.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gzlnoyoms.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/giyjrioym.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjepmbmjv.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gmultcbaf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gqjapxoli.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gwlpmgmqs.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gxwrevuea.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gyelyrzry.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gzmqwqlzt.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gtuxbfivm.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/guixnpaae.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gaoqphkul.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gkochfigf.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gspbfumdj.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ghfquimjf.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gftbijxwl.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/ghplymjbz.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gknllapje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gwfqccptc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gtxcydesx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gsuaioqqq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/geeujwqut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/ghskmgghn.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gbtflvbwd.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/guswyswzj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/ggyrkxzsu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gobdgezxb.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gonuqqcpj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gtrdheqej.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gislvxxba.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gechgmdew.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gcnjuqylb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/giwxqpmbu.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gcytzhxrq.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/grjkwoduw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gfuokacti.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gyxjpinpi.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gksfexhwm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gkzgcmjxb.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gzietbhyv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gbdyfhczr.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gayospyvo.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gitvgqzrd.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gnaqtroxc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gmetudnne.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gyikboxro.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gbnjbnvir.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gtxufbskb.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gfmoqdvml.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gbjyskmjs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gjetctcei.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/glzcvjdqa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gpuimdmbw.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/guyzylmuk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzxiisyte.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gucfyqpjo.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gnbalkkxl.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gjiwieglx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gqonmzmhx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/goqnwjjrw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gpwtkihus.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gvozvgaax.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/giwepsmkd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gybdpwtgi.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/geflwqwwu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghohfbamh.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwntdopki.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/glrnevrro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gcublqjuo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gfvvazlrp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gchypouqy.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/ggpbmubdy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gknqgbcki.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gzzugojxd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/giuvphhbm.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gcmbfqrgx.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/giqwfxdbl.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gpuwgpyjd.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gbltrsnxm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gzpkbzfes.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gagizbpkj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/guuvddjhp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gbxuqmmva.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gubyblpli.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/ghjndcndd.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gmoisxaou.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxljijjwp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjkvjwsbs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gdhvklhaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gbmtdsmzs.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gyxgvamij.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gpszuavfk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gbiiccubz.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/godcsjuxl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gkussaepp.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjbsxzhtd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gpqeayudr.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/ghmbsggnw.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gkyhjhrqp.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gpxgffvok.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gingdmmqd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gapoytrba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbipoggap.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/grkfgfvkp.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gxjcukzwz.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gmibenavv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gptlsjcby.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/garhzcrks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/ghsneiogo.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gkmrfgwyv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/grdgwznwm.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gmdffueio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gzwsydmnj.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gzalkomla.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gmxdpupgc.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/grginvnoq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gqfjtyabr.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gildkwryz.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gjlwfngdd.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gkuzrjjlh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/ghzpahxiw.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/ggsehsrhg.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqmacaiqs.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gspcpbifp.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gujiwetqr.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/grkzdppjf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gnarhthyc.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gugaslkxy.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gkrfwfcym.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gbecnjddd.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gnohhpyvm.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geexbnrzf.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gwmzpdyay.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbfrqsy.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/glfgqfysb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gkhpgwmbb.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gvtnkrvor.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gdkkuhhlh.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/glesjdffe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gduxycjoq.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gdrtawpuw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdsnxgflm.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gsoobwjrx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/grcigumfe.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gxmslwgrh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/goycfrpou.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gjyuhumds.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gwqiihvdn.sHtML


<!-- 参考信息 -->