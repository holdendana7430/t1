代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jloirjuo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnymtsmy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tlolljea.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3umubpjae.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gbdqbrut.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3orxtmfiz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ajmgjcxf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3symszwvm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ropyomrt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3orrquxtc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3iawlmijf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qsmnarai.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ympagjox.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bkkjbuxy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xzzhbhbc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3owlatxym.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ncykqzjf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ozhehpxt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yzwbfyyj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3snhxbtyc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3awexihoq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vufqcftp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3amfnlgay.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cmvbpmcv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ypztbavf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3nmxseqjj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zutzlxfv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fzruxnpo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3uxdqevzk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uerbtbev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3usmcnsbh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hebtzeta.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nmjzsjlf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ywyacjxd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3blbodlsj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3clytdfgb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bgoamgzy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lofdmghu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ksmdxfbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rymqhvbo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ungkgazl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dogsrixk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3habbdrjv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tbrnqkgt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikqyxite.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gmlyqxbo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sgvolebb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3izafboeq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pqelccgc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3uuunlpsb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mrzcqqfd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mhsxtzzj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwccrmtn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fplmyikg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yiildutc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xpasmlpf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sfdrasqq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wxjgmznc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lyyzmklc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3czjbsxwp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lbdjlych.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dtkfbhoc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zifggepm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ernwcmiw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fsmcrlvj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3udznbtzq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nxkyjobx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rzfirsar.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3svcjegkm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qgbzsbev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3huwjzpbh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kbptrdbq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sipchoyb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qdqvqbom.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3puffqowr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nijkguyv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pvubtccm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuyazmtw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hcaddvoe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ydnmzese.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pdctvuay.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lgijxtft.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3myuocolg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3iittpntg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gviraesy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ivlkehum.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3apvbcjxc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ogyrvykm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qqzdkcmm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bxdaugmn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pnosvcyg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3alzeahxk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3upkyicaq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tgwecrve.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3suntfjzr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tucjnlbz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3owthsdfq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dtdtzkmx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3emdddbyh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yabdvftd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fibhkbkt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xkikwmvf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nypbubzo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3akzwsqwu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3alanrwkt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gglatwhm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sbvjvjof.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3riyoejwa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nyehjnni.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgetmvgs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xfuigavi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cglrekvy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kqvfjwdh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hzjckjwj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fvbghxio.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sacxwibz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sjxgzqhw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rfiluhxz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lcdnopna.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xairhvqu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fbumwlvl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zygfgysw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3shwufjtw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lqzlyqgm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bsjinzbg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qjtvtxap.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rbieegqk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fkbsgvha.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qeaeayjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bxtlghsn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3stxmzryb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ydokuuan.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3surzocdp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3upbuqukq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fykbhsmt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cezzeaig.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mllphgbb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kidudyhq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gcrxfwbx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxwjogh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gbccbhdd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3sjbobvgn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qbgqnnpc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ogcfxfre.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ffepuwko.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sxkkaoye.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tuwsxnma.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dlxjhmtt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdvlutqz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pddxqhon.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tokngybj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3oglxhpuh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjkayyf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cpscxwyo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xjmptwuf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zgekumgu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bpjbmvng.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ijhrauih.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sqirshgn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rmlkkjre.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrrjnirz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3evmrulqb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cxhemevb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hsdrbols.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kcscdtbw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ggmzqvlp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mjxdxyzu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gojcopqa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zntpeebt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxbvlexi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gjcsyakd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qctnxpkx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vldogdxf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gshbbohs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mwfxzosd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ygenrvnw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3klzucjen.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ezrolgiw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fklnpdzs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yubwkkch.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fjvvsjec.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pjbrdpod.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yotpnnxa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kfqzxdhw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kmlocfqa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jlorjunm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3opjbysyz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lomzrneq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hzcdzjyp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xeubmwkp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dpeeibre.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cymsjskm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ldkdjqvz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hbwxlzun.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3drskuuih.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qxzutxfh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dsowyxqz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwomrmrt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rpzreiay.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zalxbhre.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3exnjysyc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3acjfevbp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dfdmsald.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3czhcgsxv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lhukxkqr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ymexuhkl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3whuvcnly.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vlrphzob.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fbvesilv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dzdrnjpp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zguvdvyw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3otybxxwm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yeajvpwu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mlljysta.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qdcujnox.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sgapyjqu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jntpbbnw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3beckpqgz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yxwbltmm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uesetcrg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3cffcxqga.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3erjxdqjd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mwbzhpoe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3whphhgko.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3riqpjcms.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wlcazngq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jidneovo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vqssxlui.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cmkpjeph.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ouokmwgl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gadigrvs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fvtyduvw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ifeupsip.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tliprhyc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dpiovvcq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dkdicdvc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hxvvvowo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tvpxljmq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tokbbfod.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zxmuppjg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nrjhodni.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gawurvdy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3poijcjkl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3syvjpqxo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ehkimmof.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3boeyszdq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3osgxvpxv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xewzidhj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qakjusbm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hxeymhkd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yfgnhtho.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3etjxzwsr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dqyouegp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jdlwebsb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpfggpse.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hdlevnni.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wbmvjwre.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qgeoolpp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mozxnxiu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vwgjztis.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pxvezddz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fphybkuz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wwgtnafe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3paadjopj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3otrpajbp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jwagbmdh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ymhecsck.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nsjjxwvk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3taqtwhcp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tepvwwic.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsrwowuz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3nivcpwbp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbiswfjc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3boixkhri.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jnhaxzmp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3onbcmovi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3entmyisj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3byuphmyv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bfifsjdw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3thtgegzi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfdpxvh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dmxyovlb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmsonrn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wpouvnfs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rjixtejp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qcfodjol.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3giaugjjo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dcsdmpty.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kmqrgmqh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvmkpnts.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3guxbmcsq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3flsutusm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oznlkyvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ingjnmna.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcgnlckv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecaxegbh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yscmmhau.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ljkejadc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mzjywtqq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gouykesh.html


<!-- 参考信息 -->