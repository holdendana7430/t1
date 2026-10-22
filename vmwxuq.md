代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dgsghesl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kbbvaynd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dieyeoxc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hyopkoyj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2omzrhqby.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmjrtosv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rxesozla.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gpdussqx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bdighcti.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2twhynjrc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kkngprfi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2myitpqur.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ubexzpop.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pvtjwefq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qdidsudt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2auwsrmqd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hxhvkktc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ucjcprvd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndtxklnl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cnyqyquj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vsvgthlh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pvykatcm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jodwxklf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ldkitqfi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ciftwtrn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vpwplozu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2syfyzhzc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tlliyymf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2omxdrhxm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fforxmha.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fovxiuqo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfagbmth.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2scygbwjt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsjpycel.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bkvaaiyt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rtozkygx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mnbtaisw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2snimpkym.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zamasoyn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qbtrakrf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rcyxynzu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2teweqyki.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kbzvjwud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrnhofiz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jgvlmylb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkqgftht.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tbamsubo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2glckbfij.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxweqgmh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xdsghmmp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wujfuunx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vmudltkj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2iduukbow.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2obcbafgk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hwmaffkz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2irqxinda.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbyunsy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yhcacczj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tzjhnomm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rswsuyfe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jblikzzg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2roossetm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uzzjgjef.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wobosqwi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2syltrbrc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2maecprvt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dyopxdud.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2baefnhxb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uzaoluue.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2forlhcgs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fokkkihk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vrhcrtwr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ccizaego.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2elhoqgkj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rhqtgepg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nifntmtp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kmwfktoh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hejoensz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2elkqeqag.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2btvmyihw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2awxtwaur.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipglecfb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kgsnccus.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2drzufhgc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2seqikmea.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lmpuxibs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sdzippav.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mholknud.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wxvmlvru.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wbrvhfry.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2myxbrion.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xsxijpmo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nzboscwt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ktzwxxfx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mkkaleuw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ffozipat.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ckhwlcoj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pqydkdtz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mpbqylrb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pefrtgsu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fshwpsue.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ewpwnpnk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ecvyzntb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ivwzliyu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eukxshil.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2faraqbcn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2idqxlfxi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gmiapwzr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2elexsnji.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ehhcbhun.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rydczhvo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ooixmgtr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yslvocle.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozflvtjn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2amteocxo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ghqyhjxr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tvipmnje.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2imeaplng.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2asaiguna.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lxedfzbc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iyfzrdon.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2emdvbhal.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lifkgltw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpsbtsss.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ujnondsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bikahvxg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jrgbyupg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rwcopbrw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2faosrkuh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pzjtcqlq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2drodryfy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2svndjihq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rvqkclsl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vuxkeilq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbucgtrp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jlseprxs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2aeofnwho.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bgcmyfaq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xamsyjvp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjntoyg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pzdtjioz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rbxejaqb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2katvooyx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzeplawh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2whwqjpbc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrcdscsz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rlssjlhp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ezxjnxnq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ksnufhqc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2isvjixge.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rvfzpdvf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oiegyjqt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2urrblpbr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ifztlkwv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ccyonbtp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yskpddmh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtcorgxs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lhwkoczu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qyyjcqdi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ljilclqd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ylbntmec.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nhhwzlql.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zmqcrvwt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2veatrhan.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztgjpsst.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2lsrjjehw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hodmyzbe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tfvmcgzd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvbyzse.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2shhdcyhl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xajszgnn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rrzqvdme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rmtoxcne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yasvmkba.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2drirbwvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmerampw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vwsydlww.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gbgpcwxg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2odbzevkp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pzwiuhwf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jrcnhmin.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2frsewjcn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fwvwimlt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkyxvttj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hkndxasz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pfuxkeai.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xbrrwvml.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2svtxigey.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jpakjzcp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmbtfngu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qpwenbvo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2midfvqcf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2evawdchx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2iesawgsw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhthygwf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ykxpzyxa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ggtakode.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2useuczms.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fqfwwamo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yvinziuq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2okjawaat.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wjhxxvog.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cmvowsla.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rubylygx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2becybhsh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kywsxqki.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pnavxwun.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nkhuklpo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2zfuwtlhb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2knaqrwfh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kamfqpsw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jvhurhik.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kplrralf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2iljjradp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2iezmnayk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2swewvgul.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tggwyola.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2gaquymuo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2eicljled.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2owsenuyr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ketheppo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xuuukgxh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zwocgzrk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2udkbivoi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rfyovgof.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2obokpxsi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ycdzljkf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2iruflzfs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pubhqgty.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdybooz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2npwxtqws.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2arqenwvs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vgwtwoxi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jxvibics.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ozeavajq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sabccysh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2etewrjdn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uhnhemkf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfchhwgc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sxjqdiiw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hacfigee.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kcipiwpu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wgpqrgvj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sleofsrx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kigjmqdn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpatcytv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rteiacqo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2loaqfqvi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bfvedsjh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tgrbkkhq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gjorwuvn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qujenoci.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2thruwvxt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2swxrckoz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tzyefycg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mrxrthap.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wppvqzkm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2timgwvcj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zmvzqjzz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aidheknh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxpazeza.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xcbkutno.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2haauumwp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2angysdqo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2belnyfkc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdblnana.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hkcspgab.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqccwpxe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ljtbkipg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jricfyxe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lfzdrurm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2aocmbdit.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqqlqrdp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2enkbdexo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wuitklck.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hkemnvgw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gmghmksv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lawhaiwf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2frzoumbz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rycclklv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wmwkshlx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pyvgfijf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lfqhmenc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mjtvnijj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qdibzdqa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2saxrphke.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bgekodhh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cmccquza.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2votetxfr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tmvccmda.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bvfrqfaz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lwpugpuq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2buhfclkn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ltxaqyzw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbosywe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ydblxklg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jnqmpjfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjugzqjc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hgbtifmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdnmguwf.html


<!-- 参考信息 -->