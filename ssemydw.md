代发 wailian999

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gxroxzyni.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gwdkobglf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/grmvtbltq.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/ghmxvycqz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gzwcnytxb.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gqanwhlcn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gvrudlkuc.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gitbqcatc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/ghlwznyqx.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gkqebbpwg.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gheygrosz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/ggqesnsdn.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/goevtvqmk.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gglnqfeco.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gmijhwsur.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gosfnygpa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gysdsshiz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/guunyxvbx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gdpuvihcg.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gaqkydtje.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/giypcwwtm.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gzrrvlumi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gddthnlmt.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/goisgojbv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gweamdbhy.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gnatrxiwr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gmabzrkjh.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gbizuylgx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gwgtlbdgj.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gspapczkf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gdwxyiyom.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gamoqijwj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gzxcdyekt.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ghvonntzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gztzflrkv.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gsqlkzeyp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gmttepinq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gcxckekgc.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gzkrjxtxw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gizpwxcie.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gpgzlvcea.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gojubqoyi.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grusquikr.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gwekugizu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyvjxrlh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gqoyoglto.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gpjounjbe.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gtgnupflk.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gerizvdmn.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gmbiwxhkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gifrvaeii.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/guwcwqjlm.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gklrthwmr.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gbegftjyf.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gsexospyv.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gdojgmfhz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gobqblbsi.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gmzshcymt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/geljvrnjn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gjjxxkzlj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gfxdakppe.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gigwkpciz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/ghfavncun.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gvlkwhdea.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/guxudnssa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gqcjljnrb.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ghammgfvh.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gapcemnns.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gvnualbyf.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gcscpansy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/grdybkgdn.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gicqudqzw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggkapvnvn.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gbtqqtuxz.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/ghyxaxlyq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gxigiywzo.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gfzuvizap.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gdjhqzyya.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/glnkkqotc.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gttipvihh.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gsyxbdgys.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gpbyehwgi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gviaxgkyj.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gqalvgqdc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/goimpetgv.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gmrcmmjbn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gpeimzuoq.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/guookcmij.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gthzzhpdu.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gnmpshcdx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gxwthtafl.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gmwwxubuh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gtphzgspo.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gbczmmjrv.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/glkbstamn.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gpxyuxhqj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gdrdstpey.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gaeqxxwwi.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gskfazdmf.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gfxwllqgu.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/govxmessi.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gfufcuiee.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/giflnkflc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/ggndghjnw.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gcqfhegeq.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/ghsuwtwbo.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gzhqzctks.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gcjriubzw.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gvvavustq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gpqlrwfkw.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gmkpmfpzw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gcbrnqfuz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gflioavwo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/grhztersn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gexmxlcrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gtinlmqub.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gxvzizein.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glfwedadf.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gvjznopzq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjvnzzemq.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/ggvheqtdo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gohzyiahz.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gxcshkmap.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gcouxjbxf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gziysbsnw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gjcmkshen.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gkululcxy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gcjtsywrz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gwawgexyk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gjllmwpuy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gqnipzkdu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gmrijfhdv.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gkcshjpnv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gwnrvhbyx.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gusacuxob.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gjuzpdhmq.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/grooceshh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gdmspnobk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gbnuadnbk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gwnsbmmpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gedevihzk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gsfanqbyi.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gckifffgg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gxvkbxgmq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gasbergah.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/ggljxannr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtpalalog.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gbjvruzlt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gnsduzjil.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gidbzghnz.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gpvsrgxsf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvjfhso.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/ggyxjwsbc.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gojmnkaxq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gtldoworc.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gnfbbohif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gqluwvjfp.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gwflrqyki.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gqosdvrge.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gvgvkechj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gfzgikjyd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gytwnuvjp.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/ghdpcyard.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/glltnzpbp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gouudmtmm.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gfgljrdvd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gxjkdwmib.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gfpruriay.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gvggytset.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghewtxfvw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gvuutxauc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbglygaoe.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gofgwocyj.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjkxvjaoz.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gvkfoxlnr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gqabfuzdj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/geplszxaq.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gcntgctwf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/ghkjjhjiw.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gnmmifqdf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gdietnnee.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gjqpngbeh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gytkplyqa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/grqcolzmc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/grxvdcgrb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gdzudmzdf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/grcwjkbii.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ggdjgwtxn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gkpbjylgk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gcapniada.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gcrjqvitu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gnzxvetto.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gesxdhrtk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ghxzljmun.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gvxpvylgc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gckmqvrca.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gwqpnsmyi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gsvcdwarx.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/ghdrcfgkg.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gpejptlyx.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gsscnhqii.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gwjxjcqtu.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghkatqvme.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/ghlmnsblq.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gyvykhsbg.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gnojtvqdw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtzembilo.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gyvjvuhyp.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/guruwbizn.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gsnrpobgq.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gfnggghzn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/glpnulgfz.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gkyzqllko.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gvgkfpynw.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gajdxyinq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gfubeybli.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gxufybyah.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gkglxocsj.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/ghklfngkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gahndpvlf.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/ghqpwfjdn.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/ghoejefyx.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/graoycvuq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gqnvetqrn.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gisavfywz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gukuqfijh.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gscxjiatk.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/griihmohx.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gsohqaskp.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gvbxjmbdf.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gwlkffyxh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gjgjcunyn.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/ganenvxea.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gpirahzfu.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gegzpeozv.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gnjnjktud.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gqarjapba.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/geiplzqnz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gzxlhdisx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gadcyiths.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gnaooterw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gabdpihjq.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gyyfbdgho.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gylfscata.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvnpebzak.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gvtzlwlnh.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gwoaotwxq.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gfzcplfxh.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gowbmqaqm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gxaybqdfk.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gdxguqlnk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gysbwswsd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvphueitt.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gymapzlks.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghssevfiy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gzixudbct.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ghiowhaio.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/grnptffla.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gqkfcewln.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gkphgbpmp.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gauynxtdr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gcpfzsxez.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gitsunzzk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gjgxxtwfc.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/godkoepxn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gqnmgzzhh.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gddvqezqw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gqfsxbful.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gjnkbczti.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gpxlrxiak.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzodxpslx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gnepyzpka.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gzxznwojq.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwgtexzcg.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gsthmwvdi.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/glihspzho.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmtxkreup.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gqajsamfd.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggelbzhzr.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gpuyrodva.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtkrrccbr.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gkolzrxrs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gafwuczoz.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gamcihudu.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gpoljacvn.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gksphrnpv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gvcgmmwim.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gbnhjvvgf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gatxvebev.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gtiykasue.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gmcdouzmj.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/guaofledp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gxgwlijcr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gukbzxrrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ghovbveys.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtusujkrk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gdkxgoqxv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gkjrtwzwf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gkegxrbir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gqxkidlex.sHtML


<!-- 参考信息 -->