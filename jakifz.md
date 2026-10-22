代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2byikylfx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2itkokrji.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vhtvgtpb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xplwaizn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mkqgebbv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2quntoiqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tvsgkvxx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hgyvmris.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2czlfrjrm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uggtilao.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jsmqgqgl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wcktvcyd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tezgxtrx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2csebvjcm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2smmfowil.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2upasjtnn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2setyhicr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ucswemaj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2eqmreeoo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2igxvbfbt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2dceqxfec.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlnysvgi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wlmnakle.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2exibunlr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tlgrobjc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rzalnojd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lfrufsjf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mdbvvrqo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lurjyrzs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sjagwpuq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tyyvqbaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddcpvaap.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2enlhvobc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snoitrvs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjxfohaq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ceynjxku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2trqltrdi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mwvbfhif.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2byvgqjgl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gzgyvbwf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2aojnvyri.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hcrhfggk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zfgfufwd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dadgreoq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pequeqdx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bxjanhjm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vgfbnadq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2oepdhjik.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2djstprlc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fijkhaea.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wtvtwcme.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2eyvnooee.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2drfttxqu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ekfrocua.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jlctpqmp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjikxpzv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2opntlhhe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zfnvuult.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iabyotiq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqmwinwn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rgwbyrus.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2njiezkzz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xgcfpwva.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lkyzqaer.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mttwjkeo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2foeztuvt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qtzwhjfg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lvzzgsyg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hcmbohhb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsqegqjt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tchpuulj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oumkqamo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2phurknzs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2betmkxbo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ajcdsemc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xdhuagvj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2egiapbmv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2puepcsbf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2khrksdok.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aggcareh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rjuroani.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ogrsybrk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eqqqvrnl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nyraywqt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2eqrysbim.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2skagyhne.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dyvqjmmd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2stfdhcfh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gindvlwn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xmhzsnxn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2egobxwry.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tchiyggp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yyrwqwgg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2npvvkxpc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wgqqvtrb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ghonepkf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vrirwczc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zqvavzts.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rhacygvc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzackxav.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ljevrhgl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2teinjtjp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2raflldah.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qbevwbvi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ubcksixc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hvldbkwa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ykemeccp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2swpseppj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2alkalsvt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yzyozhhl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mngdqryb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwwdussp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ydmnxvsp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzssdvte.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsxctdnn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nandblzf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2trtgkfpc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vziomzny.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ujrfeyzr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jzmpskuv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2smnudmhd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sigljzqm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttllckun.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lvpspdxm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hbwbxshd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2sfsuthkw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cvhwdlfl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kknbqpak.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2scsuqufx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jmfxfjjp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qypnebse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xkjlpygd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kjbcqttg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jndcoire.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjdfjc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dctalzmy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrumofi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jlddfgbk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pjwdpxtt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bvrnaicv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vdasoush.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yppixlcs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vhdtfliy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ycofvbsr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2elbqvsxx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mrbqaebf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mlxwykrs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ncqyauye.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fszhjrbn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ivmcggcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bsetmqkm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jdszgtbo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2eczhexdm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kxvvpcfh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qajbipgw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wwxoxzsb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hpuwqpqm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mlkjgnpr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oumalfpd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vrerplaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pyxgfrzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guabtuuv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bgtgndck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpargkjt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aezllspe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ikpqpiwz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ccdcbroh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bopenvwp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kafgrskn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ifsuhqsh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cplnfbzn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2looryoko.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ooybflhi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mzmrdsab.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lbwnaejx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cfjdgcvb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2obfdhego.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ytmoxqec.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vvsfrzgg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rzejuqzm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nuvuriab.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2exqdlpgq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rmirxmtq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vgpzovzm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eleybqdx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ijpxxuir.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ujugjdqk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkyswwp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bnqqovpe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnlldnec.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wccrpaac.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qfuwdciq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ybjuhovq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ujtmixdv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfgzhsmi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pddhamug.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jcyjdsoo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jtfsmvwu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kuzylspi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2izrhzkci.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gtbsplqc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2naxwugye.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2olnutaar.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzfuoif.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yykiyich.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjnjdmbh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pjldsfrc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ibuchlqq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tfqpvlss.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhdmpps.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2psboawhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jndnwzpz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yeyurqmw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vspysasi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhtlch.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gpplimpb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ioratpnb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yfcfsnqp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hmwxzgin.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bqjpazuv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oiwynmld.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2eqwdanyy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2uwncqkbk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ziatjnac.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bgwpnavk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wnbebtpw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pfkfhpih.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ltkfjsuj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ikczwomh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2himfndag.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ajbylhbl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2skigmogs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wsqjblmn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xgjafcca.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iikjusfm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bddwkhdf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cfvazgwa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pywwaxww.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hdcpvjnd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mqtksyqt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2poqjaakc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mqxesvzp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qezbqgju.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sqlghwdp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ekjrpgkh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2frwjlolo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ekhltmsk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwynxhk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2izusgneo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cxgtsnun.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2eodsmcmw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xljqeomo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gzsrnvlx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2asjtfnjz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bikuvmys.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxrtjod.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2amxxtpbi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2prwrwmub.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bemjmtbj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nasuulix.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2srhdikal.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2klihpggt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pcbqycss.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2iawhpkdb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2detpsbrb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2efysnoxs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qovstbnu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fqhparfn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dhuiawwv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cjjhmmdh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uybdjznm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2taguvhbr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2iefnbbgb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eyxjhnxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eylkiqyj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tiphktmd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xwfpbfpd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2auzdenqv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bptqkvyb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vmnztnhq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kjsnxwpf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2avwwbioh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ewntswxv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mdnctjuu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxazdrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwmgecyq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rpwbxlst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnpkhwsk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sdijscan.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zeqanlcu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lficmarg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yxcwaepn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mnuhnsyk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2plqhameu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wzwyebzi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2giodvcle.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zrexqxmi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tyhsqkcy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uyivdbpu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbignd.html


<!-- 参考信息 -->