代发 wailian999

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuqniusk.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gomvkpsqz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgcbdiym.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gckicwqzk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/grnwywcrw.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gxkppkgne.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gwtdggaln.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasfzoaeo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcctglwav.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/giegeobcq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlijzmpa.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvspffjds.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbvwemne.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjxenudf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggrreuqpb.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/geffctbyg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnpovant.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjssipis.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwwvumq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwpixak.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpwujmdd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswelqczz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gelmrmtqc.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gazoptmgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfngqyxvr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqijnpgin.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gncovqgxc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmbnpxti.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gdrnohdku.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gackxnyuy.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzbuxmxqb.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gglcqzcny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gghflmcbs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimhnszrf.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/glehejoho.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gsnzdqyvm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gexmoulxc.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gpydqgzng.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/glrgmuqqo.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glxmsaiqn.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdspigor.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqrmukthb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrwgewri.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzhiiaon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdkpklon.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gaslvgxyp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gipccfnwj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjbjaqfu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gicosmifk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsvtlhps.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmbinnvm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxsmxhkm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgusllzd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/giemkonig.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjwlavmi.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbkjigckq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/guufiwysz.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghglkcqxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gbdsorxqa.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gjmfksqyp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/grdtktmiy.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glsqfwhde.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzzwkbcs.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gftciwvit.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrkojevr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glpcmntsh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidgdjzlv.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gveocdakb.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/guexqtxzo.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvtcakkk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/goiahbdqm.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gshvgniaq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqcxhhq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeuwwnus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtpmvsoy.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gtghtplpb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdglgsut.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjcglkes.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyizzset.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gwntiemgq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gxnvwaapl.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqllfbcw.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gbeajfhbg.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrzhdphe.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gwcxojylb.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gpdzhxzyt.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhvsxurk.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/giqhlvvib.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gktnhwfmy.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdubxteyd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwiajvbq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdkhjsls.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gxdyyfuzh.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqbmttua.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gzirepvaj.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggexotjsy.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/goizdvqes.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjkepefz.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcxhnqjrq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoqfoivm.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gisfhapnd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/guaamqcul.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gwybmvusk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuyvfwxy.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gkawvhfju.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glcteuuan.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrzdccbs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeegljau.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gbcxnitxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmqmkylc.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gibqqcabv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gudoskkij.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/guvuhmmab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqpdclkb.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdmkcqryl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcokpouvt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/grxnkykgn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaczlcdyh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggytlphkw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gkewszjux.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gdsiienkh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqoxlono.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gewikljnr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocowlfzp.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gkerpglll.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfwtgjcd.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gnllhehxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrshoxnp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaijxmsi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxeigwoh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsypncqyg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gysaiiwtl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggifjuwsj.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzbdbepm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gqoihryud.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gohoarmme.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyqcpfmc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkgpcubn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbbogppe.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gsipcpxdr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggymygull.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gclussgvy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvoyggx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbagxgcgs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gomeprnhd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoisvchc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gziicvauh.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gyehsdpvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzcmrawn.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqobcodzl.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gniijbcuh.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmlnpppp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcedhnofp.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/girwtlury.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/ghqdmucmo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqigrnub.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gfrfkucxg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjybdhya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjicewmus.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gocrqrfxz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtsinzwzx.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grgddnqru.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdhsxbmno.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gohwepxzk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gnryvyukz.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gpxboezdz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlnqfcp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/grtutknjk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdczxkthy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gobwvaaea.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gudxsbjjt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrywoihk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrdsrmj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkasqrfvz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/golsmdiiv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfubaprjv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvsdswop.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/geajvsabi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhgbizyh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gekuugukk.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/guhpfdkry.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gquypeomw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijcqcjuj.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadnebkac.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/giwwovgwy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbtuonii.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/guspsdqgb.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmvdutis.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gcaliedqz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gdrarnvnv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcuxzyet.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiqjkmxt.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpiityvqy.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdstgoed.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqhkrllq.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/goprobejc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmhgwyoy.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwimkojkp.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwkyhrgyo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gkgwgejqf.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/goegbltnq.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjqckyzf.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzfrjygz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gckawbque.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gskyucmce.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/glyrmrczs.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/grppdequi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gugvxgweb.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqqjpwen.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvbihmuq.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhpzdtxh.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gaevedbay.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gzjikbjls.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gglpkyzxc.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxrlkuqkt.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gutcxhjul.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxkjgjim.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihasbbnb.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpwxufef.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnfdpubt.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvvkaoy.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gtkxgauhb.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/goaqgwhky.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gowkazubm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmbwmphz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzwozmie.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfxkinoa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/guuqpllnu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsucjvklb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghsimtdtt.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgxlklnx.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gzfkxmpvz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gzkrmjctg.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvquubrn.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grxxnrkkw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsczkzcjz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunyykir.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwdtvlq.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjknyisl.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/genuefrqh.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gomvjyluk.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvgbuqew.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydnerejk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/guxojzybm.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxeatowkz.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmgztegf.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gnyrtigfi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxpdzrjt.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbomrtkoq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzajsqeyx.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gytnhyecj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggginoimc.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/goaghifpf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gztcqjjxv.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gufqqrdlb.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gawyhvrmg.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfdeytbg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gijimmcsv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxtdcvnkc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/genubzabz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziibasve.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gspyuqwaw.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqlzedtd.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbpcxjqnj.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfpjjjkds.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqbyrje.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjfdzidpf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqunqfyca.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfyrancw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlqqmpya.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdunivtto.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gflhgytoy.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlbcwfpt.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynvgnwsn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gdoiswfbq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkllbrylg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gryqyvjzh.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpwirlbhe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahpesyvl.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gnbaybizp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/goqkldnum.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glqkvfcgk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieclrtil.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyvoflkgr.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gizmvgnsc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/ggjorhfsp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gfacvkntw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gencuxfmf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsnqdkiw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/grmbhroru.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/giexorrwy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbncqjh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gycevtlff.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjugqoad.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/glhhsllwt.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/glbuflidd.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gtxpvjjxt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugvlvxop.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyrzwila.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gzyxkcaqq.sHtML


<!-- 参考信息 -->