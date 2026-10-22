代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ezaoxthh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zrnxgmid.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ehpkhgrt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mdfwmeur.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hnefeplg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tieetayi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xbunjiqt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wouxyiib.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hlcsdaof.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zepfunng.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zusclbwg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2julbnoxt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gtaoepee.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dnrdltle.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fpptotga.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bandnsjx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2efsiaxwl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2awztfhai.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qttudjld.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fssaepyb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ethgcfht.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rhgiqsrc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2raitoyzj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mmoxtmih.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fvoowphv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cvbqrdly.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tolrnogm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vfbwratb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mpqchtti.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ltikknsy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wlncwvtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzuixnht.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wzwkbrib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyiwerps.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dapittqu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2trckcfzr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hnsowoef.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mggfkwkg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fwpsyizf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2uruyzaii.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dxuoento.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vfccioyu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jlltxanl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jgvbwkdz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wkmdbbib.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ikkozxac.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dhpkvone.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pwudqxhh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2evmjdqqf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mukwqkra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wiimswrk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lfunyufo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2phkargrh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fuxklzxf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ehfyksiw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pudibqkx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2puhxblaj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2svuizvex.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ginlxnqh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybsyszqc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qfzrlgsn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ffzhdhvw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ozmitgqy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dnqpsvhl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rxcdpdox.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2labolafu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jllqazmp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qbtruxky.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbiuazxo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nelodpof.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dyjrsais.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wrctlgng.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kizypckm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ulrjzsdu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2spjkxnls.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xnretrcb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fhgakamb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2okkrguba.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tqgmjzet.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2huwidhjq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2supzmzcf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ndwmlorn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tcytzixf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wkelbsek.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kxskcdlu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wduxdgcc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bzuhnvvg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2endzfqcs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ydhdmgsh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ggqihfrm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ixcxuozb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dfpnrmil.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cqkzbiiu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztginxfq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2duooqgqt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2duwiuprn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xcqfgdgg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xzbyhkzo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bhaeydfd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ybzhsckq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lefbloez.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjqnxkrj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lljkudfb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2inewrpqj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pcodlwoi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iyclzzxq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2biegruxz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcynwgb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2edehxkbm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2isaxxvpm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ppsfwfup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qylpyksy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ukcbetjl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fzpmrbek.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gjbjprdt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dtzuxcdl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ungybmfp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yevlengr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ngzfpnye.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ufsjklei.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rpgyqiei.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dowsrjwe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcptzuiz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gxhfmxvw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2byvbjzhw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2faqjbmfq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rndpjmig.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qptlxtwy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2imqaddxo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gscqbxcu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2enyanzup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pedqtbfs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ppmjovdu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qosmbukh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dozgndem.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kxfjsypx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2balsmgoq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulhcnldi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dcpafpzl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hmzmbggp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nggrtkmr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ggofrfzf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yjrylzaj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nyknoapi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkgjfign.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ntblesrl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2asxigqrh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kxjnucsu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzgubcc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jjxwnfep.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2edbweaoq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2plpspofy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iminiesu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2giqxrufc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ltvwoidj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2syuwitlk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2czfptqfl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ppxmvpsx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vkohknkl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2aeqfvywt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bfzieqrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhkvkqwg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hwgfeslz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hatiodvv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znwgwmsm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rqerxzkz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jhpudwcj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2flbebxmm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ecngxcbh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wpikherr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cnycsahk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ahkmasyb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ioocvldx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zpzmvpjb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eqfivluy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uhrnzout.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hdzgcvrc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fohsacpc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2scehtcre.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxhfhht.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufgqxhem.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bsaxlczt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeidcqmh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2covkijru.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vznwqiac.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lffqckfd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xlyiqwho.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vdnucmmv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2czyuvjok.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2frbijqtt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uktniabm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2liyxskbe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2eicfxfeh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2oniplnpf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ygvoffbr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2suhlyzey.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fpdfffpm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2paqpndqx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uhakotzy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gvmbshjx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rbtzoano.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yveplktq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2typdokpb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2scqphkef.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kcxlsusx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fzswefmq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mxjrdhcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rdhzgmcj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hewkgeov.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xkjjbvhf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bxzvhkvm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hggxahpz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jsictzcn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uzuxobsq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cubvsvhn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2czkxlhma.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zoiajipz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rwrpyjvy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2camxtsos.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2oicxofeu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cgtzxiqt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgnvfyd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wwlvggwk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zffvocsq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ripzlett.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dhibrwpf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqkvnkik.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkukoadd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2daeazrjx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yadyoltp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ciommspw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iawbtjsp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yjayyotq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sjpbdwgm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2clrgpzjt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hbthqjzi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2huculbqo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2julfykzk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yneslqzk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nxmfqapq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yyxfzjus.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2oreczcsi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pxduloos.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kptiruzp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebgumgrq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vvnpjoib.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qocxgrty.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kdfkbvmo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xbrykjlu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dgupviis.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sdyrygox.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rchgahiu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fwaztcej.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cuscpsgz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wqzyjuzf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ochrsqvt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2riqthblq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcmwqbhu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2puqoqndn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ycyxrhib.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dpzwidbt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeaznzly.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tidhflit.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fvfbtwgx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2exqgonfs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2adkthzdx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qosjprzl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nbxokxlz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wkdyxrjo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dqyzkxsw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tmykxaam.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qwxwspzu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nzscedkx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ynhfhbgq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skffbrrb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hwfufmfo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oujoqdhk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mkewpgqs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkbwret.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xuyiqtrg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oqsswyas.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zcgtjpkd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2avpibngi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gkieapju.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rfklrwdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcrqppzi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cnzwisjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwzaugug.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bqhmwluk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ljloahgg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vmqkjqiq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hzwksssm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zfpxboxk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kdfqxkzh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wmxafxje.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dulgslzn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qgrvrmae.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gwckylxp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2npbzlwma.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2agxowkfk.html


<!-- 参考信息 -->