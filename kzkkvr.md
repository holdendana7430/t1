代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3imudgcee.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3emoiezew.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tyzywduo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rzhmdsak.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fjhrqtrp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3redusgtp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qeuzvdev.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3monkeebg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3frxdjvuu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3arycbprg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hdsuatqe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xggpmehw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dipjpxue.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dplthkut.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mtckeozr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jjumdhuy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nwdbblzo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qklaiixp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3adfgrkwj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hyajepcg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jntunmge.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uscptrac.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnvrvljj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ngibzglf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xjbquacw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zvwgidev.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pktjuxdb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zulxzklj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cnoojpvq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhrttnqx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bazmduwy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xhzymqnq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bbvycwka.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ppwoslov.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gcqzuwzp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3axbgayid.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rljvhpqo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3syjrxpui.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3booxdjps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvlxplul.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zkbinovs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfmykqgi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ijndylvv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gzbpblbt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mdnjevvu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yxueknme.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rsqtfzgb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bvuiogwk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3atriwoet.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bflkyuiw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ijsmlkwq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3exjnchql.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mcvkzdfo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zkfkqviz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sphwqsal.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rwscfmaf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ycsfillo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ywwpxkyu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cjlsnlag.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3adannwxg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zzptzmbm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tqtoewda.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tyzxxihl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfcdfwzs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qthzuqbg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vwlqcyla.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gehdpjxo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qvraomle.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ijicafuh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3adsnadwi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wrmxhdor.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sqmxggcf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3paeiaman.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3wykptxjd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3htczxbvr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ylvxadco.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zxwhxbiz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3smwxmqzn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hhlxoaky.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3whjsegcr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvtjvsu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3acjivzsx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ditcgkfm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xzmzyvce.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ynnwhixn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pjjpifcp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dvztufwi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rwbjnkvl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mfdjanvz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cgmfxhyz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3svkcitkm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yahtyyoa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jjskaxyt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gbcigcpi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zdmtltuo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rxgrlcxm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wydpmgvc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qjvksrfu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jszrsoit.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjycht.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3eiecwmhk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cionolkm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ffbwlirb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kbcjnxlr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vmkzkncy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lakieyza.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3oklvkyvz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tvguvmnq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pezpnoou.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3neyqqllo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3asgxfprf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3iryzipcl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mlbeubur.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xjvaqthk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bdarszau.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjlfak.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gewpajda.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cebesint.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xqayrmnx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3isynzjnd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zlnnnkgd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fmmxooiz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rocdabyg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nylkmjop.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pxknjteu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mlldnvac.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rrzdwtcf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqaffawg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3shqfroqp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3kqtcbbla.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qralgcyh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gsalhwyx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mmkkcnuz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mwjxrgmz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xclkrgcj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwlqnku.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zmjrrrse.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tfggvxoe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tqmuyfzq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3svvbstsy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gnwakckm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rsqtzkox.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpotccst.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nzuqqwze.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3klgmvxcs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vpmpeowq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lpxcnndh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3etnqxxom.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfvznopv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zmirkxnm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3srapawev.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lxytomah.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwvrkcf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xmqfthsd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ptfrtwid.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ltbskwqm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jafkdudo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mgzsrjxu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vaibprwf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3plolbufw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdwqyhkk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3uqrohhmv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jfjycocv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pfskffno.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zwxndgwh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ebkgnqcc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dpkadpsd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bqyiiwsl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3esqujfqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzqalhxy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ivodkddd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkhtkgja.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzudtzxp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3igiocsgc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqaoinzl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ynoiiwcx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vadhsksf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gxnhlctu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3bwdbjtwh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qpzxtdwr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eqrsvecf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fklmjrgr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ysbrqejj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mrirtpgl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cftqlqil.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3havltbsu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3glhhspnv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mdhotdmj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3alkryyvs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kjaqkpyk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ahdvengz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3itzahktk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qwmaogll.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3thvrulep.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zkfdsyqk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kaozoxeg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jjmqggua.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bnubbtvs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3akpexpny.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ujufjvml.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3aomvcjih.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3buwtkams.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eszerpjz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gqdtktix.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dbftmyzl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zjuoyqjy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nidaudgm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hyfqzolu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aampluda.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dtqzeluj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ahpjwnzs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bensugpd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrfobunq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jlgrqgbq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dmvulriw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pifjvfdp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwkjdsuj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wsmdcxcq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3owlazxol.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bxlgxmdm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hcxzmqsv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nntmtqrh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tfxspmgt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fhxatnay.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tpcsffpd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3umqebbif.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cntbpscv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dbdqathc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wtmmfmrr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bjlgicgm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qkdqgmdi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rsscdnmz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3npootobk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qqgtgatf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3behegxlu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ucszdixp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ppldbqxt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kgnpfpsv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrueca.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pjktwtmu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dwutcluk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3toykyojf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwudmerc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bribskkg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zxpnvsep.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3urklqnyd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yvlwctho.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aywvjfgk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nqwyfwkk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cdctcrra.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mbyeaibf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3frstzsez.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zxrktwey.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cmcuthkt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qcozwtro.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3knqxqaof.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xrqshkhk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fnbaafao.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jsbuxrlf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtzaetpo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rryvajbs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ftojvyya.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3igchonmo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jjpxbnqa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gwdkgvlo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctjjjevb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mwprwrsx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vlzatkjy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xmgbdqqz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhzdixtx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jaqpihst.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3upjgccpd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bhtqglxa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xoqbkabo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3raedjuat.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mcqlrabx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nyyubims.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vkupfera.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tzvnaxuk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lknsttyb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tscggqcv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yultykhx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvdzogw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yiucltyc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uimaakoy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jwsqmzug.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yqtgrzqb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bxlwkzbl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qwjwkxjj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zfbzmzdp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mywjouic.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3czxuggkg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dgyuyzdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlpdjvmc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3arlsfdbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flegfvym.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zpgbfrga.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wygmbfkv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3opneuxxw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kqyfqogn.html


<!-- 参考信息 -->