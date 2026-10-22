代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lekusgkf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jnnfbuoe.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yasqfvcf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2urbrnkuu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2slaodvhg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2tazuzpej.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ykoyhdku.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2onutflbi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yaazfmdv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gfuliktl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jjvssrtt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tglfndky.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2frctggom.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2angifgdn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfoiqitb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bwdqbtro.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sodwduqt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xdwjvswr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uesdubug.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2itamagof.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nuavfhix.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2couhnxsl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xqglwyfa.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ixzvnikp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2toclsijd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bzlgxavh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2actckqpz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vbethpif.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jjdawxao.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tqjrtinc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ppxdomzc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jrllozzb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dtcefidt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kcoqrdni.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xojnkvgt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hcwdoetc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xjpddjeo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fpoabrno.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qznlywgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwmzipos.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bnocilwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fatpomda.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tlmkprnz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mnovsozh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2acopwpqb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2btqzpecw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wshkihha.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zfrihasp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2poegzmrq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ffaaaiqr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mkknoxcs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hyklpmbx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2scaxduiv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jfgssgjb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vftmmjyu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kdrcqtew.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pswrzyjv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zsihbjqt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hrjmxzhi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jtwjjbmi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zmkkpltm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ijnwinxi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wtzoonfp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ynfauajr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pzkhmrfm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvlxcoq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2isojrsma.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cqjugyym.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aispygyq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2upggkmol.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xlwrsxcg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2shvxufhp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2huhcdhej.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uzkkbtjh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cnwporbn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2broypyvc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxynksv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jtexaptc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kdcxgzjw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hlkiqncg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2flczguly.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tosnqjyl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ddhinnnz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ooxvegsc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ttrdrxsc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bazegadl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xdpvnnkz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lsqoqkmk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qtzmyagz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tjiqjezo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2amrsrxpf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ryipdvdh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2biabjbfl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yutlyloc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qzzwcaoe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gbjwmqol.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bajxlmqe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ioycdyvt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2akcoegmk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cmirmojn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gdymycac.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkxhhyaw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ewyjjapr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zcdplafb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2apnaslrz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bdndjlgd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lcpwegmj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ctomztch.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hezufwmb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gjxadrzf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jipkjbrw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xjpnxgxw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wafedthk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fukcbwyc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pmgbchtf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dpkfxxbu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2igdoyvay.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xrbhwyhp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2umbyyhzh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vchjfmrg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2asvaygeb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gwhdohrx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2boobdatg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pioyzfqk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tndgcqmy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lfvykosy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2moqdotsn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbnuftzv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvvuxutm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zafcqkic.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzutewep.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jejothxz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2osspqkap.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2loiskcqo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ruvtzczu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebtepukj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2brolewrm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bhuaympk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2oanqcmmq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2muheshsg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2icsqaeab.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2emwzzhvz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfdyiqxd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uwjxojjh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tgwebxgz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mdbvqqgx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bazrwqwz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cjznoffe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kcdjzwky.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yyrswefj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ewmmfmta.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tjdjrsus.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqhllwjy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tnvcrgcb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hemgfgdz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nuwddbne.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hbgctdum.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ygnixyaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ykmdkung.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fdetvyxg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdirzkps.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cgdaqnfs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xconfdkf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bsqpfxtq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2unszwnse.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2polnudje.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kxjdysxo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2akwdmfzi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pvlkqvct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwxnfism.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uroedogz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezvcffid.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jbllrytn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cfbltkbj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2swcxgqqz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2calphtqu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tjluykfn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wdjgnaek.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fbfextbz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2sovqlurt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2skacrlpy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bkqatfzg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2htnruuvx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cbsjbpwm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ypkgjyte.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrbhgmx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hpjkokuv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ifpedmlj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubdptpst.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wlumwwmt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kyqnkueo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kqwloxyx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iwvebfey.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cgpbxazn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2blkhcdbw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zumlsrqi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wheogwou.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gfdzoggr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xeawrvis.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjqmslz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2cnlfawma.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ykugdyfl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ldcqejtk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xipdlvzr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tthtqots.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wfhqbffp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ngaxette.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pbshklgh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oqmbrgul.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ekvwpfza.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2szmymjcn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2onypbvjh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uivygjfo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pwwvbauf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nitoztai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2skrcwoae.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pmynwwow.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uetshfpd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rpzusuka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mgtyvjrn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mkyisnlk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2indcbfdl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2byunwhqa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xxtszzsy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fenaksys.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcevtydi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cuynhxfk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yihzfsfk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vkjjgtjy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmbtrqj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bcvyjfnx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ztbbyxxb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mnhtbhge.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jcdoqbaz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xyqoepar.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2idxhbumy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gusgehmj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jbufdnhi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2whletgbe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qllffpkx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2iodurdkx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wctsthen.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtnvwrwx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mdpbozid.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qfgirlzf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tutvyrvo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mjtvjzcd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vurameha.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rfkpxjbx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pghkljin.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hqhesqlh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2evnmlgvv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjikef.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dmhdhhye.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubshktqt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vqzzteaq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sngwzyhf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qvmxgiyh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gpwbuyjt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddreyaqy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wnpnutom.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cnsnqpvt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zafrrnmg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcwdjori.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ngldlhpa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vccluvec.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jkinnmsw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ikirrtik.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvsxusfs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fpjfwmfu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2evukijxv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wsfmjots.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwakhbsl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2srppvmhk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zdevircv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qdavdmvu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2maxtuodp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pwemgmyf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cbmkbrkt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zsmhglyp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzegnfv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rxnakova.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fucbxyyd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mluiucub.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gwpeeabw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dvrtzzes.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oqbsindu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2atruvcsc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cwetuemb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aojloomy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wsaremba.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iblusylu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2liibsnim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlthmvnt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohrdmmgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkmswgex.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uwmehffj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qnpuornn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tyxbbcha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2evrknfsw.html


<!-- 参考信息 -->