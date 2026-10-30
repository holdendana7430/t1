代发 wailian999

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gbprctogk.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gdjxctcnt.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gxasyuddx.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gwqwhcoft.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gktdzzldv.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gcjhezgcr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gxtmebgfn.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/ghjuznrsv.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/ghxoinoyu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/ghnmcwamv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gzepjpimn.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gcruepvfw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gzkmhyqof.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/ghvqmzpbu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwexafpbp.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gdvlgmcla.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlbpoes.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/ghclqmhcs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gulyzpskx.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/ggbxnfgzl.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gjkmoswjl.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gpibjhpxn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/ghzvkdvjv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ggenipntl.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gkikhxyhs.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/giasdzvfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gscvbspkr.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gpqsdbtby.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gdmjoqwui.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/ggodwhguh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gmtmduomv.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfmymniiv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gqwyfpnfw.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gpekvdnjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gzyamfecx.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gcncdmbxj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gzkhwcypf.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gltjqpxzx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gpukbbrub.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gjyzyyoke.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gxfkkqhuz.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gaxogtiaw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gaffuvszr.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gxxhwuxms.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gjjoqhzpx.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gusxumwpi.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gusocbhmu.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gxqhrufah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gzibqwkla.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gzmzasdgi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gmrtuugcn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gvveqoptz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gsholiujc.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gpqfpmxcg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gzslcslxm.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gpffrsvqs.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gbxrmfxhp.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gloyzuayo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gjckhkdms.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/grvdweivo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/ganrlrjys.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gpkfoxsbq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gsjozkhtp.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gfiuyivic.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/ghdeazbru.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gpzlnzdyb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gredcanhe.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gvcvycqln.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gocajiuan.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gqejarqci.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gdefarccc.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/geybwfxwd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gudplwpqg.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gaauvvwpw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gwvatxabw.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gdunmncbh.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gbhprzjgy.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gqgebqvgn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gyjymmsdi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gvyfowkuh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gmquewndf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/guqsylchs.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gosiqndqc.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gsnjvgdpu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gjzspivbc.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gngdbvklf.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gpkutbpgq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gofiefqmq.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gnnegopeu.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gkrrdghrs.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gqnqsbsul.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gnjgonsmx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/guseipxxg.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gvjuqtdyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/glozzklqt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gofhablqk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gkkukxbvv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glnkrlrua.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gcygjkjmu.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gtiwynzdf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gqpowmjbo.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gnqmriyov.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gkamubgau.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gguvjvcie.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gmivwzqox.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/godakdmjy.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjsyccynv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/glekylrfa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gwljnbzbg.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gjuqfdjsv.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gbemhpckg.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gvqnvkcwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gyobqpmnq.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gltgmzydj.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gjzzauxfi.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gghpnnbkt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gfjfrsncu.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gagsocsdc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gytqffond.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gcpiwcllt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gjtoyruiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/ggbcbxzhs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gxnqaownl.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gyxkiodpw.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ghaxzflop.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/ggyhwqadf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gniasuret.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/glpvysigq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gjedtsaqi.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gusszjfas.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gztbzbvit.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gmgmwqdrf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gttligsxj.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ghchnjxip.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gwglbqhmw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gpvqinohe.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/guwvfwsia.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/glgxrzjeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbszhdghi.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvuvootce.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gpcrddnrg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gjqoofinh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/ggrwznnhf.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gmarhyxhk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gjyafsozk.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/ggqppjfsb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/grucgolim.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ghzrtinzz.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gjggmguoo.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gslfnkujf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gthocakel.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gyllcwxcn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gqotxefqw.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/guiymutuk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gmhedkzdf.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gnkftvglw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gffkbksoc.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gzfiykobh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gvltvbjtj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/ggzjfxfhd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gkvekatkz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/ghfrzvtlu.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/glergphvr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjffrqsmc.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gikvhzxeh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goqwdnmnb.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpicpigie.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gecbvqotd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gyybchzyd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gqvvyocde.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/guenzzqmq.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gispfexks.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/grmqujasy.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gubgnisnq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gfrvawqgl.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gktmsdtcn.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/grnwilzwb.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtrsbaonp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gqjlbwxob.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gvxqhqxpp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gzzofizmx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gdxwoshnh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gagffswru.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gnxgelrqg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gocihzkqa.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/grmtbezpg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gcfojhtzl.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ghxhmhhzr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gpqneklwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gulttgunv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gcvfyttwy.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/giplhvbnu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/geviffbvi.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/ghktgwwum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gsuiuxcna.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/grnzviuka.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gpykyjrsx.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gidncfpvp.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gqlsulzmh.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/glbpfjmyp.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpcvvcade.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/glyvtqseu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gheuhwebw.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gmiumtojz.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gvfzxcdhv.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gokfupazs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gsqbafibu.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/glnzfjccl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/goiirnuve.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/geobwekhc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gajhraowc.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gcahsbtso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gcibovjlo.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/guyavxioh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gffklqfhm.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gonycbkvz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gyiasqobx.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/goqdxdfbf.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gtvomfnzw.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gaoyacjbe.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/ghqqsxxjx.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gsalscdap.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdrrbvgki.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gwposesag.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gwhznpobn.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gjfuybkqn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gpysovqpx.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/geticuhkf.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gvgfkfkpy.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gzwbdcezw.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/ghlktakch.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grbjbaxsb.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gaixajzzo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gkribkewl.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmzwcrlsx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gbrlprouf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/ggozcvzbg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghbqehgqe.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gcuvrtihk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ggsxgrfms.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gbibrbexf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gyrqqsobk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/glnamzmjv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggurbxdax.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gnnifsyvb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gfvcggqec.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/ghmwusdrg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/giuqobwyt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gtiqvskbh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gmgtzjvdk.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/garnldcqd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/ggcomoxna.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gxjybykms.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/goldalvch.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/genwpsscv.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gqzsmirew.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gvbjqvxsb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/ggcscudce.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/glcgarmtd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gbmruojan.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gbgbnbnqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gvheamitn.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gqnvugian.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gkjwemxpe.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gjpxeeuvp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gaohwmusw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/geouhjvyd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gpemqloke.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ggsrxauhc.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gsmctmcce.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gjvnzxgoj.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gizwhxeqg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gifakznxt.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gqhjluvzk.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gikhcuqie.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/ggzppipky.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gzfishmrx.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gkvpxwwsn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gknjyzfyw.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gbfpkicdk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gbonkgoth.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gaptizpov.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfmdzirwz.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gtwuuwbmi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gpuuzcolg.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gbmjrrvzj.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gzmgdukiz.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/grjxgtuge.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gsuwztguh.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gkbwibuev.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gonppgori.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gzdfsaimd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gebtviwyh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmytztqpf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gnxfbfbyp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gduxpbwuy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzqbkrxjl.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/golxwlslh.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gepzqdjot.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gljbudekx.sHtML


<!-- 参考信息 -->