代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rlfpbfqf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2beapyncm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yikxqmxw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sbvnaozi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vpadtmmv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mhuloevx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wautjpya.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yygxgrjn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qkwzptrs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fjevfcgf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xsugnxzg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pwggidrg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mpddbooi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ranuhkqx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jdmwqyqm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iqoexdqr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2igybkioo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2edvlahnj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gwdjfdpb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cnlaijmj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kskuydsm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qtvfeksh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2sxauzlmo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ylnyusbc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hywshyfk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dwytdrct.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nbwvizfd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fspkocja.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xaipxydf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kcflniub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bstesoci.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jkxlafbk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nnhhnltf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qfwprsyv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2szvxkaku.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vykzgkfm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yswamtdl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mwsceuvc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2axezlqqu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2aiwwpqpz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lygbbvcs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bawamvqf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rxfktmrj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2eolvaguc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yzfvohwa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vdowzagn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2awyllreu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbvndw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qhlbehuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxijppcl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xxsipczf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vawvfbwi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tspgsqvj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wtcglsnv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2horuwesd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2shsypbab.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eonhqfxq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dayvkowi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hamdsjsi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tbztcycr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ntazsjrg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rjefyymt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vovshkom.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qgmvodul.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2smgkvjay.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2oeiskuww.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cimybbnx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pxvvjuqn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2iewprevv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2inztnhld.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qdhcabtb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptcbkzow.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dktzifgd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ibnqwedr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oghomixq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctktgzib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fnanmigg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwlaqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2baiblbnz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pfkkxvyg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qyljinvt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mgvqtneb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2aguupbnt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lksdweqp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gfihhfqh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ttanpfzp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2suhrhozp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2efvofriv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dxcmakbq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qvtxbkiq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2flwgxbft.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mbzhrtin.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kkvrugua.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nseocalk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nrqhiyce.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uiqbatpd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zmsnfjrf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nmbyvvdb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ervdaope.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2acruyudw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2frebppjl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iisusdrc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ttqwhwcg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2inkzcohl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qlkixrvu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wlwaslyl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2unuuepan.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2urkhfetv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iqjpmfaj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bypnlcow.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bufmkhtn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zbamhefm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2toyyaiqs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dhxvxsri.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bkwkatmm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjpkbxzg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pgxhwzrq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chvrbvko.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2earxltki.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2oirqmnng.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vpystsfi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2atfcqlro.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2inpvbaas.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2iyqmvkyl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lamlwqyx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dmogwihd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tskyrzwq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jioxqvjc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fwebvhyc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqfaojbv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2msncyege.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gnrfctbx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2agjihiqy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2eoyfweec.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ffzlylte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvxhrolv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2becbyowv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hfmlzifw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2anvlwiog.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2eusoafaa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fjgqbefb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kqtuojsi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cnpxcvld.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2detrlxmd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sdmqzbjw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kugfhrbq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hryqvgph.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mvoydhvb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2imaqvvcc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rktshekk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmblcgjv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bsylbioz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ustgteqi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pscyafmw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2biyjxhbe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vvtpvfyr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gtplikij.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zbnvmyzu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2udkrroay.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rktqyfrw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uknivgvt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ohqjiozh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ahcaotuu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2egpecnwo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ubrtzarh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lqlofynr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aldkrwdj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qpwlphba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2aimbbiwa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2paxrrcxr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2njblujau.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rrlxxpap.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hhvuiyfn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2atelfdpr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lejsmxim.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ayzscqas.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hwhqacob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrebnrgu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2serwpxgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgqzbbhm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nxyzuftz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nuamnzlq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxtucozu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sfrltpyl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ehybwshv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2crvbxzhb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vvcgdfqi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xjzmciwp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wcjbpblg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2teujjjnv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2shisrzzp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xpakzisf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wwosydgh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jibhpqwc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fcybsnnd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ozirwgaj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jpjikicy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bvzzelms.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ancshyln.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vrdvowbb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qddblkdk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2wgvfecjw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2eyndqfbq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tjjlatwk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lplleysf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jlidjswd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2btfhyyps.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dypvflye.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yxyviyse.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2llcmmxzq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aqnrtezy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cwzhydnw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xiqqthaj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2clerwiuw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fxxajpwt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ctvirong.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2quvwalmz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kffkmbix.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pulsvgno.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bzbwcajd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gkvzagzj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nuskmtvi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ibjrxxzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2diblaqxs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qxnowbqh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gcojauzc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mkrdaiup.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cpjwgakv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zbnzzobf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cwycqxru.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zczbiwsx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mvgcrsjj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2swfpcivs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wpolexrx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2txugatfq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jxyuhgym.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ifmkfxeb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qwdoxvoj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bmxfbrda.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sdevolrn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2llufjypn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kgioqqku.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2effuhvjy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rjdqnubv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wfbxlead.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wmivvqid.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ccxyqluk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fmwucqxq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2veglfesh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ircgnsso.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2waqlvxxm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gpyqewtx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2agudxblh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2awrhrctz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rrhjfdrp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2grydofiu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gusksrbh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zvkrbrwl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2juytmyxe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mfrbclsq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wdtdkayv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2eimyhvzb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qoaqgnwe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fismqopy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xjzzjkyb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fbljmwme.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2btggbiht.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtflvhvp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tnwlxxei.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2neszifqp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vqtniuml.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yjcxivzq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zurqgkqy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bipspniv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ezldkeff.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fsqcprxm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cvfiyhbd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2psiwlrvt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2patmzwze.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cjirdxse.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2bolhbwan.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iueaivfi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qqnughdo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2efzfhngj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2aduhzktl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2onlbfour.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ssmjdeez.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kcwvpiva.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efanfbjt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvqbzgqk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxjmvub.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cwhenbfe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uogadoxd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2byfxapgt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2haamveja.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nfvftgii.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tirbdabt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pnwpxsfu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bbongssw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uhaypbnz.html


<!-- 参考信息 -->