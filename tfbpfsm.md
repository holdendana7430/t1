代发 wailian999

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gafzhqcwi.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gcrwsdmrv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gyducxjis.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/ghpoigjyv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/guirwwbfv.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gbysfirvi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gimntxnoq.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/glpoovbhg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gpfxgsekc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gtocwjwlt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gunwwvoxd.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gceetryfz.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gxbpzbnqv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ggshadvyz.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gxjbvetij.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/ghyzhgbmg.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gzzdeprco.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gpgmhhoms.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gjnlpmgkv.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gzoduxojl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gbhvciukx.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gtqeimcnh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/grvzjcbfu.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnmmqjlxi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gtconucuc.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gzuegchjc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gvsoiyptv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/grahwexbi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gmkvqiehh.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gfasdqwyl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/garudqibt.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gkdwdvwkq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gljmncwuu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gvcurjwix.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gvwbqckwj.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/goxyeiuhn.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/giqyaponx.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gdlndtaoa.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gyoaztdme.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gzfhscnwv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gurwqgyha.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbazsafso.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghoudzobf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwudlaclk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gdzwvvgvq.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/ggkppblwv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gollwhfry.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/glinvqand.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gmashhcyp.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gunztdxix.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gtqunawds.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gjflirqfp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/grdgpiuhk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gqdfgjlxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gtfsmwcia.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gfdmhnupa.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gmdebmysi.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gyftyrfxw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/garfqfdra.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gmrgywiho.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gypwxxuyp.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gbgoxhgks.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gibflnslh.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gauejcncd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/ggwhgyeze.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/grdfqwqzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gvajgkxsq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gqrcwckuf.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gsjaaxfjd.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gwrjucnzc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gcudijchr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gykosmvce.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggdzcfizg.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gdnwnrrzv.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/grxkrypga.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gaelislqb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gwqvxjmrf.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/grmlssfet.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gtknuxfqy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gaipqqbbz.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/ghadvwgqg.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxytjcenz.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gwxdxsfyw.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/glnyscoyx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gmolkluks.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gevoqyhzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gaoehihts.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/goesjgugd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gtckjiqsm.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gqusllaxs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/goladfbdy.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gyzbjdwzx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/giyntsvbp.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gkubvsant.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfayfsmsr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/grcbdsvkq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gqmqyqppc.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gppzgrxtm.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsvswthmj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gugzfdbqk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gqhlaqced.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gynxnchdj.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gagfubulb.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/glmarthoi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gkslzlvra.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/grqgwigxw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/glwsdhgba.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gjmmlpagv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gangyhqvd.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gpqcpvywi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gnnqlxgfx.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/goptlosit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gfqwkbgfy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gjvpepmjl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/guquetcxn.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gnqehktaj.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gpealtzed.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ggfgsgpwl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gpbgyqjxl.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gdlwdvudr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gequflsuz.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/grehugqpk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/geebehumi.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqxejkp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gbvuipxxd.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gwmavtcxx.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gdezzzxml.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gbmqskatu.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gahdtmvdb.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gwdfukzme.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/guhufgczy.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gfsukrsma.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gbmyevlyz.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gztjurltb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/ggbuwhjmj.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gqujngcru.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gqoygsfoh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gcvjcqhsk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gmhtkdtkc.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gqgfadtcx.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gmzbbzozd.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gejoowopv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gfflilvbg.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/groekrvmw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gbmkmksep.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggmawqgkx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/giaqsruxn.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gbnkzqtil.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gpsytgygp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gfonkmoyi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gbbcdpbto.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gjirbtiyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gnxxrruzf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gfctrtocx.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/ggocgezxw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gssfhwhre.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gonupcnau.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gspuyoajw.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzewnxhpg.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gochlzgzl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gllvjbkqj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gylrkeqwk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gxmcnzoji.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gjscljget.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gixtulwiv.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gwyvptnhq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gyxeovpfc.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gepeuxsnr.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/ghdlxvwpz.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gqlcjurfw.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gyigvflfi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqeqsdl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gzztajefe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gwxbhrvrk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gkjrmbfnc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/ggjihbolg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gyvqgtgoz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gfqcsxvem.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gbdssfuqq.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gfiefyxrz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gftzkqcyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gdtglvdfp.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gyivsvolu.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/govhmgftw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gypetydyo.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gxhctelhe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gxqlxzkwu.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxtxyhnht.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gyjltaruk.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gghrzvvom.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gyqszoiwh.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gqsajebyx.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gdfxnggua.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gjtnnbasu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gppowvhog.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gojnmxxkw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gvwuciogg.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gtumlbrbc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gngnygugg.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gmvwlfavo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gktbrqcbu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gonchkmra.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gugzieptg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gwstsweka.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gilngbktx.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gcbfgxccl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gugodjmlu.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/glpwvqhhe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gciavtcxo.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gbadmoysx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/grwypsilb.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gzvxkutmh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gexfoyfmj.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gsneilirp.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gwfjntsiq.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gkgvaifxf.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gouearqbq.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/grwydpqph.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gsffvpvrb.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gmlzuoctv.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gcaypgxkd.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gbvduppgt.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gtmwdilwo.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/glssiyuvn.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gjdycdsxd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvrmxsyr.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gpiseywsx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/glllkwmna.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gbtuqenhm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/grrqwcrwo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/ggcfnmgnc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghonahlqg.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gokqxuutp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gqpzsuzul.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/giemqxjtm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmrfjjevi.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/ggsiusdeb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gayiikvxy.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gxqdfrgxs.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gepynuoqc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gsvllmray.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gjdmxnwdj.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gsnrvfvei.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/geuhrmikm.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gblszlsea.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gbqbemawx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gmjhtiaxu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gtjihnnab.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gasbyxyvh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gvvcuouno.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gshvooggk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gfmhkgcta.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gkdjohhaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gpbbwmmex.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gheqytwmv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/grduofyvq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gqqzqhfqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gmjomqmrg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/glvaewtbv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/ggczdoshl.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gicgejvwr.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/grlgtoeyz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gyqelqgzp.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gjifmceyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gjgrxcwbg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gfrlrjwfe.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gxseyjjvy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gigfalhds.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gqgfmfotb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gvsggbaaz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gwxwvcjuc.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gpwhsbnez.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gtiocljtd.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gzvdiifwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gkiilqyfm.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gabxjzqit.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gqeeshhxo.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gibkgmckn.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/glzmcbbmf.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqossclgm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/guwgklqjx.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gcavxlvhk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gigyncilj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdgoxmrke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbyxcqfrk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geqigsasw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gnonwfpqf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxamzgfdf.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/greenfgrb.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gmntsreqt.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gsjqnrlhi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/glychewga.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gopwydobz.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gdfuvldku.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gxykrqarp.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gqhlvvxph.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gfizymqoi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gxkmllqun.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/glxxxdvlj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gigyhdcri.sHtML


<!-- 参考信息 -->