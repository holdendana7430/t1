代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3elvwfstr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3azdylrjd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jqpkpjum.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yxzipejd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rxbersyo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dqpurbol.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mjlgayks.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zpxnbfdh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3emiqlpvt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sljggemk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3unxfucnm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nnlwvifd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3upvcasau.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xhxxvzsd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qsymcist.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3eommtray.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bltqruen.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3yvbmotcl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqddroim.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iankgjvz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3haxonfkz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcvkfgiz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xttldzwl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cbfjeuxm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pmdxhzjv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pceftmkr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3npbgdjpb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3semwvcqv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sbbrckqa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rdajrokn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sdeqjofs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvnspdoh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nanghgnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocxxxxhl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mrzmshgs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bttmkmka.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lzxxikgb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wnkytmke.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vlrsgjsn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3snehtlpn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hiqactqo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dfbffjui.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ghspigus.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dzyrbpgr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xjlonjfz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nsxgbkml.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tiojlucu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bhdshetm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tmqpibub.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gglsekhr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3irslgexm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3drinayws.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3oqqiktjc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tsqpytyq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eufxndqp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ichgpyci.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3anvrvoqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzlweaf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nvlikppv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iocbaygr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dgzrnuek.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wnaejkyr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yvzjhmnz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fernhikf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mymtfhuu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dxfdqptn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oocevdeb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ydddlebk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wrioxvnn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rvhjgwsp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jpczzzny.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3geajcijo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dipjlttt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wxlfyqnh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lpbekopd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mdpmtwpu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ctnwyzvc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vnopyoxu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lyosbztr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dkkbbukv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jpihykjt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yqmwkszx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bheldmld.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hhhaebee.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kbxtthbr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ihtheejq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3whxshcuk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iivuwoac.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fmmgnukj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3frlsnaxc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfjyprle.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lbowvfis.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tmroxglc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3njmwzlaa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fpjomqsr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3atjoxcvj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3metbktns.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3plbcfqru.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dnccsdll.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cvmmmkuw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hmoatqyh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhncxzf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhtcepbq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3asnvgymp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qtwnbais.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qmgazgso.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ijbmfobt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdtkkpjf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3afplqokq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kqxjlzue.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xxjgejcz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bjfkgitp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3oqmhliai.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3msjvogal.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nyalkurz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kaoubwyq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ujykcrac.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3exevyarr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dzutidvi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lcsoyatj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhngnjeg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ifeirxys.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bkccaahp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3udvolnlw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ntnebdfl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eccdiivm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yjromzsy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbrpahtl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fiwgtmfg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3okrueprb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cjfzuhob.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rhltxejz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xmyoujme.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hulpjtfe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqvgdmua.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3joanatpj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vonehavl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ctvzgptq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tafzgnhd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dygxcbyk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yazkmole.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wyyakzhh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3otrbvczn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uuxjoiuo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vrohmpcs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nzjtlsbc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cgssjhfh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3sqoujimj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qhvxgsbo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jtvjvoii.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sljefkih.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pfqhwuwt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3onbtcbvv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3firiuhje.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3smwmaswu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eljrfuxk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmqqmrz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nyvstmug.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mibpqmzi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mutixijt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lehlbksi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgoxienc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jlnwkchg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lusdeyqp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jtgflsew.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oultocys.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ezyozyiq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3eqlgamtm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3paevghob.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3djqthvfm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3clgjuoem.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tryoofmm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pyqsztko.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3odvojycf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lxksymza.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocosuybv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eiekxrae.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ltgleuyg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bwroimua.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3whjqmhcg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3glfthgsh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jcvqubio.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ywkgycbe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oacfltvo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wjktqaah.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ufogueqp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ilhqupis.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tartiujr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jnobrqtz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwpmafb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3irafhnms.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nkjykavl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lhkawbwf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wttifyth.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyrimhoz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lahyfcvh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jbypliue.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dtdhamur.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3biukwypm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3slovpvfh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ugvtzuyi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3syatwqxy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nvvrwkqi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pvlswdqq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kqnmfffl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zattslbk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3sliaozqn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kgohjqtb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xaqbncmh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3byjekvbt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yybngqry.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bvhqjdqu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vsjpcicm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mohwifzx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fupvwxum.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmbxytc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vdtxaytp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ajwuywda.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jktzluiy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3auqjhrld.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3enlfvnbk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wtagtlnh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ievcqfwz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gomktkdp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pwddluoe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ebonbiwu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3roossvqv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkqnwhrj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ecmhxlgb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3flfrtxtm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dttumgva.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xaqyshpp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kbzspdqo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nokcbrwx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsndcfsq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3aeibursm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wiuriwlq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jvzxjbgz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fnaeeinp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aftuaydu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zxmdzubi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cnvelbep.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3glrtlipf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xxhrpizd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gkmrpgta.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bpxrwlcn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qqjwylgl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jmxjrjqe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vwdotajs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wanqmoln.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3kcmqwkcl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pitdsnwu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3psrfsoqd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wmgqpzsp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bjcvckkp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdedftce.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3uywvyxgb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3elvroeuc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mubgxwox.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wssoheah.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuvqkqwo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgyknfbi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cvlsyrth.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fidrmuho.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lbjdsdye.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3unwriloq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rkpsjusr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zhagqmtk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qftiufpm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fkiquqdx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ajkzunvt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3psxmpqsx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbhaayv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wmxxuziw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewklbopf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kghjsjnc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bjaydywv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pjcxpshc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjtafiwm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hhaffalu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wusyzqwo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qpklyoiu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3baalksaa.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hyqtwdrk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vpslsxzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkelbpiw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omwsxryn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agvllquf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ivigjayu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fkomlpqz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wyuzkjkc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wlnbbhsm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wtutcuqa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3swwemezq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hfolxmvl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rhcmfovu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3usshbrjw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ufjlzhmk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lqrxcrjc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cuubesxr.html


<!-- 参考信息 -->