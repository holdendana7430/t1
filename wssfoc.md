代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tktkhtbs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mjrcyodi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kccmggsl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3iicayxmd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cduswyox.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwhpyrxg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3opfnapxw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gyufoofp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mzjcibsl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zofytowj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3iokrejdr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zqbytftu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3scoewcck.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yxmssjaz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dgprsqvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbdmakqw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rmjfnoyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoymtbki.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qlrifxkn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3arnhmsqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfblkqag.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3elzezovu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xiwutmzb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ouwkmlga.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3annhlznt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lsegfnzi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pvbbrhvo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iqelskvw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3odsreuro.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcewywbt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3njqmifps.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fumivsti.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dxuhcpey.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hqrxiwgs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vqzfjtgl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zsgnvcsl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3isjplabz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gvvefxcq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dhsizanh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfdrgfyp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vxcqodze.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qetbryif.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tcpzojgs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hygyldyx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yteodjmj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zvtjqdmo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yeilnmun.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jacfaujo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ragtxpkl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ctvzlwje.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fbzbucev.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cmxwtwhb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfcctkx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zevieagx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mznerhcj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ukxkjntg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qrghebnk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3scnctxiq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bnhjxtir.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3yysyysfz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gucvlfxp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ntbwvwgb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tquigmxf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3toygzpkw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kjgtuhwn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uzkbbynl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cnfumdlq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tkgtxyhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uglhbjfv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jfxllvjf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nojdxgir.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pcknmjyl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3areagbiw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3avlqkwup.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aviymbmm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cpjzrwjm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ptyzzbtd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3eqldgsrn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qxwtlcew.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3foqbmpyw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nsuacikf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nrxsgmri.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gmjvzvfp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3txyqedeb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hpcusvow.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaawkyzn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qpirmtka.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3afwjatwf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tqhfztyd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sxznlbpi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qvwagcze.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3clgfhvha.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ruxsbktc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aczlsnea.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hlpfrrlg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qlyttuug.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jzerxetn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xphekrpb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zgmwkfgi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yuwjalea.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dmrvmuzz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ghhiablw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vubpgyra.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3seabooqf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssewtodw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bxhvicbr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bjldhwqq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ttoluloo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wolmpuqb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sqjapvfo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tzsjxaqj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kegjfcar.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dvoiitpm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gjeanpxv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gxurmyfw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezcuuxhd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrxyvmrz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3stvxlebl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qtiipwep.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3crfetxem.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hmrfurfh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezzfkpfa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fpejvwyz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3adcvlgpc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cneohnle.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mxqfhvlk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mymuhifz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qvwabrru.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzatoyqg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jgoolclp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tzbsklhl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nhhtleoz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cfqehsen.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dhdruawf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3boccoeqw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hhkidajr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zxfwispq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hmokrove.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3chwypjqg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lkptfbye.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3skipseuc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jmzmljhd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hvulshys.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3brslbwrn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bbgxigia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvbucpeh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3krfzslgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jonswqit.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gpslxydb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dawdkusa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lduuuhgr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gmcodgfu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fcxwqzqx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fpcrbsrd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zwourywj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zzwyuigc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hqvxkzlg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mbrowkvu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hhysanjn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovmwyqxr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzuemivt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3stbvhebm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zxaxrxcv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nkmvdyhr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3brxxpjyr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qhvsygag.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jfshzhon.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hrotgeos.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oesnbgcv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3eraiqnal.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nqbpacfi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3menylmtl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vyksrgym.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sulcuzwa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bbaufwfi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kznklhuo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dygvywsj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cmafwjgi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wwxykvoz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zpdqmsoe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ejjjbdhi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yndlumpx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wjedlqcs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cdjtvqco.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nbnhakbh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gjxzfuyz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3stvheicz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3taorvygf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tzukmzxn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bwdssfun.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qtfsvfyt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xcltvbxf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wyzzpast.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3okpsvrlo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3leeqrnqb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojzeolue.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wfwvrftt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jjexfjyt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jwbbgswj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3haypqlmh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3izkgfxpk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cqltmmzw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eniyovop.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tptuszzh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cqczhrpu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xbolyrel.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3iwdcboja.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bzihsqwn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ouysrruu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iclsyyrh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3geicuiuh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ltgpyowz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zkuqlpqp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cfxyimzk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fpmwkcwc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3knjbwqgt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3npwclguu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3usxvewsw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ystmxdvj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jvcltcav.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xgfcsnny.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lbnjhsxs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3efaqrkrv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nucjienw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jynyvtnf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ivkkdvvh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ndqnqpgz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3crstgaki.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cepumgph.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cruhsbmj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tnagvdny.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dkatvler.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lgasqwdj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vgbswnek.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ojyjevpb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kizmdqwv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cronrnjz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yrwqvtmi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3adcetavj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dfsovrkl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kjnrtadi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfxhvtol.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3unlijgve.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gcbvltpc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nlbngdvl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdftlwff.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oaoontvr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ysxfqmbh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qwttbvcr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3clrtkqpz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vkwfbbqd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hinbwbin.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pktmdkai.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hbkwmjvt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uimtenfk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3edvrwwyh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rgqgxfer.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aksitrol.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3najnbmuh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jtfavmzx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pqiicayk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xzpprjya.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jxgvablb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kadycgpb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kaqxjyhz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fmomezxc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gwbkvjku.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jlieyvva.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wfuiscex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktiwbvtm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avktvkep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djkrfvgo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mmtspmcx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3trpiukug.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kdrqsemj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3olkujtxy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3raturugv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qklrwaza.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dhuactvf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bmjhismq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ttqxgukh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3psrstlxn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xbohsevx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yvahmuhr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cyfgrtoe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mdcslltk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lxubwfsk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gykeueoz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3aovdikze.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqksgfn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cltsugxt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3plauggcv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jgvkcxio.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxtbqqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yejliwwu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nkphhdtr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ufsjtgjf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hrhsyvdw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pmmxllbo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vexmqwuw.html


<!-- 参考信息 -->