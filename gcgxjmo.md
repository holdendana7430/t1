代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gcgndfbbb.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxnvjkqtp.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghcyhzavt.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnuuhfix.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwprnnbgl.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaftsmet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnilasfuz.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gbuowocje.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gvkhyokse.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gtrdkiwit.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/geoihpijq.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbskcumu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gbofvykty.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gmtnrzupq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfxjdkek.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjadajwdu.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gwxizpuyb.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gndqfkqdn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkenioyna.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyetmyeac.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/glrasyqko.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqoovlrk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gskpoanbj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsulxlij.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/glxmakmrq.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gqmiaumve.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbvfhybgq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsbqabsm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdugsptmg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gghhqvcfw.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlmmpakp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtsahhdjb.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnmqtma.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaufhnft.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcbgjtsa.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/giqhdjmgn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gexykrhqk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gxingtdqj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/glgtkodkd.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcclctpz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjplfgqne.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/grlnhguls.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gtayyazgy.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvvxkits.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgdazama.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwwnkvqvl.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/grvhijgdu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/geexipjvh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/giqsournn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtjwlueg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/grmyczdsb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeqqwtgj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvdqgzbzl.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gazsbsjip.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gewdwtucr.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyorkumcd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdfomadi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzdbvnew.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gzvddyccb.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guisxpakr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoymzmzl.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gsngpgxkr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwnzjrqg.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gynkzuxnd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/galxrszlf.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmivmcvvk.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdbkdqfg.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwxclqin.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgdyckqy.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwoakhgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkodhvys.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giybbdpxc.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gtntsibtw.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttajqzwy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gargmijis.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqnpstqxw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyukwlvql.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gaynrobvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gdpubqgge.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyllqafw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gufikuqkf.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/guaglsjqc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gweatnyhh.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/ghkkvwbqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gdkmnurxq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadfupjjb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmstthwzm.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaeihflo.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkgnehdt.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqwpzzmr.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gcbboneis.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxkqjldn.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubjpnzcq.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsceglqpb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxnqvmbg.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gnmauzwof.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/goghjjncr.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbskcwuhv.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsdhvpfo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpctapqih.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/giipnkssn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpznwpxut.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glprnxzdx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/ghpdjurio.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryiqgfja.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gatypferh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/guosblvcr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrofdco.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gdddaiwgf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqcgiykb.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gstuilbkp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsmvlpcn.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqhikglg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvslshbbh.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezylivfx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gaijylvex.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwldacdm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gxltlbnbg.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gidwgsewi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccpeqajh.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgtvtbxk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gshyiozij.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdgynquqv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gaynfnuyp.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gubyksgox.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gacvbogfi.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gvebimsss.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvejyjdi.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnlnomzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkjusye.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjdgtpzl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grvcmmami.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdvseyu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsgutvuo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqzybvph.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gsjbfcctw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpwijrdq.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggrgtvtet.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gecxmmrhn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbsofnig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqqeranf.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcflzfgaq.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gjqydhzmk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gresdwscy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvtllyvu.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgeacsce.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtccyupw.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbafzoge.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/galbtdqss.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/geggjfpqj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtnkqgmu.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gtxppisaq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtccimjrb.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gmkcqfnbp.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdplvrfwl.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/grycudalo.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnihrhn.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/grqqedxcz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/grpmreiqn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geiqokflo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gymayxpap.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gebhwwhwz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gxlmajugw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpitzjdr.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzwtphsy.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gyezcuwtf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsxcdmlc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gubtezdwj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjhfkkho.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbceauqu.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/getizgfsi.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmbpuvqc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaxzezma.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwsktjgy.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/grnbdiwov.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxqomsnt.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gtwaiofng.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxloefkk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqemgsxm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvnyclgj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsxjmanbs.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqznbbeu.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjceajj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gbnssoofu.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/ghkgplecn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbrzscjv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/ggxesxoji.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnxpprda.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/guveymtyd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gygrggroj.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrylkjvs.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnqhlwt.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gecpxqmbc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyzhgrje.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqgnkonnu.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwdxnibma.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdimiebyt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcdyfkgf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpnhlcka.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/geaucxnop.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gpvrwprcw.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcayemjxx.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gkpeaflwu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/giopvwltf.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gaiqbzubb.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpucfnawt.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gklmkzjue.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfokrhrs.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpnntuazo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gmfnjbmay.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/grxiqwxyf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlbdhydq.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbogppwyg.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpunkmrw.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gepgfdpdc.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gszcpzegg.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gztdhylde.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsrhhios.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grnaldayu.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/ggswkwgcm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkedhaqt.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipxvnvtg.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzghqhse.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykspwthq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwpqlkyq.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzyijrnv.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galazlzzg.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gpgwhkivx.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzehwfpsc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzlomhta.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaodqvsl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzyyetvx.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgebftam.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnoieemy.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhkmpvxx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihqqpmvl.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gfajutydy.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gnlxxttxq.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnuafwfk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapgdixhe.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/goysvszeh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhbhnakx.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gtdxknpyk.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gfeaygbje.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbxtkgjkv.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfndgdbik.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzuftfrc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxloxhbd.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxktjba.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gtjuwyuxk.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/glerctroq.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcmhgpkrg.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grgguckob.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghztskhty.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gczoprjao.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gapufqfsr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gskjujisj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxruyrozg.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjajcskjg.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gfacnxpwk.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfifniyss.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxduvrlwd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmgudcdkt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gapowruox.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvvrejdhc.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnkmmysw.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gngtksftp.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbwjsccmd.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gaiaknxqq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzjcykzf.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gdipqlmim.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/grdkjcbth.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghubvxotx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gawbxpvqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzbypmjh.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrlrzuh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwloqogf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpopsihuy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvgmgjr.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/goydamyga.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxazxpurw.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbsnyucg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gonzhwiir.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gfyasbliz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gccqphlcn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcgfzhue.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnojoaiux.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcefdzmfg.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/glkjwdhrk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gclwixlyi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkddehekb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geujrpsqa.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gzahbblzr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaikrpzs.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gwqhbsmny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/grxnawjgq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvgtevqg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmgvezky.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/ggxbjfwsg.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtupzghvw.sHtML


<!-- 参考信息 -->