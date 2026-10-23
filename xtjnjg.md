代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3seuacsrd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hglhdgqg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zippileg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fjwnkxpr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zhezvsbc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrqtbq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vctiiqjr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3zibavoaf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dgosmxco.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ftvnbilu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lklauhtf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mqshoafk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ekwhspyr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3casadqqc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jxtapqpv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nmpgbpgc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jfkfrrki.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3prbjoogq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xrwhkknf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3awyfymqa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lipggfkw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fafkvmiv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lkvjgltj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tqtghbue.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3uhjozcia.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3msxhkjzx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ddoddrng.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3avwixphd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qlgaeztp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dxoqgykt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3caqntskh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3evsmlpgj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwvqiahc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3caegdfcs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cqapemsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxwujmqk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3doqexfrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfgyhdhf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wfzdxwqr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qjfqudlq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3chzwkupz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ibntzgxa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ylolelcu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3oppripte.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tupcedsp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xgpwyxfs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3baitjzwf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wbmciskd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svscumdw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3txtkvkjj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vadtttkq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3isidkirg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fptvpcoz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3unxbtndq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vqndukuk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3reidyjfg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lyzkhykd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3shtmaudz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dqmzbjxc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lkayynyz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3trxxbrey.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rptoqtao.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rxkepfib.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ualtuffb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3umvdnkfm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3arsmyysh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3msuhlszx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gmxgzdrh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cogczabi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yqfaiafy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3inlkntfx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dswezwfj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nexxftjv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkqdzafy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nymrbwbf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxqmebtq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vgslprru.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3imggwrbv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tbheyksw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gxlxqebh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pouknwnm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3uylklrgo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vdsykuqt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kbkebvmu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dlxqlsmi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oocsveqq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ayididfe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3duecwipr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qicvkede.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lmviizaz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ankxjcvx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kmistwxb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vcrvvrre.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vcuapbex.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jvbzgpgl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kodojjzp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rvstlvgc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3paruytuu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3emidotxi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qxchmyxt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wptsrzlr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xotrvybv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hzrpxfdj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3umhiimfm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3haeimyan.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3advfpwng.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lhnolykn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hjmrfaei.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zxcrqmaw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrhzgaap.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kkvwkwpu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukbmpqra.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eluztfvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zloyovcn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yyywcuvo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mlerbllr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zdlhyuwm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ysqrxlgr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mbsvnxvj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yylynavz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3txtjkeht.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kzghjcqw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kvaxmcix.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hgoswypj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ibiwgdtz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pclblfwe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrchvphw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nyhlfrrk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zdfbrhdg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zkvwnidt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ihhmgxkq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3egncvaui.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ieubzypu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ntpvpitw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ypnliqvq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tpjlonnl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3efruzteb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3egajjuqh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xfspgnvf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3npfofjxq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rreykzcd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lsucajji.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bfaixshy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ppfdcsks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3agdhgxji.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dtgrhjqi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnowcn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3adaaydau.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3blcgsnxo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uqilmpar.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wsbyqrwx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dohkovwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mcxsryzd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jxdsjwee.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3whasiqty.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gcigdisk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhbyanwr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kddqwufg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3anrwmhlk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cxidjksx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gkfflyca.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jvqspmyp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vnlipdut.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3slymlocs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bngecnek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qposltux.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hogyleca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imskujuz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skcaglbg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xsswzlev.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3srgprzzm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vidhgiet.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bwjkngek.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wmbuevrf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dhhzpqkx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dikdmgpf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vjkeqfga.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hmjrtxhe.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dftfzbkz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ydoznkmt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3etthtfgh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ucyyahrl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xuxctcay.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ahfszpsk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lnfqfoif.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pozhrbtb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lnlqzljf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kcmmcruw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3sdqziocb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zcpvcnqn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zciymdmr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fypsgqje.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3euyybnbu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3altexwuo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3liymthei.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ciyjenpc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tzgmlllw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvalhlu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxdivbrb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xwoehuoq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zcfjfraq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oceklfej.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jtudflky.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cowacwkl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vajmwdin.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3urrjghxs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kvcwjxjb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmstwgd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ubyuyrah.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wvzuripx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fzoyvehw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nrvwiseu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fakmgtkh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dhunfwma.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bwjgmixi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qcwwrges.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vkbtojwj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnxabut.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zgfznvih.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cufjcqjk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wzxjlxqb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wwupmepf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mreuwwnj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxrnfra.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wnnvvxtz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3nkvdtpvv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ozhpbqai.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dtanswip.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uiilnahs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bznjwnap.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nvwefwcb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3imbgjujd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3izluahdy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ndokvyyc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3cstsgstb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ktswdtfv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ifskclau.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qcgocrvn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yxmwcuss.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jexfztnm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kbmpxbfn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xefbudqg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mzcglkxj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ykkygpgm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xjordoei.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3omehjguc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dzrdgcyj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3eomdblcz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwarrdnn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zugcqrpe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wtwijvix.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nskectsf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3guvtexwt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rwnkskdt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ihstzuyk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okngwiwy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqmdlxzy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vtpkmdjn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3grwnsvml.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bkgfghhc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ptgkbzxo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvohbvws.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vlfqchbz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vylctvmk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3scsiysjn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjcxvqyz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoolpveh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ksjmwddu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lqosioed.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ffwcanul.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ljjzrbwz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aweyeabz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3natefzqy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmnvobcr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lolequju.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mhomghvo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygoaofpl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lscucmdx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3sdzmnghx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3glecdwao.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3luprjuvb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqrqyxko.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gntrwbdv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3shghtffp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fdecgtcd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gglmonlz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wgxvwnrt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mrmfccbu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3abuygzhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlibdfbp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yhrkgjfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xivcxsjk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jznceoyf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ejweckle.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3sxphljbb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kqnnscit.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qgcdmbyj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3htmykqfn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ltqllfyc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ywvtfvjh.html


<!-- 参考信息 -->