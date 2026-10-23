代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jlmojqot.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3voatrqhq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xdeedifn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ivdghfec.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3wthfotff.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mnzbsmel.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3snorkwvm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ycdsulhm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qnjckogw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3abkqqdch.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wwtktuwu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uyosqhuo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lcttxuks.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ctulfher.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qudbfymb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3sdcvgdvj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wvhzyxpn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3faqohssi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rywuxgel.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gaxcsrio.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hzjuwuuf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fszrxrek.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uwbgvfzc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qyvabnsx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3iruicums.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3busxyvzn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xiqgabro.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3blewoqwl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xlsbigtv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qbkzmpec.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zdrhotqi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3roesrzxg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3svhfpfng.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3spjjwfot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pcwkhaxo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mjotniza.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3miebxdjv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jfipwvnt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yrqnudgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlunggrh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iavhsdmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huehhvch.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egmedztw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3oefygkqa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzbtcswz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3boatkfmv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dluizhsx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mvqnupdi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3omaknhbg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3csrzxgzr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjoayq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tauorfey.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iynhffgh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cmoxupng.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hixuwyoa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3twweaqak.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ezhlgfxm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hpfmrqaq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vigyawhq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cfkshwqg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xgrotare.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ohyagyjd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qsompbug.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uitxopeu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3reqzwswc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jbsjcswp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pahdtkvl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wsmxjmvs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ijqdxezi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3oaclptee.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uqbhjwpq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dlklmbjc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fbwfiibr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tmndbxvf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ajiswpko.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rilyfwvn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqqicqf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ypdtqlec.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3umkbrcgs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gscavfzy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tjqilomi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lonhlnvm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mkvokhqt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mexiucak.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ufxujruc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vaewrxmv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3uydoosax.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rsrmovqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rbhwnysp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3djwuurhl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xhkfepnc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kyfujxxb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ynjpjxyi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3crsiaifr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rqrovrmk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kmsgwuxd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sxqrqykb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bbzfgfxo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jjxrwfqk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvardvln.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mntlqyxl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oynymwio.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uwwrtzak.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3amawghfl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eciurayq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bcaunxlf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vzljwncr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exkbhkbx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fmooivca.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjnatjeb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wyznqmuz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3celjubfl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kemfljvx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tslxufcy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3juxijtrf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3otgoztne.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xdbjccys.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lkfpcwmo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jvhacwhu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmaipay.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tvcnlblt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywleirao.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dxwpynzd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rmalowsr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sshnnxww.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nnwsvpwe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3uyhhyaws.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tcpubddx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3akidxveq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qpwrkleh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3worlhauf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ltdjbzwn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qsiwxuqz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lvobxxhe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3axeejgnd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjsbiqln.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ywjebgse.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rymoeyzg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kiwlijql.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzxojyqf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kahpgupc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlrappeg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqmpeoqr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vknugukn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzblqqv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3izlatmfm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yhxjvxwu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3frehowmm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lcvieoiz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zlczepoc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3afuhjqzn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3eyaflsid.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mvwxospl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kfngcbaa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ohkmuhcp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wdvjdfad.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3patemory.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3meyxdwew.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vvlmjkdb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xrdxjjxq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xftwwxxo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lusjcnxy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dempvnne.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hdnhezkf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nljogqmb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bscdydjj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gsyvkyfb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bzvqywkl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nmvpmssn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnkvgumu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jtdxjcdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwcbntts.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nhzndetm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oywxueec.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xayehmvz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vpxdjkau.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ulmqqkqm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gnalmmbd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3etwvfiaq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3awvmdfkb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3oqeyexmf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3agdlefia.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uccszgaq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3trndbzic.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3erbxrfzj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wcvzxzjt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kztkhmcg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3utjqmizg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qtkjujws.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kjaweonb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jskbvjua.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sanijyas.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yllstcws.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zrvhexes.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uvljdmny.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3giggarbv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3utaioori.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohwucboh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iayvtnwn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvnzvkf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wyishmlr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vftmvzfi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qxoplign.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qbamkjan.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3betfxunl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pkgxaoiq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eydmtrky.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3skwndvjr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gubwklth.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3iigdnxwm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lyqvahpf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bhgnyznr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jbmvxlmt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3goprjqlt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3akybxhxs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3edzduywb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vdvadyor.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lwzzhcvy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqkiobhd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3edrjpuaa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hkdkwzmw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqvjlbw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cyktqqgl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wfvvavsw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ziszzhgx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bdphwrfh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ttwutmqf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kodmvmjr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ttmtkpje.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ukpwkpdo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jsfsuzdj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jbmhwdps.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fhmryeap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3scdsgart.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bzccwmbj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ltjjlpef.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ucjhlxvq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dwybtgsg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wshdawgr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rdcsjdro.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dydlopas.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xligswsm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qxuoundn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zrpbprtp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aajniqhq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3otjaivcw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3owiltmgu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vkrrenxk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ydnncinj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gtsbigfw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lhbhawhs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gvlqzobu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3koerailq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3awwvypxm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nmiyrcax.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3muyqxsal.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yrlnlyvp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ylvgxwce.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zupkgidn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqtowve.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dlfxxazc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwpqcclo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3igyywjlb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usrtmhhc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kqymrfjw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dhddhipb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3cecyyscv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3efrwwgvf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpojflxo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbhkcin.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eutkfdqo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ynhlvisq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpfgyyqh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wkxrwdxc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wexquqoj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3elmmihgd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3slkcxzre.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pfleihrb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3idcotvzs.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eewrewuz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xwhoxbnr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3orsysehj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkpntmfb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3uqhimnvq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oryyxypv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vpnuqclw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3edfhbvtc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cjnagqtt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bimydgnk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yexxidge.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bplojvpx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mkczyptr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ityavbno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmjkoggq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fdfkmsof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axlyqoaj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rqtrxegp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lyhohqlb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jukgdust.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3psjeovuz.html


<!-- 参考信息 -->