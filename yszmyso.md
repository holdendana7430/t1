代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqmdjwhvu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsbsxdrf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmzhrlkqs.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gravfhnjg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxroztjie.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzxbpyrl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/glnxovdeg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrtjxpgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwbaxjm.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gctupudte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gbiizenvy.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlkjxkyv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ghaoinaog.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdjmpquh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gperhkmkf.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/godkrrseu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gthwgcblt.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gaqipivgf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghufdysek.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gobyyithu.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtbuedhep.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjxbvspwp.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggbfrophc.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcjkbokm.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlvlibtz.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ggitgylil.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnthxqnhb.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmouxpzqc.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/giixtqszb.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwwyjjw.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmceyquga.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gsayezofu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gybvurhch.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudkekgau.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gufhxjtjm.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkhnbufx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmwyjrcx.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsczkerq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gadqcycbc.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjitfhrx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvtfoorb.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaohsuox.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjxeuvu.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gaqaejiux.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gsdngbkmx.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gmemkfmdg.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzaurvkeh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gnomtgnuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqznzbigh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrzsknbu.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjfewqd.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gxujbzgac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsvffbqw.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpzdpogtv.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccuexcj.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gxiqogzop.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gxqcgyqpy.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeemiauj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnkpcqvo.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grstdhdhh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaubgmgb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsvwwbci.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkjbbfd.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gseyvmvvd.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gkvpahdvs.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyylpwbu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgbugksi.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkacanuik.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ghcypjirq.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnevfcewg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwytbdhgt.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdxazkdc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdsazprr.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gysrbdftp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlgkopyq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gjitqpnrn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthpllyuo.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gbswqulsd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgvuwipj.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gmlhobtxa.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaiqpqjd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmgznxsx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybrblmon.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gascdddfj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gblnxskce.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gcshpuxdn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gstmipzcf.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwfsdmoty.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ghdxppqyf.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/giqwfpjsh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gojykziri.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gibqfmxlk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gugrkgicu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutrtsmwb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gehkhmhhm.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gkrpqrbcm.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gtrhoulth.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlxkjcqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyqgzmfuh.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhoryey.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gclxbvmih.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnidyzo.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwmegmfl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpudmylc.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwhxznrk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggukirehu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpdxkvi.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmrmssxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gycscietb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgvyrami.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvggkwztm.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamgqimfe.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/ghejsmpyq.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/giwtrrmth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gjmdebnwn.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzpqqscyo.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggoqzaulx.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/goxrruxca.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqhhmgjs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrfljvan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmklirlc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmxzaoes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/geesrqxic.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuqkbrju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvcfmcz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphcnctqr.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gqvokeilq.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gheaecful.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gtdubtotn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gklzhusva.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvofaoar.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlujtzi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbeewcdb.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgfmwku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphwmhbyu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdhmuun.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ginnjsfzg.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvknmhzdq.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqdopotce.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/ggtdaascm.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gfdkoyfes.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gthibcycr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gszqruewk.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnsyccmpk.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gmzkxwanx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godhntzuv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gkwzeaevy.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gkjireeks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gdxcoetmw.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/grhyinxbk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gkhzxrafp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyghkpht.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgzzxquc.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gbtuuaftq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gumvprnpo.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gumjgzfft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gnsbhclab.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnoixlhne.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmqrprry.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gsnmgzwti.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrsbfuoq.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gomcioqoz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceccbzdd.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlrznssj.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhwhiao.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepuzpepj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzrtzmtn.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/goxzmqqnn.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfxlpqfy.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gquueaioe.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsejpwqnu.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqxeaoufu.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gakqhflvf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxovrkei.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guclrzfsx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhzqbiqm.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwgxuoxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbheufrk.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gezuuipkl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlzpdpzr.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtczqiykc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthozhblm.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlvupkjg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gantepfsp.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gmoyqayvi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkpurwhl.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlddjkel.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacxbiwpg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyweclqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gwbtpoaht.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gideqdobl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guxqdzbvv.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnswrdihr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glkbyvzcc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gewpsfhun.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdthmgkkg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnphsjlvv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/geowikmem.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjkqhegq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaxpkzha.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gycoeeuup.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbwryzpe.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuymiifk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyfiorzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvmayqjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/garyugbkc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrcziwjl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvydrngoj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtsmzyam.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gglovrxea.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ganzvbnuy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoxsylcs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gnszzjdzb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpieovuk.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gzlbofcba.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gbdgagkda.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuxprmqg.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gygakvdjj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzgyvxx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpvpohmp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/geaggqcfc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuowelbf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpdktmsf.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gssrjpppt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggygabisz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgduxapf.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxicjumel.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsqwahbl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaoyddsl.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtowyrumb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjveuobv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyvotjgt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddtwfsje.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxzhxcipt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqhwqodr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxssliqzs.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwikdojfa.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwravbxoh.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigvokka.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gafkdfuxv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrteekwu.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/grltrxwoc.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gmownciwg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouizdjgj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjttpindo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/ghowhdqrz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/guwbutudf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gspxunwss.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtdwewooj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gurspufzh.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gzzajhivd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gbkqagzfi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gemlhpsxl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsunindfz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvztjeiqz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/ggdvimtzv.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gxlvujtdu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtnjjmtl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/guwxyjdvb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxoecutgz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuuaenne.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtyfghnt.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gcprcefkc.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gssnnlomt.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/ghtjjejjs.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwxsoazb.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhuozllb.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmzxhpvuy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbhfrqxs.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxagiegeb.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gcxemmuzy.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gopotebbf.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gbgkvykjh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerjqfacn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/goznpuvry.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtydfgmla.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyuexfjc.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxklkulob.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvweoulv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcboulenr.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfnmzmrd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gosiaozej.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gwljcxdih.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzdwbfkc.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxpeqej.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqmydriv.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gmsjxxqgw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfykzpbyc.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmywlndk.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gctjyjujm.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbcwxuny.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjwzttrw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gskuhcshn.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gsyeviwns.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gruzrfqop.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gotnlrqqi.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggoghazmh.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gblmrclkp.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gistodwxi.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwsyemezb.sHtML


<!-- 参考信息 -->