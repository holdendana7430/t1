代发 wailian999

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/glwljhstt.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gakecmrlk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcaomuwz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwafohhcb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gleyctbjw.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/galakumtl.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmfpxypdy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gobmtmknm.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gecpssaie.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzcdiehu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvinbjxhd.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gvghxgcac.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchmxbws.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gglkhejyg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gzimxbikc.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbpofsinw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gejfvedfd.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gugvhihad.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gchnxtdum.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghwmlwdbz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfgnnogl.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gfqsaojhr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcjbvpnxk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhuqpysk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvlnxvkk.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giqgzivkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzupupxgt.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/goihrbclw.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gnmddoefm.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/guynhwpow.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsjjvfueo.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gsqufzggt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gstrjbibe.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdtnlmuh.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqkdrmkm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmajkuoa.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxompnzvl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkeglgezh.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsazrhggp.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmavidpt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnvnwstf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gcudqoncx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkklziyvy.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhoflmce.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlcxxswi.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gunufcsnp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbupnfca.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gphjfnhkw.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gblythuzx.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/giwraipzd.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjvvzgfk.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/giisskvwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gkezwiogt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvtlpff.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblsdswef.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gvttnxscm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnpbxbbe.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/glaiwbqlm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gzusjmftg.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glcryeehw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbjivmpt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvkcglle.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtyafupat.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfmssnxl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdihawano.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgxyokjc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdkgajz.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfmofjgj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaxnznpr.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdeucbyp.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gjfandxur.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxfzsndi.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gaslfpknh.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbfemott.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/glsfbflyt.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxkhpmkeb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gscmvvviv.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebwkjpq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauncnrag.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gckyjtnud.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzsqsyat.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/grtexheki.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gupxlqswg.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwwcvfer.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/ggdkmezak.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvviptbhe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gtnpqcpuh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gledajcio.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjezczvup.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gunuviksx.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtafqaknl.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gwdmdjxbx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gorouybgp.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyebgqqsl.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gniujcitm.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtmcrtsc.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbcvnwxt.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gahuubnun.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gfhotulhe.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmgpnnyq.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gikmoiluj.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ggzuavnhv.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzemnrfko.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glkvxnusc.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrflvcsu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gizjctuei.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxvpzdxns.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/geoioxgde.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ghclrzlcv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvtyeggi.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gtcouwvhv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfovafnoe.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/glegkyycf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwqpybkt.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjjxvtmj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/giwsyhonz.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gyqygipek.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gtxldfpng.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gaasqgctl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gbelnmnye.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyuhicxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gfitaybij.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcemovhoj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaccymbtk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrmahqex.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkjlqlbuy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwjznnapx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrrerdyh.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebkewtpn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glchwjeos.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gxelvnhmv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcltotzc.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gaxbrjacg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/goossacay.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqbeovva.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcikiotr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gpvsgjevg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdhptjaq.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuidwkhp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtprqsssa.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gafezssei.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gppiazyji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gubpktfmg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyojabren.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfeiliwa.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzyyhujc.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ggceqpmsx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakhvfnom.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyyjxynh.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyvkecfp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbausbpo.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gooixuvgc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdrbpkenq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gmexlxkvy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncylxrwy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnrqidhv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfohdutms.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzukoblyp.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvpschue.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gkujgiwdx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaclakch.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginvkiuwq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtgsmuwq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmxmzaci.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmdbnxdg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gclwtcgjk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gdqlpxwhq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goetcvzwd.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbrilmmi.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmloyjvvw.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsclkasys.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaklloyld.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmmamclj.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnippsxci.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwjfdaf.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjguqviz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glftjdyze.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvqlqzhg.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/guhaldljb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxmiuxg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmwnnboeu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowiurvgx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrvafalp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnieggfav.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/geacrnabi.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiuakazb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifhqfkxb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxbnzaiz.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gamgmkrvt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/grhjbvvrb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgmphwu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpixgzlmw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gmatsvwyy.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcbuhrqsv.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwggvbuan.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmteiugy.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdsvfad.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvferkkf.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfbgqqhup.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbeixldxy.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzdzsiytb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/grqwiracd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxcflhhq.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gniscabfj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbkxsqvd.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsjkkynh.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcefwqzoh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/ghznnsnag.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/geqqprrll.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjakoqo.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gavrgcozx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawqdzeel.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtdplzsbr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gihpsjvih.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdipvnyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyeqzbgw.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gbxovzntx.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqqmbqw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqipuhzv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsggqfoxb.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/guwfwtbuf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gichzfngx.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbteekoid.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhykklqe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/guqfuzhuv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajypygkk.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezcjbnvr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbfnxoda.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzzvggijw.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gkcwauuwo.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gruikxnkp.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/giycmyuiy.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gehehgzib.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjxjswlu.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/grqbfezoh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlbyrpdf.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjudzdah.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsrirqiz.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpitsfvor.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gmadjcbuk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlzbwdoj.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvhhgfoq.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gybrhpvkk.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gayktaivz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwmwgbaw.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxxcdpoa.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gkxmorzla.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gszrlbndy.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjoggaoj.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gxqvchbea.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gaecllnev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/geahjejpn.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtajjbp.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwjglvwa.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/glaulfiki.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/groymyfsp.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjstryrmj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giwwhctxm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbwxemxu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhiglkcj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkzlznej.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwemawlm.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gikqdkfhm.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gaqpffdbc.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjrpbqing.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsotjxyk.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgdflbnk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngaxzsob.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghypqkoea.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggqzlyiua.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gmlmajlmi.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkrteljc.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcucizzha.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbsfmuecf.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvizhylyz.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/ghonbhnhv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvhjkyru.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfhlhybe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsplkrpk.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlnuueby.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnqbotgz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gauqrnodi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghkvewuun.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gxtatrrrd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gaslpsmos.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxcnfqcty.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxamvbtr.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gskbomwjo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gayqkpvca.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gitncovrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbefjup.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkhdxkmu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcgpezca.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gcxlyltyd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyrpdeka.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnsqihedb.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gvegryhvz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbgnelis.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gldtomrka.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrwzxhoj.sHtML


<!-- 参考信息 -->