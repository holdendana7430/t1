代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://rd.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://vc.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://hd.huixiangedu.cn

[S03] C：读入整数
来源：http://ds.nszjky.cn

int x; scanf("%d", &x);
来源：http://aw.9csxet.cn

[S04] C：字符串复制
来源：http://ot.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ym.szxytkj.cn

[S05] C：字符串长度
来源：http://vo.bookmarksfly.cn

strlen(s)
来源：http://ad.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://gz.hnjuh.cn

strcmp(a, b) == 0
来源：http://gp.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://jw.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qj.521024.cn

[S08] C：动态内存分配与释放
来源：http://qk.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qq.asd995.cn

[S09] C：结构体定义与初始化
来源：http://ar.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wb.hahajie.cn

[S10] C：指针与解引用
来源：http://ue.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://vw.szxytkj.cn

[S11] C：逐行读文件
来源：http://kt.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://rn.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fx.panjiajie.cn

fclose(f);
来源：http://sb.bjjhwx.cn

[S12] C：写文件
来源：http://kz.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eq.shxzukj.cn

[S13] C：宏定义
来源：http://aq.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nk.colortex.cn

[S14] C：枚举
来源：http://tn.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ov.huanxung.cn

[S15] C：类型转换
来源：http://qk.shtwfgs.cn

(double) a / b
来源：http://gz.shxzskj.cn

[S16] C：位操作置位
来源：http://wx.szxytkj.cn

x |= (1 << 3);
来源：http://wj.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://lc.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uk.jctech888.com.cn

[S18] C：命令行参数
来源：http://or.jctech888.com.cn

int main(int argc, char **argv)
来源：http://re.yuntaijiaju.cn

[S19] C：快速排序
来源：http://th.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oo.nicolike.cn

[S20] C：二分查找
来源：http://ii.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ms.gzmigu.cn

[S21] C：字符类别判断
来源：http://sc.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lm.shxzukj.cn

[S22] C：字符串转数字
来源：http://ib.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bc.szsharing.cn

[S23] C：随机数
来源：http://ex.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ax.lnxyls.cn

[S24] C：获取本地时间
来源：http://sq.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qz.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://mx.nszjky.cn

memcpy(dst, src, n);
来源：http://nr.nicolike.cn

[S26] C：内存清零
来源：http://co.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://rj.nicolike.cn

[S27] C：定义常量
来源：http://mt.hnjuh.cn

const double PI = 3.14159;
来源：http://fz.panjiajie.cn

[S28] C：静态变量
来源：http://hn.jctech888.com.cn

static int counter = 0;
来源：http://ad.chemitech.net.cn

[S29] C：变参函数
来源：http://am.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yx.huixiangedu.cn

[S30] C：头文件保护
来源：http://aj.jianghongdianzi.cn

#ifndef X_H
来源：http://bf.huixiangedu.cn

#define X_H
来源：http://nu.hahajie.cn

#endif
来源：http://kk.newstarts.cn

[S31] C++：Hello World
来源：http://cp.jctech888.com.cn

#include <iostream>
来源：http://sz.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://li.nszjky.cn

[S32] C++：字符串
来源：http://fa.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://jt.haigaiapp.cn

[S33] C++：vector 增删
来源：http://fi.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kz.shxzskj.cn

[S34] C++：遍历 vector
来源：http://et.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://rp.panjiajie.cn

[S35] C++：map
来源：http://sx.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lf.colortex.cn

[S36] C++：unordered_map
来源：http://pj.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cs.lnxyls.cn

[S37] C++：set
来源：http://py.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://az.jctech888.com.cn

[S38] C++：排序
来源：http://rf.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://vp.asd995.cn

[S39] C++：自定义比较器排序
来源：http://du.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yz.huanxung.cn

[S40] C++：查找元素
来源：http://lf.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uy.hahajie.cn

[S41] C++：类与构造函数
来源：http://nx.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nt.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://ao.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://gc.newstarts.cn

[S43] C++：智能指针
来源：http://hl.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://js.haigaiapp.cn

[S44] C++：引用传参
来源：http://nq.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://fh.szsharing.cn

