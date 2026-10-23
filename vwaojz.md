代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ukqmvfru.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jruidnoo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dknunbuf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3gxgavcul.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gnstafid.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3diqzqsxz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3molpzdgb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dpsukvzt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fgmhmssu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wcisdkbz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xcwlwcza.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ixndajzn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3idmeoezu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tigfuwhr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ttakpvge.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jgolqvwi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ujqponga.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lfrfktvs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3miduzgby.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kiqljntv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hbgxbdns.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3fsngbnjc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vjwuuufl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kjtjwlbs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cpeyenee.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3omrklnle.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cqaqbpdb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3okyiddgx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lfexvxly.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eknssbst.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lnfjtkbg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ywnqyhaf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ujjehjhg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ezpisrsj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xxzmixzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygrcuuhs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lgjyyzpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzhgehdk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwjqiusx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jockbrcd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxmloazj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kwowoabu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ktdtjpmq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zykagswt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cvsbgori.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3spdlqkrn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hzghmhxn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsgiincf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgxmcro.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dwcmtdjy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gmjrwlas.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dwocmygb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3euhwgetd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3enorcmma.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pwwebbvj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3srbiypwb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ebtrpbee.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kpdopmyo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gosbocxg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdibteuv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fwoembxl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3avgyxyhj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ozuuqljv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kkfxahel.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lyvpjqvg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cmvjovyj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3edcdfffe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3evszzozs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wvuuntzk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3kfvmjjus.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xnfrvnti.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lirunymk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ebxmwsvx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3itnfcojb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3shjanjvd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivllwoec.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ltjtjnep.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pwilmlze.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nszzvqxr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rxiyoyja.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3trgcrtpi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zlojzmyh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xyqohsje.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jrubypde.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fscswawg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3piytgwqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mainkxlh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3larmwlwj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3btgbnbwo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jhmtheqs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3osaakaoz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3voomamlq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3inlqmeal.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hhtviyjl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3glqrmepy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctpcfott.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bxqicimq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fdwwpqbf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3toioenrt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3giyppdjr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zctcseao.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3abauxizf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rfvenqdr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkjqsvby.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fpasirvy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3olgvxyfs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lhyhjcoj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xpuzvcjt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3sgytqyry.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wqwhsgug.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qbfhnume.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3paprwqob.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dpxwlzsn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3deqdnkae.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ozljljff.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fnjenbpv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3klhcoyjs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ulqtozgy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rjvwrvmx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wwzmqajw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jqtjwkyy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sidlvatk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3luullcfr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3coslomta.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fqtojqoh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qfpdtfwu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pwtieimi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3equntmob.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kkrhpzsd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dacrzent.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3puekdumk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lbzrigcs.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3feekzngn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3avsukbel.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ljprafyz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvxptvod.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gwssspge.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3obprurzn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqkbapfr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fclxdjck.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mmvlqdke.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oclrjdpc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vbzipwai.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3haamlvsw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gijrxcbc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sulhlwis.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uisjxmbu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yglphacw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3knlfxomj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ncyucygu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3imvazzor.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ktcxsafp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mnypivwn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tukwdjnb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3awyypwqe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pcobrbsk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3khvjjwsu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zitombcn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ghpwaplj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3flvghpar.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gungzphi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lensdgbj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3afutwabs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3asobqlna.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3glrmiujv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adzudlkq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fvaeebmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcftmeca.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3btggztyi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jgpileki.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cmnxomuc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tpcbvnir.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zybpxkkm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zeebmhbh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cmcepgsx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lfojwkvh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zasevmem.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rtgipezq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jasctqrk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3owzsdvbo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gzsuksyb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mtcqtmol.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3frfuiemk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jabpfkgi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkoksfri.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ntdwbhis.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3arnkqosy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3adekqsqx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bxwosqwp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kwpxbnvg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pquwulff.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnffnqow.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qzwqbtks.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxiggmmc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtmyurdb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpsqxqa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gffgbcng.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jtyjjozc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ctcafcsj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nazzywwc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mqbfgknf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zewtxiwj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fmjkpsfg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zkaeslil.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3djdflpwl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ckzuhylv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3janfwacm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3srtfsbhf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zikypokg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wjpghrdx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gxtabvlw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ymemtdzb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sozmoyjm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mbbyqnak.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kvsbmjqc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjadkyab.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gsmuvxrz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jrsnxxlj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3igfffjbw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jrdncfyh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vbkxhjfd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3phtvloot.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bwvfzlcr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jkffxmah.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cdgjhwpr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iujuvcnr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nlsejdnc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ndoqmwwd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xlsyfshi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tdhprrad.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mmoykegw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3henmkrwg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3oxzggtae.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3znzcfyrd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3cupiiqyv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dpkyhrew.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nmprywjc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vayyllpp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ennbfamt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ncxvnvpf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hvrevlql.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vigoqrqd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3geevoahp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wodiahbd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sjcdvfas.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lckvbvto.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vqcqnesy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3quonxmtc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wrirzedw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lltmxdmm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pywqpkix.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tfieqqaa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ixqsunoy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3novkujdr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3egimwkbh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wgfxgxjs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ctlkhqdd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3avvszjho.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3lphfzsmu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqvduvpq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pwrdksvw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3adrlrcyw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ymweyplz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qvnrzdti.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sznejdvq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zizuvlwz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yrkcfepd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yehwnvkz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xbjypqxv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qiyyropm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vzncrnms.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvecdpbe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3knskvbwm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zbluzkkj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fjhveikt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wzsjdnes.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eaovzjjd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hgqpnhxw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3oyewyusr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bvpzkdxo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3niulxgba.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ntfzmyzt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bviucmmc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gdxifhbc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zjwbftui.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zbikwmsr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jomtjulg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sqwinywe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nshczwsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lykjbeix.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jtzjxtaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksntbiyf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hyrxcrri.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dxoabcva.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iohhpayp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xzshloyb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qrojhkws.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3yvszxkpu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mmrlntmh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lofxmbnk.html


<!-- 参考信息 -->