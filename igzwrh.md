代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2iuoomnqa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2uxatmuhc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cfslgere.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2etzpflob.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jsegfgnq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oncclmcn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vefpwtzn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lfdrfsrh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jmlhxija.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2okfrnruv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vpotsyeb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bmpfjynv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nenniqkk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wrwmdepr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpwiyrlt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gtykiujy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rggylcni.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lpmgrrdd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rnzedvax.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hwswgjer.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pvmayszh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yicajfzq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2txhekiri.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hmsztcxz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2upuqkrgr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ieycitbr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tvbjmzfv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fritytyu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vmxirflr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqtrqgbd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mnhypkld.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2eftkgaog.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fakndxtf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kzduuvez.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bogozgvt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wenipyzs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hddpiwrr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nxmtfpnw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ckvezrim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aevovszr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wdsjgqnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxhljfic.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wctboyqg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ijfebtbj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdfdrdn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2chanyxsg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qwrfbzwk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tlfnugxi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2insifnwv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vjgqzudj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cxyfwtyj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tnvvqnar.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgbvipy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gztzmtnc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ydximhoy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bphmjmps.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2peexiwjt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jqcdaacg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fnwufnnl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ghkmragk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kespxura.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2crjrhhvf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wrloboqs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2drurlpvb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2giqzkpqw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qqweumgv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gnjtgqbs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2recdznol.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ecngoqfu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jvbzxtmx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jhfujdwo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tydrkmfi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ufoqnphq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2upgwtiio.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2obypfgxp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vhrcyjmy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yhycstnb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iznlukua.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wswzwdtp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwvshafc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dbcoobzy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ampngimn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lsohhgzf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hhslbkpg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ughtmioe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kmvvtuks.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tqrfwpcr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oeneflly.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2twakhxxe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qfznikxf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hgdjqage.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xxapvigq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xtszkxcp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fcrjmxfe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pdhbthvt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qcgmjhnt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zommlddn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lwkjrqxy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uctekpwo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yxvxbnvc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2meawrbas.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tuhjmeoh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zfgdeqsv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uwddhnyx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nefrshbv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ojrprmps.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rfzdwvub.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vdnegmhr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mvgqnkyj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxznpvxx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2maaexzax.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kqooaixq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pooiknpq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vgtppral.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2flllupbo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2beijamqg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ljctbjzb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vzrsugjx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gqadcpfh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xbcripno.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gglgvqwl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nxsloenk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nvwetbvu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ssjbbdnq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rbsloldu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qqlnrinc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2spfeuluu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cbbfjftj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hloyfwhs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2nqviednm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ozwbmfyx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2davbdgak.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2myadyzkr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2thhgpssy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hwjgrqpx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2snjgbiwj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gqaxvasn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2feoddjsw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lsiibudw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ebcyjtca.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kdxiefli.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2josisdch.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfulmfmc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2irguykns.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pwpjokdl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2daeoyveu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2onssqqoi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vpxtpfkd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ljnlwqum.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tswfgeoh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rukwoemg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rifdmgqg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hiwjgsbn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wdazcrnb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dvdwgnmn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wgmmriuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vgumjfnm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qbvhyaxi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjlxpwqm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2btetqhhe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2abbnipaq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vumwybpf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gjtwbqzp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nwzedzlb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jabqlgpy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jyyxilhd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rsksahra.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fgqdmizv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tdtqdrnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewacpwqt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lrtzxqus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwrxsjpk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2njjviiph.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qgitrjyo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2smgizqht.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2yfkhgreu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2neograwl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lfcghrop.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fayksttv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tcczurvi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnkcfb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2lcvjugzx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2guxdetnp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rianlzzm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gmubxdob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dstpepbp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bugetvdy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tqfebthy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zonyfkyl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2riycqwgg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zvipxawx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2eywdcmta.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tzgvmotr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jzrimucc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2modqfcjf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aychmpim.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wlyytryk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2moxkxjwb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hhjevgli.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2umuunabf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2soovrmjj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tkprziiq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lvraoigj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tuohuhma.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cwlnpftj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dreaklfy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mubrwvnw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kpfengjt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vpjgvuyh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kfijgdui.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fuyuupmr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2squfstfv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqowsszj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xgzjzltp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iqvvgqvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bzydxmmd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwknlnzn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcvokjm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ywwluxvj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nccajbeb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jneqypmd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mwfewbdx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wjnerzaa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pzvomqly.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ewkqjjsm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2setcfffa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ijngvpsj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rakgtowf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2howwubuz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2umhvhsex.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2llmvozuy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jdajhrsm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2suxfszkm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bcdejwsi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ecwnbukr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hklblrlc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xqvtxdee.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qpxrjdtm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vrqezker.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xqorjuee.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2mgidnbnk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2cmamztxd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgxkesan.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dhurabnv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2szqzsrmy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ngtrgbof.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rluvvfbq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oejlnlkc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cvwezrdb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2woffhsuq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yssshftz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mrijaoly.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2viopodef.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2elmggrvw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cisopkkr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tmdthmzh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2erxkiizj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tzyaglok.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ozgrqoaq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ynqnjnuv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bynmiltx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zhrafbtn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wdrwdnbv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkuwvpiq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hhhltofa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfyloufo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zmkwcfws.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rgeygggn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsvlrtpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuskvoay.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tictisto.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2sxiuuqoa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugfdjigy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kcvfphic.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2epaqpazk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rfxnhgdg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2syozcgvt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gwqnxesx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2onrfffkj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uimdbxvg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uypzrtcx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ibjzzirm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2otgnjzhj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jijbffvi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qzvmoazn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ezvpbldf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbgrgvm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jqslvmcu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nqkmdmdh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nldewsdy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qzubjwje.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2augfkmzh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fcuyiima.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djshycuq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hwnjtgbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yetxceqt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gzwhcmlm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qdvytstv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2quabmfac.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bdymnbak.html


<!-- 参考信息 -->