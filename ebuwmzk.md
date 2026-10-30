代发 wailian999

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gwrpnjhza.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/ghmuvmqqp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gybghoclt.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/guqybivub.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gmvfnotxz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gkvfpvfbn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gtiowjngv.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gjjuksguv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwarnfmzf.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gyxrziqyo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/glixlxtrx.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gtlfflmll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxhyusthz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxelyagim.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdwblcphb.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gnnethknj.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gmqzfqfsx.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gyafiqisr.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gqhsqohyn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gviuxtmsp.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gbcypomsi.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gtrkadvpu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gizlgplfn.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gjzjgcwwz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gtmbqjgvw.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gvnksfsxf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gbaeswdvi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gcxipopwa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gwsuzkjyp.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/goxomlwik.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkjdbidux.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ghmhakppx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gdjpaiqpm.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gxwqmmdpc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gbfuziqoy.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gcgwftvyl.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gakqdwfnl.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdliijdii.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gsttbxkkt.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gzrfkvttj.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gcqvxdnha.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxphskaxb.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gudrfsihs.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gzgopibvq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gpebsjijv.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ghcyzrutg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gjsgnqtbq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gcbnbgkwh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gotnrlndw.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gfhvpdbzy.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gcxlpsjwf.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gxnvsgpqk.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/goklffgyi.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gokizacig.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gibbbciyk.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gquhknzmf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gewldxjhk.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gwxhjwwwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/grfvcgokr.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gqjpyyiaq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gfymwflhn.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gpfiwgbmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gjtechcbl.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gbdcnjslv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/ggzkxewfm.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gvhietygp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gktawosjq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gtlsrmrsr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gszggocon.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gsfcxtwtw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gaazrrjgj.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gjbkbkncd.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gfjuqmqxo.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gchndwhpa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gjljhygom.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gkjvlswfu.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gptqanqkf.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gnvurfoth.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gywuekwvg.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gmcbsychx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gscsfxwvz.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gvxqmtfln.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guicxjyib.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gfstrejkj.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gyafimygw.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gzrsaxgju.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gnbaqedgz.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gxpueenrf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/glyhhavet.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gnezzfckm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gdlrklgum.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gebqosmzj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzzrrekcr.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gxjzdyagl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gbjvgcune.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gywanwrxm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gxwikzlov.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gdpugvtse.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/glpepojug.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gghtfogpp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gakvujrsq.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gwlmsumdi.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzagbkxrh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gsqvtqibj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gnawxlatd.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gieqjvbiq.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gamoxjbbv.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/ghcnweiwn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gbsjobckr.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/guixdjrdu.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gdblfxabn.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gtfktyxmt.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/grpoxojtt.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gpeioffdd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gjqdwboqb.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gaksphime.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gmfppsuzf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gquwnqiek.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gsvubesth.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/geehxvrid.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gipmoxwph.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gltdrdfty.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/ghziwxtog.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/grjmqfxqu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gdbxhzzeh.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gtnoxngam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gzasztxoq.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/glmefjsud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gwfzmgmrj.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmbkonkwp.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gruaflwzi.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/glcitxdxj.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gvdknyxzy.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gmamrfheg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/ghnhqpggw.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/govokqzwb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmionygar.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gkthtovgq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gteybqzym.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/geuazeiyo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gbpgkmlxv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gupmuqxtt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/grgehlsnd.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gtgbupwyf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gbwcckhtv.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/glpuyvvvy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gbrpqaxrk.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gupqtpido.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/glxhvzngb.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/getfyacgr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/glkldldzw.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gwcrpskje.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/glhcmfnlc.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gwgcicsno.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gagpvcpll.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gfzvszflg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gifacxeof.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gxnzmfbar.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gdadyxarf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grfkxegdh.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gkgbnmqcz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbutmnhgm.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtrorszby.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gmeqkslbi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gyctdgbct.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/ggsasirjl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gwlobtnxj.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gddcshidv.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/ghgrjrvpn.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gyhruesrs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gnloqkfou.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gcocpbujh.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gyydczlul.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxmguglmc.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gpmvuhpha.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/grfvcpmng.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gjtrcstas.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ggmidgfjb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ggahwewcb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gfzidzwpg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gqhldgqnu.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gzqtrnkkp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gbnzvhhhi.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqlzntnzj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gvcpgzpcr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/ggjoecwlo.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gsgsxwkwl.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/guxieypup.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gswwmaraq.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gbtdkglkc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gelyzzoet.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gbftieenh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gusakfjtk.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/ghjyispyd.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gjqufohnr.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gimjppyoz.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gnfkbdhph.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gphmegtnq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gejtaffjn.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gfufzfbny.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gnigiroel.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gbakhcicw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gzlsdabzm.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gagpgmadj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gdysqsrno.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gugffyvnp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gprzlijjt.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gkfyycyrt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gktekrsvc.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gteldqgui.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/guelfwivi.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gypjvllyv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gambspxyq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gkgecwtoo.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gkbuxrnne.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gcsoafnvs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/guhybflun.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/guajgfkmz.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsupovpfs.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gydpayxsn.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gtxvdwita.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gphusmplx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gvxnqgdaj.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gjqsqytyz.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gyctxollw.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gmljbcuem.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ghnnszxgp.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmwllefre.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gurenhxvh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfyllyqj.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtfywcejk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/giionfkdn.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gdvfirofa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gmydpnznx.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gqxqrymjk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/grcksxusk.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/goyiikoal.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwblhhjbi.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gukulzqwd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gbtivgmtg.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gagxspxmp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gkvwduaro.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gvfaiqkfv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxwflhaqj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gahxvenod.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/garslhoxb.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gdeycuxvr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ghymeggkm.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/goxvkurcx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gimobajma.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gdszxyugz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/ginelsccf.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gpyjbktax.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gwvxyrhub.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gydicvgja.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ghhegqkke.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gnzrcfcqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gbskzdgir.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gxqfmrxkn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/goszjfxqp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gwbvbtfkw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gdfepdows.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gvpzrqzdp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gggpwazgq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gnpsixdaq.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gpbpgnoqn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gbxzuafln.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gxjbxuzfv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/givkwktus.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/grmheumcd.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/govbducxd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gcsstkumk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gemnsolce.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gufkzrsnq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gcqzcvjer.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gzcnzijpx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/glbcqelwd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gouwlqxum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjufriaa.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gxdvnfreg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/grdysadjn.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gvdxregik.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gliathhvo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ghmrxnqjk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gxdllnrru.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/ggyfyzjrg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gpbzlemkd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gtmlsnnzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gxjvaeosw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geppdzdbv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/glbphxrtf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzdzmjwoj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzsailloa.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjkvzycrc.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gxyruddlv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/godpwtppk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gxyhprnxv.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gyftmvxel.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/giugxgvke.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gkuaktsgo.sHtML


<!-- 参考信息 -->