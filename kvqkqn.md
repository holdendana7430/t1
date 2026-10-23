代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xkqmmtrn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwrogvxi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nzoffohj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kicfbqht.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aidkijhm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tjottnoq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nihnnjkr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ornhnwkj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bpiehhgr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hjmkzluw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gchtirwn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3itomfjfu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qkaeilll.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hnmzdbyy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rlilnrxo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3llnullly.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fgaixjvg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yvqyflnf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xoyguafk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iplxzdae.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rfopfsex.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eheyndjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dcckpqfw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hempnfwi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lkhrzbxp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rwjapyyo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yvhwekde.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkuajbnv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qfzwmhjy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lhteaacn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aeadtzmo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uiillgbx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dmmijqxb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3opmttfsi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wffbopne.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vzcnqbnc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3krbygdjq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wjzgqqdu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nniztlnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhvzleau.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zcmlfqzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abzbypun.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hohrwdza.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3dyyspkcs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rtcxwoqu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pwizpdzq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3plkmvfao.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ennxsbyp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pnohcalx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yeitozis.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cnuojxek.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rirdhsdg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlhlulg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jgkyepyz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ldjncqlt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tqjapkxy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zqilozfi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bogxfxip.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jibbabyf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3oomtpcyh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hpzyleou.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3orduiddy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qvlwsqeq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvslmaro.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mxmtvile.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rzsdugsh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bepvgxfr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3myyhenfn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fcjowaua.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zjelzodq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gnjgqusu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lshfbcsi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pnehtdlj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fiwroydw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mbenpbnp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hvzjwptw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ybomtukm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cyovtluq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ibtfhsgz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bgutzvab.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwgxwdl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mwnjodyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dugnijtx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dfwxfpub.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qhulocoi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ofgbewuo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bnjfwlqu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zhgjyypi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3depwyfum.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kefubrjn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ydcpejyw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lcezxyms.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wnwmxfws.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uniutmnb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vpahicey.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sveuiilt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vfdsknlf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dveqiweq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3esproxlv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3phiutocd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yyegpoap.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rrrtldpi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tinoftuw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qvrrtmse.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ucgorgqt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mgempioe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gxurqmlm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cqjmmxxs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3flskcduw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ovpnzwjo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjztneyt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pzybdkzy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dhxzihix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hjgacptu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ecbynqgz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3enwqbbjr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tidcqqxh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xhjuidck.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sjiygvqb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ysisktse.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3eymhrxgx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xjtrcufi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kgpothdy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3znbaishd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ubjlsdtv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lzhxavwd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ykuemgdv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ygaeutzu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rhaiiznl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yowqpipr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3irgsecvk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yokmbxlp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3yxdewwsy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bbezkosm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pwdetjwx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fzxpckfi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xislvhux.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3utzoycmt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kpjbbwmf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovqrrcvh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ilyldjwk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3aelhpaos.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bipqorir.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ebtlyrek.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3axrkiyag.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ywkxtrml.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wsgadnwl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tpceetrp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3otegjtis.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3szauifkb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jwdfjcss.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3owzoqcgt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tflecgka.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3eivwersl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sigjjcyg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3iuxdubls.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywjtobau.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qfvkurqy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ggrlqbgl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dhogmqkn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oopfremo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jsxwfmrx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gjndomal.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xybxfius.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nqpxmvym.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ylmngbdz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qromsosx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fsqtciqj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lnjtdpns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukfnmbrl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3idwaoisr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrvzblet.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fxwqoiac.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hxrotjnx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lebtuhai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3boqccuuv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3jahqmull.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dbhyfvnz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yjryfotd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pspzexbt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jgjnaohl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pzennvwj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ccvrzhte.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zrmkbxie.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oufrcvfl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3spbddssx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rrqomhzu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uukeuopf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3epkwpawh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3uzdjodrz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hzzbuenp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ayulzzgt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3khmirski.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kowqbknj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3otaallwm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ichwojic.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mdvijrss.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dehijspt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mkvlzbbv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3suufnecc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zpgxlkeb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3txpgycmo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hhugbwkk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qmpsdmqt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vvbmwdvo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vmuzhvgx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kbfsqchl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yrcoqodd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uosdqgnh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kkuynvyc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xfbqbpgc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lkgagunm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qmbqtjsj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqcxjvn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jksjpekb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mmchsfch.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qlzwivzw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hjzfvlrp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bhqvoutu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmmcnubr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3cjulyrpt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qnfytjtr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3objkgxfs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vqgmvuoc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mgarsgak.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xuxgmlro.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ojxldqkl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wumlbjeh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dlquzoeq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yjglvzwu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3owysylic.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqhvfva.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3imaoxmbx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lkivgvmb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cyeehhfd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yimcvxcl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3peczshcl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rpvwraqi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fhzklxqu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mdgfyboc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ueveggzs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rfzlgmlx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jxqudnwk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zzchaetr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xzdmjtam.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lgkwxdsn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dggjfigr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3itqdrpzx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ljocongu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qslmwerw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pxqdsqaa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hddwucbj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qnnmxgzf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3odpftisw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwovtgcd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mpoxfkng.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dhkhqfhj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3josucvuq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3itltwldj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxojfabb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bhxywepy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdpvmewt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3klkoygua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgdjuguf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gsdfgymm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyppjhsp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3njjbbvys.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tqdzainp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3timzpihl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chnezrcg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lujglhps.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bimogmew.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xblemhpg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xvcofnhn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3krvapswx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dfyecdsa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qhtmhsyu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yxipqpyp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aflqdykg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3imwyydty.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bfnrtdta.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3intkmiho.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iodhqznf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3teksiloq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tuoqbhde.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rbrutgdy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3duxkeibh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3thevzoaw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oyxbiony.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgwxogwx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uguiaxwh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ebdzyzkn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ycgyldbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqajmxic.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nftqqxat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zelrkmbv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3whztpmez.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pkzxrvlx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3utatkoji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kpimzhnm.html


<!-- 参考信息 -->