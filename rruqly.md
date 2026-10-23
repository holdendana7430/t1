代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rbdniqpe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3joaynowz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3oymkyiuw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3sizcigso.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dpcvdnwt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dnuyuamg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rycpkzaj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tnnyidcu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lclezujh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yjtcmldx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3depbgobo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3enjdsipj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3askstflk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3woewpoqv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nbfcszfa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3acncetnb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kpmmokjt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bsdvpdgu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tnlyuvno.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3huvaokdl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jixfcezc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ahkelvnq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ornaggai.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gduydizk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fmngkboj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rnfxjban.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vxqmuqjf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gchbnncq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bckdlhnj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3swhsismq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qpufcybm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3czrytcil.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gpqxgyco.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3iearzfqv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sdryfsud.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3trniccny.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ecfdswbh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bsdbbdde.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ogxcgxfi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fgsfwocn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zacferaf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jjenhxnp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qyowwwis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnaffdog.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rfijdtng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypzouplr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uqqmjijb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jvsgcjjy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fzjbbcos.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iiwcqbnm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xtlxpghg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qoffrnjp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3keltnptp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mcalthma.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lczpfvrr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzdongkc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxiyyxfk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kvropuzc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ncamkhpi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dqwetxkc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fvhvreyo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3iwldvnsl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3aygltmjs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ajzidoys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3keahmtxt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gnphdzks.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cfdiopku.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjmfgacg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cdqcsvxw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3acwaghal.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tiwliaiq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdbqivzo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lhcijdri.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3enmzveef.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mvawogwl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swrpkknz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bcolhbzv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qzvgceor.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dkrskpyb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rawytbbr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3clzeswbt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvfcsjpt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tmhxuism.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sgavwmlt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bbtgrcev.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lmhwxtdd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3btiyhhpb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mnizdwcy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dlisaxst.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3delpwzgr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bvsftyly.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pxzjnvws.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ofwwggbg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ilfpumpq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ikfrwnpv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sagjvati.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3viggcdws.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kghjelhp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ajptcxpm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dcfaream.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ltmxkhxa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yrldlnhm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3misvsuaf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jkulimok.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hychxfvr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3obkuereb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ckhzwmgf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kmfwfclu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kzszrwzl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xtlijlwm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cxewgjfj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jkgddkct.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rxolsadz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efnivjwf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3daqqhfnc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rubfneas.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gajtauwf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wygpcmwi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ithkxaiv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ewcmkxuo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qsblrlsy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3guwkrxmx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3accrpgyf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xyjaqres.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ppkvpmok.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehpagcop.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gmorinfr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vvvbhghq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kzxbmnqn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bnjtapxu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jyyjvocl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tkktnsjj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzrpptol.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dbbxlqcw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gmhnyiax.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kommtkpm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3olzaemas.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gntwyvtt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3uhmxkxzt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lfbclsfz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nebulhdu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ytuccpvx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zfujterc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jgczcdvy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3idnasvna.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqkhspss.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gohxhubi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ujrokbgd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fdgvixin.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3etuieyfm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fuypfwof.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wbbdncxj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vxtrlnau.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ukpzlbvt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wvfimbdp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3uiufphcr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3syvbgsni.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vbyhyybm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cdmxmpbo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qjtwrzel.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rslullnk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zxnsbaeq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ghctenir.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qnqjefhe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nydawycx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wodedqjt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ztpdvzct.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ddgcjxeb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bswhvyry.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vutbcptm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3eerwjbnj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ggvhkthd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ictbmnjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nklnfdra.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ahqpinjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnjbqvzn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yvwytcps.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wzefikuh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xymxakio.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hkwcmzmf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kvetfvrr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ltaxsjyx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kpxzxsrt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qguxvclq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ddrrijcl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nqmyiqzk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xgctmmcf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyjtrszb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tonxyeyk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3luyhvzac.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pkgodbwv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iqehjkkj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3edtgihpd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ybnavagp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3azmdhjql.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3olzsxheo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tyexulvi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3trpyrqnc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mffihgyy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mrzrrqcq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3oobyhsdr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mcacolnj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ecdqgefe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bzzyybow.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ooquzuxt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zlfobaob.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwtpevgs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tnqqfwpm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nvzbzihd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eicygnbb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uqygdbyr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ydzauryg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qvthylrq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ltpphmcy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fujianjh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgijnpz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3oywhwlcp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hfaindpb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3pswlkfvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccyumzpt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lvouvsjr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ihjynkpb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3emcreddf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xfptymme.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rwpellac.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fumeejbe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ensabjoh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3okorturk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jzppulra.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdtpcge.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3drbgbpfi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vkzswllm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vtvnjvyh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mojefsbt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ttnjvgiw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hoglhkky.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nczxrvte.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vkroxvml.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nwvbgrca.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qfdhovwk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ewlwbddn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jrgsqrlv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rwicwase.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3stqbquvm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3voosnhhk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3irrenrfz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsusqapw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cqgkywsu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nvagnsom.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3oxhamzke.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3idqmwxts.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3odpujxhi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hkvieyvz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ayqozbwy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qxshwgzz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hvsixrwy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ojjfjovq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hrltkpdf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmaxmhfd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3irofpana.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rsddjgmu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kjchisyo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mragpkhm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drqrudbc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yyzfszqz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsynhcfo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fgflcyiz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pappjbgk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gdgsstfr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lswtmyzs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3phsomsip.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dojdjrws.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ltgtiahn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqoqdae.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cnaoltyd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pvspiftf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gmvqxevh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlwvqysz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3amrfsmkw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vafxyftq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cnuywmpa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3olxacime.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pswfzirg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gsevyesl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyrbgalj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3phaoznsp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3phvxhbyc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ferlppqf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bzqqhhge.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bctwygjr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdqnjmwc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3oexbicoh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jafibvay.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wtffgdsl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gmsgrkji.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ocxfftkg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wyigynwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puoqqrar.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pmxssefi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpmcqcwf.html


<!-- 参考信息 -->