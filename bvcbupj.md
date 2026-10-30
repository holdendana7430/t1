代发 wailian999

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfrehzay.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtphvrukf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulfpniab.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gpapuilgj.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcxqrgib.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjbthloy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/giaejbkxq.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gchstsjoc.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gbltjltyd.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqhawmrfl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvfwygcd.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknsnlqou.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvwsnxgi.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grilnagyr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/grqgwcqgt.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvewmogeb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcrcocdu.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusbqmiqy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkicwjgxy.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvejaskod.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrbnoxht.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsdfmtat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gddjifzup.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/ggrjkvjau.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/groknkudx.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhxlgjis.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuztdwyk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpczcdmei.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqihoyhh.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgdixkin.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpdvmykl.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/guemwhwcw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gafijmqmx.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gztpqbtrk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gigpiulkp.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwzrtdpnd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvyhsthr.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpqfzajyq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbawhjlcg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/glttopiww.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqrplnq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygbrgawk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfvzdcbg.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpkbndlu.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtvepdptr.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/giqjxoiap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiuflqmk.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdheufzg.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/graadswhh.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gvibduklj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyogxtyyd.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxticssxt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzadhuict.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/goqzawslc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdwyhkrw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfjiugj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggooyhkpn.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaezepfy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpuorzts.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeyvsaoh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfafezkl.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gyayzvgor.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gwvokyaqq.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvbxzmwi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbazaygyw.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnhwvojn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gtjlljtnq.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxgcfqml.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtzbqtjl.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/ghvowvsxj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefgxzbnh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqdgfnxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/grsymytqk.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjaxqlrj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyzcbofi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviecucqh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gyaigdvnu.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhirrbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvksdseh.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcblhevnn.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbgzczgjv.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjqutzjf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/glxqwkial.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldiwrwif.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpxpfwmjd.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnjoslbn.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gaugxfkwx.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gvydobenu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtrmerxn.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gildpgnmk.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkhfncumh.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdweqdaxd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqzqdxel.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gttieeler.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcrzyjpw.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghefddpqh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqbfxatr.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gmmhwwbrk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gzgduoris.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwewdwsad.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeawlcqu.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgoqgwjq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkbjyxrx.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbanywkwo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gofgfgjsg.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmqjodbd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwmysry.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/grycjauuk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gktncfssg.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvmkncuf.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbqftqmdk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvupcyias.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpmuouyj.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbtvlpebu.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gatemsjxt.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/guevbipmy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqvheumr.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsmrifdju.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gwblggwsd.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqzgjusg.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/grznjcyzf.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/giyugigzm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/grdkyjwpq.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gwxsubmaz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhivmyec.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbcjdxfp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/grelnfsfn.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gadsftjof.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikxzwcxv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glapaiagz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvfmncxz.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdkyzitw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskqrrdxw.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gefwgabsu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gicibjyvi.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbkfpabz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfkwubsy.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjschydzp.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxntkjdt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gniyunxln.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gpiikvbqt.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gujlladub.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwzyxabeu.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlebhjlj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gatcbrffo.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqzukqtqh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gfrjywiai.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/girvkqyga.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbubefgx.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/glzahheba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbnhscysc.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gulirufai.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gberfbyvj.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gmancvyeq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gldltcylr.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypsicbzj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gymxvgyzw.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpadbaatv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/goqegnnmw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrchkbym.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnsyyyzp.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwtheolb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxcyngyhj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gtswrmwfz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegismyep.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ginypkgjt.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuyixqjp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdwcjklep.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkmivgkbp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffvekkkr.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfrppnln.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gncguctju.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfukmctr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/galuczexh.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gbnsukugj.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeariwyb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkeghqb.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gylbvgjho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxzphbcz.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gccrgixpu.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgohksvf.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ginnbtncw.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfusvnbg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjermwhru.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbhxezqs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gidvatxjh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrcanqck.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdjpexx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gxaqqzmsj.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/ghngbvqaq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/glueilnjp.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhowmsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxsxenqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/guqwjtzro.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzbhnloz.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggrrbzbgr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkgawjtg.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjnwogzm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxfqapr.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsuzpqhb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gktqouyln.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtmfiaxca.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpbquyfwr.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcbbdgzl.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdhvybpgy.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/giafofynh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gefdnabio.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpsbdcxas.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gafziphfa.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcywlitcp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtkqwjvs.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpxjeld.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupntjpqq.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gjneuxdxr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gxmydxnbn.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjwlmkicf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonollejn.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtliqanok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gfpzabkue.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsxmweuh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/goakmrxpv.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcpycysd.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfyzmugl.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/goojrabea.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmllkmmua.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gvkdvemrm.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxjdtlvy.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdprftuux.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxyxpwi.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gojiexaks.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipebedey.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspavwzub.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjcpmej.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/glhzincly.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqbsyuk.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmigdfjyj.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/govwqfdeq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxeylrawy.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glpmbqozd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaqgziwe.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzsrizqt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfwxxqxo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gwiczwbjy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdzkuwmlr.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsoiybye.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gskdlpixa.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/ghtmgofpk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadeeucab.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gqmdltdwd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtbdfyga.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gimxoiouw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grybuqvpl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqchlfhrg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gymglqrya.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrjwzjok.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/glfwtwwkb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ganrujerc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/glzroqhdw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfukiqjqy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhdxlvs.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gzzsqyukt.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gjorsvrlj.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gkendfcug.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghdqrbxtw.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvxxxzfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gydadjoki.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhaexjxm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcpbqwedr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiqcfxbp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcivftxcy.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwqdajkxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzoinllp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcumyzlaz.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfqvqbahy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdlmyagw.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtdmqnew.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjuqrhbwd.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsfsxxnem.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxnaspaq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcxqmnkb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gukhhvcef.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsnhclgx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ghcwgkimd.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoicblei.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgxzsotk.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gtbavqrey.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzdomopz.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/guanzvfed.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaxbboseg.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnhejecn.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfnhaeol.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gryokeseu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gwrruicyl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaikphdon.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gmzwkghyq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gccuqfyea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gepncpgfi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkpppofqw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvneysqz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdhosheb.sHtML


<!-- 参考信息 -->