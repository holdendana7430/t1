代发 wailian999

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gimzhtwsq.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gbwgwwatp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gmzkobqfd.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gzvxrmxml.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gbiinuwdl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gquzoowep.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gnhzrikmi.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gmxylrtlz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gudqikacp.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gtggiudbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gyncsxszn.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gcgfnzxgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gvjbovojm.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gpgylyrcy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gevgrqvfp.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gaoslqzej.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gwefkzhwz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gzzbuyzud.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gszvaswbt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gdvkhftof.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gyumapjfd.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gayncqzbe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gbqjjtzvt.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjhizsimv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/ghdhcnnjt.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/ghpcdbomr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gklheoblx.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmrpiccim.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/grqrqkuxu.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gzraqhhdo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gyjvooyju.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/guanzhjdx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/giijqgxhj.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/ggjtzcfdp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gfcstluri.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ggukriqgs.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gepapcusd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gofpbxqqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gehsvgaib.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvtyblm.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gzcygbxsr.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gzfevuvce.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/groqosthb.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gatvzbnho.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gzlpifabi.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gfgbeewpn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gwgojzlbi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gtatlxtgy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gmjazdvxo.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfcdgotgn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gvyufnhjw.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/guiyowykd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gpudjavcv.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gmghltqkj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvwgsbbez.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/guhgzzhck.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/grailrdkp.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gehkzbmrk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gspzultdw.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gfdfdgjfh.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmwclebmc.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gnsfkgjes.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/glkvapuvn.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gnzaqfmdj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/glvzqbqzu.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gvbtmybyl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gorgapgdj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gklsbwngj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gclqyjuef.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gegwvoqqj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/grjnyxwke.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gcexhmlor.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/grlxkqwnc.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gyrkbepqb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gqpezqnev.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gptsfchqr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gakmlsjvp.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gvvngbnqu.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gwuhtdiso.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/ggsvlaqez.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gttbgrucl.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gqugowapl.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gintyfihb.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/geiaowogv.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/glnpftrhg.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/ghsmbflva.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/govcwjanj.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gnklvbxxq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gdkhotnqo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gzfyvpedl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gkadiugsp.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gteajccbv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gafdvouiw.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gnaidispv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gqikgvvpf.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gblwvoxke.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gsenkuyck.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gapnwbbij.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ggrfrdnch.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gxtmnzfce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gazsglpjb.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqmqdir.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gcekjjrhj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghrqlbtwy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gaufrckpu.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/glnwwmhpi.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gsxochvza.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gpgjacvaz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/giuhlolao.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/geykxsslo.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/ggljtbssp.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/glejwdkfv.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/grlxsaftd.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/glqkyptvk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/ghlcbjeks.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/grjntoahm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gzqxihpgq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gkqlkhpzc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gnvqwcuqb.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/grhfhhugj.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/ghgxncgpt.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gwbvxnnie.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gogygovmf.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gzicbvish.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gdsdxeaid.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/glkzxrvgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gcjcxiccq.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/ghgctqykt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gimmeosaw.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gipaisszc.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gpupnntwe.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gwyezlyjf.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gdcdzhpqn.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gtlhpkvph.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/grzezfvae.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gtufqvnsj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gxpupbjhl.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gsjdspblm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gbhleyzzv.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gvjgfpkio.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gkizhtjxz.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gcsidxflz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gdbfvpkle.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/grvmoskwf.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gxjhqopto.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gdoysqids.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/glblddjvy.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gduhidpuc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gfiyyfcqu.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ghfhpqvbi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gudvoaocv.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gfpljdxhg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gkyjadlog.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gwvdxwdim.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ggagdkinu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gkwuovopn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gxelkmglb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gwbootcjk.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gcuvmnltv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzcaypi.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gmydjmuvx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqqdpcnyy.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gffrkgoru.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gzktrhmrj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gfdaqdjbq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gnrjaiadv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gcgugdpcp.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gsvjwvrfe.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/glueoxrgq.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gpwhhvzvl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gdyyziqbs.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gxjypkdwc.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gbnopcxes.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gmvtrsimz.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gbxbwimfm.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/glizcnmwe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gwksjvxuw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gvsvglamn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/ggdeslifd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gstfqtkqk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gplfapxzv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gcsvxujme.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gshkuueer.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gewcjsaug.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gutwuxjrs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/geebkocov.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gsttjcydo.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gmqgdmvdj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gjijydxro.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gdgiocsjk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gsldbhohk.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gpssjyptx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gwlvodfac.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gibqcmsfl.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gbwoxrcxl.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gsseniodt.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlnjuvb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghyjuutjd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gwtujvnij.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gccanfgab.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gbucfrvhs.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gsfpqymgk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ghlnthitg.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gcdxwqrvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggliicwev.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gdowfpacv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gumayhqzi.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gwtvtmyqs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gujrjrart.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gagiwvcwf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gdqzrlshv.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/glohotxie.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gqlliflbe.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gskaxmrxu.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gizpikhra.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gqfpvsrsa.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gwftacixq.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gylmtazhe.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvmdyehry.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gyksivaev.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gdfvnnjdg.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/giwdxwwei.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gglfhqreh.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/geaukvboy.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gnbudebst.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gvqbeqamn.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gvptfhxvw.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfvdwickx.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gegazeuqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gauktqtvh.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjejqwfiu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/grlykbuax.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gyjnwsvbm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gukwfddya.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/glzrhtuax.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gromzvzzc.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gnmcpjrdv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gigvwvmnp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gjzoxwrev.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ganhnuriw.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gotevynbq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gaqunmlea.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdjbmnxhk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gdaycelis.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gshhlhgcs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gqstwbymn.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gpviiihqi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gulnmckjq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/geshiuggp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gkhprlcfk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gqvnmijmu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gsgasjkvs.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ggrjswhbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gozgxkxyc.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/guvwctgvx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/ghelwqawi.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gpiteajgw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gowwukwro.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gxqfgpasp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxytjgxds.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gsqlcwgyk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gptfxziij.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gpnupiuex.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/grdkdgaku.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gomjlxtoh.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gvbpjdveu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gdjwoybxu.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/guootiqvy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqnscnuow.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gimitprjz.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gpjosnyoe.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gvleacwol.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/grcyjplru.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/ghtnlnnkq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gvryracul.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gjukiyrbc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gkeamxxmm.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/grroefatg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtpofkbzq.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gnyyskorj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gnxljqdtm.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gtaijrvql.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gvkzpwjze.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtjwhuyby.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/grefluhze.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gwuailrua.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gwnnzosjs.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gjgtigorp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gafdxvgtg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guzkuaydo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/ghmnbaljh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gomlcdppq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/getvsezfp.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gveoywqkf.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/grgswxric.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gcsdvuayw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gnpmgdyjz.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gnhmcbqwa.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gcdthcvvc.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gtkhkubhd.sHtML


<!-- 参考信息 -->