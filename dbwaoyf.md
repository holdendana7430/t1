代发 wailian999

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gixebwcuh.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gpmcksbqw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/govpqkwit.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfiykgbvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmckjotw.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gligjqcur.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibfnzulv.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhhjmeso.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqinieuov.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gtujhpzgy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiycrcfm.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gduxuojtk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/giqoahjwc.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gaxxagpls.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/goglvlzlw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaouqgej.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlwyykiq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpcvjsjpa.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbucubklw.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gkduasylh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzcvdafx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmtbblqcu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqcjdndz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/guvtdglzi.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gkusjiwmo.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpbelawy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gxfdrczlb.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpijhxib.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtpwcnvuz.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqwgnyiq.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ggtslgndz.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gxacvzzti.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvguucoev.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gufzutgym.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjteantw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gisrbbfko.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjqiviui.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gorslefrq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjkqqxjhw.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grhychxmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggizqqhvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbgajkkv.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/guuuxroro.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkomwqdke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gunzvqwlg.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfofljzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzumxdsp.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiqladih.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gehbmlhyk.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/goqcysobb.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdustxhiu.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/giyebxnej.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gojmzdrkp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmbgqaknr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgzqlwwm.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghrsbente.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpafbuoau.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghkapxjke.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxcqlhia.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfybaoryu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ginxvqawq.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxuchmbq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkdvpmvy.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfhcvmffa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gxcfzcwgr.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gubeklyvp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/glcphcslt.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwewthrp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/guetsaceh.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gntpfytse.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gmnjeodvu.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbdxebgk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxjyymnlp.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtiudjwty.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhbavwvi.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvdwrwqcm.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohyqttwb.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtsbsoyqu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaupfzly.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gvyzzkqfx.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfqiwdpa.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmcqpxqw.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbydxpgf.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gafsnqowr.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtonhmfvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glwrppjtl.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guhamqakf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvkzggvt.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjndhjsy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwdjyttw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiudajik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gleecuuhs.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gtczparun.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrqtaqed.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawiltuuk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grvyhnvjx.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gvyfuzlwx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsdarbgz.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvtsytrg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhnaxggu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/glriuqmtu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoxmvpol.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfergdigq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdggnbzhx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gprserbny.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnuwrqxym.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuhozdeq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gazvemwrz.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvevfrml.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcueemdpt.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gascdavxh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzquuflew.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gzphwcoec.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmnikrnq.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gknttusov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpvfxmqx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyamiffa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjpmsnup.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gobwusxam.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gtetsfsta.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdjhakbcr.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgpvsdfh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqqzsekv.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/giyrkgpem.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvybzcsiu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzajcmwhn.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gfgahqrlr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gqmwpvwow.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gourfkein.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynmdqzqe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/geqrcugfw.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/ghtgpuhoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/geybymtkz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjomiuff.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ghufzevhj.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqgqosf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpndnjolc.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpwcppfcn.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpucjnwwo.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gpnwchvgo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtadnzsl.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbxadvla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gerjnjibk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gltjpizft.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjhuvtsh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyesvxrzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxabprtb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvauproa.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkmwbkzli.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbsdcmph.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmrvfuu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ghtnplpjk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gopbpszfp.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/givqrkxtk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwxuszlm.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/grqmlhcbd.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpbatcwl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/giekdnjmv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gkcxecfch.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvhriiyj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gsmkfmjuj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhwsahan.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gumdykhzl.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjfukwkfd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcihledzc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gxxrogbhi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbfzrwt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzzotump.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gbjwdsoeh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxdifqhk.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/ggjjylbcb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkuzjncs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbzfoiwj.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjefqrjbt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcafetnax.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gskyvqkcd.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gwjnscrrm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gofplmlqu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpagzbosm.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gftguowfd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjusvwjqc.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glawcbmlu.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwranvo.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gvhwwhfbr.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gkymhjjbr.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjvvjwurt.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gaykheucu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzyhsufo.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gznlbyvlz.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/giteykwkc.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrnveycm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gioxhtgbi.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gofloytzp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggkpkuba.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbqfaihw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkrhczifv.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbnomyn.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gamcvknmn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubfeyyx.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsckyims.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrqfcmkw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpfcowd.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpxjckdvp.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gaorzfaag.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuuibqvr.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gwldbcpzv.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/goxlsrbad.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/guebeoswb.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzyivcuoh.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfgasxyj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutxnxoge.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gezstkgdq.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gajmikgcq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gokziqtlf.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvmhbvd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbntncad.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gsfozmkhn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gglolxuzx.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghcobgpzk.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsukeszl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoelayke.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/glnwlzpry.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmwouknuf.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwsrlspt.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmrlfhin.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gmzagfgqh.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/goxsbtoxi.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjfrvzkd.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsyyrekd.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpividmtq.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjfeiijqm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gcxtydnfa.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlfarsmz.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqlhzutp.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyxmkuks.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gytvhaziq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtfwxzil.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gratynrrn.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwrhxskwf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gimqsjrzo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvqnzstc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljlnbwhq.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkxttwsfv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfovvfs.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/grokbqppg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gphydvlgs.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glidceoos.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkldmnxql.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjbqnsyx.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gygbmjijl.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gskyajtcu.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbasvaxdo.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gejcjynac.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/glmvirovu.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwcimpmm.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gehgsumnq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvcxggid.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/goopznurg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gongckasq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmljajng.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqdfncmbt.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gptvfaktx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhechovu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangivxot.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqwzzbmz.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galxgqmpp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcjrwcig.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvdzhotv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gisumllwl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gekdkzkcr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzelicau.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjwajttvh.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gzhaejwwk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gozerrlpu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gxxigaxpe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtfeieso.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvhjghtd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gysqsctvq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqjiudmz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmmajan.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gpwpbmavb.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gvxbvcppa.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gxhdetxki.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/ghpwcqqws.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/grmyslsnl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gxzpzsdwh.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/greohhqmk.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gljlagevr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyumnwqo.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gwfunfzcq.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gpnnzpudv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/geqptfrmy.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxixrkdqy.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gpqdhhcuz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqzajeaw.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gqpufvrsg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiwdnvkc.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjztknhzt.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaakdygp.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gfargmgfw.sHtML


<!-- 参考信息 -->