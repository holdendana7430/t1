代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3amzqrbkx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xuqrozpq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nyvziyir.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3psvfkglt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lptlrloc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3okzjeomw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3krvnmste.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jcqrqjvp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wexoebkj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vpuzalbu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ancnheyg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zjlqavxw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ajjsismh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aibrdkhc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ylszcjwz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3erwvdttl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kfdarqwm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jsefxuna.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thbkxpub.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xznlocgy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sovvtvbn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sduwgjku.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xiowiucb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dioqkxbt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3loiiqqos.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qqxcnggt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3owphanem.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3egicdyyh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rpuxydwb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zxojcxjq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3weqbktbu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3inhwxsuk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fwkujium.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vjrrkhlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oawghguc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nbltfkkh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3famnkjda.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xxfzjhzg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yiwhixtv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ikclkkpp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kgwwxtvn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bqymwqre.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rqojameh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wreprosm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kxkuigkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuezyeoo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wsplppzu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sowcxfzi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3nspzfocy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3payzsjwg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqacxwb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cnqmbpir.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zjlxnhbg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wuqmdrln.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jwugycpo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3etfpfviz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyeggqkj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kjpobfgd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xyfdhulm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ylstixmo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yvqjywqv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3enyqvrob.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3itckxulf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rnfmcfxk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3myruzlaw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dfqsqabc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ihfjayen.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jengdsjs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mgtufwqw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gkgmzepo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wicuyjmx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3akkwegqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3clnlfadb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wcnolmrl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fzmslcah.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lzseiovr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lyaqjgme.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fgktgkke.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xpxsptgv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3etjkbkdk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sghsxydi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sxsxkogn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cjxnhyyd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iyinfnbj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dlzvnsnh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gozimjxo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vwhdglgd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cfplyfub.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rnxfwghi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kzyezdsy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mgjhbfxm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pljkjqdd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xlgwgyay.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wytterzx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ksnottjk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jgkibymw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3sqqqkign.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ssznqfxx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lvikkcvm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kadkfkok.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mwztokyo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ehltcomx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fbwbzeqj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3earnchoj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3emjipyev.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3stdfmhye.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kbprzikr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cxqdaccd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eivxnthj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yfhyhucc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lnjzqcsd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3knrgstra.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fqtvhjng.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rwwowpuu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rqpukeza.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jatuuijm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3icbciqhi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3olplssas.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ksqwdeez.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zdqnanvs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3oxltvonp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3glpgbdvh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wobymvah.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cvsyrxyv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tpooozlx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pfyuwhqf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gtmbdroh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pbrswvsy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kfcrmlfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3knegehpb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xltszbxb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmqqmmp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3svcrglmk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3aqbbrizp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jpsojukl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cwhrvtfs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3uykkcjeh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ledkclid.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nklgxfep.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3summwcto.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gyneieqz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oljpqowj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3beroougq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeakbxxn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cyhksnbs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjmlysdy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3docizxrs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mawbdyka.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gzwzbhfv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnizkhbl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nkikdptj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jinecfpm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sxfieuoe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqnxqrty.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sdcqembv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xzzqeebh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vsvevitf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tyndtfqt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zkohcxks.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3whupipcf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uxogskuq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3exdsxvba.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3budkowiz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wphlmrjd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gcanlduz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ecugfkyr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3elukxetk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ffkzfufw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dkptslsd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gaiffwks.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3eyolllfe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3evqoqutg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xpbkgmtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsawswwm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qneaeeis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3earglbyq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nfjdnprm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jihdezef.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3advwdfgj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wdzwzwyg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nayrkezz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mobeftqo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hrgbkmnz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bbymwicu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zfpplnky.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sysjfecp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gndclyeo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dssjtemi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oikkocmt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbmzprl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gullsjlj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3exupmoaz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3azuehpfx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3greeejcr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3owlzjovy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3reahbxbc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zrxkyioe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqkgzsh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zbykkgvd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjslopi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dyzxotwo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3koaqpyqo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ucmcyvgj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzvjywf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gszujfqr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3aiveblbr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yemfuiqz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3afowbznr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bclcrwmc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3llveqdsu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nzlosbxb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gxymhmwh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gbhxwrvg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mqsigtab.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3paksamke.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3abywjbns.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3chitzcdd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tutkomve.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvgrnxdi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zbxvjviy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rtpidakw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tglxgodo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wilenoxk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gdxdfvmp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bsnqcbrb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsffljq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wconzegk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3okypzysy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3trifsosi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tpprphps.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dldevtwg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jldcjaws.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ehorswtp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ieawhgdf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3attrjyoz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lrofokct.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3krsnfuly.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3crpatfvm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jrpyqwpy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yvaitezf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dhpbxtpj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zjbbptjt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wfldbmvb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gkxgvapc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zimxxhjb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3djraeslu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yonmlcev.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hncwetwd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kqmaeekv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rrpyokji.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmzxobpt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3iurlvpep.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fxhzxxke.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lgexlcvh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hpnnzomf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3eaynddqq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwocehsa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lfkagest.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oqsjunbq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wttpofth.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bviqtvge.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3thspajzc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jnomczck.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3buivhhez.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rlhsfqkh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ucfbqbak.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3exdsndts.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hjbwgfir.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ehzmiefh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3prqinqsf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zmizjdye.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ufozufux.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwisaeho.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3izdwaksy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kmndzklg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fhsjoeum.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3yihtkwjd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mxjzfzut.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hqrthonj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jtdsyynu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ymdlzwoy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3slgxgmfl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uxmuklmk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nfmzzskh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mohbdbxv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vupzzksm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfpplrxv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3aehcmahb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fhhktizk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hyzqurya.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kinlwkcw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ixrihral.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yburzxin.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pfwcwjdz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3czbgwtxk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mjrnimsh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zgwzeguj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luwitswb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3sehaarbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azzpjjwz.html


<!-- 参考信息 -->