[S45] C++：lambda
来源：http://nk.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://az.shxzskj.cn

[S46] C++：函数模板
来源：http://co.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qm.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://dx.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oo.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ut.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ir.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ro.shxzukj.cn

[S49] C++：写文件
来源：http://pd.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://er.nicolike.cn

[S50] C++：格式化数字
来源：http://ts.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qg.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://de.gzmigu.cn

static_cast<double>(a) / b
来源：http://tr.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://wc.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://av.shtwfgs.cn

[S53] C++：移动语义
来源：http://rt.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://jm.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://bt.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://te.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ct.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zp.chemitech.net.cn

[S56] C++：optional
来源：http://xt.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lw.521024.cn

[S57] C++：编译期常量
来源：http://kq.yuexingan06.cn

constexpr int N = 10;
来源：http://tn.szsharing.cn

[S58] C++：命名空间
来源：http://vv.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://wd.haigaiapp.cn

[S59] C++：静态断言
来源：http://im.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aq.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://wq.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rw.yuexingan06.cn

================================================================================
来源：http://bu.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://py.nicolike.cn

================================================================================
来源：http://at.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://cz.bookmarksfly.cn

println("Hello")
来源：http://nc.newstarts.cn

[T02] Kotlin：变量
来源：http://nf.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xz.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://xs.nicolike.cn

"值: $b"
来源：http://dz.hnjuh.cn

[T04] Kotlin：空安全
来源：http://mm.521024.cn

val n: String? = null;  n?.length
来源：http://wz.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://sp.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aa.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://to.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nz.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://nn.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eg.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://hr.colortex.cn

data class User(val name: String, val age: Int)
来源：http://db.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://is.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://de.colortex.cn

[T10] Kotlin：默认参数
来源：http://mz.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fs.jctech888.com.cn

[T11] Kotlin：协程
来源：http://xe.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qy.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://xa.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://qu.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://id.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ql.chemitech.net.cn

[T14] Kotlin：循环
来源：http://qv.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://cy.colortex.cn

[T15] Kotlin：接口
来源：http://qy.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://bv.colortex.cn

[T16] Swift：Hello World
来源：http://er.wgjwhj.cn

print("Hello")
来源：http://ds.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://mq.gzmigu.cn

var a = 1;  let b = 2
来源：http://et.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://ar.nicolike.cn

"值: \(b)"
来源：http://xv.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://bq.chemitech.net.cn

if let n = opt { print(n) }
来源：http://xg.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ov.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dg.hnjuh.cn

[T21] Swift：遍历
来源：http://lm.bookmarksfly.cn

for x in a { print(x) }
来源：http://fv.9csxet.cn

[T22] Swift：字典
来源：http://ev.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nz.9csxet.cn

[T23] Swift：函数
来源：http://zx.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wt.chemitech.net.cn

[T24] Swift：闭包
来源：http://fb.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nt.huixiangedu.cn

[T25] Swift：结构体
来源：http://px.huanxung.cn

struct P { var x: Int }
来源：http://bs.hnjuh.cn

[T26] Swift：类与重写
来源：http://cg.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://nf.521024.cn

[T27] Swift：错误处理
来源：http://gq.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://xf.chemitech.net.cn

[T28] Swift：枚举
来源：http://xe.nicolike.cn

enum Color { case red, green }
来源：http://to.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://zz.szsharing.cn

guard let x = opt else { return }
来源：http://uv.wgjwhj.cn

[T30] Swift：协议
来源：http://rk.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://mr.lnxyls.cn

[T31] Lua：Hello World
来源：http://fl.bjjhwx.cn

print("Hello")
来源：http://hs.lnxyls.cn

[T32] Lua：局部变量
来源：http://df.yuexingan06.cn

local a = 1
来源：http://lj.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://pp.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nd.521024.cn

[T34] Lua：遍历表
来源：http://ed.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ei.lnxyls.cn

[T35] Lua：字典表
来源：http://go.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://rb.yuntaijiaju.cn

[T36] Lua：函数
来源：http://sw.shxzukj.cn

