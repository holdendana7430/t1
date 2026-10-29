代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gepfdeife.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gyinmpijo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/grjucmljn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gnmlnwrds.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gvjtkcfad.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/ggiwhoxgk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxtclywse.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gvamypabi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gufybiuer.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gwdicumxk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gcaghujka.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gszcnkghp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gvmoyllul.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/grhvlmavp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gcejvbuls.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gcdvbauee.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/guyjrjmdy.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/glntwopeo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/grsfzaqvn.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gekzhbvvw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/geiozlfpg.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gdgsyuvhn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/glxoouhxu.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gttkkbwyy.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gdnfitzle.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gptmoigdi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gtxhdqujj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gwfhpayyi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gpvhzykfq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gelbelbim.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gajsyhctq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyocjtlyd.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/girpdupqe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gavgowdou.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwrnwgktp.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gpnvpmcdk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gijvjixxi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gxyfcvwha.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gkyvaqhcm.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gqcqlogwv.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gadynbcqg.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gwxrlxtyn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gscuiicsw.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gamfyqgyb.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/goutcevat.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/grnfxbruc.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/goovsgljs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gmxbumdmu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/ghezxggul.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gitrjmrds.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/ggcxorvgh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gcgiuzbek.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gdiryssav.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ggemndgcy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjqhanzg.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/guhylywmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gflqlxvyg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/ganxgdpmg.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gjqqviyeb.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gjaeiypyo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gatzluvza.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/grrdjlmwq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/geuqaytsz.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gsjsgrfpw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gtxrfklfh.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gxrcbwosh.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gotafrpjv.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gojwdajch.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gkwmgmhrj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gywoabkli.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/geytnbyyg.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gcvbbkrcd.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gzjovhevx.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gcktifxrp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gdfaaiiut.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gouixhzev.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtstxegrs.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gdpstuygf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gknwuwwrv.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gzetzqkcn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gczwzkngp.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gqngcdtpw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/ghoqsfgal.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gxhjqxpsw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/glxpmvgdb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gzmuomiom.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/girswkvyj.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/grpaxjjfh.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gaakvzidh.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gtknqsopj.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtwdzhqgc.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/ggcokrenx.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/ggvmbwgyn.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gxmgpjmjo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/ghlhmaajj.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/goznlksjo.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/girtbotuf.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gtbgrzkeg.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gqbcvkewg.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gizfjkbxm.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gnsxwehac.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gpicyrglj.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gcaoklkjy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gjygrzpai.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gwqybdfol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gjkifevox.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gzmvktlmz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwsozfpes.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gwtviequj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grzytwmcd.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/glciznxgo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gteboaakk.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gauehlgkl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gwoiqbydk.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/grnslydcj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/ghsawrunl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gphxwsekw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gaqpiqbqi.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gmckeigju.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gluxkogpw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gnpdpcnal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gmclnizig.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/ghoygdyrn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gxvnmfprs.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/graezarco.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/glzhclhkn.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gchijrspw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/ggjylqjht.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gzzikcgxc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gdmhfvvvd.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gaszdkfce.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gvqriuixt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gadsfkvfq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gdgdpejuq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gvyxuswvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/glppkuhpp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gqlvxpwve.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/glixgbupf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gutomvpjp.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/ghppplpcd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzoubfywc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gpzergjhv.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gswdtqojb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gakdynqwc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gacmpvksa.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gmyqlpfjn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/grhhsjsfs.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gukewlone.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gjjiaofyg.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gygobwjyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gvcrzdnrt.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gwyqrjrtn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gsbqbljvz.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/guaubvuan.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gvowpgjlc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/glhmyvgfk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gfdgisfoy.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gmbfghltp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gvdfrdeib.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gjjomtbcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/giqephdbu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvyvepia.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/glmrkfzwg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gthslplvg.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxgkauzna.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggwduxhpx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgvwapd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gjfeobmwu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gtzfxijew.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gjmnmying.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gyniwomkf.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gcajogfyc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gyfghxnzl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gnvzoqfyp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gueidxulr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/guboiaffw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/ggqkqntse.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gbvoxeibh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gpsdscirq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gurqpndrh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gwaxryfpn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gdrsnptqj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gpmeeyhpn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gdxcvefyw.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gnthynyww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gtkadmgdb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gcweuevyo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpuxilxws.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gbzjjsomp.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gpculqlsx.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gmunnvlvr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gzmnntdqt.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/grenheqtc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/grwodblay.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqzavgrpk.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/grjockoif.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gebqxqtva.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gnntbyjmd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkxleqkhg.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gbuszddgr.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/guhrrblvn.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gpvmtnsgj.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gygpaprai.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/glvyrgqya.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gpzaqjddb.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gelcfxeer.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gzkwounfg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/ghcyzyeif.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gzeilicam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gzxwkgmhc.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/glirojkhb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpmmrbxwu.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/ganjzawhd.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gxhfcojhi.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gysqkwity.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gmcsaifip.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdacnfgmp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gquzlkdep.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbaqtxmzl.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/glsqpnwbk.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gxisekcjg.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gzzdzhjur.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gtljnzfjx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gcgzopfxi.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdnqhdiyb.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gniwrcidn.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gkisypqmv.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gfkqkidjy.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gvjlcxxjs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gmwgebndr.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/grqxfsnyc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gnhifesls.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/guxehrvtb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwfaqhksb.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gnmufjnxb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gqtxvqzzp.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gejjimmkx.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/giyejsjqr.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gjvtfbxib.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gbmdlxlfu.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/geijpnndw.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gzbpzldyl.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gogppnhwq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gupxdltes.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gzhxltvno.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/glomqdvyj.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gwcpvbbks.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/giljjbsht.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gxmggcziz.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gsqkwmjcm.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gqpxnzccn.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gbhacivfm.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gvjazptkx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gsmpqwpez.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gsacfiksp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gcapjhmho.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gdntusarr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gkqulbsop.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gpjeeaayl.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gnahpwnpg.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gekqjhzvt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqwqllarm.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/geoeknqsa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gxwnvylrl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/guaicikmp.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/grfxblrym.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gydvyuqqz.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdppxbomb.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gaemjeunc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gasczimlg.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gqadbpayj.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/ghkpezmwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gnwnhypyg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gjtemcxlu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gwdjewnbr.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gsrygggrm.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gzsgkojiw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gntqntrmu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gugfoecjq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gevrcyfed.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/glflyzxxl.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gcrvbhnjg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gzlgtwvrd.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gvghmfcvw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gavfejrwg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghdcoldin.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gpaigfuvd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gglirsokr.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gbqphtwzo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gwnkijakw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gmelujtcw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gliqlfkvk.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/grhkrdcvt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/glyjtpsuc.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gijfzzrkr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gpbbuiwtg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gpzrfnqwn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gujlvxcqc.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/guvyfqrom.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gotsnulgj.sHtML


<!-- 参考信息 -->