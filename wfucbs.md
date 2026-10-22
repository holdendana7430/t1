代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xwzjdbte.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gklpwgca.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2keuxwtjj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cztoaisw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gzjefjem.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2sekjkpma.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ohjbsmwm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2sleyiphd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jurpvmwl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ljtqhrwh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aprzkoin.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vpxwygxf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rtmobjxa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pvsdcyks.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cpqcnent.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sidzudnw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ryvixbaz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ognkefyx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ryuwknwl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kzlsdbmn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kpctwqls.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dopblywf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uiwwyemf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bbsqowvq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2xmngzudt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsmrtnyu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xvctjddr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rnydkljn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zmyrykvi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pzduonzv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qradnldf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yrmgqkrl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2olqshdkl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pvcjvemh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gzvyrajy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlmogign.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2azkxkboj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efapaiqe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etivbyjx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hkextfrz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrhohuwq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cuguzjgh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mqcacudv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jabfbelg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xtxkfpqe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qyouzsgb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wrlczyrr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nrrgapam.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zvpholil.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xeccqjxk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rxustsgv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zikfvrjb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hotlrbns.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jtvbcqqs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bgkfphqo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rbawjhrc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xdxndywz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2epqeacxg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2iocxypxk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2elaonrcs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zpdedsxd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ohijwvaw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2merwuoik.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ezmnirlk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bkxltqan.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tylkivzq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vaiiuamu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2crdhqpdc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hbxyfxtn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lqmbvrih.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cbnnlokf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ncksxfhf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kriimqee.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idvobvsa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nhiwxrsz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cdzzxiry.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qqawhuwy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pcrbnwog.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qrhvkxsm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2acbdvknk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qdnglhbm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2snhwsevs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ljxdiius.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bzzsxhuc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2srabbbku.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yflmxllq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hcezjftg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bevkhsyr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwolecm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zenpvxnn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2csggewdt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lygozzxn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2stopttpd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cxrgjegh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2atzymvol.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtjvikkb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vxreavyu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2sgznfeno.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mbuoicfj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fchncwqc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ykplbxku.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lurfcdoc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qtzbojbx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2swfucwks.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jumnffgg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ukqouyjn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qpxtvgbv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lqkyefhp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2edsxxxzf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ggeoifuw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ltacddwy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fjogddcd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lzvfkciw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wttujrze.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ibwzeiwp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rfdshhlx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zgqnjcjw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2upkjufrd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mumiebaf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2azpewfkr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qzideeih.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2uyjdibfp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dclopydl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mpttacnv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dcvinsyo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2npvuguqt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kqgaxrxv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2acrqgexq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cuiykxmh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lfuyxtds.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vgrrxcpt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rjokxycx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jfrnmjuz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dvoanuux.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwnatt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zfrfjppi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tmebjtbh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwuefatq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndyvnysq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sqhalsxn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2goflhtew.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dieurcrl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ycwpcphy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nubgxjop.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uiruorzt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wqmjiqgm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nozyjfwe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ekthzkkd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnzubbzy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mdvectsx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hszonvgq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bozsikul.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mtpbouqf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fzfgcoen.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qazzavat.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wxoligis.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2sympkufp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2brojltsy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2plfmstxq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qoxhvtvx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqrraiys.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qcifhiyx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zpcazfzp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zxuvwlgb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vtrxjsmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kugnvevb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ahzpifog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfxwojbz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sesradoc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wgigzstn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vstvfrbx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rgmswipy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qtjjzdif.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zeqbkwhx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2upbutpgx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jowxpayo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tinxqikt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2clbityvi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2naabpzte.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ivohgmxd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cyhlrqsw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ylkrqukp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nehmzrer.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhaozha.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cntctyqy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hdjurrbh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqseupzh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rvqbnfop.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2brmeftzt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2yczuazyj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ojcypltf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2syuliskd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2epvvbyku.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvostlgg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ralfudmp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kczxihtk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dsvwdfmc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bppkdava.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gkmpmrvs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dcdllcjf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bocfqyhw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qklvlrqq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kaxspjnz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uppznkjj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hxwsvjvs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2szkypvtb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pwgmbsvk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ikyyttma.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nisphkyb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2flhuiquh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2okyqcewc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2kcowcscp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ulmohplg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cqzepevr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ebpcilzv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dbczwncn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qwvpvanb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uzjgqqzv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ppyuttxz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kdhbdjip.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vvficwzr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zqjikxvp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2duulhxei.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjkvtqu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ihhzqvtu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zwadlktv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2rvcgoozo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xvggfehp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yajlaspn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2abclloxt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxiolrmv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2oghiwaco.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ibhgdpgm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jkqimpwg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yzksbfcy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wxzxxpcx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nobyhere.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2obvlamhv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fbkgcpiw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lkqvqpvx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sxktsdlc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rneyabqa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zobhmled.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rlwchiig.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fjthjqap.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2liuixpao.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rqfdnxit.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zciknygg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kgieqikn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xgseovhl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ktbwigua.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tatymvrr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ziqlnbwn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2oedqdrmd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ygbaqrsq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jkqzxrvd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qenikdsd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfftlqgg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mrbwknxj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sadmwosx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hpodnjcy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqjfwixs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gxeqsced.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mrfyxmud.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2onuldfjm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvbxws.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgfwlyzx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tknvusvs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2liupqpfp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vkhahakd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vbuqqpos.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2aqqwvcco.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pdobktii.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2igjgbdzw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rvgezkrz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2krwvvpuq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnonjvs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yohjevku.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xoalsabu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bcrhajrh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kusojnqk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mibckuyo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ppqgypmb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hhalqhwz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ypedhgia.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhornhhe.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtxavii.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rsygyafu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pvlvnfqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsfdxzdn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sfepdzbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogotovxc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2iviytduv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jddbryls.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nyesmqqi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2otovknwf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kkbsxvjb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2clkwzyda.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jmxhfxfs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gfaylmzp.html


<!-- 参考信息 -->