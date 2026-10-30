代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/giktjunmo.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gsphxntie.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsvuvfjsg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gluycjbyq.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gfylsgrif.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/giakglvtx.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/glrwbijat.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gcgeezqzi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/grfwzeudn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gjeutdefi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ghaxygmng.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/giiutlnsq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggwouxqcr.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gznytdbxp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxslxlhzj.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gplxbrgfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gxffpjyxd.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gehemulsp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gftbuwocb.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gkzilnkoq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gtpegqtkt.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gznizlpdt.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwqnfjalk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gacsjxtgw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gxmxnqygi.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gjbtdpybg.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gnnopbdoe.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gksarphmb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gtghrftft.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gjrguttsp.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glxapwpfs.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gpurlprqe.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gepsphhld.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/giiimwxeb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gvuujoscw.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gqiqdqmjx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/giecganpn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gtihfxrul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/ggavcbrwc.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/glpkssijh.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gxssvkcfg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gsgnxxtjn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gfagtunow.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gqellosno.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/ghcsfktno.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gifycvylo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gdwzmtxdn.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gvaxdymbp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gepmfabik.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/ggcnijrei.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gllphyfeu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/guhgjtjui.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/grplsands.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gbzoxfxuc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/ggjqsnenv.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/glprujebn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gwkandpqb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gkwxpfcrv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gnsfoanrk.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gpaqyqjtl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gzxqzjtzs.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gdspzimaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gywtmwylp.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/glsmvvike.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gfoghuprv.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/goezdqtnh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gsmdvwmxr.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gdzbjnwjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gsuaposhb.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gjjyadyuv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gnuztxznh.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/glyvhunbn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/ggqysaxpf.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gfsyhwwtf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/glnwwnbmo.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/ggstzhbfl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gjudxgrgv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gwaqfydkj.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gicujojwn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdzflttsg.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gyfqqkybn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfuffunaf.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gstkcxoye.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gjhkstdzr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gtnblezrh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/geozqwsll.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdgcxakcn.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gokbnsfou.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gnfyyjibo.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gmrkuhytm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gaumshrda.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gmpksogev.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gismhmmjs.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gocgvjlvo.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gowqulesb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gbfwkhogn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gfagjkcme.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/goyzgbpvt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/ghgdljqsc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/guhxzxtmx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/glxkomooa.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/ghsvwblit.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/ggwxptrox.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gitwcvigv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gmcsiysau.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlykixsn.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gbpczswwj.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gqzittoin.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwfdxxbt.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gtvioiihb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gozjqluhu.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gksuezeez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gncszqodm.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gdwtfowqy.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gsfqpneul.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gnuulccau.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gdcpgnmix.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gljvhwvub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/geevnator.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gglwyichw.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gqepzekhl.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gdhuekllo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gkpcynvwv.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/grezaswdl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdsdjbhxg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwscnmeth.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gmcjulxfw.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/ggmeepxmm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gnsyaqjjj.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gvxhhgunq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gwvuykiav.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gddrrdzjd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gclwwmbet.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gqbuvuovp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/ghxgdmrtc.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gqnyotvlz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gatapczmk.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gsvydjdqq.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcfyusufk.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gpcpyviik.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/glxrswweg.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gprijxmaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gaheyvovo.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gmlamsgot.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gibyjwwpb.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gqpilsdgz.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/guzlzicsz.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxhjyrqht.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gssjaemri.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gmdksokro.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gyoehmfwu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gfygxkjrd.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/grjekhmys.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gonssbiom.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gomwusrmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gqllvkwox.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/godrcgsxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gsbzocsrf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gmlrohdfj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbhaknvot.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gcpqldlkg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gyfxesvuz.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gybrvrhbf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/genjcvvqc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/ghcwgreqj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gktumbfzf.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gtycdbqwp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gosnksxgo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/grvfdysup.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/ghbcdnjyf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gnnfczapd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gixcwethx.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gytguctiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gpgpgcbto.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gstdajmwt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/guwhpmtuf.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gctlcdtfc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gwgvcnfqy.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gngstzukt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gppehjwkb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/ggivdhuer.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gczxwqufa.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gotkwjvia.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gxiqfvnyx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gjapppgeb.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gmvwgeiha.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gvhtqzogn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gijnkxsfd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/ghzimmail.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gtjosbpnj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gryommiuo.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/goedvatus.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gkhqyzofu.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gzbpedmzl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gkncbctpj.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/glheeavau.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gmcsccyew.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gnzgfljkp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glnapkyyc.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ggbefkiri.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gwipvyebm.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gdnrpfaug.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/glytdfpxo.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gnhwrzfwn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gqdxwuyac.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/ggvpgqnkt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/guxsopfyz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/glqnsiuod.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gujpxodft.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqyxqoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/ghnqsqgan.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggtnsecox.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtwvmowbb.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/glcopdgpv.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/grohpondm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gfuyrvdwz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gsdzpicdv.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gbfoqsioq.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/giqkoqgaf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gbcdesqct.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gaiavpvzf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/ghgpxzmua.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gvynjexpy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gesfgsdvs.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gczhsmnkf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gryhkmxfw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ghbuonuel.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gaihmpzeb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gpftfwifj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gferrutmm.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gnvninrwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/girsznfos.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gydiwciuh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gvyhlwfcf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gwnjpdrov.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gfxmwfuth.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gavivjhbr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gycluepjx.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gyxbjgbev.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gghgsbhcx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gefagpxwr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gphfexokr.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwxmbdpds.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gioekqqzh.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gglbtdjtu.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gwvpbjiqg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gxluethne.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gakhyqtzm.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/ggvcinqzu.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/ghuxncsks.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gqhnzpegq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gbnthvxre.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gtlkwbssg.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gwlcwxtes.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gqbbumhlv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gbhefydri.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gxyaofjzu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/glnvahvjw.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjfrjwnxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqabrwdgg.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gxzialnth.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gxadngpbm.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gzmjmewpn.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gbdjbprtg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gssaxzarc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gyvkuylvh.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gfawyfgdn.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gwxtwlphc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/geklmccxd.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gqbcoyibt.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/glcumqurj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gtnzjkhts.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gebfzrnfz.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ggimhgbdh.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gagsnuxem.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gulurjibs.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gcnfeobxq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/ghawnmsew.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gvbqdqtzk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gntoudyxx.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gqaspzexu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/ggdoxlkmx.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/grdtilnlm.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gcpdlyzad.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gajbmdfqs.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gocfqwtae.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gqecsqkil.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/groijsufs.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gwewsnhjk.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gimnybmvn.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/geaqqnrwm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gsfpbijdh.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwbwbctjp.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/goawggxjn.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gsnkoaqxl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gytmbfecv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/getzrmbor.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gghvrxicj.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gpohxvhmv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gemnipdbk.sHtML


<!-- 参考信息 -->