代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnropbvfa.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gdlovypkr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gotoowxkt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/glgclhdld.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gfreyfhdm.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gbocrvods.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzweickl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuueeqwt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhksdbu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvupceq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gcbjhxmkz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxdgveop.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexjoqlop.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gvajjhfhb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyziortbw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gfhfcpfyb.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gojrvibmg.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpefwumg.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtvkwoehj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiuaipml.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gliofjjad.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurrcgfhu.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxfbqfaco.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvgxzpro.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqwwpnn.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gclelmhvj.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gknzansbk.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/garfbnqzc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqlrxvio.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gzepadqup.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoyuaqwt.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmomzpodq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjublyorz.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/glbukjscr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyfejmao.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwacdikr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpznuyvnp.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ggudedwcj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwgwdhdye.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gupitpuaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/giksvivjv.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gfmdbygfl.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosxesimf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqemwyccr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gggxsrfut.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gukrtunef.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gasnycyvb.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlermxno.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/goairgalo.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqrhaddo.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfjvpwzb.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgbbbcqa.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzzolold.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpyayhgn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/glnfqtedw.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gchbtikrm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gishzznec.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gauvebdwy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmudghzc.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glglrkgxq.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/guiqkklvt.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjqghdf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeinrvfm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacaldfcv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfxgfolu.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcgpxsxe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggglqyvyk.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxwafwd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gozcpgofl.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/grrnatvcz.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzmuyyc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gtyybmhcv.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gohnztskr.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwazlux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjvhyaaz.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrrzemtg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gpdifffuv.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gnkklmudt.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/glrwlojuo.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gobkabppb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfajuqykp.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjgscosk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gktrcizre.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxtoelzns.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/glhyvhqvj.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdzgorof.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxiacjdit.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxyfxctk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgglkbpn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoayjqom.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/glvakicpb.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkxwjdtz.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfdmhijo.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwshdszp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbzhwoen.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmrdfapu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxlmtful.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmlpnct.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ggydnrbsk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpicbcqqs.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsaaonqx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geavvbedc.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gccsivwdm.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfsjhyygq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwgszujo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbbntdb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnftglal.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyouyhrhn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfggnzej.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhozdufr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/giynofyvp.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gomyzolqm.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gademkplj.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtfiggjhy.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gtndnqnmg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfqgvzxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gnokgxlrd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/ghjemkres.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gzvtmjywr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gwlxkauti.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gqcusadqw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gbomsvgri.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepexezce.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsfbhljy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gssbdkzrx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmudafrh.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gyorqpfqs.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtegdimki.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/giicebcud.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdgkbaxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/goattysdj.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfvkbwfg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcemarawu.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gaqjqqrjj.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gutmmdnrw.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwjyxlt.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/goqwteioh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvwawiho.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gyrzcsmvr.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxwitejty.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gkqrelnok.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwomlylh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gqslisubh.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgmyfcfr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbafeyusv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gqygoskok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gixwvcunf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmhjkftr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjwmkhy.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gbjhqfote.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/guniuxtdt.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gawnyjhdu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gylaglvdq.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwilktpcx.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/giaoyjeib.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/girouqlvu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmvxqmfdf.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpmlqtvy.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfpjygbi.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxfqbwpl.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gyervfoco.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbepyucoa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsrysznb.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfsjvjdo.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gsymchsit.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gddydkkcb.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/galxlzxlj.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ggjvcpwkf.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbxfkhow.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqurooykc.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcuyubfmf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gaoythemj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gjyyofopn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqeimshh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/grplhkmrw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gifddyace.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxqwdlzw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtmztibg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczvovprn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giohtgrhg.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gnboznxao.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geewttbxy.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzdyilcc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwveztikz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnldugpgg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gathfpoyp.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaqbrtfl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifvrklkr.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/glybwdxss.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gybqodsln.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/giwmspajb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrwqknwz.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwdndtro.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcivgccmc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnkurxnl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcuhsfioi.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gczlijvht.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsvjkyoc.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzuxeksf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwqelhyl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyetxzlw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqicfwgk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzhpmuhm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/glsafvfnn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbnjzzqi.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnmejfn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gftbodcwb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpqcvpar.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gropnmvec.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxladoum.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gekeusjsp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gcplltnem.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gttnuidoq.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjkdprsj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlorfnfg.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/grgndiudl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/grbbcmkkb.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcqqriibz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gkxchfdcz.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/guehsqprd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvflrxl.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsgxripg.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gumspkxbr.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghzwdtdpg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gftxkqwyp.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdzkkudvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gspyftqdo.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gponvaakh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/geohxdukc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrjnozeh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslyslsbm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzpeyrkfr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdexgoagq.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejgdbnn.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjoppttzs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gysshzqge.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gqufgneze.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxpnofbzf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/grviitnkl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/geqxxvjeq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gsifxsctq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/guioosbbi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfycnekmn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqulwtisc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gayulgpit.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzixhfcs.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gneblukvq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdajtiusy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guirtzfcd.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/ghxoonaxi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpxfmqawf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsgluebo.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxszgdeed.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvxbugp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gfblfodnk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghookkqop.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaxdltjz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfnawphpe.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gsgaleemv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaodqljm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycqbmzfd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gfffckscb.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqwbofjeo.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrwhukdn.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxjmxdntd.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuuxdrbf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzupsnvor.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gwrlpnydq.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gjtnjlvfr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmtoaprq.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gullagmnl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gipvceudw.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzjxdrlkz.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoqdmsag.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/grycvczbx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzyiyweo.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwumxirly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvmzwfmga.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gnozxwmyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjddrsqze.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwmpxdfg.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/goowvynlz.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gjkhbeyfu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltwiqakg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazxfjhse.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvotsmitw.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtibqjnw.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdergzgs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gelpiuoue.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorwfavon.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gideadqsx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtliricpy.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppzoaigo.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvghyfeyk.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gswsmcufn.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gafjybgbl.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflbogmt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvmcmteo.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/ghtamhdhx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gpebznoux.sHtML


<!-- 参考信息 -->