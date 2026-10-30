代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbfquzpg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvowhgyr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzfuuccy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjtkhtuc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gjoxemoof.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gmueogslz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtrkgqj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/geaxoxgfk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gepuuqzrs.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyljerqd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvbisytb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggwnwumen.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkuaydord.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbgxalvh.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmbjsmem.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcgtqpb.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gqbzqctrf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpjtrkno.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gatzwgqvz.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbgcbajba.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gvnizlrbo.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjdhzch.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhobjbdj.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlpoeyxa.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvlqhhto.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqbgspkfq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwabczyq.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggskofypx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gejjnzgyj.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcsfrgdzd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwbuuttm.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjslejwyy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzgcxmwm.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfxarmzaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkpqlmwbj.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbbxzfpt.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlfcgeyk.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqixfyhc.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdaurdjf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/galwpzwbc.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gxqdnrksw.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gelgfxlbm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ginutjnvx.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/giybfarpq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbwpysigd.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gzcrbdljk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnbhsftq.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvofzqffh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhmvipzp.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqakbokjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdesvdbx.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkujdqhj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfukarxcr.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gaulxmszh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceaifftn.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/guynwpmbs.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gppfsbgez.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqywjboyk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmnczqfj.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnihpewem.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmmdbxfft.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyiqfbxu.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyorernsa.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiwtcwxb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gultvnvvy.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpydrjggp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gswjziygv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gqxujolwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvimevamf.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/golanegvm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gtmoeguhr.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjatyetx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gineedtzo.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmwykwus.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gstusqkka.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gteibtvsu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfzvueaf.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcqhabvvt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmktqrcdd.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpelcrsic.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glqnnxrlh.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffavoff.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmwvepudm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnbrykvl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxndoffo.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndblepjj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gslzxjycs.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gtebbvlzg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadhckvb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqbyfuwfy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gotqapudn.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyuiudftd.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvzqnblm.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gesonottc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqlhpasc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlvqndvg.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gatkhawbc.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/guvdirany.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gagtzefhv.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcamjurk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyboqpvk.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucwdlmkd.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyjqhjyc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvojeivm.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ghlpxvfzx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwwzuhpa.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshvtnsce.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvizdlgn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoqnujax.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlaeeliq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfwohwkx.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glbqqcevu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gffkqlnmi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gwlzwuocj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkttcxxl.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/giojnmcwn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gysilyilw.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwsodmcde.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbpuvkocg.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkndwypf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gluukigqh.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gerbjymfa.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwzvauj.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gskkxwutq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgooxmzc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwgudjcr.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkouyhvrz.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/ghusdtfzr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gkuktwwsx.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhopeol.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gequhhapx.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gigskwrgp.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnholzhtg.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmcawsrfz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcolucxx.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gfovzurnj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbnqftqib.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gyjiseszw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gkuopslkw.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmgtixaon.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxuuadbp.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/grjscdqoo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gixjzilkc.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gehtbnbyr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/goivrscmc.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrvtkhzl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfknuhmrt.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghimelmif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gqrxwfyze.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/grzrtlsxw.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnvolpnje.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpxsdwrl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gfumwzfdb.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gsymcxaox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjroacua.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/ggdjkvbhg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gpahilxul.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/glptseqct.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gzlmelizg.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gszoufxij.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gmvraohpd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzsuzbkm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkpazykm.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzklangyg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylvbxmes.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhtgjwqy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guiuqzbvd.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeooihwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgclifgn.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtzxhxxui.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gieszavbh.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gaulbsdab.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gyotnmylj.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyzyjyfn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/grumuvgba.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjuekacj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/germejewa.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gpqpgcjkg.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfokaflub.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmhbtdmc.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ggxdtxmhx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grgjyjjxe.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmbvqort.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmnegyzc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwixijeu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkolbdil.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoiwwnph.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gfvvgnflk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcrztwoa.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpatlkzs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gyvybfknr.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuswqrxg.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghmxrvews.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/girukcses.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsvpvqoe.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gefnlsqqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gxyyizwbe.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnynpkoj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsvxttcx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpivznnte.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdvxcet.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gaqderfzb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwslbttp.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmtkihls.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gokshjeaw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gicocgmrb.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugakyxyq.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmrdymzl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqabuvasd.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gdhledkax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/glbnqqbgm.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwftsvnn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmbqlxno.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gytprdibk.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlodgfth.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gotqalpaj.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrndhlhr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkshpwws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdghlmqif.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzdbnlmef.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdngbbgpi.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzkwtnja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsobjime.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkuglhjh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gkuxgqylv.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gewwwvyml.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gkewniwtp.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gevvbwlir.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/goyeqeykb.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gtwaiwtzt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpazdhojp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gapspcfxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/galgufspl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjowgmow.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggolznmfd.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gwwssyolr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gvpjtyiza.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdxslfcub.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggacyiqb.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/geqqwftam.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdejvaimn.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/glvlzjbdg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmaievvm.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbvhphrn.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/glzkddvfz.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gilhhlfax.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gyjgqlcct.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geppidlle.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvrjspwu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gowcqcwej.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gndvnuvfa.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gpuhxptdd.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpiismvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gisnfrrao.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gzxpinpxl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdfhqrfop.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gujcevpew.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gttwevscu.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gyjhxrvqo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwixsmnfo.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gbwgmxgyz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxedlopbo.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gijrgwtrq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnvhqqon.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqpjhchht.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gjoqlnqxv.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gatyifwpb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsywnlcau.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtfnvwjpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwcuaoxjh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloywjtgw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gmyowbwkl.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/glbzycibu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyjmugwj.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gtopwhmow.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimnkserl.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/goicgasjq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/golcabcks.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gbodrpfku.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaninrxe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyabptly.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhjyvtzl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyefjnhcy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerorhhmr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbqunfnj.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxzmupwy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gxzmdfmja.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghauwmkqh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbedhcdm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmlayxps.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqfdhycfb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gygyxniky.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnprruyf.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkroqmqml.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/guhxcdrbg.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsehcmtf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtlfkakz.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gckmecgty.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzemfashc.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqrfmncy.sHtML


<!-- 参考信息 -->