function add(a, b) return a + b end
来源：http://xn.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://mb.newstarts.cn

"a" .. "b"
来源：http://jz.shxzukj.cn

[T38] Lua：条件
来源：http://mi.hahajie.cn

if x > 0 then print("正") end
来源：http://lz.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://um.bjjhwx.cn

string.find(s, "%d+")
来源：http://es.bookmarksfly.cn

[T40] Lua：元表
来源：http://rg.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://of.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ya.gzmigu.cn

print "Hello\n";
来源：http://er.bjjhwx.cn

[T42] Perl：变量类型
来源：http://hv.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zx.szxytkj.cn

[T43] Perl：字符串插值
来源：http://dj.haigaiapp.cn

"值: $a"
来源：http://nz.jctech888.com.cn

[T44] Perl：条件
来源：http://bn.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://qu.hnjuh.cn

[T45] Perl：数组遍历
来源：http://hr.colortex.cn

for my $x (@arr) { print $x; }
来源：http://lu.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://oy.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://px.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://ox.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zp.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://qs.hnjuh.cn

$s =~ s/old/new/g;
来源：http://jd.newstarts.cn

[T49] Perl：函数
来源：http://ol.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://at.newstarts.cn

[T50] Perl：逐行读文件
来源：http://zo.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wp.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://it.huanxung.cn

[T51] Scala：Hello World
来源：http://in.chemitech.net.cn

println("Hello")
来源：http://py.asd995.cn

[T52] Scala：变量
来源：http://qa.szsharing.cn

val a = 1;  var b = 2
来源：http://lt.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ev.lnxyls.cn

s"值: $b"
来源：http://du.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://mv.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://nc.shxzukj.cn

[T55] Scala：集合过滤
来源：http://pg.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jt.huanxung.cn

[T56] Scala：样例类
来源：http://tb.szxytkj.cn

case class User(name: String, age: Int)
来源：http://hh.szxytkj.cn

[T57] Scala：模式匹配
来源：http://li.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fk.newstarts.cn

[T58] Scala：函数定义
来源：http://qz.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wz.nszjky.cn

[T59] Scala：循环
来源：http://ix.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://lf.huanxung.cn

[T60] Scala：折叠
来源：http://dy.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ow.9csxet.cn

================================================================================
来源：http://fw.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sg.gzmigu.cn

================================================================================
来源：http://ek.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://uw.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dh.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://td.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vj.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ou.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zq.szsharing.cn

[U04] Py：变量调试打印
来源：http://tm.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wz.asd995.cn

[U05] Py：列表去重且保序
来源：http://nb.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://je.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://if.nicolike.cn

{**a, **b}
来源：http://zx.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://jl.521024.cn

{v: k for k, v in d.items()}
来源：http://mx.hnjuh.cn

[U08] Py：展平二维列表
来源：http://ox.chemitech.net.cn

[y for x in nested for y in x]
来源：http://no.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://kz.yuntaijiaju.cn

max(d, key=d.get)
来源：http://vh.521024.cn

[U10] Py：按值排序字典
来源：http://ie.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yz.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://uo.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://jx.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://az.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ey.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://jy.panjiajie.cn

deque(maxlen=10)
来源：http://rl.newstarts.cn

[U14] Py：分组收集到列表
来源：http://ni.szxytkj.cn

defaultdict(list)
来源：http://og.bjjhwx.cn

[U15] Py：高精度计时
来源：http://bl.yuexingan06.cn

t = time.perf_counter()
来源：http://ni.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://pl.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cd.shxzukj.cn

[U17] Py：初始化日志
来源：http://hj.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://jb.panjiajie.cn

[U18] Py：预编译正则
来源：http://jb.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://gx.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://kv.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ps.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://px.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://za.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://xu.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://ae.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://yl.huixiangedu.cn

list(zip(*m))
来源：http://me.newstarts.cn

[U23] Py：分块读取大文件
来源：http://ss.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aq.jctech888.com.cn

[U24] Py：路径操作
来源：http://wl.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ox.chemitech.net.cn


<!-- 参考信息 -->