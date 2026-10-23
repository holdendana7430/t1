代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vvxrskkn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ikxlnxmz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3uihejjfu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3scqqahfy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xnjmvcgm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sccotodg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fcohlxmb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zecfnjdn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3szkucftw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tnbmfdki.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jywcjmpn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3keulvtnl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lsbtjlvc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3athqwjih.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3efxgqzju.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aapcirxc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fgcizzna.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3izgqbzhv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzhoykrk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rviewlnb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tmbuqpwo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dkmhmocp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gbgmronr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kyongbjn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eibwjhln.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gutvamqk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3abjfxiki.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tithylxh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fgctgshe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qwfotexf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zfjtkimg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eozltlzc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xjtmbkhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxbgmmxs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qxzhnypi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yqlvcovr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kwmkspef.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ikyzixuz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hnvbuqho.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pwhsnuat.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ebguicpq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3avaowslq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xbulpzae.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hfmjycce.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qkbyreay.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzfgruko.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sexmkhyz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3povdierz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fdrorbmo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3otiptymt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gylqcywf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gzjdtdlg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3svxcqkzc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gjnoqagv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lgazlwva.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rttubxru.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3apexaryy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gepvulbx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zvdhncyw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vmnbmgtk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uezejlwu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jljhoxyq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3riehjfpv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kymkinjv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ojerofhj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3isfozilo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kegtphxl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ibcywglj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sjryiaiz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhqyovkb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bcwyotpj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3chzzpwxp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3efzshypi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hskjeyeg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ufntlouy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hfukprul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ljilqeqj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3shbyzlny.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3apksxxti.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eejdjxjy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3idlgraxr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ezvxzxab.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dqqmhvwy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3onipipgf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jrqcqhsf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3avjpwgxv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vxxsqkxh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dvoqpgdh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3untxpbvi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ywycnvsg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rvlqjcim.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gspakzqa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vkauaegj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pippfvcw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uryydkew.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lvpxrljc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eqsukunn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3znhaphlu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3suzmrhgh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xxgtficb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3daxkwbgi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtwsgpbp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftvhtyyj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hjibjqbb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rsswfqco.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gniulucr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3siylyqjy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnpyumyt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qrfuektt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lmubxqzf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mudckfsq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvfllfcz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pgoktjrn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukufgpsu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hglrofhe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cnfwdtbi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yqsfzbnq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wzuxrgkq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3phqjpyis.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rkzuyirw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpmyqnrj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ldwolknc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3itjldolo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xyrcsrtm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bcuhfdom.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xdhxlaai.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3iedbyvga.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3okkzcyoy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ccotcbkp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cogkftas.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jxixheoj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3lfhkbfto.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nlhewryo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jzuyrccu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tgmuegmk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ttglvknb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rlmlrkbh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3iqehftdw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3asmzirri.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3biyivqke.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3glamkfms.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3schahuiz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rupkzqej.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nkxtjaar.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhvsvbdx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tvuhlouj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3loepgmss.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ztqflnhr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tmdnhpzn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3akjlzzzo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ngmlhgbv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jhdfklnq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mibhxmgu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zjfhpqfh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yjwzztpb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rimpetwx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwleynly.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3muwimzgm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rxjkdbzo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ytboxcgy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lokpnyks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqsjbssu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pbqmkhhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwocolvt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rgwqessw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iuhaoibu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wnhyidqs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jpzayvas.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nskdjuvk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ptgvqiqd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jbzdmguw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dscjzlxh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hypipems.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zniswreo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kfealfwa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aypaxzgz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3swymsnzp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vqgsbnfb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aekbluxx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ginnguec.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkqzyepe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3guirxwzn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dumqjnmo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3naunmcam.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rqiwlxqd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zlxpvkax.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xosqsfqj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpixcjbh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zzgjuplp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bvxfeujs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3aogiyvak.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rkttnbga.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sgouwzlv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tsawuxlm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpiuemrp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ulapdnlo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ysrsmbjx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cajwzska.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3myzqblxr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3owknrztl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dnopudil.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tsrnndzs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zrfnkebx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3efoctpmp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xeygkopa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ntsclhao.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ablpmeon.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3notqajpa.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qviwagyj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ivojpxzl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uresekiu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmkyjnub.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cmnmfnli.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zzsitgea.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ausgdpwx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3drukxwdc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pdzcayhe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3auqsvhye.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lcpkpfns.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxbglv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kmsbwjzd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zeewgczh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vrlthqik.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wbhjdhfa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hnabnfyg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vorvgthl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcduhzlz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkphukog.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tentizlg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bzppdntf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zorprssv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hnfsoang.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3axuheotk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gqptvoco.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ovpsykyj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mndtkllk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qkzmmagg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wcosxsuu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wgqslcqk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kbbcptah.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wharlppy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cqgknawy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dstxuomf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hknpijts.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ykxjugzs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3akymxtup.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oqmomuhg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tdhkemqk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bqfxakeq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xavcbvfe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ybsqqgln.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqdxvooz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uwkxioji.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3udfnzrid.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3untihpen.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3murfehcb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kzxsnqaf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zxjhfnux.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uljelogw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kkggwasq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzfzlkuf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fekzqhtw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tnaatevz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zjvqdfvy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3docdbnwt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jgyalkup.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3porweqre.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nfnbvhfh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3exffkusk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ghhfbect.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mhtheoon.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kwmhwpfm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awdvepir.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jqtucqxq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyuyqjgs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wyyubfuh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qftdnivk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cubqnetd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jfsozuft.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tzkmwjfh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sleihess.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfxiqkxk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kiqcoaah.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3docffgdl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hyymakkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssuuanyf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxvzwyqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvqkjhpl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wefbkwif.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nydnhxeh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qazwhrwh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nbgzdmod.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qqdmbskk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tzfetufx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3afwhhobm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uomzfujg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3adgilntw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zjhmodnu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pzfwlpud.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iisgzpzo.html


<!-- 参考信息 -->