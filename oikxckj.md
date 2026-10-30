代发 wailian999

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkovvtcrw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrhxojei.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gwwejgupt.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gtkgqqaon.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/goswobjio.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnpoxcuj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gkluksbkf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/giesldkyl.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gygxtobwu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaykchyh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggggcsjll.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gpotnhszo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gdsschgww.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbgkdva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ggahvxzbb.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnvecuuk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/grnbgkmkl.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/grsiauuko.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/glslvfrrg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gnrciqzgf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gqvfduinc.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gsinsevap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geamhoheo.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gconmypnx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gmlkbxbpu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/goisccchl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfccsdra.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmsbjbtzk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gothpkqdv.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuzmbmmb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpbdymvkk.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gehviahgo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlqofirj.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/giecmdrvn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmzjdxfzt.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkspjuvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gipcwvcsc.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gihsfgzdw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvleacqil.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzrbzyia.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljcfzgq.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gnijxwsrp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/geoieizay.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gyxqfeskz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gysksyzwp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ggwfviirv.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gjodkdmgf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gakdjvcuf.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/grbznnnxm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gepmqesfz.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gugfyhxse.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gocxlfopo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grrbwhqwp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxzxxhsab.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrixqcx.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gelafhbve.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdqmypev.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxbfnlrz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulgjhdgj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwguprgfz.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtibbuovh.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gainxblxv.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gmcrmiqca.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvllijrym.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfwkbvre.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkuhxtj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbulncls.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gekxjwuvm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gzcmxqapd.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gysfsvyzr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqgnmdbc.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjodcemul.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/glyhhilhm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsobpztmq.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gzkiuejdn.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guncxflyb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtqkeyw.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gptxkkazo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glmhwnhqf.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gborpewsr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/glyfpusha.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/galxcdssr.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gttgirkiw.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/guwmdnvyu.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqnnhxu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ghwyweipk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gdwqmoclw.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkmjzatrh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexomrnjk.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjrfecedx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzznwgdui.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/giqnumbwn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjrcdnnr.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmxwjjhy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyfsoicf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoalyjck.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gficciyhk.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/giarvgpwb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyisrdabj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gweasdrbp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsejernth.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhayijed.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavdeervm.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gndpvijxu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnpexziv.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gufrjefkb.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gvhyaxtmm.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcfpmfod.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ggywopizj.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gldtjxkhl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gnaawxmwr.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gyclagpqq.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgnjjjof.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooqjadmi.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gfpmnkbsz.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gywhbscnm.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbooqbt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkongcaw.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gboqbjttn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gtmclyhlz.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gkphjnrxo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbikilmxc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gohmeczac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzkrhned.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gjwtpkasn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghqewattq.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/geaumjawn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntxzguod.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gzsqjugou.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gerdctedo.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpwuagnl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhqlnnfi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtxgdvvnw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/glqkogmpv.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/galthssnm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuobkfpi.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfcneklqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkqbchumh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gckidqvyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyacuuuh.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqyapfbv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdumrmmnj.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlaosput.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gncjmjgja.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknsedrv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gazxxqccy.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gpquyrcyn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjopjwvin.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/guopywhkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnegpdxk.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkvxdmmmd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqiabmma.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxqubspt.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwexxdjjk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gudtmeklo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjiwgymne.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gsiwptxgz.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/goozgpugz.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtgytqrha.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcgvycq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaosuakp.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gigbqfvqc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gkhlvbefi.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyswjvvl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzqpdsdu.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gdgfsxtwy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gyygyykmc.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/grpoozuik.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyomigqr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqhtxth.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqjbjsvm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuidkltk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwymxbhd.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gajdtorwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gliucjlcf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbzbcewz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gvaiizbrq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexehewey.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/glkmkkohq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpcvxjhy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhaqeed.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gutioiles.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkqknzvl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwczskhb.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuthqwfb.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnluyzmtv.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ghdsqubfa.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gareaefbs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorijzigl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpulqpnn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/geokdbfig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gihmrwgzx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/grckkoanx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ggfhxsmvh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjvzfsxp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/glcmlyuew.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwvotzosh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/ghempazkg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gayeekvud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gftthwsnl.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjzgpfjq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/goqymbmcp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gkzeqhske.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxwnliyi.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/grcbnuckw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjrmgfagz.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gcuqtfgri.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmdpyrhi.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gubldvovr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjnhysrl.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghxrqpant.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbtpevarb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grqqidcjt.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbtysequ.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwfztezsu.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gkjlaguog.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvrgdvra.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxlrnlyp.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvzqnpwu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxfcbwwd.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gvlnxgkor.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwilcjs.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqhmpnfgz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geroujfit.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guzsunjfe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnvfwrh.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gllxxufck.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgbqhht.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gioumrfnd.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsayndux.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gyqveuywd.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gnxofwwdy.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtnqzmtar.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gemkueegj.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzarrqxce.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsreyqhcq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gajwfipfz.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gngcxlmls.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gjqdawwsu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gsujnfxcz.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlzefhxj.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyavubifw.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjhfzxjnh.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgseuptu.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gfidoeuic.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/goxatwiub.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilyqhrie.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzamogull.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxhrgsiv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznuitfda.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gizpgyepb.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gynxbmpop.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gpejgxlds.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxlsknql.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gubexnvtg.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gsikzvray.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmchzidbn.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/geuymwqjj.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzahbzxa.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gjahmmbtu.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfmfebadv.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxpacbqy.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/ggxzcmzsa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gemsaptbw.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjlvnfdyd.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/ggfembprq.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gonlaltqo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrriaul.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gtjiaooml.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcvkblzk.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/grryoljoo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvhkituy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwynpujc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmgbuxep.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/giswjqimc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gslpzyguf.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrqvswt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkefducvc.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwrwblwd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtbgocbs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzywczauy.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxxzinbb.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gilxxbrib.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbyhlmon.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeuhkrzg.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gelznpzen.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/giyrrdmbs.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmenqhkln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjjwvfjj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdczcypef.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpkrdvxec.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwybmov.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/grhlzduuk.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gtzghixdo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnivcwjb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjixitmgc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtnbfirf.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnaeteee.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbegjqhv.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhswrraq.sHtML


<!-- 参考信息 -->