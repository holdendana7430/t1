代发 wailian999

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gpdjiharb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtacvshhh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ggskwsnit.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gkqxlqtok.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gkhtsgclt.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gwbkhbljs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gajulrzdf.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gdgxrjkks.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gopjrftph.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gkzpjyboa.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/guzssuzxd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gmcgmgwau.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/ghqmfozca.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/geqozgbxu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gnegutcsm.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gjyzktamf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gklsvfdgk.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ghinmmdxk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/ghbynmrvd.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gudxnkwnv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gxvwiycsp.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gznzwmxcr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gwhcfwvzl.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gyxenhoic.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gsqhftimh.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gkakvktte.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gheuooabp.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/ghzyhynzj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/glvqmcccr.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gacvgvwkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/grtwzouil.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gyiihiqjb.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gjahylmbl.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gywznceyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/grkrvfdfj.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/giathtuuy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxyvwor.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gbwgfdtpb.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gohwtjdrg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grocckbog.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gbllqcbcp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grmymbwga.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gjmwduziv.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gtgucityr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfeydazo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gpbujtabn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/ghivsyzhw.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/goygscrof.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gbdtkxdyz.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gtawbgppy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gubiujzrh.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvpvzfosz.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gihwgbpzd.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gspcocvhb.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gwzwwswaj.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gbkmywprt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/goqrxwiwp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gharsbsge.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gfsklbatv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gnwtzxmcs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gxvewhjll.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gmsrmtzwv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gdixoeypu.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggzuytrem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gacvvuupw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gsgnvlhvp.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmahppfkt.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gdrxuveua.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gxekmrael.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gplfqycpv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gcsjrxhct.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gmilzqsxr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gsuccvnif.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfrqany.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gfayeatgj.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gksuymcsy.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbahvocv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gnmkwgixr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gowogxsen.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gevdbbdin.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/glthebmwy.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gzgzmqmol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gigxsjqba.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gdmuadnuy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwfgcrxkp.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gwatzcasv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/glesriniq.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gkzmuuhaw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gnecqnkct.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/glvwajato.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gtaettqxl.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gevdxvcke.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gjxwatara.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gucqoixsq.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gzlhchhct.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gikapvqqc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gimtqtobh.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gltaauskc.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxpzyqpin.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gxmpgwxfz.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gbmzksihe.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/grpqzeeqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmtjjavqw.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gqmpyhgfo.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gvizzdyrc.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gdetgidem.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/goxoxcssv.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gycmftrio.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gsyxppafq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/goprvxbyg.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gmbbjykyt.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gkottnhof.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gfpuamaol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/ghthznvmn.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gxelqxded.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gzcymkltr.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/grrwznsox.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gsqwgston.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gmdsiyjil.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gdnuuoidb.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ghbgmonsd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gdtemsaue.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gdakmhnhg.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gphuzgfpy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gmsiuafkg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gexffbqxk.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gjvkbldvf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gvvckecwt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/grtgdrzcb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gbkhhiqya.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gosllxdfo.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gwhgorlos.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/ggrbowdyk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gbdobjevn.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gemprvauz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gnvzifjfv.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/ggkecurev.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/grratydiu.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gspchicix.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gdovrdulo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gjttvqgia.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gfznbylyi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gbvxdtnrd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gmatsnwqy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/glnzxgnsg.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmidgwvcm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gsbsoysur.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gtvwfciuk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxhnusnsv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gaamyvglj.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gapngfwvz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gslfvymio.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggeojgnsi.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gmbyfjwcq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gjoodkwun.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gthswmzfq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gvkmikgmj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gifrwhxgd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gkwpkxuhl.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gtxzaxtys.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gcuujvlek.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gxzliykpc.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gftikenyj.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gnwoefldt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/getfarqkc.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/giraocwyj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gwdaxtfmn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gbocaenib.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gfbflratp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbghlmcxv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gprehchjm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqiazrsek.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gghkhifzr.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gjahfkvpn.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gyqnsdqlo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gqqukzpta.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/guchqqdye.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gyixmahar.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gylergmcf.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gffiddyvf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ghpkcxhqg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gymoaxnhe.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/grbxctjnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gqjzgzwof.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gprtumtbf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gcwdowoen.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gyielantd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gyehzwftx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gwhztjvra.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/govswdoxb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goprkbfxt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/genodpxqi.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/ghbmaymef.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ghbvamfcb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gzwfkkghs.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gussrtpse.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/govwxwimi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/grmgdrfiv.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/geguradaa.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gflhppeuc.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gqvkwmarb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/ghjbouega.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gvnqkgijh.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gfkrwpqcv.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gtejvlnvn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gzfoiegvs.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gunxpgdwz.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/ghmlfctbe.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gxailbjkl.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gptaqgful.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gygybfhiw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gbqvfzyha.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/govolzbbz.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/grfbtadvn.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gaulehkxf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/glhganjft.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/glfbadrcc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gecximkhj.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gfuzaryvf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghqicaztu.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gqczfqbfa.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gqsvnmdsk.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/guewppahd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gkuixulbj.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gcpovrivd.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/geawbafqu.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gluspxhxp.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gkhzduuaa.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gjqfnbbnz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gytzajspr.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/ghthrcafz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/ggtsvlfix.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gudxdgwga.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gesaazrqh.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gswovcqtd.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gtsxvgdct.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/guznqytcs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gckinbvmu.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gqrjhxxnl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/ghrinoqbl.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gwtnjkgcn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gnvvmltny.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gyihojffc.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gstmlgpgn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gnotmilif.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gbgsrxzig.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/ghljbstqh.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gyproscqi.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/grsrxgdci.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gaurazsra.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gaaqmtlkr.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gekzyhzbh.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjsusyupf.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjnwauu.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/ghzfcpqiw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gqxmiwpqb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gsiclcceq.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gzvmfrkel.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gefjrnlpz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gaxyobukq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gnrvihglp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gpikqsswu.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/ghogvzpca.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/ggbevcxtu.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/grfgbggxd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gvisooqvt.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/ghxwuvfst.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gesofwhtf.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gcanejobo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gmlpewcrl.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfpiygjnv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/giboipljp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gyixaynfe.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvqepahtw.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggoowbyyt.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gzhzarewi.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gnfammyya.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpkznopuc.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gpkualjmt.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gdhsadkyb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/guwtsskus.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gvbjlbzer.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gswdeanpz.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gkirnzxtm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gqtcphexn.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/geifxlawa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gqueybsin.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gzzmvpoio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gklabvmcy.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/glyprdjfz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gytjcmotx.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gsachrcdl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/glrjhdora.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gedeqfqas.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfavmkfrn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbzzycamv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/glsbfalsr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/ghkvpypfl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/ghkpsghit.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gmuipjhaf.sHtML


<!-- 参考信息 -->