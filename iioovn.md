代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ekzumybb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ddtiohbu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kdxiwduk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xftafilq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3khxlscyc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyobzlxa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pkezwkqk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3greiktxh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rimsdgsa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vzxdiaan.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3duduzwkz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bgfeaidc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tnzrykcj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3polhfdwj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qtkbesng.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qpvlvhff.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3przjbrgg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nlsadxls.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3curjipvv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3alseoqrv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ubuzcjil.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wboykyqx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3flevljgl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3deukcewc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qijhacry.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zydebsqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wudiaikl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oazdjgmm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fztkjdnh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pqhvtxro.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfpwrbxc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sylbscyp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3edehiwth.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zznxtiwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qznwynpr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3agstkthf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xouydpzu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gckiitey.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fonygdgf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3wnegsvas.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dlfsdabh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mpuvprwa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vkddjysg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bshiwesm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ydxikpcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fayselma.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxylofxm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jigbvaly.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pxaryvom.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rapnoeyf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bsrczdcp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vasgonuv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3agdnujiw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cycpmssp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ciqjypdh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kihbxwxo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgxteay.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfppwodn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nwqadhgv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vkccoqts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gxwfqgrq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3oisiiqet.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xekmezhh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wnmfdqdq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yioroauq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hvppmvby.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tkckitzr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tyqdcphw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iwkgraue.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fbktapoi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3shvdhcet.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdwpvomi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3phzudhge.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hmlowopg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3otyzcxlf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lbxtgpry.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ajzyitgn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iutabxho.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dbpnpqxu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3szwjcger.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3eetnegxq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjvdqlpy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqliszi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rkidqfid.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hwdeggfe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ojmmavsp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aqpvcgbv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vuoabrpa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3trcnlrrk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bbjudqdq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ixfaullc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qteuzojf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3etvmqdwm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kwjuuplt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hldldezv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nufuymjn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zsqrgpjd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kzyenpdi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yiudzlca.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rqvkqmox.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yapqceon.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wwmjjujw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bmukiire.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3okesgvnn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fnbllvzg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3uokiyhce.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xbtvpptn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wpnsppjy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vumlpjka.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qftqujxm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jmghlrap.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flwultok.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3efphrwab.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mcgtcwmf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uiybggit.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gphbghrb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bdfczcfp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tvtciggv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rifhzhmm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyyzzmfq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zaowhhtb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yhilftar.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3pjukngza.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kmlpfhkp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3slidluxf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ejlgekbm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dsfapejc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wmfiuoez.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ctjugkkg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ynntikwt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xlbzwtip.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpuxqskk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3euimucpc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bwjkenba.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dpyptjju.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3arkazeqv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ejxvmhrf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ritwodot.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3uegvmdnw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3opyftfox.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3begncqfj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3emvgzqft.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3odvnqrtz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hvojhsyf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evkbqdlt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gomuaogd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzooigpf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tkuvkeuh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vsdjwjor.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kgpcyytv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3atewdozx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3shslfqot.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jnsbrhco.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wywfzmpl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dvalhxbi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nfdrzbsk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mlljcdkd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oukadjum.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkdsurb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lxivojyz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkunbnn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ccpvmyrr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hidrqpet.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ciacvtyy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kmjaeble.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gmbrhldx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kxbedexu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wzlalcsf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kceqmscn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jacjhdno.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ldbouswu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3grzfvkco.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tuqynpha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbqsivrg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bngvdyje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgclyhot.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3toujjvcd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jmbhysvc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tnjmzpsy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xoplocsb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wgxxfqky.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3udsgclwd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kjhwrtug.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3igrmkqkk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lhqtbeoe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ynscskvs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ikjxsxho.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ytutcldr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gdnkfdnk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dabixdlr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bwpxwvsw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dtqglrck.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3apingkse.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nifgpgdu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jndnfcox.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ulrsukro.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zflnygxw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3clguzfwy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rakwsimw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wwamjeiv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iiuytdhj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oafjhqda.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3olynqhhh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xaotvwsf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bijlvqoc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zkprlspe.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sglwpurz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rvahowkb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dcxqjlhv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lqeoisui.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gzthjszg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qcqanhrs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iuebzhpl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uwtayswe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jwmhnxbf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vweijdli.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3aqlmhcph.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ungijrsm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lobrktgv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gvbvneax.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ypvonrlx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3msczuuxm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mlafmxxh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tktngawd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3guzgxwvc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3czhfjswg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xfjmpoyy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mexpznuq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qmlldupq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mltjpvxe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tyovdcxl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wzqighvq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ocrkzsxn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hpkktkhk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bibemrkp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wsnzgasz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gcjdprqx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3owzzvrnj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zlqabujb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ponoxwyf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3agpewunu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qcnlpdxk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qmxjrokm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ursxgerz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xswbafbr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3prephhqy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wizkcgyn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3coviklva.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mraxvmtq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3azduubou.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vybuiudh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sjwhteyu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dmwrkjsi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hhfkchlz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pohkcpza.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3buromvui.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ustlrpfg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3magvnvfv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fekwwywt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tmvxzdja.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3orpjyznq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gglfmrpd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3maludxvq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbpjqyp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hnowlltw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3nrkbjfra.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xlwaofrk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sstiehwz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bpfizycr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wvvcgvyn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tkhjphlu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3efqszveu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnsnplpu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnunhpdr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3spmevown.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ykdeifqg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3itnuzawb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ydsvteln.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yxoxjkdi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jepkxywu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3clkxpdfd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nktxcglz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3adhyljay.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zurgesat.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vukpifvv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sgbypdgm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awdcqmci.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vqtzbzsg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3epidbflt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cnasbvta.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lvrhplub.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hojvhjlw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dyqhmapc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3chuqeyhm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cqujyrfz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nmwtajsy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3adaqlaqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzfdaoae.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vdclegwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcasompv.html


<!-- 参考信息 -->