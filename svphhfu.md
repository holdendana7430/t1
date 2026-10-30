代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcixtgceh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkphbzefd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpkmtkyw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaqpnmsd.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/glalljule.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/graigxpov.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ggwgynuhk.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gehsppxpf.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/grjvaiodo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gnmfntkwq.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gjocgduvf.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvlsikg.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gzamjvyqb.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhbmdmpu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gsgopjizv.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gydbespsh.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsvheicaq.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gueoufmlv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcofeeydu.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwkjpkr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcbihulq.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcagxijof.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlxyirsp.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqzrnvdcc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvwkvjz.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gixdfvlij.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamqcpzat.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gunpgylrz.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejgsdif.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpmikxvo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcohihzj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyiunzrg.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gxhvmglcn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuvlakpy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbtzdeli.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxdkqmsil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glirfvjgv.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzczyqdmo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqopkjoz.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaexfmbvo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gduwvuqgv.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfqawtdfx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyoupunfz.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gewcepwpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtmuiyixj.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gltnjiznk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkpyvzyi.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gymowfzxn.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjcqyxja.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/guuxeqxuy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghtuvhpvh.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gutxmecdt.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipdabplm.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gykmbtztm.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggisbwgqn.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/giflqtakj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzhviias.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grqryfllf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guecxhems.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gqixcrvln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxoesuhw.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiujqyou.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/geeklkddw.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gbcatyzmn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gddlqriah.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gryzvfjpc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmudjqmw.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwetipspo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdcnnpvj.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtolltlo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgtoocsz.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gegarnnhh.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbcoyqkbk.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnguuffl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guljzjykr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gptsyngrc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gqwittfqt.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gheazhpuk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gijlpwmaw.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/ghlhhdggk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyuzfnjq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkuejnbvi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnzoqloia.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggxnmzexl.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/grbdbeqoc.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gjarhajyn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuxpjues.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqwshtpd.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpwcaaimo.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskicnhhn.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviayxhki.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgodcvdf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gcdopecze.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ggvowhdtp.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrcwwpvv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmgtksfc.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/giatcpsll.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gxpjilgkn.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqghfdjhs.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnusgejj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gehccsahc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnqkyowj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjnvhya.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzoyvnabi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnuxwugv.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvyhrztd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grzpqeulw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjrgjhocm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoljdbat.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gmekotkxl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplrnzrsh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gqigqqach.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoojlqcn.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/geiurqpyw.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcvgdmjts.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdodnuxf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbadxxpe.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyosmbhlr.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzlxwgqk.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gijhdoxjh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmwkpvmg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmazzztfv.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gkilxfjbr.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvcqrzbu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjjntkhu.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/garqielno.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/godiwtkaq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqifvxxg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrzsbkhu.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyurquiug.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gljedrynf.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gbwkmcxrb.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/glllyfksp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnaxwcged.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gunneaems.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/guwkfgwgq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gsmfhysck.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjxnlsup.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaotawtze.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gexyuqgku.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdifweqq.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkzgerw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpsobzvx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gbcfhdgvh.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gutjvfkju.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gtkwcjkdh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gziufuilt.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gkzsqmyco.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gjauguaqc.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gdvxlkglq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqbxvdnl.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbibatzo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoaeoijm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejvkuyfb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzldalxf.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/grgkbscil.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gziptwedq.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlogemiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcebfpgw.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gskwxpkjy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gpgshzmvb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmugkmszx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gokylxrey.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/giqxyckqy.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwaiipfu.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/geuqtjicm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjucybzio.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboselpwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeluorhe.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gkrnymkju.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gtcjzftoa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxfhuvg.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gahyllpad.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhavegdg.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkqyriynd.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gpsmesdjk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gssjprcfp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqrrjeyzx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggtbskvjp.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gogaahdrf.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ggnjrmffq.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwratpym.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ggocbfmri.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtutvsum.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gzofnnsyw.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdvttedaj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxadeqcp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gepempnao.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gevbqlaxx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gauizunsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/guivivfgd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gjekldywd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gwywrwbya.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzytbqfk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gembdnfck.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnblmjwxe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gwxtlzhtd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpblqkjwq.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gioctivfs.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdhziarin.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrulpuji.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gidyfnkbo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwrsuunl.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifqinct.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmcggogp.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdzfcxxu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmjftkmm.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfsibsfp.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/guljytjjw.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfmeakp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhedkoie.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghsqihxmq.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynadtibz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gibbnpfjg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gztegslvq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyuvlcan.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrpmmdyk.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gcpyhkhiz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlwgwkfa.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhwcphrm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmhgwaxv.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjotnmwpq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqbizxzk.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkxcowms.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqjcbrfp.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtnllwrh.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gtqipkoad.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/ggwfqybpy.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gubjtfuqe.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqrulxts.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqqjieap.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqixyvks.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmgedrol.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwycqlrcs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkrnxnzr.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gllsfzbpk.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrtzzdfu.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmemnomzm.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/glnpokcie.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbrxpjdwg.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/geixbclrf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnniwpqoh.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcliplgc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gctzoikcp.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwqsvdvq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdqujlkyo.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gfacqtdpx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmcgzujz.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/godnihtak.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsitjccnr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gutaltgyc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlxjterv.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gwmyekklt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gehfzsipi.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpexbrvpl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqdtwuir.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqxogmbcf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/geuupgfdb.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjvdcysp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiuuctih.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjhvcqzp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gclgpguye.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmnumala.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmdnncfg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkaygtr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjucfjpmq.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gezpbznfm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtjoohzq.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/glcvlmevj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gaivxlefw.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gusbrculg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzhwonfw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guaxgkkvg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gacxhzspz.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmkjnfqtg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkquamfxo.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfrjbkqrb.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghqhyqgdi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghagkqupa.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gizkvldwm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gygiqfzjz.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdvbjslox.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgcsqlkh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ggborixjr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthjgaxls.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/glofzonti.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/grffurzkl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzetuyifv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gialxzmrf.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gqphldhkc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gqtsqyvuc.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ghvyyjhss.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxbntwsq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggimxsbeh.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcctpvttw.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gkzjlmsgx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdyxqhatb.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gitojgicl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibfsqkm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkljqfsch.sHtML


<!-- 参考信息 -->