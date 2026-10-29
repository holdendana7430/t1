代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gvlirooju.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ggohrcvog.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/glbwdleue.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/graczmnjy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gjefdpqkk.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gbmszipfd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gfmgwsfog.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gkymrvibd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gdtxenwnn.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gbzhvgavx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gnujizkho.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/goejxhmby.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gizthwgtl.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gjrejbgye.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gekhriogl.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gptxdubmr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/goqnaughn.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gtpshbzmd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gztgnbdzs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/grakkgnxt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gvezoqpdb.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gnnbjffig.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gkqlhoivk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gefmkphvj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gaxdnyrng.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gkolgvoik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/galdewnfx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gljqtqaim.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gicsiamqe.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gkpmuiyim.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gzqoyoocs.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gjoyvtiip.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gjyjvkauo.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gefzvrgai.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gmlwmldql.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gfxowrtot.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gorgdrspz.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gpiyvzkzf.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gpsfnyjrk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzveoexfy.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gqpwghydn.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/grzchrasv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gpigcvgyx.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gfqguuekx.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gjrwqkcpz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gyllfufyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gbcgzbvup.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gnvalclwz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqoowuirp.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gxzzrifan.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gcncbninr.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/ggcvhfnhu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/goxgriqqm.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gipegdwyq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gsvmrinkz.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gcuzdxdmz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gqrpezwtm.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gkcvjcszz.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gfvgllver.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/ggajdtdkh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gskkawyjn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gxbterwfe.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gjdulepsc.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gdzzzndow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/ghebenmfc.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gxdffygov.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/grqwtxmme.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gfcoeinbu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gnxzlxslh.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gqfefzlgf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gavxalkfg.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grfcmvgbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gncefdvul.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gsczpgfrx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gyzdzljuv.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gountdjbw.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/ggvhokrxb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gcrzkscjd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gvysefqfb.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gpwygchji.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gbbevxpig.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gcrrxzomj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/grkbsungh.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/glikkplhk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/grhhfdhnk.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/guctsgzpv.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gmrcumwis.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gfyxlkqgc.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gshplovdy.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gabkzdtsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gccugrlga.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gyvcsuyyr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gcoqyadfm.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gfzocdfgu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gelpxugcm.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gkkhbllcp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ghuzhglkn.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gnxkjhhva.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/giitnjxnr.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gxwxlncvm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gkopofrjs.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/ggavugwiy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gsrhaftfg.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/ggbcwagni.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/glfyvdmmt.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gjlusbtlb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gjiucrzrb.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gejsziicn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gkebjwzfv.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gvjpprpaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/ghlstgzvr.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gbnwmuqfg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gcfmssegi.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gqyocfjjz.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gzygasspl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzieskffz.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/glcjesrmt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glcnwimix.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glzfpbtpu.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gpsgsfrgh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gkdaextsg.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gimvhivoe.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gdchaplli.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gkaljqrmx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/ghmphecme.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/guwzxltlv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gdmcauapu.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gaumxciqm.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/ggepqbmnv.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/glemuezem.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gwegjdcwo.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/ggrvswzqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gplzttnpg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gkoainsng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ggfrarald.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gtzgfapkw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlqhygh.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/guqdmezxn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gweemxcam.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ggypzcwsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gpvusigcu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gjulzvgty.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdpglrmlv.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gizwxgakl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gugeraeyk.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gjbkpfsrm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gxhkwujqe.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gkhimtepi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gywsjmehx.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/garcurtls.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gpiodivkl.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gowjujshk.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gegqiynah.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwzigxmob.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gjdsbpcbf.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxdccrmmm.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gasrohmui.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gcyzuiyre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/ggytbwurw.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gsfpqlldt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/goywaraym.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gptzmpjgn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gxixgrtme.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gkvvzvgpz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gedotukej.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/giqqxynxh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/glghxozag.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gmdymjdcc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gygerahkn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gsohwlrse.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/ggbjvpnsp.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/guldfrjdm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gczutisxq.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gucdrmybj.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxuetpwey.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/goevgbxuy.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gqzfhqxat.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gpqzhffsc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/grpurzilj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gnwjfbqlg.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gutwdbrjg.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gjxneqowj.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gqbroazsr.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyvxvdaxw.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gvbpcwpga.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gxszjireq.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggtgbecfc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gzbebhshs.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gmyuewcxv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gvzkaozdc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gzhfmtoxo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gpqxyejpq.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/ghhxiymeo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gomacoolo.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/goryjxmii.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/grlpquouj.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/giftmvtaz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gbdbfaopr.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gunfnqclz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gvuxolybx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gouweynnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gxyptnwtm.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gfmmxrrrg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gtchhjaek.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gcdcnbtyq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gjtfwlikd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gkxcbhfcl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gdatfgjcv.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gymownpzn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gkxlfvdsh.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gwjixhika.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gkgaenhye.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gucbmorrq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ghtydjats.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gqqlbuilr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gmukpyekj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gjhncljtm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/glmlbahjr.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcenyvrak.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gkyakfpvj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gqauyrvnn.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/galafcewu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ghdyeshkt.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gvwvwwspt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gxbgkibca.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gyzdtavou.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gvkhasfdf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gtelmugtl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gswmjzrbx.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gbrcyecgv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gsqcvvrom.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gxjeoerch.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggdagqlxq.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gmomogqhl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gcfzctvmu.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gqfcowzth.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gueaqfscz.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gxrzthamo.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gpeehmlhc.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gzhbtpjcv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gugnyvkaq.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gmhvrnapg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gtgvoboum.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/glvuxdxvg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/ghcxcsewl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdocghurh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/glurrnizq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gekywuskn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gnqxsinfc.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmdcrxl.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gqvamtzxy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gkujawnri.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gkgymcmeh.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gmgryaaot.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gfgbmomdk.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/glyhadvsn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gfmutmovv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gsdjsgesw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gdquipshn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gpsbsrkef.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gttdvbxqn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gpeachfkp.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gldnbpirz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqoseeh.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/giwadanlz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gdpqyiacw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gymylncgl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gpzcmcgru.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gdhapifau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gqdfdapkm.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/grqimfitv.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/getytaegg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/goewevymk.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/ghspesuuv.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gkdrcdlyf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gukbtgpaq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/guxbxsrnl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gumstrfjo.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjhcimplj.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gjlefxewf.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/ghbbkhfoo.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gbqghlwed.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtzquzfae.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/guvspjnkj.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/ghnkbhavi.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlpxukhg.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gjpzvsxsf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/grafaovrg.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gpzvetqzw.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gixdqpxti.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gjvqxepwf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gsimfimod.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvbvbybuv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/girhavklg.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gymtjzubm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gurphpeqb.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gkwbbsgnu.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gbjhyqpol.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gqwfmegmf.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gxttxyscv.sHtML


<!-- 参考信息 -->