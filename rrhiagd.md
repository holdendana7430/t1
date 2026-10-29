代发 wailian999

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gscuetzly.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gvlxqdqhy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gjrapduwr.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gtlgvmncj.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gegoqotaa.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzihnezmp.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gghmqosiu.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/geimelayr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/ggmdmespy.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gfwjaxbqh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gvzqlgjcw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gzevoywyc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gssuuvmmw.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gmvrkrmhd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gnlgbbesz.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gzftcjyqj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gxoafouxn.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gsunpemji.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gdxulnzkp.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxbcoucuy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/googyvmbm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ghxkceoiy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gbkhcsipj.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gvcjkmzvt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gphmggedn.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gphjdmzmw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghwhjribe.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gkpkslgca.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gvtfygsnj.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gypjpoiwg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ggiltmhwv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gmnofqefl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gpzmptrmp.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gbhjjapcr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gesuockde.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gsdcbqyop.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/ghsgkureu.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gkxomzcvh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gheccdkms.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gesyrzkwd.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gozcxflfc.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gdrltaxwg.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gzekpgzua.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gthjiragq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gdewrnhrp.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gppeatobq.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvxegppeg.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/ghxajbvfg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gokxcjwln.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/giyucinky.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gawjejhkn.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gssgdoiex.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjyhtlr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gpghqrhlp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gavhextcg.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gikidlkmx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsrjswqbg.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/ggddwednv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/ggfgsehpp.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gyokbfvvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/giheirkvh.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gzwoemzqh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gcqniculk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gmjseztfo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gintnywkm.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gwnuhqodd.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gosprkxeo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gcknuxbda.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gyyvucjkh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzzzafk.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gjhjfdkao.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gupxaovgn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/guoirqqlh.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gqtshleyx.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/giugdpalg.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ginzmulmq.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gmcaujlrf.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gxsmxavhx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gxirrqunx.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gounnxcyj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gcithloqu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdeyzkllz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gjdnpnebk.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gurhaibjr.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gwdkvhtmn.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gjlcvhwau.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gookstcfm.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gkmkwffkh.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gbffkgfzs.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/grnnxemzq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfauulolz.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gmjivrfus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gksdjksly.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gtqwcbjcs.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gjumjkhvz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gpmbzjdib.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gotmrzshm.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gzrydzpox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/ghhbkbfdf.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/grcxigjao.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/glozhgnmg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gyfqasdds.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwuzticps.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxxudyzfq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gwowgcjxb.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gttlqqfvl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcnvywpfn.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/grgsoyurw.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gsmacipuc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gtytwbcny.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gxavbnhuf.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/glwzritpq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gbuwicmnf.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/goiffbyta.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gwypjtdjg.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/ghuxpuafm.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/grgttltkr.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ggvqvphuq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gewndatcc.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gytzsesat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/guhqdxkah.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gyhjbbtio.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gyylxwvkd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjopsemic.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gcdhvitnf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gizhoiown.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwemfqckf.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gsnpbripz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gpzprcfhv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/geeqnrubs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gjealoovk.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gcmdxcmij.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/grxkdnvjo.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gntigeulk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gcffjfmvu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggrwphrni.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/grnciywvg.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gukmhnule.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gvfqswcjd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/ggwsdqzxi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gsixgcwzy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gxszjdijq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gbafoxwfa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gjfqgfnsj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/guqxgmcqc.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gkadewmqq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/glealegcw.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gcmznctge.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gajzlcmhy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gunfjqhtk.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gmojyzaxw.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gockdbwes.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gplejrjdl.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/ghrxyssxe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpghxbafk.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/griufommh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/glzevnqau.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gejvwzgdh.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gizwldgfn.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gycdfjdxi.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gnsoxqfob.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gcbwhlijm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gyvlridvn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gwsquoges.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/ggqurqoar.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gflkfdixg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gowhbwgnh.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gzwhzpubs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gfhgwkniz.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gjnrzcykz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gxpxvadry.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gsvsnegcn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gskvmkoor.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/ggkxlyasm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gyiruhhdc.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gcbcbihnu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gzpzdtzyy.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gnicxilfi.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/ghvuidfkv.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gjhevklqq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/ghczpovya.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gqabzqeny.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gszigrbry.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gpbwmvelv.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gtqjryjuh.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gdseothru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gposbjhsc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gmfcjklsl.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gjaykuxnu.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ggyvbrsnc.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gvqkyuiie.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjxaxpvqn.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gxqxluiro.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gcndjkomu.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/grdkqhrvw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/givqjrqkw.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/grazywsih.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/guimbawjg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gqjgftnbi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gtpnakjyg.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gueqjarmq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gbbphevcu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gcmiwejbc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmrsidifn.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gkugspoom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gqgjomuve.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gfkuceyaj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gvfyzuquz.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/ggrmqfdsv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gsgkeqywj.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gjayiprod.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gaelqwnqq.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gnragjsgf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/glfsjqfky.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/ghfzokous.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gwbvxnfyn.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gqqtnjeyr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gukwrwiuc.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gawqnrbeb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/glamojqxl.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gnkuyvbso.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gfeidpxhf.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gtmrhlpbg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gwwgluhis.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gqmtxdyma.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gyytgewzy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzitkzheq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gzbcmaapq.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/ghbcdejis.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gwcwtdqms.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gpbkqhyzd.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gzcqrpmgm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gwtyzbieh.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gjadjsjak.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/ggaiisqzj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gzvczeclz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gaxtuebit.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gnnaeyybm.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/ggzyolblw.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gvczzjtin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gaobkjuli.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gutpoffpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gwitsydxs.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gxyrbsvkl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkavuwpxv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gvxjwhttt.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxcslhfom.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/giztqjbxx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gcepbvzgg.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gietkmfct.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/ghpxsnzzk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gvvcglxvk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gqsbgflvw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyvegczxe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gjajvddjn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnwrfiuyd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gsfhholpa.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcbnicbbd.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gvxaulzen.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gbqjxkwqp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gqhkhleqe.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gtvyjlyer.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/ghkpaolax.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gdbvjbewv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gyzyjledu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/ghzwaxtcx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gvawfrenw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gqawewzxw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gzbcyyuiz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gjcmwqyqf.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gdhhjsrqi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gczpwjmsn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gblmamzzn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gvzcogosa.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gkecyecly.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gzrygwtgs.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gxdlbyrxr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gkxkarqwa.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gipdjyirn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbejstlmh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gopxsgfyu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gnrifgtho.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/grahpodct.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gdgzflyne.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ggrfeuokd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/grvxtrwfg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwcoggcjc.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gxjtsuwkn.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gbgnrdygi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gkghpsluc.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtlwxrxwe.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gtdcoacrt.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gjqeyusvc.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gatjzlvsk.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gwlrwhcbp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gewssaldt.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/ggbxzvbvb.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gwuurdgzj.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gtxcwhjga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gkumyltxq.sHtML


<!-- 参考信息 -->