代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gjebcqhad.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyrbiawr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzutkfht.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjqbhwp.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbvlnrkt.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrehikxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvrwizjg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/glxnablsm.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gububbiqe.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gsgabwtpa.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeqrcvkb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonptperx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gogqlehnb.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/girdmnasy.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyxyffpv.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdgjvcc.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhebrceo.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcsogkbgx.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeuenjqv.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzmeelms.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/girvbimes.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/grtzjpnff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgufslld.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyotlfgjc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgyvpqrz.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gumatgfcy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtybswfbf.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gikqjbtia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozdzyool.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gaogmeott.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gutyvtjrl.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gcjkfvotk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gijlagtvl.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gazjbebai.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsbwyim.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gwshtawmb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/godejbpef.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqembyrsa.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmimfvhu.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ggfxduddh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkingdoy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guefkkhmi.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/grnwlfyym.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/glbsdwdig.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gxjvlbwjs.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxludpboy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gwwmeikss.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoofnrtx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjthqcd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkzcjkuu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkzljboq.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gixgqgbkk.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gfdxjmcie.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjgjqdhn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gljcfchgd.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gemsowxjv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/glrzklcwy.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gyotgiuze.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnltnyft.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuvlvuzj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaspncfp.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmebgip.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gaeibmbxj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbteldmp.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpqwdctk.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtiwqgql.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxaommen.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/ggbbvtxhv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gbdethqhx.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gdtruushq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqrjszfw.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqhgiotp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpzyjbdh.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpfaeymc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkzbavad.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuaaxwmg.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gperpmevi.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gdescwugu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjmtrvzox.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdmeoajob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggxwvywd.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gecjzuutp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gppbptmcv.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gashqkkbb.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/geipsazmm.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gzluaxnyq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvfwcycaz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaqcozpd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gduzbxipv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gppukxoml.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gajiaseds.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbllysexf.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gnosyajvy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsqbdoksy.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqmnwyuut.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gtrejzxqk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuyxslgf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvfdkpuor.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gisoxjvha.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkyatgep.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxetfyqym.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcjolvtx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gqonoaatd.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkufnqeuc.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfraijqzd.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvuagnvzh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlbwxfcv.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvxuwotsn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gypihmxjv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabpqcahw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauvgrlym.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtloskzoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gickkbkpu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcvtmpkx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjxswlwc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynlttruv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/geyakodys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwkqxwrc.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoluzryb.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtietjyft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/giijpanid.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmorsopai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgfbqefy.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gxowwlxtv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjtlzbgu.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfvuswzx.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gonpppzci.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqegpke.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gppwxogyu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gammqwazq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gzitrccro.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghotedcts.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtehayozp.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmegejkfa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gifhastmi.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gdqvpmooe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffjyphx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/guilknrbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjbfddja.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvnevecz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeklspck.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gmuflbzat.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmprlszt.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdywudge.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtaguxdf.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfctedfyw.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/getohqxnd.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gelnrnfky.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqmgfrmzr.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqxswplua.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvxcysfo.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcrryrqud.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guszcxjid.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnpbfkjfv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/grivvsqwl.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gcueyadqh.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxxwkxzp.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtambbckf.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gfkesrwpz.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzjesvqrw.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gysldbszf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gliztmece.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glmsnmqsc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/glazcngoo.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gadnearml.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjowwwah.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gndoxctxy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyblhqiz.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gdobqtgod.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvnaaimgx.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gxyyndllq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkowupns.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gbchlyjoe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gfikidrvo.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gatsrwwuh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaggeqku.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glkicepvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoumrvfv.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghnaqsh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdegkwiyw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrrtyjwx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gamupqwqm.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcovbhgv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobffmfat.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpgasrzt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gdegjtccr.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnilgnnq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvzbudrp.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqcfuvnx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpokgowgz.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gcizgvrdc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvusqnrm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gqzrgympb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwmdtvzld.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxevudyep.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gluonhufn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkajcnobz.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghpknqyti.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxybeetmi.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpcaswp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnmirznc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gheetkgff.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gjdtyroir.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gvsbrvudt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggonkefrl.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgelsqkq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gybuvufck.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/grnwreeni.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkgwxmno.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfcfjaju.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvficjgb.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/givelphfv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtigdtinx.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggogkkvaq.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbqxdxek.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gaaykjdec.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gqajbukcn.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbaxaxxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gleflkvpj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwsecegw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjhmqfrg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhjoopct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquoeiggm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grqmtprul.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmxmkaxae.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgfyctqh.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grwjjezps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjbpfleq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gdoftzkej.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqyopgxd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnttfykw.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzkjhpefc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkrllaulh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffeprqoz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfkzuhsey.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpgrelcn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gwngnxrjk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxztvtsn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmkhwbax.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmqdrzyf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guxszufer.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gitamdcqz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfvubmiof.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gnxqrxtnd.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/goydjcmvl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gzkehhnny.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gmuhhcymw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gduhsyxub.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxwkgtmc.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzjqpsjc.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzcdgtvlg.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpklnozg.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gblrhvria.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ghixccztm.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekapmxb.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyftmacg.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/guniztgje.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/giidyadgb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gybgjfczd.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gnnftujve.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlzxyiqq.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcagtsbm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgakywuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbznjnul.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grgamzrjz.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnduhkkof.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoazjeua.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gunczzshu.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/grpeuqbwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gbsmxzjlk.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gficnnykw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghezzftyi.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqtqusui.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gqldbaqaa.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/glylfiemv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gesmyxfyr.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmaurphj.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqynrurff.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gmumagzqs.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzkzamlt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gzibquwqt.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbhjdnhb.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjjsbbsu.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gdzxxwvsc.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbjvnwaoc.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnjgresp.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gympwfjkw.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gkvasfyok.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gkkvlkhye.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gmeseaoif.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gwcmftaiq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gvqynyxrm.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gbtbhuecb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjcbcmmb.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsomioldp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbimyhvs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxivvnnda.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhymbhju.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmtgtptpn.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghroheeit.sHtML


<!-- 参考信息 -->