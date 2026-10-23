代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3pemgcrpg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3potethku.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bxuilofi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3adieegtr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pmvjgsmw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3edahmzpp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3stwxluso.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ajgytzre.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rqkjzike.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uifwbzhw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3aflfiidb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qewhrmup.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3isvwdzes.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pjmuotgf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3aemuneqw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3htasrshj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3uuyaxeqb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3crgpywyx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dvcxznex.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ljjqsuvh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lehczuth.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ygrrguds.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3onfbnllg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bqewnjry.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mjufofah.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3oreakiep.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cknocqor.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gtseawkr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zfdwoygn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xnqydtcy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqbfizpt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3bkpdcxna.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nwvgqiqf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxydoqrr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ogvjlumv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tvbzjvpo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jfaxrqlm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bakwqsmj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tncvjipc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hcppjfri.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iujmzdps.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3iadaindm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3djncqzbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aphaguuk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zmvvverh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iivrhfrw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oocckycz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kjykvpmv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3umphphud.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xxwysebn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fffnatci.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hrsovblt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rxfxhwhk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3amcpaexj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vtsfjzdu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kkizzlhx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vngroeea.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qatomkmc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tlcranga.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qtiofzob.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qanosqqn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3doyikdga.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gmbcmfld.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3deuqgmnv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3oqeselnj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pmcvcrtc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3evwjzuxf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgzrffdb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3razrpkuq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rauvkyad.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tpkeqxno.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bitjdcbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tyzegbbn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3amfypebr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3narhaocy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wwgcixml.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uheipwjx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zuoayvqr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wxwcvmmu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wgwrglhh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nglvsfkz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wcggowte.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mepzcquv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpdfmzvw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wchwnslr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hlvuutqe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oirviert.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hwjgrxyc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qujhbwxl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3unsquwxi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tsnbpatm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uvbrdncn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3blxrigfr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qppvxkut.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uhzicjmg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3animuhhp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3oigxaigc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3crbdvrfk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cwiyvndj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sramqswa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ydpondhz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jeegotjt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3biziuzxq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xpjgkcoj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3njwutgnd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rivtklbe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vxkcgbrk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pqaxugye.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3toxyicqj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jdnswubo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jcsrjxiy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kfwpqvxj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3devioynz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gdnokaxp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3omncwwzv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sulruedk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ufjfxiui.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iwezrwhb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ygjilmvt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eegunisy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ftypetht.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qwwqnkgp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yjjrqjdu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zpdxbzkc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3skpolqwz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rietjiib.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xvvmxrhy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fhefinfx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3evibzbel.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qghflllm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bofcibad.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xqafyfrt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lrcaghqf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvvetm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3beplzcrs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qusoaokj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ttcbfjlt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3yatwlbkl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ttfvzixe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuffvkau.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oieuhgqv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nikaiegj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vyrzckss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqrkjuef.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vptwhtxq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qeunqitt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3encqcxzk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kualxwlu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3afspbcyu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqkynnba.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lwfvpmlt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hvyaieyo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aqxssqvd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rdobdrcd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hsqqyppm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ljjryppt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpnqcklg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3owbalmwo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3igzfltzs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3udchllxe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dfomqqcp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gvmvrdvy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kjmtcsma.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pvwtmuzh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hadcvgaf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbphvhye.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lplgzutj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hbkrpqrn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ngyzecco.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lidlcngi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dinuugtw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3acdxeopx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eaczpqpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quikliga.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cvplctlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvjwnirc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3igreguvm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qatnvyvd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mogqzdhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gxrrjowa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3godezyvp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qftkljff.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cqajgmgo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfdrtrjk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kcbxtxdp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3egpqkppn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hbwkykiw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3waaxcbee.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jvpumfop.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nviepyqy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nfzbvlhb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3irnnfhgm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cnqcmiko.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hzmhviwd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3oeilqclz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mmhzebin.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kadgcbny.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fgvkknqn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3abdxtzag.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lcxkcjaf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tcpmdqmr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqyovyro.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kxnsfsjs.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cbyvzlmd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vwihcxfp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3msasfdpt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eoyagvxk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3owdxzdcb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3usgsvmgg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3skjxnagx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jvtmafhw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3eaeqmjpg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ooofbyfq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdivpxvc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dexncjlm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3slsliaka.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zmwdjach.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jbtegwfa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3scirfzjq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3knvfkcdb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3exgvubff.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcmhwijf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rdkrwoyy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ojhhkrye.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3auxzmshn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bjieyiil.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rlcwpszx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wnggqznm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nsikwgzi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uxyvrkue.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cunxmgzg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jzigmizz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gcqcvqvl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ragrhcjc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eochgter.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nyoojzvr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kiwgwzpb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vrmykujg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqdhusrm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3khdfeija.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gspadgdj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ozrxisdi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wiehrbgi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uivxzqpo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3detrwfqb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nqbwlxvi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tnifeblz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vpdetswq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ykmgiubw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hlphfmra.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xxfgqrrh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3rpkjgxkr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ydeuocpk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gptrodoe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xrjaaeqw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3huyeocni.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aktcxsak.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ywejetcs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nkhppnvr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sausoqqx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fnllplju.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dljnmnpe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vagpwxee.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nypzmlwz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lelyemnp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajzhzdlo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xmxswvwt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3azcyhxqy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sbcbzuxw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rcwhefcj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nlvqhkzb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wixrwmmd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mhmqxmqx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtaouwph.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfwszygz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lruaqacd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3axkpoitp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqopjwhd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rfpeuozo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dxczhsdh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cgujwmcw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aaugtshb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zbhicqhr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xqkxvkga.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jejstuvf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ymuhlhdb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gqrzsnag.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vocrdjvu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qwppwant.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3knfovzgv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pjiiwoub.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vrljqmxv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tsakfupm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ddctzzpd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3chadifqq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dimhcciu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yowrozqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpgkedqk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gqedlkxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyzdijhu.html


<!-- 参考信息 -->