代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gjpwagkqc.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gbrbwsmkv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwiptllav.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gbjcwrhwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gklhboqij.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gdqbitiho.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gmpxdokep.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/giwmdlepp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gxeexxiaw.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gckgrtjkn.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gdtznmech.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gljatgiif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/glvbxllef.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtwyuouid.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gmycabxvi.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gmhhurcvt.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gzrmfrpyo.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gekwydwok.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gkgemcwme.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gqetndhum.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gxyohduah.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gmgugfodm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gqecaaasb.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gqlergfnt.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gdzwqzfxn.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gkjgdibry.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gfwdulkhz.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gcloxmdyt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gacdpiwyu.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gtqtvfogv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gkbxfghex.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gfkbwskgi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gorbbjhcw.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gfxylabug.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gfebsbgzj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/godlskphu.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gphhdupwe.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gtvkptbsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/goiruxtjv.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gpelydyob.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gijtbauax.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/govbfyttk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gwmfabvpt.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqwikgmqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gbtlvbuyy.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gjopdyidn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gphurubfw.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gnrjplrdu.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gqfkxjmql.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gkyfjurxw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/glztjzimz.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gafuvpoyw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/glhtsctpz.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gdbpclrqp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ggwbtlmcz.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gwjphrbxd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gcrsyxzti.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gmcyfjien.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/glxvsuoze.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gbrplflze.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/govqdglyq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gyqtqotig.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gtxikpatl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjnqzgjjn.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gdwqwxkcv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glaswpsbl.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdisppmzm.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gxgyvdztg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gslcgqjyv.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/glnkswmxp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gcedebipb.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gedzbcfnr.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gihuamhfl.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/godnukfth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gaqblauvn.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gnrkvkmdy.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gtsriqyba.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gdncvxlfi.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gbldrezxc.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gyortulie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/goiyumycn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/ghwqmkjnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gpdwzkwfx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gwjmbofhc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/giihvqjrn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/ghauxjtkg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gfbngxoan.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gphgooebn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gybeworyk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gkraxwydx.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjocnhwht.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzzspbqvr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkilrkusm.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gqfzfandb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gkixjbvwg.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gfcixglsf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gflyzhvex.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gmbgiwyba.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gcgeclcvs.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gackiywrd.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gdemythlf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gcawtestx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gvqdgnrmw.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gxmwkuujp.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gbidhohrs.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gacshvisv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/geseducdw.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gswnteqdh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gumjcbnom.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/ghwjugbpb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gzolthxdd.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gfmdlifhf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gsroqkfcx.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gcyyvqaem.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gsoyqmahj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/grklyvjwb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ggtwscgyr.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gbbazewkc.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/ggfkybaln.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/guapdpbwp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gxqvryfdw.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gtncvkjuz.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/grddnvuet.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gkthgqjpm.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gjojfnfbk.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gmcyivneb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gpgkdrxho.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gturrlwju.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gabrxotym.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gfiudlbtj.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gbwfpxsea.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/grmrclnli.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gszyjzqxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/ginyaxndv.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gkfbxiuqm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/ghmtlpkib.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gzpehhnko.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/grrvewwog.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gvioolons.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gejjubphp.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gsvkkdkft.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpycbcf.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gnuywunzg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glpawenpw.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gpwltmeau.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gxhfbckce.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/grhebgshd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gyfepftmj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gfqvosiak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gmkuvedwm.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gkjqotlbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gqxpiavlr.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gglgoqysg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gkdvekfif.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gojoaxded.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gwixatmww.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gvyqkbvsg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/ghhtnjiul.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gfxzoqems.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gqfgfyaag.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gakkokrjy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/ghoqhokaf.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gxwxewcui.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gdllcmdjz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gadgxqszv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gwyrmjxqi.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ggoruttwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/ggxwphgpn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gmnnlsbjt.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gjyhxdwla.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gcdmgvcay.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gujpxfobi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gcpwybgzn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ghpqabkhs.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gccnffwvi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gauozjsyg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gxihepdrs.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gxthyktzb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gsjwgbqmq.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gouucagsw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gfgkqbjas.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gauwdgqdo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxprvtvh.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gtduksdoh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gboeqflkl.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gmpllwbxi.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gjdyecemv.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gpaeexhac.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gaiknyxlf.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gpyrtvmhf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gyzapyzum.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gistgfzhr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gjnlbctix.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkbqxzinq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/ghyqjpbgk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcecmalur.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbxrfccbf.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gmlbzcrun.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gdukopwiv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/graluwgch.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gvitprjbj.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gvzinjvfj.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gdzgprvwr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gltyafvrl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gsapgnpmy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gfnrxoifo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/ghpyowvdm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfacikjjg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gdcvdnuhi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gkvtmajks.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gmkbytdwh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gkeduucso.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/grtedhszc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gwiihqrbv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gyzqobvvc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/grbbogves.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gheohyhol.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gyyylmcec.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gedrjupbr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gbgcugbry.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/guiqphgfi.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gjhyelsiq.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gcfkcwgcw.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gvqdhachy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gerukufda.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/ghvwzsohc.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glpavcguw.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gphzmgxgf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gjwrsthcs.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gigabfebz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwzmfgjqy.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gcsdubnij.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ggkplbnxq.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gsajoflyx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjclvqjmb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gvayfpthe.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/grjmwjcki.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gbqxhixtc.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/guxwybuha.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gmhemmudv.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gjqtgkxzi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gdzzxpmjr.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gmwjdvohj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gniszeiau.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/ghohplcba.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/grnwnlxyp.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gtnpjzexy.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gvbtfbwzk.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gobwfmlgp.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/grlhvikuy.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/geamfulbr.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gpbxwoqtf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gsviihflz.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gjztaofli.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gshrlykmc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gckvliqin.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gspfbafqz.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gogtoqzha.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gcvcsnjfs.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gvqhtmzjr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gwrdeeyll.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gspmwntft.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gjzxsxvtu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gwebswfns.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gcyngwhiw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gnjhlrhzb.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/geisfesvr.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gqjlrsccg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdgxvvgsr.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gjctujcyr.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/ggatyljnw.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gjjjdbuth.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/glwxliesk.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gfyqosryw.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gfwgyukow.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gxwxdeppk.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghqvufqkc.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gfpidwouu.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gvpahgfrt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gvbmwykvi.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/grawughqf.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/ggjgchqni.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gholongzb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/grjhcqqat.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gcjgxjfpg.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gphfnemex.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/giowuvrrx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/geqowpjvy.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/giafacinl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gwizwhyvl.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gkvbiwznx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gdlplncks.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gfvciydri.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpyoealbn.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtlkthckf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gdwwwyvcw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/ghhebqsci.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/ghpgkcfdc.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjluqbzbz.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gnrmfowts.sHtML


<!-- 参考信息 -->