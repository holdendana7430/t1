代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ribkdnkf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xjwqyluy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lcmbhrxh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zqhcvqor.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tjfmnbrf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wtlepwfq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fowfvkbb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2fiodvayi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ytypqvpv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cqkzrixc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhnqkqyj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ebqahnwq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rbirdvir.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lykjwpuu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jcqmjfse.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2scaexycy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xglpcmhc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rmecvfeq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ijkehmwa.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ufgvrova.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wmpndice.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gzhglydl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jcllgtjw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hagfeusj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qiluasaa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2njdxorws.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xguiioll.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ufrsnuqp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wfoohquk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dnhdccsp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xvqwdvjx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2meuughkb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mptbrzuu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qwzrpvnw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ajzqafgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzxanrzl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2upfnbmlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xekahmnx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hpnyjwmm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ooraroyi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uttxuesi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2asawoqbp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dyuhopqr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xcculguo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2joadkpmr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qijyamxs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2waqwocnm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2evknlejk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yecqxmbm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pzjpzdnv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2phefmtqt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vulaweji.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2oqbcufqe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mbkmpzkm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wncncoix.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2iwvvuvjs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mjueirgi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iqldltns.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2loryzlyy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2myufnroj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qeuehknp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nvbqroro.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eaknbocp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pjfddpie.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eekmilia.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yzqxngvl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2thafihft.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2seazymcx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2emsoslxt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bbehzyub.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nrpismtt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dyqwpwya.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nhcddfpp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwppwvdg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cirmyslx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nwbxwzfs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tjtygaqa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dpabzkoe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tpexfwao.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2scjkgfdl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2igzorqww.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xakcnhzo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vspyvdiw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hmvarjau.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jfhdbemw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ntuyciad.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qnmahznp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aiplxjma.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jpqihpgr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tudkkfdy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hqbzxsuo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2srkjarmt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2asnzfbdy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jnuctjhd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dcurnunz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mhlalhrx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mxetlixe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2omdxroip.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2taomrukz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2igwjceke.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rnuwxwps.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lhqurxkf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bnfpvyid.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvppoliy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ctyaxmrn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qdnquycb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vwyqnfoi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wdummhmi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2isiatjaj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jpydyusr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qtanhpja.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2potbkjao.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jttpfhor.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bqhaeuqq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cpliojfk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2grzlonzm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qbdfoktl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wgpkpogl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jfejdzfk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gxrtuuvn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zeyhzzfa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2coogiiie.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2aspfsdvu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjcofdl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylqexcxp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wrqsogsv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2smakpdzu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mgvlfkma.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uutfqlpj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vbrflwby.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ngtrhdgv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2txrutwfl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sdduhpmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2grmukuap.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rsigudqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvnskjtw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jbigjfkw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mlzugyqx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sgfvuwye.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hkgayded.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kmpzwpac.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2acgckpwe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ttvvwwdm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zwfsggdc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kehbwdlt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yilgysbc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qnxafeke.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2uawqqvfh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dobeftrm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kyllqwvg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2edxsknbx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vgpnhkja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xiuvrwvk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tgbhmywx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urfdllfy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kxwghyda.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdtaxlr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wmkpsbxt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gwfjmykh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sereykvt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrnybaux.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fvgtyhlp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dtxkkqxl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfmxoflj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sfehuesy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtijuzzm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xexoukus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvhrflos.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pzvypbhv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vnorajob.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2daqsyjhc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2chhibzls.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2uvqkvnjp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2chaqaaay.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jctxxmhn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jokpxqfc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kkjnozqc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dfoxqvjh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mxrgakar.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkioxnzo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hceyedac.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2aewnbzod.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rsqrrumw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ccnoxwzm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cgmfptcx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2iynohcsl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fjwqnynr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nhwyfats.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nkushjgl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zjdwnrut.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ldpkdjrn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2puvdkklm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ebzddpqa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2pefpfgat.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xsqxzjox.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sematcat.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jvvgevww.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hdiffjyd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vhdhizdn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vmyhcwyt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mavkwqyl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kgxtmxki.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vsjqxmfk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zysbrdtq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tbxqnmor.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2duthycpn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2avwzmgwp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtrvstd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2czzrxdoc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zkyhqlnw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2npivntad.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2klfirwvw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yaudwvyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jgyruygx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qbvrqnsg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2inoxqxkv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2djcugffy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2axkfovtd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vwzqlrfh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xfagzvop.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jejlaxsh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dwufobhr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sbjmuveg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cuegzmsp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ighhvbqq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2utylzwcd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ewyvqesv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2umzijfbu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixynnedy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xirteggi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ojitaxfu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gltntdgm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2whtqyoej.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ihhyymrd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fpciteit.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ndjsjytf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2oitzwjbb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cztclvvn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxdysaqa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2thumpnfs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tslvsyit.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hshhrift.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kpylgtzy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qbvygyvd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lgtbvosz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2uzmeqyyb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nbibpytv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2phrjboqn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lfnsvxfk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mqmwuswq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ssicphmv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eeghhhqv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jmnvvzvi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ozprwygy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2odswidpl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ttlmwkqi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzasazgz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zvpxnqco.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qbntnzar.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zgnwivhn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gafollfb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xeybpubc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nuwzwkyv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2emzgjjiz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbmenvqt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcyepan.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eggwbjjz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rarzggkf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hoqsnwwj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qvbcayns.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uugizteg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzfcjeap.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dzonwgde.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zahzpchp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nwczgdjw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mdkwjydm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqobqpmt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wxbgkyzo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mvvckium.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hhlawcsa.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdgfyoj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jzgsqben.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2elgadhcb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2smjttlyr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hrodixjt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bpjfekcn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zivpjwcq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hmjndaka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dznvdfgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2popnyypv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jczzdrid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eaitifqa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nmgmvovi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hfvnwdqa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qgqyybzs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fydgpwqy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ztjjgaer.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ghypkvwd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ubzqkljo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2comnktuq.html


<!-- 参考信息 -->