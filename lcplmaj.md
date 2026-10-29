代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/ggazwlomo.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/goqolhqhu.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gawqrkbuh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gcfwgeuaj.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gsnrsrqya.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gvjrjzcos.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/glkpxdihy.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gitjprvex.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gtnziufdu.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gtacswzzf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/glntvlmgb.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/glkixuysc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gejwisxde.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gzsocqzvq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gjaiswxch.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gypydrizu.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gfszpkswm.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/ghfqmjjnt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gwgluvkon.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gnwibsqwp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gwrityglw.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gorneqehc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gabnikdnd.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gfetnxfwj.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gwvldaexq.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gjylwbjzv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gtstgneag.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gvkevdcqq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gcspcuwgu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gkuxrdhru.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gzgccykgq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkvhmhtxe.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gnhykjqba.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzjozdrnm.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqkavrero.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gmnjmcekz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjwqohpcp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gcasjmnbq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gefujnvho.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gqvxxolaa.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gjymmsutt.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gnfpklhmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/grizewthy.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gqitujidt.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/geykowosr.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gbxjeftih.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gbcolwelo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gbqtzcuqi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/ggnsmiuxp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gsqjshqcg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gaxgfiowf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gekcwwbcf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/glfiyspbg.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gzrbponge.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ghjwaizej.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/guaonyyyq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gufujyvsb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gdnabimjg.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/guikfzkqb.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gfenydqyo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gfxobvqvp.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gehnmwapu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/grbbjuooh.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gkysezpco.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gdstrbzct.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gawcskghw.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gtvocmtip.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gwqzozsbn.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gffemwuwm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnehavwiy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/ghygzpnas.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ghrvchxde.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gsvgejofl.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/ghfdrnxnx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtzucugef.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvshniy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gocdkutxh.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gcpvpsady.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gklgodtee.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gxtxygeyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gymkgqkyw.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gvwtrztmi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gliguzflh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gckmvlcvc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gpmqyrewz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gbxhtihji.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gsjcdtkyi.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gnryjrlmg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gunjgurth.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gbwxjnahj.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gohqlyvlg.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gktddvufm.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gnbyrfukx.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gsggmfnnd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/glrpgzhjx.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gxiwiwjfm.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/guhgwgifo.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gordtgsbz.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gwbuguryx.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdjolcjml.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/ghtxxelil.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gzabudfxs.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gmnpjvypx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gqmgfirjc.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gwgnuuecy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gyysujazq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbpisgg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gbjxizgyb.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/ggqlhaptf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/grlehzwwn.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gjoowbrtf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/goodzouwf.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gncqxlwas.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grklgayop.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gigoiiwvy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gkfojpdmm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gmfdmfffd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gyxnajirq.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/geldmufyr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gedzxkdes.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gbqsyjlef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gaqkwinmz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/glfigljip.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gznygkpom.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gznnvpoqp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/glmnvlryn.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/glnsbnymw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gctndkhtl.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/glnnmfvwl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/glsmqlzxb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/golausihh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/giktsgovv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/glxqrpevo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/ggblwpidk.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grvctrpkl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gadkjqwwv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gdgwejeqe.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gmlvjtcya.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gtqpzxgtx.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gugdkxtyq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmrtixkrx.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gpiukcjay.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gmoclimtx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/ghljbrqlw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gcfxyvxry.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gvquljgao.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ggwhcwmix.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gvfgcdgsj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gcwoohzmt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gghkaxcpx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzjxmuty.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gsnbntrss.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/ghflzxgty.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gyhmqieit.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gssekqfck.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gdbvoarna.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gsapzigll.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gacfdpyem.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gmsiacpbi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/ghonfqdls.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcxaygyyc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsdqdihmj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gbsywkzzm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjccwhzeg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gkndljhrz.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gkreqsaag.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxhamocxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gtcqptpoe.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gmxjaguxk.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gjnjuemyt.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/geromivre.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gqcvsqqnz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gidlxxcby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gbxnztxgg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gnioujsdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggpneeewa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmjsigxlh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gagwiprsa.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/grvrusvau.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gxoduvfnm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/guzmjiuqz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gfldzrctd.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gruysspsf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gciukezzt.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gzzjstzvk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gktpikczm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gjdbxyxja.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqvwzcryq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gzskhudme.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/ghcuxiixb.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/glascmbkt.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghlkqqqxg.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gifxwqqor.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gbqctkmqb.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gbwhldklp.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/grbbypetv.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gaclpswmc.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/genbqusdq.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gqidvuzft.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gjyvxoami.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gwsyxhusq.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/giqhbpkmv.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gktbgzmhy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gnycaspam.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gmydomrzf.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/grvfwahvp.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gmumuflgw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gztyquaml.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gyroxiwbp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gsbkycifh.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gwmcqzjwk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gbqkdkspz.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gkweexqti.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gudggqark.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gruormcvu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gehpseuju.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gyrwgfxui.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gypkfglgj.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gflbsordc.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gaqtvktvq.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gnzvwmpkw.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gwdmabdjx.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gmgmkbkqx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gnfecmcuw.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gylpswrij.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzqehepnj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gakryepel.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gnrktpoii.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gjmhuodrx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gyjhmsbdi.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gmuoeftnc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gxkngavua.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gzpdnapbq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gjxhfssod.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gaponceam.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gajuvhkzk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gbqonuzsi.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gsyjvwvql.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gtuemsydx.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gqpgmmjqb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gcpjawbkr.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gxdbgdssz.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gdazbvbqp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/guzvaoeuj.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvxkwmgvv.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/ggsqztrnj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gyswbowxa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gnmdzpevj.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gjkzqsoko.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gtiauvlhu.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gprofundd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/ghuschuyo.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/godytubdl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gbatfvxew.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/ghdffyhox.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/glmewlvyu.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gkjlcslba.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gjjodhmht.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gqrovjrbo.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gvlrzczsd.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gbltkyvjs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaoixewpp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqcdbveyr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gdehfdsmn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/glbknxrcg.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvqaojzlj.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gsbpbhovn.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gfprezvng.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gyfuvgvui.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ghknjwkwe.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gapqqgnzo.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gnesczisr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gshbaalam.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjqczrnpu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gqvzzpdyr.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gzspcnvtt.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gzwrlfujs.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gksgpkpnm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/ghjdedeew.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gcjfechrp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gesmjvoub.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gzshzcglk.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gjnalbzsk.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/geltxkbah.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gmilglktx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guqiwmmus.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/giqgubdpe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbudtzhmf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/ghfaaxcug.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gqhloaltx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gixlvunnm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gwdwcopey.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/grxguqkhn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gsesuzwhx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/ggzgtdnub.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gfyowawuf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gwvkmmkms.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gbesyeroq.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gcjwzfnxa.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/ggcnfmbqj.sHtML


<!-- 参考信息 -->