代发 wailian999

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslrvvzvb.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geubtilwu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvetyqyrb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gphdjkuou.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmpsnhoo.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzokgtsp.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjtcyfkj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfstlrjk.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gjvvacvzn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwgfjngb.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsykwmaqq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylardwml.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbcqivop.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifuxtfqn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpiawmqc.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhclshfq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfjdrkc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gthhnyavp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrkwsjwn.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gattmmbcb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcvqstiv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoujejot.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzkptsxj.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcfbwetk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdqltmp.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gggqzzlwu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidkcibpa.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/glklluugc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/goaqdstda.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gdimoqqlb.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmjebocyy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrtojdbv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnpgnflc.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzavhzkvw.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvxixiwba.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlxotlry.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqcezwvw.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkwwnlwx.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmpmqmse.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvnuacdr.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gstbftges.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/glekbqynb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpyyggpw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnriwpmee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grbpbngkx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnzcwaz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gttselkvd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbeecvsp.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmifhtbem.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtomawsdo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelzhtgru.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gsoekffdh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gxkpinugf.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmvkkppk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkmiqact.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdhskdrxy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrvksoji.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grflygroz.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gctkmecwa.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gqhducisd.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgpzciiw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdwxshbc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvqkpcb.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/guucdfluv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrqyjcjf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaylnlwk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gokrovpdz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkoyypvc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntpudjnb.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gcycnwpui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gykkgygbn.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpdymagrh.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gyxttgyic.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoczigkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glqniqsuc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govsauosm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobhqret.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzayjaln.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/glvcvjqgh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrpqpjru.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gwrduoohq.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/girqpcuxx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcuakxho.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/glajglkza.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghdekktjp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcgwuewd.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpsrsymb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjvafmko.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gztkdcpht.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdfmmsxy.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbguhivcq.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsmizibl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafexxrxe.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvdtbeybc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuskrzaj.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gycpcavup.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqugwaeiu.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/guopamxkv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gridjused.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gooxroyvw.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndduebxf.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqzqhkjc.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gipxmexnz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gjttzsbor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gputvkbqs.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gndvjjcod.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpomefeq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glixiibjr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaooiakt.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/glpjyiypi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gyytbmjvf.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gywbsattb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwttcuymi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/guyuoprti.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gulzxpdep.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdlsoqhl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbsrvbvft.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggworviie.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqikcocn.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gktixmukq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gwgvbdwzd.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gygnvvoma.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacxegsgv.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gregljcpg.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gzvyonjqm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gypdemcer.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gznvzgbld.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gobnksaig.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gutlwsytc.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gknbmmueg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gdxhnozlh.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/geeccxjyn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gkedfvzxy.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/geowfhlkl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlevubqz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/grwuhbjhx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmmlohto.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/guceaaxbj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkzhtgbq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevnkqstu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqxhjxzi.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnqhimwo.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbgydthm.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gbmvkphic.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzsprjf.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnxkhfau.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grkcwnlhg.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvnhqeibn.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavbnnrqg.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkamrjdde.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnctfjin.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyruenla.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxcmokdn.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtnzihms.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrnlyuaq.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvanhylac.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gmninxfga.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhqebnax.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbamuvfkg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givzofaib.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkqnebif.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrwsnbld.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gsfltkekr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grkhtvywa.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwotcxjr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtatalwri.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqojnbhx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/guozushsp.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gopwzcloc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gwmseiccr.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfzltgbdd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gervmatvn.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbvaojjsr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/grlccwhnl.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfrsuzhr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvtvlrfs.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjghjrcc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmpvmnxsv.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grevrtoou.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/geoqaconq.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvjbpnp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgaaewa.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhitbnop.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggwwrfxuk.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gqrxoprfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhnvmdsg.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzcvblid.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipwpprv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzkesmnr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxksoyqdt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckfwjrqo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhicgili.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gssnihgbd.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqlycdfac.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gksonbkiv.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gshbqaahm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvfuyztq.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gswhukrtj.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gokyxfoxr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwpxgqdb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtlzeup.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/grrywrkkw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gfivrhmyo.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/ggcllzeyd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslazbcbe.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gdqdjizzv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfdcdwnj.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnlyonuxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyggidrs.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghozyiipf.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbwicnub.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gotcqjqzk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gginpxldy.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgvwdcgl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gjoiilgnh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqopjdlh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghfnqczms.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gleiqvpmj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gayphrzkq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwlcrnpf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyksiyjw.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbetruwb.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gllmkcgto.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyluudgx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gfzealvsw.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gswbueaje.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gsewhlgmv.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gkpvfpvfd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnigxrrs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkavyztc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/ghaztafhy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/grvephacv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbnaxcze.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgcybnov.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufxmipqf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwzbgkbl.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzhsieexk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzvjwjwz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gljbogxia.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrybamls.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gqjlctufh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/grnbtfmyx.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmbbqfc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsvaqwuf.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gnecphguq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnbbajz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaakdirc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabfldvsg.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/guynpgnst.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gerfqygak.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/garluknhd.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gamvrudsw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genhfjnpj.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxhwxxklp.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gitviakxl.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtsfcxzy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpurcblrw.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvogojoh.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gidqtrxrc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhbhvekh.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gunkvfvqt.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gseqkadak.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwdymfaa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/guztpmwjz.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyqwjuxw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvubcgpjn.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gwomffnah.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/glewompkd.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzzdwoth.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gykptnvxl.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gksbbfwtv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrwscgpn.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gngpfypaa.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkwbqxhn.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbsalgdi.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmdaihv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjmfslvh.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gmcglrttv.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gywjcolef.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/glrxqazya.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffwycltt.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdmxnefrv.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfazarmz.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsbmwvhr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijqxnexm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjfdgrsm.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gagvhxioc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqguxegza.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvhviaz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcbagkism.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpnpyvhy.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gmjycwgkg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gsbgcoqnx.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpkmuwafr.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnprpogdb.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhbwblr.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjdxvyhjh.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqeykfg.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwulpfrm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdviekrow.sHtML


<!-- 参考信息 -->