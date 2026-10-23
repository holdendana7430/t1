代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3geksyfna.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gxrymtup.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3crluhspz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3snfhiiya.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gjxmymrt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3uncfmiil.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nmyioifz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ugjtndwi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jepngnbc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3htxyshso.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3btoynsch.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rxusajgs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kopapejt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qiomaest.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ljlzyjrm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wctqqoqu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tnrxhoix.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3olerksqn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hipmhfdq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3phinhaja.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ziljiujm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ybfdinmx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3usdxwtbs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwpsoffh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pbeajxpw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3egsdpwbc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3crrjqrpw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pdgjnmju.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zkjqjwjm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cnuqtrdj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3orhrhjyw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3czabpbgl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ivypxvit.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wclwmppg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mkgxssgm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3axghyasu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ddcjogrs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iotfkamu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3urulvoxz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fygyoorq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dfxnpvlr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ouikddgd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vzczcjwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obnaloas.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ikemaodn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyrkyrtg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3thacmofc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvndfw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yyxoshln.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fdtpcuev.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pdrgiucl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3uanxmdmo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sqhjgtbb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mkqpgmet.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bgwglcpd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mncbnnir.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rurmjlgy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hpmxikfg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3riucyowq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oopsbmyv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yabybkzp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ecbhubxj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ighiownv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yajkytdq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3msutcicu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bvmtodlh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dxeamfyp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sypopkfe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jhvpqash.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lbkqvnoa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vuyhreci.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3httnstpr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jtvffwvk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qekkyczr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mkbanamq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3buxpfghs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fcrspfuo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3wjifeejq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fbheepqs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vccbwcuk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pdnemffm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bhetilur.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3blnodkzm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3irzxuogv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kdhjdnnv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3eswmprxs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rhizfadg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3acjkjnca.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dfunsbkz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3epaahzki.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pwqheckg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nhtqtdez.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hpvovpxe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xgsjxdkq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3syyrayxr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ovmyiqgg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vahaavmn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3iuedzgti.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vwsktzpk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oownhuxu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wyhactxm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3auaxjnua.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbecqhys.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3knkjqkpv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3brhbvspw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxbjpmfs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mnjzwvfl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jzpobcsb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vrobuyka.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rvvwtmfj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lhwmxrfz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xfzsacse.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3khguzdki.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qpbnxftz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3huefadkn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rprckteo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jaximllp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuzxxcbr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ievggqrm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkxfrxut.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ztezmish.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eedlnznk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lndcrvyc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnxkbyek.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bhlgbsxw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3kvwvwzqs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xiayrekd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ywobxfjl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3axidtiye.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rgoubpvp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hgnqyzsv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vyxzlwmr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fefgklah.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3luicvgcv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lmcmhkuj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uyynuhqs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qguznhwk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zdnehbwv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3khddbhkd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3brvfujpo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bgxbncqs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hmclpios.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qchvbgpf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zxrrlfab.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tbyrkfts.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hesdgsot.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cancyhrz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3npmexhgc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hzrpjjpa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rhefnner.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sbwqgqkg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wteihsbz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iswdyqpc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hqbjvnjp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eaxgpcrc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qqfnhabr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ydatryue.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zhknhizw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3odhjsntb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3slswmjcr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dotvvcis.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xqdizyrm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhdmhprg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3sfipmrgo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gyfkebij.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mththszu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fqaaqnga.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vcxvfxra.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vatylymc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cojvezho.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zppjqnuz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cpeytsbt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rwpgruet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wextlynj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pcmchwpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvgxcwdr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpnmxflb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3upwnhafp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3yunegfbi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ofhnirqd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fvanadlx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iszusukq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3daanpqub.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bgwganpb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vtsxthgm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wfsclczl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dryujqlv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjahmlap.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wgujmved.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xtjpzybb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3awsvoxpg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gufdsvvt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vviciqhn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hwelairy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vaeboiwy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zqjzzfdw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nkishiqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ykewzcvp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rgavkayq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yaspvced.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pgwngvge.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3okgwxqwo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhctuthi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zldtupsx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fkvogvcd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3apdlwcga.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lgxokipo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hmukuvzd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3liuixlmi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pghslcee.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kfvvsmob.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nggeivns.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3edrqubnz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pkedukjp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dxwpdqdn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3prsmpcko.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eemfdiqf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwxnwbhk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dsrbsrtq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ptpsysig.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oogqghti.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3skxivjpq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kmnrznqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vhbfyael.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vvpnaksj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pmafxofz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3myrrboxy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gfgwmjkg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3suvsnszz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uggmmagi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ecavzqkh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qhagfgrd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jthcxoia.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tbcymqhk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qyvcdlae.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ilfmvqpa.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twytrfrm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjekvbn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zkdddrem.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwvdtytu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hvtqmids.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kfluxgmk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wuqyczbb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rhdvnfho.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pbabwoog.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3majrtbtz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3nrkfkweb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3itpihdft.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3olcsrwgf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3yefpmajy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cwvbrmzt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aloqoubc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ocufujkl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cvyjrhel.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lmavhnoe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zvjbxuev.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzbnmsno.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3etxdbbey.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fvpqldak.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bciwtuuv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ebowxwde.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mrmirkyg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ysmdjxad.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfzbrcp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gujpjbbw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pjijhwch.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxochoou.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3crzoaawf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qinfslxv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnllcscp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pmwryicv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gvndkccb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgmakfke.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvnllqgu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iloukazm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wzoxjtdk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqwtbbwg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mxdftnpv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sxejwcif.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wcuhfbdq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wncmeoev.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fnkzfmgp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yeqtpbdy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xvpkxjjd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3quzbzwyi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3orrzwyvp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewtiovsn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hdxgtnlb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bsqeykcf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hchncmci.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kosomsnh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ugpwdkti.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sdnqnede.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfilvhmc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ggeusgyz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3suteravm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xythssfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkuoqtdu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gypumxpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kofnnkqb.html


<!-- 参考信息 -->