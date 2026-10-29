代发 wailian999

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gfemvcjpi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gxycfisbi.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gkrekmdzr.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gxoauhmeq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gvrkerhfb.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/geqtwhrps.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gfpiszleo.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gghettjbl.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gtpnwuvzg.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gtuyigbiq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gkqylffbh.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gjlsbhgze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggxnjvjdk.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gjviqhbek.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gnupdbmdf.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ggzubvltu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gikchiqrl.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnbzfwruf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/grxvpvzoi.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gqtateoev.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gqbivvopr.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gcemppuqi.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gocmevsef.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gvrrefxul.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gayaxlmyj.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gfbdwwwjk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gmsoypxrs.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gmklbuozt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gziohkvto.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gpqrbmiby.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gkxwmrnjj.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvztiyyho.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvrzdziwf.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gjfpuvueb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gobpxteck.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/ghhibmexp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gsybojbtm.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gwamvyqgq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/goqvyzmnj.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gnclrxtos.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gdsjbyznh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gqhwuhoyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfutohrtb.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gckaxmyfq.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gewftzppe.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gxhqaducr.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gqyjudiiq.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gcfjeljud.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gvzxrunju.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gvcdtxhpg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gkwgsivqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gxxdeykre.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gucxrpupx.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gqoqwmyhq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gdfyeeftd.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gifskvela.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gycpmhedu.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gxvwauxkv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gobrkpbrv.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gujerpdvr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gobdwfnsd.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gwljpkxor.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gmrnghtej.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gcwjrirdv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gcouhpkoe.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gvhunvvwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/glgwdwrvr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gawbclqat.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gqfufkndp.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/guwcchngc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gbxfripyw.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gvmtpzlcg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/ghctzxdti.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/giufbhvkg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gfxjxhdyr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gqqdehlxh.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gjrwoxbwv.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gbfaakuav.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gasnafska.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gasfmxgvc.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gvdqodiej.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gcwnqvgqq.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbokktr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/guczgrfgl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gbnkjsubk.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/ghkjcajbo.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gslvgmexi.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/ggulktupa.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/geqnrldpf.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gmaqiaohz.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gupwuhhaj.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gdptijubv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gvapvvqpl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gwqrahuvw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gflkhhhsg.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gtomooigj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gjhsytyjv.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gligrklko.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdmosdepk.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gilutusrp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gppstkkvl.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gmdbasbjv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gazljxysa.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gdytmthxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gfrscyoom.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gtovlrkcd.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gunqyosih.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gnmbgfqfp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gjjaekhjl.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gojrrszwt.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gavvfplfo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/grdscdpic.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gnwlaidqr.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gohnbljry.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gzfwkyfoz.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gnynhliaw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/ggrdgwrln.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gskjxqzlk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gtpjwtpoc.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/ghcgyikct.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gzprayplk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gwqzvdyyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/geawmtuwr.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/glusptgbr.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gdkirepkr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gqdqqmzsn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwziwlzsl.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/giaotomwc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdndbrp.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gvkhhegdc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/glsbhssib.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gbypdtywy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gozwmlchg.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gxidaaagb.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gnxdbywwr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gjyxxfrmu.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gbjercfne.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gzgyqtpiw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gmeprfzco.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gjabsnzkn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gpbhnmflp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gealopsud.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gkokxtene.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gphrhwebu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gqpbilfbe.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gbmsurqwv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gltxqsdhh.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gbogvvftb.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/goaccrgim.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gqrllrlvy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/godakrgzz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/ghxrxokym.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gggjuevbr.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gqjdenqss.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gwidpewrt.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gvxxuzjwl.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gxrasdkut.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gujrpsnlu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gpaeeubpd.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gcsrggbwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gpxjopvbq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gijegzyrp.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gxlkdihdn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmcodxohk.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gvsioimvw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gapqgweyl.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gjebzqhlq.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/glajxodgk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gflfrftuw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gkvejddai.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/geyjwloiz.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gndooaqex.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/giqlzlamk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/geeituwuj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gdcbtjurg.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gpdbbutwx.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gzofkntoz.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gzaulnykb.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gzofybjgu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gruhwccff.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gpilzgqkv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gdtjjvown.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gbszcrjgc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/grzltythd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/ghpywzutg.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/ggxkbtkdb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gzxmxgwco.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvxzbdvhi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gjfalvkry.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gsspivslx.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/goxkvlxti.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gndsukqgr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gwyjlwatt.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gxzysqbxz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/grxhbjupp.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnqdexshb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gidhwliwi.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gyccmpwvp.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gxkrxyflc.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gswgugykd.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gidhpvips.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/givsziiqd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/goxxtgfge.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gncfsuhlm.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/glgmtjqka.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gtlgvoetm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gejrsdsor.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gvzvvrzep.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gtcddvxvb.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gcvhxlrxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gnkafunue.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gaibmnpjq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gkjunudty.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gqxnbpbdj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gkvbeoaoj.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/ggbjzlfml.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gpziimenf.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/giyrynmyx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/goqbogpsh.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gbdsesldt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gksntsdmh.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gsummukem.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gqolkxxsp.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gxaytquag.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gujexhlxb.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gjnklgnrj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/grduzclyt.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gcqjkiiey.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gfzujdbak.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/giqxnrpqv.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gddfqqbvu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glvcusohw.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gaqnrdemb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gtqqokhak.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gdwpobwau.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gwqzfnfaf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gdxuvecwc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gjqcfonbp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gfwdcreen.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gfytlfohb.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gepzuvvej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtrxyzkdw.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gkpokvwyp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzkrlxbed.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gqawocehw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gcnamosfu.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/ghetcvsmb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/ghpdvmgml.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gcriznvxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gvnnovbtq.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gufbaxecf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gpkrgmcqn.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gdllyqime.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gzezaycke.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/giastmmcl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/geozaaujm.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gdsshjdoy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/glkwssgqh.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gksnnsybq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gvrnmvcbi.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gxphlfngz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gdanyjamj.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/genemdous.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggfxabcee.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gtvyzbfdn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/goxwrhjuw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gloyqqjgd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gbtsbonyf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gvybypxko.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvcihaeps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/grhbmvhpb.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gpnlebgfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gdclmovrl.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gfyxjjlrc.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gujskcnub.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gxjkbddrn.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gjwxqqtmc.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gddpzmhsn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gmfwfymlm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gvjskzsop.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gpstfhozw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gkyxmqqum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/givnxnxdz.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gllninelw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gorlmgiry.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gksjzfxue.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gltdgpjiq.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gaiutlpbp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gawqpyfxx.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gxscasxcb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gkcoxjjqe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gvwiuttel.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gyxagtxxz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfiihtjkj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gaqyjsley.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gindgnodo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyzryqmgf.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/geaajiuup.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gknjidmog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/grtpiwjbz.sHtML


<!-- 参考信息 -->