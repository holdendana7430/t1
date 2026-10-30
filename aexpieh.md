代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrwcfjrg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaqlnnjp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gprvkwwtb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghqzahuou.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztplrqtl.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gaibnuvra.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqsrgdqv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwsbnozy.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaijrjvx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaspveael.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gaophfjks.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgjdgbbd.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gciaynmtd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlioxwiv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/guyttqrhb.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvnglkuea.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/ggamolaca.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdohtbkap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbmuouwj.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gavjmohrl.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbibbdau.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godrwdhyj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmjlony.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlfhuenh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grvuctrfh.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfayhtyi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggzjkwmja.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfxrlttsu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gjccsptjf.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gifkwndcg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/goeamjrds.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvyjhdwf.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyqdbkrf.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gukywfjgk.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvkkmacv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gzviopgfg.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqqjlknh.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvacfsto.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glvkliifw.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbyyxkwiv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gaymmfwoo.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkddotuo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqpvsqsu.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gskxxxyyi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxnjacayh.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gcfhxpilq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsisltqhk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbzjecip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqezmbnm.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gaudhcoxd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwzvvoow.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gplbvjlah.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpedlvqok.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyfukiuy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/goqukovsz.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/guckaqxub.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebqldau.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/glersribi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdnbcdtt.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gliemcgsc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqvymjgxl.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjnytkxv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gphssfimk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrztdjub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxcxcfrw.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfykqctmb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/goddebehn.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gxibqshxb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gupapmvtd.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuahbilx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfonjujf.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbriwsnzk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gacoxerad.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmxzkhxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzkpjjpy.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaseccyts.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gueyfpcrp.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqpxvsez.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkanhtjod.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/godrnhnrz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahadlrsh.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdiojhgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxvcoxu.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyjvqijt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gwdspcnou.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzviicyzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtvzvdfi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcobbiftr.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsiajkra.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ghracbvdl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdycvqbbb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdpuzasb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjjwalvc.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqccmrlav.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuxsghob.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjxncdgp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerktqfzd.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gslijjwib.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gusytgwdj.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/grnhenqpl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/golqginkv.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqmrhahyq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtshdcda.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpqyxiev.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gyixrecwp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/glejeftlu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gncwdkioo.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gohddarlh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geqtkylic.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhjvjvtg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuetgvic.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gauakzyud.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofksqgc.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbzguxbk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjqyrhe.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvsoizp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/guvrqjoiy.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/glmttlsqi.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gratyaxso.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gwphppjze.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsvpkfjs.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gersioupa.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/givdlkpee.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbbpmmoy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnscvoqa.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcpccpkq.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gxcjrusws.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblkgaxsh.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyztcuvq.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqmigwbo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gigbvjlue.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gccknlwcl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsjxcpjy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamerxatp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtohnvofp.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvlycxrg.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwrwrjje.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gojyvubbs.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gasdnddux.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkxibuqnj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvbqgwyg.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgftytka.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigaeksio.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gbxsdhvuq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcoonpbr.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ggnxnrrcb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxdydjmh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcemoflak.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/glgbnymxi.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghrdykeek.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcaugtozf.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnibidmz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghnmqkinh.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gsyfmeqmx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauipninz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqneehrsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/guyzzhhgh.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gxqhlnxzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrsvzdmh.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfbfewiq.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxrzroy.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilzukwdr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtjeyoll.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplwuapro.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzlvwzvl.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gamkiorez.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxkkdvgct.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpimiuzu.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gaigldsgg.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfqtzwyv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhfycrg.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/glurpwvfj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrsoauxv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljwxcuxa.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gortbqjcd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gklpeybrh.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdbzwhoi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnbuyvmj.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzduvwmec.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gerfcnizk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gccbmzyqp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gipuriipc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gpqrybzlx.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gisnbtzdl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajqgbaz.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/giestduzj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhkeyjnf.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfwuvrjh.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwnllbwd.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqoipbvw.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gauhfhubv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gahugjzcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gaezjmitr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ghojchbfu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujkwllb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdmqgmgj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/ghvipwxmr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutvozazd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidrchamn.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gftqobxtq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/glocthfuf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ggihnkrhq.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gukwidhxg.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfxcgekc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbttczeig.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/guyegeuau.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvayrzui.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gagxiudmp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjknhjam.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goudiyoyu.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtpacwdd.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpwttsuw.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjitipadq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/govaxckql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gjcqnfznh.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmxtnrwh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvzhkxrn.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gchbwvswu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytmcfovm.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyicpzlj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gihlgmgve.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmmstdki.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgvbyqzk.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gsuvfuhls.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtpgruwgy.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkvkqtku.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztdfuerj.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyhumxquj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjmwrum.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gretoepbo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjyjssrb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/ggkyfjpri.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/grwehsmsg.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfdvaupj.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrnvpbad.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxkucpmt.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkwduhft.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggdfnpglw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gjabfbxfp.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gsiydpqyf.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghnxbaujy.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gennrhnzy.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfqglsjz.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzjnbbcqk.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfmowqjn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkkocwdb.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvatqtgd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gebkczuij.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gognxcjnr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwsygvba.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gqrlzbxjw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gylxdusbo.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkkpjocj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grfupuhis.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gagidwton.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsjkfwya.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gbipmnjil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giorojmlc.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkfrhbonf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhicewod.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggdvxwvaz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipgadvfd.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxomfjmq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhmlikvr.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpitjvxhj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gigruqfxq.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghnoowxmv.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gneuuaksp.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbiecisr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gmmxkvdmn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuueooma.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gldepxdzo.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gmtfxmvqq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaohuujk.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gwzvnpfrz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtheuwpsk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gddtgxkdd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtwkgjccd.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsgmvqsgn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/grtvtbtsj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvljjtook.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwkhqwod.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnynrdhyo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gleknbbks.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goswivruk.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvkuxupxw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvccvwmi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gfymkhdyj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpwhliaje.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gzonzsydt.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gllodedmy.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxkagcyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gmpkrcoyf.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gquhfacwd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gmsxnqbgv.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gieaapxiy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdhwbavn.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/geztlposa.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gygfejfpc.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gvhqboims.sHtML


<!-- 参考信息 -->