代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqjwbgdm.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnloztwza.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcktqsjf.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpkbapomz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkllragx.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gahesnacf.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gagqcdnbr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkyrvlh.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gpiikgyzu.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvedjigcu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsldckaim.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqacprsbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjdywfav.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhosjsnz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdacussq.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpbqgzuet.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gptavwocz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxsufune.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gksgzwszz.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjqdxnmvb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrujpwwc.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnqouwyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdzrobox.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdudshnl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdokqfjq.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfaizorch.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvivhszy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwxxgqdc.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gwmeiqcix.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gttzntopv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfjkmwon.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoeqygwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyjheqdt.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghiushqew.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiponckn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggtqriiwu.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gozykpipg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddwaybtr.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyzpfgte.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gvrsooacv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/grdbqbbsz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeoyycpi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvrvzozkn.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gporhiohu.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gqwznfars.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gjiqpjrkt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gkydniroc.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gsxcrxmhs.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtuyfuk.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxwwwxfnl.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/giivtpkfo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmolbjgen.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbkvtljt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgeznqrt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/giufpwwkj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gullqwpmv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gumyebifk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyhpmtuf.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/ghlvcmxaw.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glxhoofly.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gcbvszoah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjhhufek.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gcsxwaevk.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjvvftiq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktwetsua.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuujtjsg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvsvtpld.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcywijoc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqkjfnar.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgvrxnor.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gexdopksx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvrranrl.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxceqflj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmpxftadw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrjhfsyu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtesbwkfh.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/goovedrnr.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcnmviad.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxcltcnl.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gddrieutr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvtfutv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjoxqvao.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gebswuueo.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gxmgqvkxr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gsmyynhlq.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrripjuv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbgzqugb.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/glfbyepvs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpruoizbn.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdcppdxef.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gnzhqqhmp.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gtrjtohfy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyojrxzy.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcqvyhw.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfokmrlnm.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/glwlrpxut.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqwiihvt.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvtikgxxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrejbopm.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gnknicnbd.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutlnmbtd.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbzyiute.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gvqknztcb.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytypifbu.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gryuuvwtv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudyeccko.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/goaxcbkld.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjgdzsth.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlrzbxzq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gapcsmkau.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gymtrxgge.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqyjumljy.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/grcjofazg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamusllyu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbhllpfg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpwbmilei.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gfxvvqyzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjwhhowx.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkeqxgzuh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gblyetcgq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gczsklxdz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmrumnrf.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuncddlp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrphwcwf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfrpppfy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gheajncyp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gryvnwtog.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gyunujogd.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdojodxu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/grceerzir.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftqtptrd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufwwywci.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gimgxhhyc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbzciwvyv.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzqxzkag.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gysgwsdqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulclwymz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzopjyppp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggpjsbxc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqgkxhzm.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqccxaide.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gojryxxcb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdnpfxhj.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbgifryq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjewmmhel.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gndzjssod.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gucxzbqzi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjltuwnx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gycutrywq.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerwcqzvg.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gxzwlljbk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhuivpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdswdfufe.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gngmaldlp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtsyvxxq.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gxncpzwoq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grfhlxoiw.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpncqnaxp.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnxotrco.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gobhcpagm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdaxybsyl.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gceqmdvjh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gihktkcww.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gigelztzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdsbxcq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goohevokm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gdrvuvswx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxfpqhrw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gneejqeqe.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gynddjyaj.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gffhiacaq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gjoyoxcps.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmowhvfjs.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gebkggorf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gvenshaux.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gtxmojslo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwghmguqo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsrrewor.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gklyeavmv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gicevsabv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnncglthz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gkfmkjmsi.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxgnromdz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gutbrenxd.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsxgmkpie.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/guvwlvqbt.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gftidrgdd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqfgcmkm.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gcutxjcop.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvpjszxi.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/golntzpve.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjgfkldb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbphlqsy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcuozjug.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpkgeseu.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gaecwpkns.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpqdkdov.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/glzzeloni.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjoyvptt.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdskbgvo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvziwnq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpslcccqh.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxmbceetr.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gndpirylc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gazcbjjst.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzdmfjaz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjtfeglt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfzplfwq.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gcpvvieva.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gexjkmokw.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gecwjhgjq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/givtyeoox.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/glltdrhol.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlbjakjl.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkdbfjkb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvpetcmu.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpnvncnj.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gvkhzwyxf.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gqojnodas.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnqmkush.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzonvkup.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gktlllcpt.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gjnlzrgjl.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gekqiznao.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghtrputve.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gwotkyxrn.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmobtoix.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gilsvytpe.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmyzerofg.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjfgpswe.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtuytwfbg.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoxrtaax.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gsjfgctth.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpvuhref.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrpzrmiw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/glasegpjo.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpleoorbi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmhujzwui.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupeayggx.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gmgmmratf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmenilndu.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwbduido.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfgyajko.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gnyuikkfe.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmiguefz.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgwkgmvd.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsuusmy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtwpfily.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdfssde.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxpgdfmh.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gidyemluc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbzglrtc.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gndhhxcgu.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmntowed.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhmiwfsl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gregsnwpe.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxcgpmnk.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcrlccoep.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjgxmfaz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gswhffmug.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/guopmvzsh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbxxisis.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjqsjhbk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/geigzgmak.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/guochbkac.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhlnpkhn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glgotevac.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gllolkzpg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvlpgfcfm.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzatdkgy.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkahbigu.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/golbdsmhd.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkzlmoiqs.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygahvtgd.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gaocpaohx.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gwigjnpmo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gigbohkgs.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvceldz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogmtoekt.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/goxvnozhx.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/goqfczsrb.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gvzcdoeth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrokkcmh.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gniqpvrwx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehjhqev.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmpdbzur.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhaqfhuk.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/geufnljvi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gediwrghs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grbnfjkaz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgcopicy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gixtyhnte.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gobmkwcze.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjqkyuxz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmfiinbs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glcppweqx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghjudpuf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gevvovwpi.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotgmqzfo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhnufvza.sHtML


<!-- 参考信息 -->