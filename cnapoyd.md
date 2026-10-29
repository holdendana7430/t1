代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gamqtiogi.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/guepeipuk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gqxhnpgfp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gewzrgxvq.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gcunowgwn.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/grrskvqtn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gljepurze.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/ghwfqhevp.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gaupauxny.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gysysmooi.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gxujefdlm.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ghdohmosu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gnzmbwxfj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gruruetlw.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gsxqayjcp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/ghzaawstr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gssnpvwpa.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gxpjauens.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gzsirgcfb.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/giroliotk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gcoafstxo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gtscowrdi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzhbmkywm.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gltfwwdto.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gahvwvjzi.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gjihabkyo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gedpynmld.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gerqeuisr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gzpkiajqo.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/ghdhlotui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gzsiaigiw.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gfqacixlr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gaddwfvyd.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gtfqmdcuz.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gqdbgkkzx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gsbvgsjrj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhwwlju.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gnkggbvez.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gxfgccelz.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gidiejuia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gcebkawaj.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gigghpbym.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/ghjdmqanu.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gfvfvdker.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gocjpfegs.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gorwsheky.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gpmuuxmbz.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/genldysjh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gnxlwytdt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gftokaghr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gukvtfkdr.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/grnezkumo.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gwevnbptb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/ginznuglv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gxrakoizs.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/guersgrdn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/geqkcztmf.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/ghhsylhsf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gerztivmf.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gwypcnmrh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gmhwwqfkm.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gzzsymvgw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gypuxnhbh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gtsusxril.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gpumkmhyv.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gkrlsnwnr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtbejblal.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gsgcswwwb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/geitdovzf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/galhdfefd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/ggpxfvsct.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/glrpaneea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gwwkqhlqw.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gldfwbkjw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gsrykspad.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/ghyfepsww.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gtqiscgwu.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gzatcdumy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/grauqqnqx.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ghqdpotjh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/ggnqqspqe.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gdcxumrge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gunipydoa.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gisrhtwoj.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gmbakpvvd.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gcssuwhfu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gikmasbsa.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gtwjdiayu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gaohqosmy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/grcqhcbfk.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gbgbkmfqh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqagdfzej.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghhzdgakt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwmqsxdvj.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gscmjjotm.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gflrqcrtv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gzeslziuv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gqquxrvky.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gnyvrbwgl.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gcqqutkbo.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/ghxndwknq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gjtwpeufl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gbnfsjlae.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/grfcnfjam.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gkangeacl.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkqihogcy.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/glthomhhn.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gypkkxzgo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/ghwdzardr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gyyhqcurj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gaegtfvdb.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gkqhagzjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gvnrfvbdy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gixbpmarn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/grgmmghdk.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtgsclolz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/guezvdusz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gutifddky.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/grkgdthtx.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gltxavdwq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gycamscpi.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gjmgollut.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gtfaxvdrv.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gesrcmhfe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/glwmrtkhq.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/ggezykcqv.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gxercfako.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gsdfkhqfn.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gdeyqsdhd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gtpctcnzx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gzaxxxpnf.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gykugcepi.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/ghcdxbrgb.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gronyivtk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gkihplxmx.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/ggbmuufgb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjtazldxm.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gxsjvseii.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/guzpdfiwh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/glwwuccco.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gvleyktkv.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gsalzzmnl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gqwaiqdrs.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gsgbeuytl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gkhndiuwf.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gzxhqtnym.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gtzxeqrry.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ghohbuxwi.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gevksuqnu.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/ghswoarmy.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/goamabvun.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gywedifai.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gkyyhfeqm.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gffdutsek.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gayzyvrdd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gujzmyban.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gsbuiwwlu.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gcnjnguoc.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gmrxwxcbh.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsuivypbj.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gtavrcdbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmhxqiu.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gsfyktahv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gvtljmbhz.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/ghezqpjfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gdrrkqokb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gxscwqvte.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gcfephkfo.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gctzjyqzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjzgwuxvy.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gnfsikzay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqzefchpc.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/glraiqyrc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gvvojkhpk.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/ghrgzbten.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gulpgdtwb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gzqnfhbps.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gmgdshdoo.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/grtivjign.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnjlcgkas.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gvyinubgc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/guhqhauaf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gidzwthzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/glorlgpyq.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gjtdbzqqj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gddxrtldi.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gadnltzsv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gqjpeehsw.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gkarnwsdi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/guspfyzie.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gatzponks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gojblrblq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/guskvosxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gllrfrnyd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjmobeewj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gpplggfbf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/glwjjrpks.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gfpnabhmi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/glgbqhhfl.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/guumvrdoh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbshcrfnc.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gtbfqkymg.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gfzkyeyun.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/grqqjqtga.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gucuxbnev.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gxddjyzjq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gulcttgfl.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gkqqxdpeq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gnahxcmen.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gdtgxpupk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gsqogpzwp.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/guspxatdo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gvvpwhduz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gkbotmwlh.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gxojplkfk.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gnvazefst.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkeeulx.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gqsjpzvgh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gbvlhknxh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/ghlunffbc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gzihslufi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdrkruoyq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gllpmpnje.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gogdwouwi.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/grsfjvxaj.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmzfdxauy.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gnusvabqe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/glqcmfrml.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gnvvevvzi.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/garxwgfex.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/geiwbvudo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gfbmmgdbk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/glgixdufz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gnrnxgygg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gadfdpbdj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gopbvrejr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/giyznidax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gpjfxmsjy.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gpbrueitj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/glfcugdlz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gjzwlxidp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gbmvuxpki.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gvvennmyp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/ggtcafctv.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gxesxtctf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gxwcfoulw.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/ghetjozgz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gysbfdqcb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/ggmbanorv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gxlekgskq.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gmwpzakei.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gfhawxzgi.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gzyisrcvq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/glldhbinj.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/ghgeqkpiz.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmaszsahd.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/giyoequfy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gtwidtley.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/ggtrxxjdd.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gxrhlpynx.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/giqnmszwb.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/giygbkfct.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gnwuzboeu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gaetlypnm.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/goqmioxwh.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gwxkysesz.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/glynepaja.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gzcvifdjh.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gvlkmlmbg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gphbvqeje.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gmflkwcuo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gahzscyux.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gimdppalh.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gsnrtccdt.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gbxqplzov.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gdydeyzsu.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gasnixkto.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gzooowgls.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/grbmnqfhq.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gctjmsqiu.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gtxnjfqna.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/godnngcde.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gfkpbyroi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gfouyopfx.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gvlbecsfy.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcmwirtth.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gtbhblkat.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gxedxzotv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gmclckgnx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gpygosxzi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gcimlzukj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gebtqxqpl.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gwjckvsnq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/geekgohqd.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gepmmmljs.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gqvnldmhc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxwtgxiyp.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gygpnptgo.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/ghvkypoqn.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gyrhquewo.sHtML


<!-- 参考信息 -->