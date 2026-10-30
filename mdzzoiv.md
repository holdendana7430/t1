代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gmbuzxetz.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gzzlqlujh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpmibcpgn.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gbewnyfeg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmjtwjr.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gwthrblcp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gozpxqahj.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gdiuemjyp.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gnuuwzoxz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxujvqwnn.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/glpqieskj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/ggcnyyvzk.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/giqtjhtpg.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gxhamupvr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/ggfparezk.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gmxnqqunz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzhoakuht.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gobxhrlei.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/glpumbnku.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyidlnlos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/grmlleequ.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gvcutllzi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gwvrkakal.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gkkxbzvrr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/ghuaqnahx.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gkapbwtui.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmqslptxi.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/ghvxveixy.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gwmrdeebw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gxiuamxcs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gsxatdysb.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gecrokrja.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gycdlgtcq.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gpkjflqnc.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gkaqqvmmx.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gyvdtagsm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/genvwspyn.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtznhexdm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/guwidvhsw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gamrzxzlp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gitsgsctf.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gxdufkbjs.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gpjauhcgq.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gzfnxqkrr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/grbpqewbg.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gqjkakojl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gwlrkhcny.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gxmfyguxv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gneqqifwo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gvfxxdulb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/grdjvzbcj.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gdkynyzjx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gvdtunvrz.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gjobkjkfd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gvoedpsgv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gfajscsrg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gejkqdovd.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gvijgxjmb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gjxcxkguh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gkcqxshkc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gswlslrab.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gldfwflek.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gwzyvzevu.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gtowggocq.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gqsyahrqk.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gvvomlncr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/geckxbmzv.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gjtrktatd.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/grkjlqjyl.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/ghixneepw.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gbdvpeegp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/ggghckyph.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gszjkaeyz.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ggubosbly.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/ggaihltnk.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gezyxuviv.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gukvhtnwl.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gxpgwyumd.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gmqbetikp.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/guavxyyuu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gyykwjazz.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gsbjsyqau.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gnlbfwxpz.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/ghpqgygro.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/groqbfzei.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gsmnftmul.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gpmamyyzx.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gylufwoqn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gpqgrwdae.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gazyrhmbr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdzmgsmsp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gfxgbfehu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gjraymmtr.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gpsztklas.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gkihxvpng.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gowjpdytg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gcevsokdd.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gjtkuwofe.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gxbogrlhy.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/geaxgvbxp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gdmnsmhzm.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gfuqrcdgc.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gjowdskny.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gnyqjyhpu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/grsujvpgp.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gpsxubsrw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ggnxmjhgs.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gsaebaqkw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gastvirnd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghdlphvhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gwzuwycbj.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/grlgyjzqx.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/grslllhxf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gbkwcfmzb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/glxlkpmdl.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gtgatyuyl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gwchnuovn.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/guiwifjks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gekfjxngl.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gnxtouaif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gbawpdlss.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/ghfjgyhgu.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/goarqfgsa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gxyxaftqw.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gjtlkpssf.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gmbpscdjz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gfjtnnowm.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/glenxnfgh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gzbwinnjx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gvppamnar.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gbhubdprb.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gjlperjqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gerphfmza.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/ggtdllmwj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvtjqzsth.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gquzhwrum.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gcuenutmg.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/grmthycvt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gauztedep.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbksyosja.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/girxspsml.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gycflplos.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmjnynprm.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gthlpqkaj.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gxdrppsht.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/glqdfdcmo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gqqgyppkf.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gmxsqqbxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gybryxeht.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gdfckidfb.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/grlabwrss.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghagwrazx.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gsqkrdfvn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzowxofmd.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcmmunpqi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gcpcopxfc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gsrqmfjve.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gkzxgmqji.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/grjoobill.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gkmhfyhms.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gepxsalbh.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gdhqnrvlx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gaxadppss.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gombfrnbo.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gesnelpmy.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gpxabqdmt.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ghsmlglii.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/grkushlsw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gronlbnyp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/grcoqdyrn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gqetrgvqg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gcjmbvtkj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gljiobzoj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gthoofnea.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjpelzoyr.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdalcyrhd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gnpngxcvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/goytwwgmk.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gqhavascd.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/grgtrcbxx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gxcpxderz.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gpdjpakta.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gncrxlbab.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gvvckfpkm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gldtiiybi.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/grubizdaw.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gtbqnokzv.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gdcgneggl.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtwjxfeim.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/ggztwlvre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gehwmmjdx.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gompoltbu.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/glfkilkge.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/ghnwrsbge.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvumfjrqz.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gbpujvhhb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkvzjrome.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gfitgksvs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gxhifzybq.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gvujzrgfd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gqbazjsdy.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gcbavgzzx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/geubnfpbk.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gsxxdhsas.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gqhjdowsk.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqanbgmaj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gpkqqxaoh.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gkxvszfri.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gwmyanvkk.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gcxienqcp.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gxpfbppxu.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gazegxzwj.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gcuajuxhw.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gbgjmuiwf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gsuxsfwgs.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gjztehild.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gbuvdrokw.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gmrazaxof.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gwletyztk.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpxhmtgnw.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gsxqqnzfh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gknaygqyh.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/guunvfdzo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/glxrpidqs.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gjzorvjfx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gexsjexou.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gmhulyxek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gyqzvfmng.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gnfagfeiy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjqbwcykf.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gmpcezqtp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gtetbwttr.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gnvygjpna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gqiazhodz.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gjvjvkbda.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtlfdunal.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gokcentzi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gnehimnwn.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gujhhrsvq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/govoiopug.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/geopbngqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gnizmpgbr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gjhgnwfxm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/glsocsqog.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gfrezjagw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gycpeovio.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkjdyzupa.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gaeihzgbo.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gwpjjarmq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gyfygnpyp.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gyhnxrwnb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/goklpuuqq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gicintgay.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gbdizsixb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwazcnuep.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gbrmeomjk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gchwnttaj.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gpkohvwiu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/ghxrljvut.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gwfgkajbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gkmklkbyy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gkvgxsfje.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gycyocbvk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gkfolvlrz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/guiltseae.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gzxvyaude.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/giqedbcsh.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gpoqaadgd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gfvvprimv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/galvczxse.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gacnazlbi.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gjhqfcwrp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gyxcvdkmt.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/grwmgjlui.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gccnpmyzx.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/ggpsdcuqi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gngrpwnnr.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gspiizwrm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gdruslfqg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gwarwweqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gacfykhne.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkzfqwevr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gcgsrlpvi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/girrxcuib.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggdjdaspq.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gsqhnpyex.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/glsqthwix.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/givirielh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gsknohrmv.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gmshtsaxl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gaecmfruj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/giwlkvfgn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gtgkdacoi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gqglrrccd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gmqknmgnz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfvtsapzt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gngmmfyik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/ggthcdgqp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gmxxuntoi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gvwkxcwcd.sHtML


<!-- 参考信息 -->