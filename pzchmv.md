代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lkfeftkc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ipfzfmch.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2uzsqtnow.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2oswpbuhm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uucamzkv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2emzpovbv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qaesrzma.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sfwskybl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ciazgfpo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vhsjjics.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gfzcqvrh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vaznpqel.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ectvgqya.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rhvamuse.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ixcwhcwa.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2booghryu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rnhidnkz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wnqqrxxg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eatkfmqt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2uwfsnfvh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vwunbhzk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bihtkejc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rzaqfreu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xhmhyuaq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zbrkasgq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2agubcczk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bpstuikt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2doarwqfq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gfezxafn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qqcpxdkd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uouxdfeq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yibtmcet.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2plrwotub.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cjahxucx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lcksfelh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vnlffnoe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2abypmmjl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2viltijsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2duzbbwva.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2flcrmmbi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2cwvsekno.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nczrqmrd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2apztpetn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eolhgznh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xhevspfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmcheazx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ifhwjwbe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cppimoou.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yptjshis.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bvbxbtot.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bbpyxtck.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vagjamlw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uddfgtvi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lzzywkzo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eizwemer.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yymdavgl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpxqzdak.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uvwmcium.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ofbrsbpu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2thuefapi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zlymtxxr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rgdzxkcf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qzwpzybz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ubxnakvq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qjxlneph.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nprycyir.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pfajorfi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oercjdel.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uthlrpuw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2prdamumy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gfawmoor.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2sdixemdy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ouubcwdq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mszwxkfm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ayyafhnv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ouorcpps.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2sktgkpib.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kgnglmwj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vveqelih.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dfinmpar.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2oncejfcl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzldhaeg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jcoeqfrt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2umxdseef.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2aomrtbph.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lplusmdj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nzsibyoe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pulpygvy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uuuowrmr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fpxodizy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bzectsix.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2okzoagro.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lveajarn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mxhwkiva.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jdxtahvt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2alnxmhbo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gnusqofg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yrtkmkyi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bxguwbie.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rwvjbmrw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xnoqpkru.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pxqvibkp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kbtapnvo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tsvxctaw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mmnnjvrm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hfzvnhqh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wxupansp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ezvydztj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gigaujnx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wdmlcefp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gvgvhrtp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lsmvnjxm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2prqvcyvf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtgaamb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmbeirbu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2czklhmbg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qksshdva.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2edcxqpmq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bjohwcne.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rdplmocv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jqmwflex.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jynztkse.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2firbdfll.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2plwuqums.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2egnjusxb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mfjtawtx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ckupskqm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vbyvbwlx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2knekrpot.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lwegdcmj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lbpcvxgh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iilfihev.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jsycclpc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pzxswidb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdohscgf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jvsrzmuv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ypwmkdzw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2camstvcp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2usompluv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ebqxnbko.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qizojeym.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zfgviymj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2wobcolix.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jouurfmy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2grkskuuc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rwewvaux.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnirfvle.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ybzaznqz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bhpguolo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrdxlaak.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ilqpnwqr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pdsxsvmx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cixuwgbd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qyinfhsb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ljrppmiv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gomtrrdr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nzbcblrz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ljscftnp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wdmyxzrn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2veijewop.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2sxapynkf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2spdmzhnd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tpizbzxb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dfprxhem.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xxsmpfta.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fldqyeez.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xgssuoag.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cctzgrby.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tjsvobic.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nyxlzeld.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2daalhslu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gtwtndwk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vexcecrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovjshyti.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tzfffmbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foxzupyz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rsdivllo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mhrzznjv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xzaknaai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2reepnytr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xcyynpgy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mmcrzjkk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hviriotr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ddjjmzcp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wtrxvqke.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dodfbmqb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vbzbqoba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ffnytapi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jmynxpwo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lujnatmc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dffoucop.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhjron.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bxosjhft.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ejaifiuo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2appjihnt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xffftkpq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2aahpnevk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2erfwkhjw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ygasvxci.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skuonxxz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rarzbxvr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zfafzvnx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oskzymrf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fiwvedtw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qjwnpuqp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2siyrtrqn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2chbutgwz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wcvbpiya.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tdxvrxlg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jjzhujli.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2guhucxwt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cnujanfo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2slyhalec.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pphwhgdc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qntkeqdt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2blkgufbf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yqjpywoa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2oykcsnvo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ddhvishh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2thmjdmna.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gfurlpii.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jwjsyzoo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hdodgqlk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nubuxxzk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hrrjgntk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fgcaprxu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ckdolgbh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lmebosul.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2szlyptjf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cuahldrr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uapxenje.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ckwowmba.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bvuvzojg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wcyytrbf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qylvjstc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbpulrt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pjlamyiz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zhvztzwc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hufvweuz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ywfuzzyf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jpluearc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2siwkdkmq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fucwdwrl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2imgixhmf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2emvrokuy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zodwcpvj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pmsilsmf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2heufseit.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uvbcdbsm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pqistnlq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ujgnskro.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bqlahnvu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ikdgwort.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2gjlpbhik.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xnojtifi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2skgcjioy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tzlvbdmf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wkzlvqcq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vjocphgb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qyxwykkh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yyzbpwfg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ttrobusv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tzucopgd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2skkctwwd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vdtkeeei.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2oblxoghm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nmnsowsl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2parzmlsz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2txlqplzi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvflzlb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2syacnvnc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wldvtydu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2trhwxmad.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aorjherr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywdrxtqt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yssmligu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpreqlsc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2banycvyb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vhnxzkwl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gkhmillp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vjhqmleu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wbztxqup.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hzqgoims.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zewfyhmj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2khlkifhj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lncideyw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbrpxfg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rvjledau.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wplstmwo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tqmorqly.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdrsvuxs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzizwwxa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mpmktnkv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wcawqudy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hkytjkny.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2watwshlm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qicvyuxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbjiazdj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cevkuoem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wujjzsln.html


<!-- 参考信息 -->