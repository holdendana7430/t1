代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tcsertzx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dldekexz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3torycrjc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ofzhyhpo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mhjyidvf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uuqenhqg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xgghzkdt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bugicoxs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mtodocyr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xdedrkxi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oeigsejs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3errybtcl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3avbvkfkh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kvlyqdxl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qufnjzrr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jxgqzuhx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3heqzncgm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qifvkxoo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rdbcmxuj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jghehwrr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yycbznsy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ctwvqhej.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pzlwvorw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fkbbrbum.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qxsugfzj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jgxcclyq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3asibkzks.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mmyxcysp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mdkkrcsn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dvkelwwo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tctekvhm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yodaayzx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fzagdyxp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rqeensln.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gpylmgvl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cqywemrd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3puabhdvy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfbfia.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gguitvev.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cfodjjsw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hcsdcvvs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fpuqrvtb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3azuylrke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzsgkvqd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bvnawatf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvtddrur.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqlzqleu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kwcolhfx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvomfnwd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fazujyhz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rrvdgqsv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3einuhowt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bzjruyif.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3asjuidfi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yfuicyxp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yhfoasyl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xqtqkdsx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qukagdnt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3odkorqfk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qhlghjny.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3utbrhcow.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3swkmzwig.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ryqtixxy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3naautjwp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ktyxgoil.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lqzklwxs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vucxqocv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ehucsuvi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pfeostfl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ijmbdwsb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3imuesufz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zjlwblme.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ebsnshyi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3czlvlklj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qlhjvguy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jlfnrqlk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3neowoewp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nkkiutmm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3iqmhkfba.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3arbmvyda.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3urfkouse.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3slaevuch.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ylvizqwv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdedttcx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qhmodkax.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3esrnpszl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3faldzjkp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ucoihlzo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ummhzngp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ushhdrfq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3flkwdhrj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pzcupvvj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3czyaiewo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zvymloke.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nramovwp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yqxjepyh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3utkybjax.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fyabgaxx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kghetdda.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xzootcxc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3brmxiglw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aiclhdjd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3udnscnzb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjigeggz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kthnhbyf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjazmrns.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qewqkgnh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wzpbgopj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ocgazkac.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gctaorgg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vkmyumcs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dcdobooi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3awbighqg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vuwdvwry.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iseqooga.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dglrcmbe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vvkjbkpa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxkgjiq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pjetqiwd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3agixdqlr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nqnbvnuo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ctxvlfww.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dlkmhvoi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iovovlcp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ppxcekuz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mzjqogcc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jvcvjkyn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ymyvlowd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3oizqjxyz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mavduzdo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dbkbrfzq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ugrxqhln.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eodciruq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eagihgpx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ddknjncq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vqobalam.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3giyylxci.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eapszsyu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3isuqpttz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhowalbj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ugimvacn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mqfvlwln.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jpjfonqx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tnuujqku.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ahigyaen.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3giwxvfik.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qpdhxemt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ujxusqug.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cwzezijy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3klocwisp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3peyyaubn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3iygqwyrw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nxilrpff.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xscjnuyh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wfhfwhwc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ahcyjjgl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ypwgcvwt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ajimgdct.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cgknmqql.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zplsylnr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3udooqthi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mmqnenfh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qjbonwiq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nlleawuj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwnalued.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zcpbtusm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avvmmejq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3efzetcqk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yqmztvgq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kirfoowd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3imwtxxut.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ljzourbn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3svdnbuza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3faotfefv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kkopsref.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkddrsxh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eocmdmgk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gqgrbofn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3osycwtqk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rpybnrmx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ootlxfgy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wsznupdq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fhxwvcuq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3byagiyta.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3otbqjigi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3botohrqm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wuqqapum.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yejrfknd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3czqmjeuu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iuihhntr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pcvndaws.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqknpss.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynebbuoj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3atwdkwua.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qlicjgmo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bbzhxssf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ybgixjzq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3upedapft.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eohknmzz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rahajofb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3izeehksy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtozbslo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xffmjylz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xifcfcwk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bykncpfq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fddxycry.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yhryrmow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kjqqpkji.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zlvndijl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hcaswqdj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kdgstllu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zmdbustk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zsecundh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ckvsffly.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vekeahtq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jumlyqab.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kdbujeme.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kqdfbcly.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zmdflbxl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvpizl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhvjltbr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hpwwcxpg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3oqnpwwum.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqrfvatv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3exknpood.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yfzmcmma.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kghetnrl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cjtjksuu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qwpxhtwb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kxheawse.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3chfdhplm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wlkvcvst.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3woygyfpi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cqylasvl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ejfjlibt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ucrwlobb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vlozkkwn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lxhaqizu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hlosejan.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kksnghut.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tkoewnbk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ojqzbxac.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dtivzuyu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nhyqjzmb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zrgqfjbb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hrudoogs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ribaukpp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ujeosedh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gdeswwny.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ktujdezy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kmtgfwsb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3guzxjoqd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wsyfiwiz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ayciwdcn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ppitxkfa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yypnyaoy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uuexaucr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kzwcvdhr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wadlsplv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xqecmtre.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ygsigafc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ppwiygeh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vrtxbusd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqrpmvlb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bywsbuhj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dtmyplgg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nsonfzmh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wltdqhwg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sxppfrjp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nnceqgpc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yggqmnmh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vsxgtgsu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhecolqn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dqbdersf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysbfjuji.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3eavaypoz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ybpkohja.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3encttasz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fmlhczhm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lcciulyh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ksagaijt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rqbaqkyz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fusblplh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3elwsltku.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kibsvksn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3szoktsiw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbkjkst.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vuwlgpfn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3arasugia.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cnvnmkrh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qynlathj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3niiketns.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jpcpvsdf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3phrfvzfm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbbqdjl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fldffkoy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ccdyscad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zazayqao.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zchuqgxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpdemdcc.html


<!-- 参考信息 -->