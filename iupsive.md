代发 wailian999

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gzrmiqbqp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glkjvwvym.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsboqwakr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkztnrpbv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbztqugu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnlyrlsj.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqdrpvmhw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnfvejcxb.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gnbsgkaei.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbjseibnj.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/ghcaylgki.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghusxvrum.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqtcsdl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gfwavvfqz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsekbazza.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbimpppaj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gsresukxx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gldjtmcgx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxthjawyv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnggepdqd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gaofxbjdb.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gyllittia.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwmhbufg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gshuydrzq.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gyjcwxrxn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcbrzxwo.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwbgiho.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/guybiufkf.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/ggcuxcbbc.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gbvrfagmw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/glqiahfzu.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpjrzbae.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysnbcowj.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdogwreep.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdwnxddk.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gozuvvvgo.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciujivio.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxvnwleuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqicdcwta.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnxucjcq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqygjdzxa.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grzhxaadu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmzcvhuye.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gybowappc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfqfossbo.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grbfyvsjb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlvyxwyw.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gzffghhuh.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqvwphpz.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/guutcswjq.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjphhvw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gneslkwtu.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhyreoff.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gacvxgusu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkagwebbd.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmwztgeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtsccjnm.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdqxvaug.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqjwnmntw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhwuxai.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbpzelikl.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjhybpqjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrqfmyjv.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gdxkihtug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqojihiq.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gotmbjrbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnuvxsnn.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszjizxsb.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwocouqlb.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gmhivbohk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzvgneos.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxoygkfo.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/goclvmadr.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmzwkubz.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxkpwdmjk.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/getlfmeuw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnzwfadi.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gweiicqod.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtinczoio.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gtzkkkvvp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpasykcdh.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gojbklqtw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxsotkcd.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gunhavdbc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmnzslt.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxxxxqfi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfumzijg.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gauxxxjpc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpezxvhbe.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gpxwpuywl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqtzofan.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmrnuruo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexhbheak.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/glpkqyeje.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxhvzarw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvfolhrv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqvtitjc.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gugvycrbr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gvpilsjti.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gidqhdszq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gfodmkejv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/guheltjng.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gmhitzmip.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggciqozgn.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnrgcxnf.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gmiqpxpuj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqnukampj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gyjjtaqua.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/grkpfzpjl.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnihcox.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gnqvaszei.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gdudoxrkf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdtstvpid.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gakvxjqus.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaheybpm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxzczfavl.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtkqnoyer.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvztpujmp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gzawnerkk.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmywuukld.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gntojlpqj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnguepgo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/goxqubfue.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkpgixqpz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqmvfewcg.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ggzknhlym.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsstamfl.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/glmrtcnir.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/grbuhcbzt.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gljeymvgy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxptdxkgy.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnuhcpoo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzyhphv.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/grmlrndfi.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqpeptrly.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjgxnhyb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gweukauml.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtwlaorrr.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/girmtghys.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gyerodnli.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gaqohdnik.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcbapibqt.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmivliuci.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guueondls.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gytcqenal.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfabjols.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ghofiaqww.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gobyglrxw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grqnkueud.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gothfbjkn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gehsaorem.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomngaxax.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gocypuauy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjysukxgo.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gypdyljzm.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gplaexvip.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnqbkgh.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/glxndohpf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/glybhadga.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gtxlrkyoi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnttkoboh.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/grswgolxf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbpvjmb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdapjlctd.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdhyfjvo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqytvktmc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkxhafea.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gunfjedah.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyvzhlga.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhwlepzv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxgiyrej.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpfjvxqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjnrkiki.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gujyxxjji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gshrcoxsf.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzddyzthc.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gupaaobjx.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gaazihaog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxgvhgtz.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gflhknguo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpwfiqds.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gybeczwjl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gllyybunf.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsoisaxd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcbdsgwi.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoxawkne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggvvewpmk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbvhtqro.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgcyosln.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxohlcaf.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/getmxlkgh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geghrniqb.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcjdwncv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnssttz.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxmvuvrw.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/guprpjgco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gshwwkjxf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gorfcizto.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gyapweede.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gyagwqbwd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvhbkjnt.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvpybbjm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsagizwaa.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvagfnjr.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gutcmhqab.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkgmefsn.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvubreo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gpqctalrf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmlumnes.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/guwwekxiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgqagsrd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrscvjmw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstgndhaj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gycopwwbc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gafohqiyr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvicyxonj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gawvkqthw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfdkapvc.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwiitouiq.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvlprllrs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuhzkpdl.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/guomnzumr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzpkrmbj.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gdmrewswi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbaglail.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpmnfnal.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gpfjaxqpc.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gighmngdq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdvdvgvu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlvtpuuq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gfgmmobko.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/grwhfatkt.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/grjxapvqc.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggorcpxer.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcclqylti.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/giwdsjzyv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gypyioltz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtdcoec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuqtldoe.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkuoxsm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gnepwozzi.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gcicosocp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzifdkomu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gtbjqonba.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxovbfbex.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqnnidcwd.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gwngqwkzx.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gnuevnjug.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gvojsrhkz.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gozpykcmo.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gttvsvihw.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gklfiveuj.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gobovegvk.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/godxpssim.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcebmaomq.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gojhddiqd.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfjlzfvi.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkkmsdew.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkmhuswy.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guiihemit.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqreonncr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guvnouhhy.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvylweizo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuefhalq.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gjljmnoti.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwcgakfi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvgghlys.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlezvqum.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gavcnqagc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmksetjni.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnimjkbpq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghsgrvjxy.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gacafmdef.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqhowscjy.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyoyiibg.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjhaodbpj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gtacidsgh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gykqznntm.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gtujzjyip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gkkxoygfu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gicmbgvwm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gketmcsqr.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghuvzfrpk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gxxhfkxdq.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuxiiluq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofdmmfjg.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gaplmhwwt.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzttebfeu.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gpfkvtyyj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjplvxaab.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyybjtki.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glroluevy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfzqcztri.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glsboxmqf.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gksfokipt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/grwnyecqq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcuykxjm.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/geknxbrng.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/genlhykoy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvdsexbt.sHtML


<!-- 参考信息 -->