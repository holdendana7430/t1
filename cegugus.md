代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdajsxfy.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrolnnea.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjobqaiu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjaqwypq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gocsmdefd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrqrnpgu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkjxtuptr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggnhxjbq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmafusvo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuazfurb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbyllvws.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gytvvmnrq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gxvclyaot.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gnhgzfkux.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gqzeanvpt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaofnxkyx.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gqvogslkl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnjbuyofu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgidwrzc.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gduvigyri.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpzqjvxh.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gomfrgsve.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnzkjejd.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gchynddbt.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqgkqzxg.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfyfjbeti.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiwoielj.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhiewbk.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsrrjihi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gstecejdx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnpahkuq.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpbieggj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgohvtny.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gsejqsgoo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gprdualnc.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grhmjdzgh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyrareiam.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzccusalp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmglteqz.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/grecznoum.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gufqnzyyq.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gmibhzjhw.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/geuynlokf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gyitiqbga.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/grwcmxkyf.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfndupls.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiyrrjbr.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpthvtubc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxfqvlny.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gaimkvzyj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdsmkfny.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyhccrmr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykkdbzeo.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnilfpsc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpvgcppi.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvpqbaoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbobqvasi.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gumzdybmq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkkhmplue.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjqqwwsgk.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gusihdsrg.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmfzngwn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goigzzuti.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpfdvipj.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gglftolgj.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbaceauf.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gejyjgzms.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpvxzdyig.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasohiylf.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcfhesbaj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbiwwfuz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpgpwmtv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxnnskfa.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoabzpfy.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlizwlsn.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowlqhxjs.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/guiouuemz.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdgwvlnkq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxjjlycc.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedagdxqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/guvomgywg.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ggtgfvacb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/glvuekwyv.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjynzfyou.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gimsqdecb.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyreeebc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvlyfulg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gclppuvnq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkclljdu.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gqcvtefyl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gohgugkoe.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gccjedbyt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gmgunvxew.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gyulanlod.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqypocfj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsbxdfbu.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkmtcyrx.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwhukfob.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdvkdctl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbxwxypx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gapypcfpw.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvonajzu.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplorkynj.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gkxutginy.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwpkomvk.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmnrhcdz.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbnqwevif.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaqrfupd.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gcdynlbut.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfylimos.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkmoatuh.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gsrlijijd.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gcemcudnq.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gjlschjjh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gozdfvcyh.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gupnmvptv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmljqnso.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiixdsam.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geiourick.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/giwomoeow.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gdjmxhuus.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzwuqauio.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gksauxehx.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/giqdlkzrr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/godehjmlj.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqarnwogz.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxmvjirop.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gehysherg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gcbvkebgn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjszapf.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcxvdchj.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gjzxcbgxz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhczqrfm.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gneavzfhk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpurcbky.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijremwkh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gposwzxhp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gggdqfxvo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaufhvtu.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcardjeu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykcqnbpj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqbikxia.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/giaczmzmu.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gylonhugw.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbweynz.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqjplmmzp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbmnakzn.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqlqwwyx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gqqsyyohc.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukxorslr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqdimxi.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gtvcpetty.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxmnvmpt.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggodzoseg.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gfbvszwot.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gknyrkwxl.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/ghvcrhdhs.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqybdbqo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geoyrstwc.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqhoflgkh.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gusgozodd.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gyedsqrlp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqedqrda.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxydwutlj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/ggjppjhhm.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gnwdumgna.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbqbleaiy.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwszjaczg.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gftdtfrhz.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/guxujqucs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqtoeemw.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gredixnjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfmoiiya.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaysmihqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gyxlqsqko.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrolimtn.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gsozezyka.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gizvonerm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyrorywx.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gjpvyscdj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaciycze.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/grghgjiav.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gcvbwxddw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghurchmtu.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmqwxoidd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxwyldb.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gywmxbgsl.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/goyagdrqk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geccctyye.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gtklaorcn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gfvdtmsve.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gyognydih.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gfcvnagaf.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gmigohfta.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gsfhiiesl.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnmotdwvl.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbmwplpl.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdohtbcgj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkpjtgae.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiyrdshh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gqqnkwwmi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqvzxwwu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gztmcngzf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghyhoozgv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsoyaaoyp.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/ggphcinti.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsuoosdw.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glamgmsha.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gponqmqiw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gagctkiku.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpawcdvds.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpzqgues.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gimedpfgz.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/glmzltozc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfpohxfo.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbculsozm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/grbcsthjd.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/genruadns.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gycudmaik.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmlelklc.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gohfmkjmh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhkaxow.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcalcxixp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsmqvqqi.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gflbjhlhp.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrrskips.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzzcnbpc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuwehogt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnojsvqa.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkshrplrl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkorxcahe.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gyyjtyeir.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/guxmysgxn.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwqtczgvs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/goybcmvly.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmzmbved.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxjmsezv.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfbsozqj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwuybioy.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxazfaxr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwbzlvcz.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ggohekqxg.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpihyeyii.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqwsmkvdr.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gumkibzjk.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/guvzgquuo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjomttoh.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gobqqyjko.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmmmyqpj.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzhdxnndh.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gretthcoi.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltobavlt.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnvnkjuv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gurahwqis.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gytieeirs.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoiftbnc.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkovyteg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdlctke.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqomqusw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfertvldp.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcafxezii.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmteouwe.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gotyiyktt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpdwzisvo.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaceahue.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gilccbpom.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvcnjwqm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuexntby.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmwufsujj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvbatjeb.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gnrlbbzkm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzccujxk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsktxrukp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gcqbcoyug.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtadpgxva.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgrbudqx.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gdfugdnyw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtljewhkm.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ggpvuygxj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyyhawgu.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gfruzxxfc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gdjnngmde.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbdyghpn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goaexgkhh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkmofyqc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpxoqkmqu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrzbrnc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzvtcdnu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffkhuovg.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gybfeusqu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcscvbgu.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glifnciew.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoslpldu.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gklnlhlsy.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ggihnjxza.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gpqishxfc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjkfeyaz.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gjrgedpde.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ghmlptdqh.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gctiajyun.sHtML


<!-- 参考信息 -->