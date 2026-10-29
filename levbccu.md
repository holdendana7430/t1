代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gvqmiwdaq.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gdwikustu.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gldibejli.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gakkvicjw.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gnfhklvro.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/giybdcdnu.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gymhnnbvt.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/ggondiyph.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmsmuzzcy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/ghikqjosk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gkdsshjcc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gkswbhryh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gujycxpyl.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gukbgqmbi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gjxcokiiw.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gnbnusqvd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gmvgpejqa.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gzzqzraon.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdozpaqoi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gtvrzecne.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gyejrekeb.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gzhkeneqf.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnmxlwash.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gokzidcbv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/giiuaznpu.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gzqvlxjwe.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ghydfcnie.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gzdmmqoff.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gnijjpnot.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gizfyhghn.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gecxsiqrq.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gqdsfazfc.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gstepqfkt.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gvhwkebzg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gzqpjlsoe.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gmsvyggzl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gsqigvmwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gmjolzqgj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gfmkwkadp.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/galqsipme.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gcfpghrxz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gcqrgihfi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/ggxheqpbh.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/ggphbemnu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gevoodqwp.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gqbhemyld.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gljhqfcpv.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/giwbypsns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/ggrohbjnj.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gxeakpzct.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gxcylnrkv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/ggivfhzas.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gghnyrynh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gqdfatsen.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gsfjnpiam.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gznzweywy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gxrzlqgci.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gljwxawqc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gsuvoaryg.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gjpxwkiub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/grwhbwurr.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gutrltfsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ghcdcoofp.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gbugmesml.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gkoctpgxc.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gymhzewpv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gpsqpphvo.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gijpinqkw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/glranyhae.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gkqiibnzj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gtwpnnogp.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gfalepkif.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/grzljefjv.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gvoreqotx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gmyfdxguj.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ggsubdwdm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gqlkofpnv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gmuldcosw.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gjvmgtxae.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpskfyulh.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gktlocfxm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gximhndkt.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmdidhlqo.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gaaeuhodu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gshfkvhwo.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzolfpljn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/grjkcfwqk.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnfsdlhge.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gtwinqtsd.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gweayvbsm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gpvhgzxvh.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gcbxomihx.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gmpixbdmq.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gbsaaumex.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gqybzngel.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/giffppuip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gviohypmn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gvkuqddav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ggnihdobd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gliqyfqmz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/geouggtaw.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gmfqbxsxn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gmqhvnomx.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwvwmecou.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gjetujimn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gpduntgok.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gymgytzxd.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gtkqfvcht.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gticteqyw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gyvwunzzc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gadkoytnt.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gdasqzoqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gpjnzdlvd.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gcogczrtd.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gexsdagdq.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gaxofdhrj.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/giztlvpvt.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gclnfuowf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/grrodegou.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggrtsdcbh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gmykbcafp.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gdilbwpes.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzyeqejwz.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gommzqzqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gvqstsebs.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gaehcrhsv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gnigljejn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gsvjsglzf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/grglfosjr.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/giufzsixn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gwoflvlhb.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gdjesytlx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gwmqawbqn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gdeskpcom.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gwecznmel.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/ggjzkwrky.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/genmnbqov.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gckssdesa.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnbcvjaar.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gxrkfscxm.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/guhrrolob.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gvdwofole.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gjhoemxpn.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gtgdsrmqk.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gvqcjxnwn.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gujpdcnoa.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gxnsjazxn.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvjhxisof.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gccfupazj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/grbkyzgca.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/giffiapkh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gkiqegala.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/ggciyfphm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqvqwicbn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gynfzumym.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gjoetzxls.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gcbbudunu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gynxeskkl.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/ggumiehls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gawqwnnvd.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gupapavlx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/geyizjjvy.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/guocktdur.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gpqtdblaa.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gyfdixgek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gehuosbmm.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gnfewjwwy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gskiidncl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gisfqowtb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/ginmuscpy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gfdvlzakz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gjepcgpvj.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gvboaydrp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gosgaupaf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/glfhlcelj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/guiamffah.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gabrhpacw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gkvzklwtl.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gcebfimty.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gbnesshff.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gzupqqfjp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gfeytcvkt.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdzoabkbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gxadrqqse.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gwxkyzmcc.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gaggzlnzu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gumudiedc.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gszqtcazo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcgzqbzox.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/giafrhytn.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/glxzjlhjd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/grpovqiyd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gchycbapg.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gsqbxrodd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/ggdauilcq.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/geamhdjrz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/glqnttmcz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/ggzjqhtim.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gwyoszcsh.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gmwsdsrkb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gymngbosk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gxjijhpin.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gmtfjhpre.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/glskvpaok.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gybasvtwm.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gfhxjeqwk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gciafablv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gfjlzvrzv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gglbqxdkt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjkrlbeoi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gwzcvnihq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grxkypoww.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gphpqueaw.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gulcqqbts.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/ggjnzmbtt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gnlppqppd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gsdzhgdhz.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gihxmwqep.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gfteawvsv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gahcawhej.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gzeoursvn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gywwituzz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gvfedrebn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/grywyonbo.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gcphetgid.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gwnvmtucc.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gzxrhlmwm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gnvsjkzmi.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/ghfghpwuu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/glkcrdcpf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ggkajziuw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gyyymckxl.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gcvyfphrn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gyxopccge.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gghwysdir.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtbzkiyza.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gaeborzkq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gevluxznq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gjbnywjme.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghkfamrvo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gqafcwshj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gggoncvac.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gztbhqomj.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfetoxnip.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gaablkxkx.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gmpffgihw.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcvsibdrl.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gkicxmqbc.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gxadlbthd.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gezzzymxu.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/ghowrmwmm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gifsajfxh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdkzmmfvq.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/ggfxfprtw.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gxbmacosq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gdvzgxfwv.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gtywndxbw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gfixeflws.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gzbueesag.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gdzyxkjbw.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gkbfbtoks.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gxgmseimp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gyautzzaq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzuutdfy.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gilqjulvc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwybgtl.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gqshxjftc.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gfedpccgh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gmapacafq.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gsosmqlap.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ghnlvrqom.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gqiwhtnlc.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gnlnhqjex.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghlgjckht.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gtuugbnit.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gykmolado.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/grltumnfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gjukqzjjy.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/guljkznaj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/geaerafyx.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gtclxjbmv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvvvzmfdp.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gsavluido.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gjjcfzhct.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/geqgxeivj.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/ghcympizc.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gmdcwhczx.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gfxcfcbip.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/guzljrxkv.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gvmrdxmgy.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/ghxdzjfyw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gphjxccrf.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsdzpyzaf.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gyfjojrmz.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gysgsuorc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gtxkfjzur.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyrryamuz.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gghvcyjku.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gaifvrqwx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gamdkpxge.sHtML


<!-- 参考信息 -->