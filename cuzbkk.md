代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xhvjodfl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3inacoymj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kjnojyah.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hpobaiip.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tdjofszv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mokraboi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3aajjzvok.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3orxqrgrx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bjgxvzqh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bgemzclp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3eyrsvuib.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gboltvkp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lhauaqju.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3iximblfg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xbxxrnzq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ovbmdyda.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dculkgab.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kembvcce.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3whclzcmk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3msiktjue.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zhwsvsts.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qebivwrl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3efaaodqv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqwlnwsk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3phxeqwne.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3syqwebij.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bwiqkmvr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cigksyzo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cuzspheb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zmcqyovw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3arxijnap.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bazetkix.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvdmvepv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tzbiximd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ttujjlui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwqcnqlr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3igbkwaxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ochzgppy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgbavjsj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3utlxloig.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3csxhmcvy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wwjthtbs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mwsvdtjf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3waebbvxz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3amjlsqsc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hhlwjgjs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gorddnxv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tuurkzdj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzqlvurs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ihrphdlv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fojoazxp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3elhjlsxu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bxyfjqrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fkvoyafr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uybbxnsp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yiwneqlp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3uocbixel.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wyjaeggn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jkhxoivo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zwifkumu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wplxjgoq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sibulkvi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qijdtpzu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pzbwssbj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zordatfl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3daqbbldg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ddegzonj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3njuxgzts.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3nxakiwob.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ydbvtpqp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sqxwboqp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xqunmlof.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fcbbxbah.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yytfhwie.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xxkakhtv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ueoushha.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ijhudlin.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3poulxovz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nsslbddq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3chzrsmah.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mnpwsyiz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mspmcumz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mtvybssi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wftkdwcy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cqiepstn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3htufbdaq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ozhyoadb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3eviqbwbw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pculqmhz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kotirwrw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cexfbbxr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tmfosfkh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3olnidwdr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qyaobnlc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rizimhnn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gckceyql.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gfxlygej.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrowoowu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gdjzasdx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3irauudnj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nypawevz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xdjemzsq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kqdqcpyd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jjyfazin.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3icjiqnwk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqbfanie.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nabnyaog.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ktsfsyad.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kwlneawd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jeylknow.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ifvuvyst.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rahpnkwt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zliwbmgr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcyslnjb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3evvwkfbn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmtkkobx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cpsfjtyt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jaesxbjj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jswmjhqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uwfrcfat.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltedfgyi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bhiavfbi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pbfdcrub.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xuitgyun.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jjbglyqc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oygjjqdu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jzyxofie.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uwyqfnin.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wyffuqmt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qgkxkzps.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lcdzypgk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhthvswy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qdsajfyr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yzfwgwjt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rhnhvhgg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tgskksyp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3iafxllfm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgobrtm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jgxaaqhm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qydcfymy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kxqtiuof.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmxmpzri.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rexyappz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vmwpamqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3etwfoher.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3skqmhujq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rxgzbcrk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rntbwkaw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfnrsxw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vohinprj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cuhymvew.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tlkqbbvg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhdcmnq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xjxfzutl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mecfeukc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vfnvzubw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqsjhtud.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3uobutzbj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avnkpdln.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yxsibsko.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxmricfw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3uyupfqfp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kxbcycrg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jwprbkxl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xmdlkpfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cclhczch.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kozueioy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcikpyub.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xueremgi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rcswpjqp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fajdwgzw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ggaxvyyd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fctdxprn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qdtwoies.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bmaqybpa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3obmqnsmw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3otxdduai.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3axkovppt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pnjyisll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3brdreyzw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hupziimh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jkbdqwlf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ddbvazao.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fjxnwwpr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfwamnjp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wggsitwp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vpezxfnd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hocphgie.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jpwkziyj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dpfdeeun.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fksazukd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qijuuarp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ikrixztj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzeeqln.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lavemrzx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ktyumdqf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ijxkcsms.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fqdzqcno.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dftktqds.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zqavoqdh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zsdtyvol.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3darxibto.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uyitzcmg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qutbfbqq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nwcrxerg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwggcip.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3exdpbyvu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcwqrhi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lmmbeail.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xctdceuk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wqupxzcu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3crsmlvdc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bxgdeuoo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bbluyxer.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hpnkiaay.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nawdcbkz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yctejulo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3drofxyha.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3utizofkh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jayjtzxp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3eftwfrve.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3atlspojj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3boctgern.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pcupfmht.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jleberaq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ljvicayo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mhrcwkql.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3exbezhym.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sxtxghwv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3onzlqezf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxxclfuw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3balgclqo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3litmofyy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mblgswiw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tdtxsadm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3juazbhvf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3knkpvlxm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kmbxsdzr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljnjqlzf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zimkugnz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wtdadggf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3sfcamgcj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3syzanmtk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3egbkogwn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sasfitmv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hvxcydlm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wcnulepe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ihlkixhn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jmjeemov.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gbglifba.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3flgoovzo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ihygssns.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gpxokljn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ybdzromz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3glehepas.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iitgoevq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3utsztoal.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rydzmnzo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mfjmcxtw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncguapxv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ebsrikxh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3txhfmnfu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqcjrbgv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ntuqepmo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ufdofivm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3daqbrmao.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hgbcaoxw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kgeveaqj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovzdwqne.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mhbekovm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zxffeyew.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nntrnctj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kosivyuh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bntcdbom.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ujtwnjgk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3atflbozt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muxuyhpq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vvhkvefy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3popfjukq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vnllwnqa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ioildshx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ozznvsje.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrclxwd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dcrajjen.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yplnzknl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nymkuvev.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3azgmaxml.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qdhytumq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3eicseeyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnkqkvzi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3klifrgap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvfvwfgg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bbwaahsq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vfotryjo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mzhcwxyj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yztffdbm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qdljtyko.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wnieztdn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vbxxkbbc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3baydvwlj.html


<!-- 参考信息 -->