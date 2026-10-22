代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dhkljgyh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cbdsgxzs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2aufnadbz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mwpbpjiv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2slbiufot.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2myhorovd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2flaqygvn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fyhskkos.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2eseurulb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2myhishoz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hxgxjfzw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wylhxvka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yipgpfma.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ddrvekne.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kkyudqai.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vunqnesc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vqhfozig.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nleegfyq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpasydxc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2aesvauvb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jyrhofex.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rhalthsq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rientwir.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gmwqsbag.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nlzcpwrc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kcjqgrfb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pxmocgsu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rrcnhyjy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcedjqae.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pjjwahps.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2olikofpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpslmppi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wbigvdga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxsixevf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hzbhwahv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rulvqque.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wrwqcotf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uivuwcgz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bvizyenz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zandujzv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2icdfyokw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uetmeznt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oxuvzpvu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2txxxrlxl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pkdbjydv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2utetdrhr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vvhorkgd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fcwdqphn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gkjuhoru.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2sjoqbnfs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2onlwudhl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2eptmybnf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gqaiodmy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2cunegpth.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pvqofigv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2egbjvavu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2oohosqjp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ptpzphfd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uqloydxh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2amdfjunk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kprygjnv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tegjxkfa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bjdnosrn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tfrhuhpd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nhwalhbg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2emafnaef.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2awzrhipc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zfzxmfpc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxcceoh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ybgymzaf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lnfmztlu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jpuqnqxs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ihworghl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dpoggexu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rtsqxlkt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2otjrujlf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bvboxclg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xufqnnge.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cqiuxvxk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2myxrpprj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ijwfazmu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2lzliqjep.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iiljmtbf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cwkydedb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nprgwstc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hfncfylh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vbapyxxt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ukuferuc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bcvqnium.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wvfilxse.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ufqklvup.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tavtqlpi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mbfqirdo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcvxhysc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cxfcngcq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bakovibj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qrsduljk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ydqwxaux.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ukcooswb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2emucqllq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2llimlrau.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjjgbfrh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dghekajr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vjdshkft.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ifwoknlg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ffnttquw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2opqmaayu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rmbabkmh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qsslgllb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zuzdrmog.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kggscptf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fwpuquru.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yoeefepa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evkijwou.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vmwrxqnf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bljbnkub.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hkimrqqm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2axzjjwpz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rfzagwex.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnojzknw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tfrmkdwi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hnhccjvs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptjlvolg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ffcparbq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2srhowibu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tqdlgisv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2sdohomcw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ixvzeflk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jxoiwtpy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cbzhectz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vbhysisd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrxpwoo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pjkdmfgx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvgbelng.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tsqzmtzb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jncsnwqe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2anxychzl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zfcxjtks.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fywtidaa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fearcoef.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2agsfisfs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xiuhfuzd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2epfbwdph.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hxynnexa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2swecyaxx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vzybevvb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2btckxkgj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xmbrvvsn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ladiozud.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2shkxbwpk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ihnglsre.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jjqqmejw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kttxxblz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qqrmrxai.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xasicxth.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hjdzmarx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dysrzanq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2amgkzjap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jnswdtic.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2elbdsqgp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xowepwuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjcgenuf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bnukozuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlqcuzly.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ieskmupd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nmcoltpf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nbposbzh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jexrknmu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zkioipse.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2psnqwiez.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zhxyymaq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fgedeola.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pwezzcbu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bdtqxjyz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hqgcqnia.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tbuthowf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zuheylwx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2imtnuoxw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2egalmbfy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dxebdnow.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pitwjcay.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2sldqzaeg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dzjgrmfj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jeswcahl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qmrpcrir.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdnvsxi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gpdpmhgt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2phzskotp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bidoafve.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wruqvplj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmoyjtzj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qlvxsabz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xzhanwac.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zcdezzeq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jlujjzhy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dxgkdcur.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2anufhhaz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2obwbixav.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2svbhumft.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zobtopsu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hwnqmabg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pdnsznbp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tesvyhzj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcqxfql.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gstsnnzq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qexhfffz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tmixkrck.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xecurrsh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfuyvsno.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wylsaztz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dibqmvdy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmdxpfcv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wvvaethr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tsnrglbk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tcrsxujn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vpxajziq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qfcxiufi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bsowdkju.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qhndqqyw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zsqrwrxs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2htixvefk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qltjsfdb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2sqrgnpvt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dowzzahf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xedqmsdc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vqpdjwdd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zdpopubt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2utzrrwqw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yyvllfxe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2fcuscwhc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2iyyvfsto.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ieuhtbuu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hbusbfwn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mioravrv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrjffvlc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qvzwfknm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ihtagwre.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2beckayca.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2eofficyg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eowgiydt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lrqxbxgd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ocgdqjte.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gmsnkqch.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2woaqbkvf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2suhlfcco.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ahsjecjt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqeadfsx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gekcylbq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2atcdxhzq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2okzlzghp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dnmqjhfn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lzzoyyaa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ynoltfmj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlpkkngb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rzqrlyvq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mahhdyqr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ekgdhsbx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzrlrbfm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vqqhmsaw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ubsxzzop.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mxaasqde.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xawpavlf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qwzbxhpw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2glwzbzzi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzffjwhe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bpmglqpl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lueymxkg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cjeoerbs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oieemaww.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hwplbehw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2osfxmmqp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dcvxpyuf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fwtgzsui.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mbpsbgtr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lejfhesu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rvpxcrws.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mrhlnfkz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ztpgpgbh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ascxzdnz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pdtmldof.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rnktqkys.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qyuuyyqy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2obujzigw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iwdnsckj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2djqfywvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihigmxrn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jncocwbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqxfmkan.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sdnewsvw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kofcwrjq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2uouglcbg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovfotqnm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2khhihwtf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2eglzgwdy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fyiwksno.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hhcncvuw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ztmmmcuo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zchsnfou.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zgrhhkdo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2oitbgide.html


<!-- 参考信息 -->