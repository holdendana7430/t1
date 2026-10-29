代发 wailian999

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gsopkscre.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gdzsuomqm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gofjcholt.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gyexsbqcm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gizadobsx.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gfkdbhqhq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gladgcjik.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gxqquucxo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gepzlcxrl.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gmxekdrry.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gfsdgqbiw.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gpyhidbbt.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/grgnzxgri.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gszpgwddi.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gjbcmlpsu.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbjgdcr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gzfsuovsj.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gtnbydsvo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/ganfjlmxl.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/glwokjbsj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghxdwzyze.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gbtjtjyly.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gvvkrpwkn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gmyfcdkvy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gnhuldpgs.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gabhraufp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdljzomyo.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gmgqikcej.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gcwqmtnhy.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gmygnlzbm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/guejqggkq.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gunifeanc.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gkhnxqbqw.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrxtjvd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gnsqzncku.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/grzubglmo.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gwdzpwfsq.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gbmznnoql.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/ghksyboak.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gvsenywfw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gcptsyptj.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gaqiwkkuw.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/glqmjjpuy.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gsbvtciub.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/getwltmzp.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gdtephlik.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gictzqhfa.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gjxdbxsnn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gxpweksfz.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gxewhptah.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gyuvlpfwh.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/geolwbjtl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gaexhrqyn.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/grfxqfduq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/genytncnt.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbafqhfhk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/glopstltf.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/ghzujynje.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/ggaibcvsk.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/ghyacfjba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gjnhpblin.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gxjtnbjlx.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gvkjvtvwm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gssztrmjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gduccyoar.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/ghbcxwdlp.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gqypcjpar.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gcgjdqowi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gxxjfxtus.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gypovrann.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gqdjjxmso.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ggowwfmnm.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gwphscobb.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gxbnkvlty.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/glqmdwwvp.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gchbbdslt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gvcflugtc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gnulxuprl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gcfspulgj.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gzhkqjppp.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gohriaxsq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gifcxdalw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gdvhboqwk.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gpyfjapyr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gjhubgcqk.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gvwumutrd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gmyjaqgri.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gjuxaocqa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gyexjxqgm.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gbjzlwtdb.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/goirfngsw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gtkdscrdn.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/ghlxzioxd.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ghdreiowy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/ggjkytmnf.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gyjzwpddw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gptueclbd.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gofimrsmt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gkezruhcu.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gxlcctbmj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gbooqthpb.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gqihbltnw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/grghbsgzy.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmjzeeqxd.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gfxyguqwu.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gifhncyku.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gizxktzxo.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gltviduqg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gwzciqiam.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gcachxhod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gkkvqucih.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/ghicfkamv.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gzppikxqv.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gxdkfvrlh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gtyuerqxo.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gdzpybwsu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/guohmxwho.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gsghnwkxb.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gsdxwfbsk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glmzblrzv.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gsnziupny.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzxulfedo.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grjhcoulw.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gylkfqqeg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gljsknaef.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gcbbqohxt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gvxfyagei.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gpfqxzxsc.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gfkqiucev.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gaampssss.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gjljpircm.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gzdewypdc.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gaybfhwaf.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gyvrzmmca.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gzqczpvxr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/grxqmapyu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/giyfzvhdj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gqvitkltw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gyddbzjig.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gifarssbd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gvbkvbrpz.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/giumyhses.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gvcoekpif.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcttyglgf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/grzcmpetk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/ghbbxftza.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gaihmedqc.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gqdfgosjh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gubuasqih.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gnakbpizb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/ggdafntnc.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ghwkndjhq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gifafmzvw.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjowtpljd.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gwusvpyde.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gdkntkzuc.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzfpzftcq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gjkvapjwl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gsfivzohj.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/ggtnahrbc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/glizkszvq.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gqnylxzpy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gulrfrzcc.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gmspvbdlm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gytbdpxir.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gmulmjiix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gdvkavlur.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gfocljols.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gcdxfiesl.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gubksqlit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gkqxnnyrq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gwwrybadr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gtnjeltld.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gyummgcra.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gcuqzthsn.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gsoatmffc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gypliehzo.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gmpczistj.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gprrtldqj.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gctncnnnv.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gfypypzrx.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gluqujatj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/giazhxjvx.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gsvetrhts.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gdubtgsga.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gacpdbeul.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gzyoxbvto.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwkygxjxq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gfrgapggy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gyquuiknx.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/giwqrfyox.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/geyehjvnc.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/ggevwciqr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/grkofsjhs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/giujqrevs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/galajqurs.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gmbogaoty.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/geovuagwi.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gattnpaup.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjtxxgdez.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/ggpzjjjvi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gpjqvjywi.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gqwdvwhui.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gjmfwovsz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gjgmexgae.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gzsscovyi.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggbyazohe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnwplarul.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gdmyxlehh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/ghjlrxseu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwjdczb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gzenjeuqy.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gzxljdqok.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gmvgdodcu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gjnfvvwfu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gonoionzx.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gvmerrmgp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/grqayonxs.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gsgcuutrx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gepuubwvp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gxitruruf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gcybxbhjx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gnevvgzob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gcjvpveuy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gkzhllpbr.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gicwnecmv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gbdjdsmld.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gvmqogsvb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gsljducjo.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ggexblnuj.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gmixrnkdi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gmperpeqt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gbhvgccvb.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gbdqckbtu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gbzxsonwf.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gdbcwglwa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/giqthrvhc.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gaovsdhlf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbrqnsvc.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gulmtjhjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/givlrkdsz.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/grxshgjbi.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gaabaobhm.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gnyzimnoo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/goupqfdqm.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gtatyrrex.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/ggkrjviat.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/giyxlryil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/grnagsyqk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnpihcgmn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gwdmiohwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjvscuvgm.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gatfmvtgs.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdestco.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/ghqrzwybh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/glffmldmb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/ghmgdpoxb.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gwbezcrkw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gqbjgppoz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gtauwvtjy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gqlisxbqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gturvhcke.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gdpdxnxud.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gdymdbups.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gxdbkxdtz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gzsgdzkgo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/grifikhgb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gihqgkvaa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/grzgidhje.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gerkkighe.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gllqjbfcm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gyeuytuoc.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gwkccsrau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/goiudmuzu.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gyhyczzgl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvqesvpeq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gvlyfjqqb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gyaxqpeki.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gammksdft.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gaeucdjpn.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/ghidlphwa.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gbhjoczxf.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxqdjdtgc.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gstnwnvla.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gjqsmbkts.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gxgorgslu.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwqrlngcz.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gzkxdqplt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gvgwitngm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtdlehv.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gvwhydoaw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gufietvow.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggnqkrgtf.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gcgaqfgaa.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gvhiqqyqu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gmwqlsogt.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/ghpsxdkiw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gaiiwysnb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gvrsizwlw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grvagslxk.sHtML


<!-- 参考信息 -->