代发 wailian999

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/glxosdvti.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/giqkdwbhl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gyaqtmnkd.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggrufcnkp.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/giphzdrth.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjsufefh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopvsujve.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrirdzyl.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gndzuamoa.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gevzlcwne.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxbgsdkvx.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goabahtdd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwrnaafx.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkcwzutg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gohvmejhp.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrpcicsw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbniwfkn.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwjvybdxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbqncjuic.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtsfuqt.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjplvavy.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpcozrnkg.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkxpxotv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqkluhomu.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/grzozdhpw.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfodqxkvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnhjumto.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftqhytx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gadafzvno.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gqvqhqyoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwltvrzzo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxhybvkd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkzsytkoc.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gllcimpwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gujhmdyqj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxxhwyfs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gazrjgros.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktxxbjz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsxbxjsi.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnblxkokw.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glefhtezz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoxogjft.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gziufgbew.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccsazilu.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfvgehsk.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gmbcsskrp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsdlykm.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggoegwlxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkqoqcolx.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gofpliajz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gglnadhjy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgmtxvyj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnedejrg.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gngmavqmw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gojndgdic.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gepvpejqg.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gguhsevgh.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/ggttztyvl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnwgpzdx.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkwxtkqn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbltmjvtv.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdplcmbou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/ggulorhqq.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/goutuimxs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjtxzmnu.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gwbskkmda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glfqzoutp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gvlwwtjlc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gwbsltxqh.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmpmyxni.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gnqnwgspf.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqgzfxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbfqovga.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/giihkxewp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqirywxy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaedoceb.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gchkkhvbp.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfwexgcm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcccjdfk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gosboucgs.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbvzrbtx.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmuzolwcv.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfpisggoa.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmfmbzsr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbwzmsyg.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gaarzjjme.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtuwudfs.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqtsfsker.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gaodyrabu.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gywzfldbg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpygswjkz.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpajjwhlf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjfjmmr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppteeace.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gayiumckq.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxafqauei.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geichiosc.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxgewiivv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gugbgxgxt.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsbupdqdj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaudautz.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdsrfvspm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdppdpwbw.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gupzovtju.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyuxomhy.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxhkcncl.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gigvykida.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/grkdwkelq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvbbglge.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciegukff.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gitzaquhf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbwwermc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyplepwv.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxmrihoww.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gvoaupzgr.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gorhmggxk.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gvwsvglvc.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokikxxfo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gififhvux.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gemujqcqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/glwlsqmar.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gekwmsler.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmtaewqb.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoiytyxb.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gpohjpczo.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcxrcopsh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gsmtpidml.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdzptzni.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwskerbxe.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/goudlejei.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gepubhihi.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcblrrdvj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gzqyuulps.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbjbgepo.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gdpthbcnh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvaqqehr.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhtxoedj.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gjmzfftyv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqbmobmo.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gjnszoggv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhhzgefx.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ggudjdcmq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gnqzdbqtm.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqgxejlp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdphsvq.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdygwenob.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmuffjcyk.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpmiolyu.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gxxemvfjj.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybrzpepj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjssodzl.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvytkahdp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gndbtxkdw.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegxdivkf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsbupskc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygojxpnz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsishxul.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgffsmpv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwvnrvrg.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/giurevzgb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzscplp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gykusyptt.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gblgupsom.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwjaqjvb.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/giibxfrie.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjpukwibk.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmokpwlyh.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxcnvkm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzngyarp.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxesxaail.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkquewqpf.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyejmigxw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtthpkquw.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gkahzyrhd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gydcmybqd.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbvvvmnvo.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhpykdgf.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gubhzntpv.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gnmegixtf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyutgfmug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ghmbpzzvh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfkzohzb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcadqspwo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gyeqyurvx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gfdwgliog.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojtwxhny.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gildikvfi.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtiurpikv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/guzrgwqkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatumzwyo.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyhfdnsg.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glgbxwdvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoqomuea.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghfjujguy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvlzeiit.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gitjddyne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ghcyduclj.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlxwgoto.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmoskods.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gwanxyqco.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhuojock.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbwgwynv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjhbzbgo.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqejnjkqd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gintzrbzg.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmkskvpt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gmgigqlvw.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyimtzss.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxskaulgx.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/geyvhchkv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gysyjhkio.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjkvbttu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gnptvfeyx.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyptnedl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmofzsho.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gaccdikez.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gokrrczkr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkatqzot.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gyjonjrrs.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gzotoduhh.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gsqxhnssg.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaxeiulc.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gykrubcij.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhifmpyj.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuxkwzqe.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gochwcscd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtziopkkv.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhluoxtc.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/geqqutgoo.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnctqjyg.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwclolmh.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqctclic.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gzhcvcwmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gphdlyhpe.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmmvuvffg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnalosjia.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkvgygsi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbyvkhuqd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gvknhtxgj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqiwaaspj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gkwnqeixj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnyfvhkqv.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdyxhmjg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghikkvohi.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gpmsblelw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gptwinfwq.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gamkzzynh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnhwyaie.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvysqcqyl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gyplxlggx.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gydlmzouv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhkmeial.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnskbhuck.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gktwnlqkh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmeerli.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gvhhichjw.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gdcptuemp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldfudznb.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqnuswlyp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesoubaqq.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/glozyvvhb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgepuuhg.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmobldrqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glwcuftic.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ganruzhia.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gazbhqurq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyezibyn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzyuxsbc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmibbslld.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwnwhguog.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gogyzyyuh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcknqtzw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykmfvyty.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gulpljhjz.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gfaogzmhg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gndgnkxhp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzeocdzso.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/goksnmseu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzglsvdml.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gibbyvwyl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcktmvjkf.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ghyccljyp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gomtygcrp.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gmhrmjmov.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnhhwhlqo.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzorcmrs.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdatozyc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqtgqofc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwtdmddyf.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gjguautfg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghatuhcvu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsaueivd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gqdmncsas.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glpzfoudv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ggegxwfam.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggilbxqjw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaxxnncf.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glwqsscqr.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpweohygi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdhsonv.sHtML


<!-- 参考信息 -->