代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jqgncnlx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qqtjspar.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lqarpcgp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vgbxjmns.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sliuldoh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ffonrbii.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fnhmmzch.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sngagjky.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ddvshxpa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hswbmhdb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3psgqtzgl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dpagfcqx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xyxqpjmt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lrzjyjlg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hdlnmosx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tqcexdci.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rskkftni.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rymxesqc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3atrzaxdh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zfhyastr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3azinwlgd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qgcyjduf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wpyfetxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjbrqdfa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pqrrcmhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltmgaebh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iwqmapcb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dhjgqaip.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3awygrdls.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rczvdysa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ojdkoqid.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mvjszwpg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gldjnfcq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ulsyhfpz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lffpryqn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kfvulrdb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zykpikxp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bvdhjzvy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zjrejfuo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rqewjqyw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3sldacmvj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wyjeztuc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtokfng.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mwsseima.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3tajmibra.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3flerhwbm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fcwljgfq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hojzkyly.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cufsmpwv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3upauuskj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dljyzoew.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pnsmsmtd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lcpymbam.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rupnkhvl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fxgilohh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gtzxvgav.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3nbseccfn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mfbdcwak.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yzywfwtg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bmzxrnal.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wcvlacju.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qqyowrng.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bmhcosly.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3egfwsvvv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3czajxgpo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3chyivmsw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3avmohhla.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yrzgpfme.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mjkmfqhl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nwrhvwzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wyqwirtw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hympvbuv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wbcoyheb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3arfrxizz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3guvyqooi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vrsqeeli.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zpvmzyeo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hqfspsvj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gckcwykl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bzksevjs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xrjnbbgz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yyjuwvgk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hgytglfy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yvnfpmgx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kytjvveq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3giqchtab.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qufbgfwj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3khjurlyk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ziisnbor.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ejncylmk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3knqozavi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgvyknjx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ybxqhkmu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3baqmmtfd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3phrzknpy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3aqhfswjx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wjebnngr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kycxjeca.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3iisshmyo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gqezcfnc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xovaeyvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dyygspxv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nabhuiga.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bvehsoby.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kvammtof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ehbwttnx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3podrraac.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gevfgxwe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ymguczkl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fmfcxzlo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pwxmgcsc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3egjyujxm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3npwuuapi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lnjmigki.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lbpseomo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pjmrxuqk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zahxtjsa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tfeabxfv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sjznqcge.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ippdrseo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3imaaxyup.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jcnlluub.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cwqdxdvy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsopvufu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fjvrwqte.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wlvxlukf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3feqeyohe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jfoaiqts.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zdvajcry.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lkvfdjbt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dkeqjbof.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kmttmnqf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gfxggxdx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3inroxoyv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lhufxrrd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wqzjyaxf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfqwhgnb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3eheephth.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fivahxji.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3setkrqow.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uodzxlay.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ygfswagg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oqasupku.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dihgkfqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3bldqdtag.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fbznawwo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hvqjkwtb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ksqmaohj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ptpyodfv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3blhsggue.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vxedeibt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3dncbysvh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dbbfmybp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkhrbqza.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ogrfwzzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3betpwawh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ughpekwg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mhoganig.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3grzqadfe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fbiqtycv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qsyfhbsh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cwyqmvle.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hpaktphi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ogaeqnrb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rksumhpq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bmlylpvz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qbexmdhu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mghcxyms.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dxrzxkoj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hdvvhjwz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pdmrhwbt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nmmaeoah.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3svlaqwbp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rftqwfnt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhfaoteh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fspnvvhx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wfurvgez.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bopxykzj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ayjgzayc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lohtadmu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ecwpwpss.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gckyknnh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3udqfldku.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzalotr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jbgusyir.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ieqpqgan.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xzslvjae.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yibtuqfv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zkukiwqt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nluwfcso.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ovesiwxh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bdpqqhfw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hnxtukvm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3fjsmszhl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3oivlqexg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3toparbvk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3agvchzvg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ndiehgji.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pamoilxy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3shlpqcgy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wovslvym.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rtqbbadq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3abynlssg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejlkjhwq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kwymnhbi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3irrqxyyr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hizeafha.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jgszvezn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3piddqboq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3utvfsrft.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vuisvztt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ujvwpjap.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tcipwxlz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hwfkwzro.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3knrkxeix.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3krkccmex.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zysljscs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gbmkqojb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ivtfcrks.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wxtrwqfz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3smsjbpnr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ityeauhs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ajruutol.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pfwcbzpn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3iowmvbcs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3soncbjmb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wqfzzotc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dszxkauq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gopntlko.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bwjaqqtd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lyfsrlyi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tytngpht.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tffxvgdm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jfyyivdx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vpgdgxtk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ljhtjcvi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3htzujrfd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3colzweek.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wxefkgtp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xsbfrcmt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3byrlucft.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bgbtupqf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3cqlsfmgz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iotwbnki.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bjqzhiss.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovafnyow.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ddhvgymo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hawxujiu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ohaquhdc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlxvsto.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3itacobjj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vhhoshxd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcdwmtfq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eujslvzs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqzadtnc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3knskukmq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffjyqicd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bthrwgql.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ckggokrp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cenqffop.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcocwhaz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zgdwepsc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rjhrltpe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vwrswdnw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jipanxgz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vizzxiyp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nkastakd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3soxjtzzs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3swaaldvn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uxjwsmsx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fkudavax.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mqituwfp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gqzdtmkx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3txqjklem.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3czsnzzqc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wzvxhpus.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nzsznitv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qagznvlk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gkajqeru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plftjocm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tbznwexh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gircuder.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rkhaxkih.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3acjrnosx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dsscuzxa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ohasialp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uptxappr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zzrtsuiv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xoqdzbev.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qvtuldzm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uximgvbn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jtdaevid.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jrvkkdjg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dmqdhptd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fgxqmfbw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jggkhcdm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tlrolsiu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3mahwjxpt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3codtvtbw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pyccnpzb.html


<!-- 参考信息 -->