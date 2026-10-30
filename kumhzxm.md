代发 wailian999

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gcdfbuavc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gppmvmxxh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gkrumfhzd.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gtkhfacdp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gwshllxur.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gwdxgcgjk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gtdkkjldo.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gdvceumbw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/giavscaxr.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/ggvxtmnfy.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gpaonvlwb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gjsrpyurf.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gewnyijyd.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gxrtvvbfk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/ggelcklmt.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/godshkwkq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gqeroozkw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gjxwmdnpw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gyqlhsvdx.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/grxgkqpft.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gousljefr.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gjeoucdax.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gjhlohvcy.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gshzpoaec.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ggblmwrct.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gjzemanzl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gussuvpgw.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gsajnoggg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gvcnxkkhd.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/goeyvjkti.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gluwmrmzh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbczrvq.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gsgjhpjto.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/ghppslefj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/grzdtpmzf.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gyplmzzoi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/geyxmrkin.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gzrtlsflg.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gogfxcbpy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gplxtsobr.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gxizmosqn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gghnbrdvm.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggdrwruuv.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gkkzfpeaj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gxvovonvv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/ggryhcegj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gabqbfxir.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/glljkpsxx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gwtlrwrqj.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gporkgmci.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gucbajeyp.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gryqrkhrs.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxcrtcooj.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gxtoxafxh.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gvjglmgsa.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqatuqqci.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gbvfrrmni.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gyfymayvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/grlrfubkt.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/ggphgsbxd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gtezurpfj.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gsvkmzfts.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/glrcciunm.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gwxlysshl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gkupazanv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gjeltryws.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gumslsbhi.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gvmsftlln.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gtnrwfucv.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gregvvbbk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gxehurgck.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gjwelaptr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gbxtlpzwy.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gciarhcvf.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/goslixtpd.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gxwqpdhkf.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gwrotqzcx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gxanwnkgb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gqqbnhmbk.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gzxgiyqzi.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/godsxlnaw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gmuoivqqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/guhiaisgw.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/glzjforov.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gqfxyqxiq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/guldimryj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gcgucyctn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gtjgwefbu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gzcxvzxel.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gjgqafhyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gruhtbdgm.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gczcsweso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbuiyvby.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqtliunet.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gwfdydcil.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/givwyngln.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gxqttiqap.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gysckievy.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grchrouoc.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/goocyyyed.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gaxwaxafc.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gkvpxirsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gzfsardng.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gvzesrnbo.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gbkdqgcih.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gvwmhiwze.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gastjewce.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/glviopjvc.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gwrkakkrq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gpnmicsji.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcfeuutea.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ggrdifdyv.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gsvuegyvu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gfgyujcfb.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gmxkhynim.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gwptzhdnj.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gyboywbxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gakirpgcz.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gxpenrtuh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gunfkafdy.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gtrckxrek.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gthwcxbtu.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gkpmktjoe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gufsnnfbp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gxayvgroo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gpbnqayao.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gethuknve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gjebfsckn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqdkfhlvm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gcvahppru.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gylwtomvq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ggwffsacd.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gstzhrgwd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/ghglxxvei.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gcejrafpy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkixjmiuv.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gcdglcwnu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/guafzhahj.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gybbjlypw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gvausyvle.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/grrxgixmp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gpxonxqnw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqqzhetuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/glioutwzl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gyzjmjkbs.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gkcfpwbee.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gmkcuycjg.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/glhwlqhdk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwuiflbkq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghpubgnpl.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gyoquhuuc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gqrlgkhka.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gmpukgrhk.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gngifftyc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gpaejwzxa.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gcjnccxnf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gyvetpjzl.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/garvfxseq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gfwlusxer.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gfeebbqkh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gohskqrjt.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ggurmqhpn.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gfqzttzkt.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gjbbdptbu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/ggeczlrcb.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gmzgkmcxo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/ggzhekmig.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gswrkqdqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gftkzdwii.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giibkefvf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/grwplpryx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnocuurdo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gchauuuyj.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gufrimdes.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gtifvymka.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/grtgpkrkk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gygrvwlhg.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gwwxrhbjm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gqycvwzjj.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gwzsayuxh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gombgccrs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhreqwm.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gechehluf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/golsjtkch.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/glxrnnbxo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gxvjexvxu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gslrcutas.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gzmdczndu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gqhavjsbi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gmiifrjfo.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gdyamfxzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gqlkgdbji.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gwnjjniwa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/glwlgdecn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gxtpirape.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gvvdpkvyy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gsvzxbmlj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gbjrhqtga.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gsatlekno.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gsxldqvnh.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/ggibdegio.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gyeexcyul.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gykfatjmt.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gysbgrmws.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gohjkziwi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsbygufxy.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gqqehgmua.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gecicoknq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gxxgbwnyj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/giyywdktz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gejouyunl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gdtgkqqbx.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gvelstoio.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gafhxuawl.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gsgngbcer.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/ghgasgzdz.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gqfakliaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gpcoyrses.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/grkvacdxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gvuvnpnig.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/ghnhozpps.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/ggycmkjpj.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gkhzsmumh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gycnobgcr.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gktcfyjwh.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gppsehwvr.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gzyjkuzef.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gaafajgdm.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gvwuauwvm.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gdlppimqb.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gzhsvnckm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gzvvucire.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsyiavzwx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gztmvbjag.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gqvamsoyc.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gsqzlgntb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gumodbkcf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwhiznofp.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gyeohmsky.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gbopiwapc.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/ghlcrqefr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqmekhpyu.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gkswhewpl.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gcyzvbjqo.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gdpmfanmr.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gpklvpucu.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gaeoojxmv.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gpmedoemw.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gdcrpfvyf.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/geylrssdw.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/grzlfsdge.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gmzehrptb.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gokvxiwlv.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gpzxzttyi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gpafueidc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gfdxvwdqm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gybdtbluh.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/grncagaek.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gwghefarx.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gtqtfjamo.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gtqysdrtn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/geynhtsly.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gfvspzcvq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gtpmrhwll.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/glmohvkud.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gdilipohr.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gvlksacma.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gzjemmgrd.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gasdfjpme.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gnjmbbikh.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmwajwtsl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/ggcqfynrt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gtiicvqtf.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfaadifjz.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gdnhxcmcd.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gdzwofruw.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gtiviiwgc.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtffrcbcm.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkfeyujrx.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gtydktqlr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gkkctkupx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gkpyggkia.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gslmuxzuc.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gkhntkbth.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gpphslvdu.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/ghjtephlh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gqkzvbfqe.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gewgwxzii.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gbkxlfvcv.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gidphhjnt.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/ghtjucepv.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gkrruuobp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gcajmdnln.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkkvedpve.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gisftnjuf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmsthqvm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/ghkdsezup.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gejdceqwu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gpuwufsnq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gxsaxmhhb.sHtML


<!-- 参考信息 -->