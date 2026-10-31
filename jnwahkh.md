代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://bf.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://kp.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://zx.yuntaijiaju.cn

[S03] C：读入整数
来源：http://av.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://hu.gzmigu.cn

[S04] C：字符串复制
来源：http://da.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sb.huixiangedu.cn

[S05] C：字符串长度
来源：http://cs.9csxet.cn

strlen(s)
来源：http://ha.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://jf.chemitech.net.cn

strcmp(a, b) == 0
来源：http://qs.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://og.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tn.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://hf.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ya.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://ts.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lq.newstarts.cn

[S10] C：指针与解引用
来源：http://fe.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://ce.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://zu.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://lv.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pv.chemitech.net.cn

fclose(f);
来源：http://az.szsharing.cn

[S12] C：写文件
来源：http://jj.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ge.shxzukj.cn

[S13] C：宏定义
来源：http://xj.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kt.bjjhwx.cn

[S14] C：枚举
来源：http://ts.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://bj.hnjuh.cn

[S15] C：类型转换
来源：http://wp.bjjhwx.cn

(double) a / b
来源：http://ih.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://fo.jctech888.com.cn

x |= (1 << 3);
来源：http://ox.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://fq.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uz.chemitech.net.cn

[S18] C：命令行参数
来源：http://yc.9csxet.cn

int main(int argc, char **argv)
来源：http://ud.huanxung.cn

[S19] C：快速排序
来源：http://ow.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pl.shxzukj.cn

[S20] C：二分查找
来源：http://nr.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sm.colortex.cn

[S21] C：字符类别判断
来源：http://mb.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bf.panjiajie.cn

[S22] C：字符串转数字
来源：http://pp.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oo.szsharing.cn

[S23] C：随机数
来源：http://gp.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://na.shtwfgs.cn

[S24] C：获取本地时间
来源：http://yo.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yy.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://zf.muxihuayi.cn

memcpy(dst, src, n);
来源：http://ez.shxzukj.cn

[S26] C：内存清零
来源：http://no.9csxet.cn

memset(a, 0, sizeof a);
来源：http://jt.bookmarksfly.cn

[S27] C：定义常量
来源：http://lm.hahajie.cn

const double PI = 3.14159;
来源：http://ni.asd995.cn

[S28] C：静态变量
来源：http://gk.yuntaijiaju.cn

static int counter = 0;
来源：http://zh.colortex.cn

[S29] C：变参函数
来源：http://cv.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://va.szxytkj.cn

[S30] C：头文件保护
来源：http://im.panjiajie.cn

#ifndef X_H
来源：http://im.bjjhwx.cn

#define X_H
来源：http://fc.gzmigu.cn

#endif
来源：http://dg.jctech888.com.cn

[S31] C++：Hello World
来源：http://ed.asd995.cn

#include <iostream>
来源：http://ou.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://pa.newstarts.cn

[S32] C++：字符串
来源：http://hc.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://pl.gzmigu.cn

[S33] C++：vector 增删
来源：http://gr.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cv.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://uv.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://nn.yuntaijiaju.cn

[S35] C++：map
来源：http://xd.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jj.yuexingan06.cn

[S36] C++：unordered_map
来源：http://pm.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rs.shtwfgs.cn

[S37] C++：set
来源：http://nk.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ye.jctech888.com.cn

[S38] C++：排序
来源：http://le.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://wd.colortex.cn

[S39] C++：自定义比较器排序
来源：http://as.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://im.wgjwhj.cn

[S40] C++：查找元素
来源：http://pd.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ta.hnjuh.cn

[S41] C++：类与构造函数
来源：http://rs.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qg.szsharing.cn

[S42] C++：继承与虚函数
来源：http://wc.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://vv.gzmigu.cn

[S43] C++：智能指针
来源：http://kl.521024.cn

auto p = std::make_unique<int>(5);
来源：http://tu.chemitech.net.cn

[S44] C++：引用传参
来源：http://du.huanxung.cn

void inc(int &x) { ++x; }
来源：http://mq.hahajie.cn

[S45] C++：lambda
来源：http://mu.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vv.bjjhwx.cn

[S46] C++：函数模板
来源：http://dn.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sb.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://ux.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fi.panjiajie.cn

[S48] C++：逐行读文件
来源：http://lp.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://go.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://kx.bookmarksfly.cn

[S49] C++：写文件
来源：http://gu.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eg.chemitech.net.cn

[S50] C++：格式化数字
来源：http://eq.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fo.shxzskj.cn

[S51] C++：显式类型转换
来源：http://ir.nszjky.cn

static_cast<double>(a) / b
来源：http://xd.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://va.huanxung.cn

int size() const noexcept { return n_; }
来源：http://hf.huanxung.cn

[S53] C++：移动语义
来源：http://dq.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://op.lnxyls.cn

[S54] C++：异常处理
来源：http://td.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ip.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://eq.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ly.9csxet.cn

[S56] C++：optional
来源：http://ed.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eb.szxytkj.cn

[S57] C++：编译期常量
来源：http://oc.gzmigu.cn

constexpr int N = 10;
来源：http://jp.colortex.cn

[S58] C++：命名空间
来源：http://zd.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ew.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ci.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fy.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://oy.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wb.lnxyls.cn

================================================================================
来源：http://ka.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yz.panjiajie.cn

================================================================================
来源：http://mc.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://jt.yuntaijiaju.cn

println("Hello")
来源：http://cm.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://ge.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yb.colortex.cn

[T03] Kotlin：字符串模板
来源：http://pa.jctech888.com.cn

"值: $b"
来源：http://pw.gzmigu.cn

[T04] Kotlin：空安全
来源：http://ze.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ei.colortex.cn

[T05] Kotlin：when 表达式
来源：http://sr.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://be.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://rb.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mx.521024.cn

[T07] Kotlin：集合过滤
来源：http://cs.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xs.9csxet.cn

[T08] Kotlin：数据类
来源：http://ff.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://jt.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://rr.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://bx.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://ba.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hi.hnjuh.cn

[T11] Kotlin：协程
来源：http://th.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rl.colortex.cn

[T12] Kotlin：解构声明
来源：http://qm.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://zt.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://yy.9csxet.cn

val m = mapOf("a" to 1)
来源：http://st.huixiangedu.cn

[T14] Kotlin：循环
来源：http://vu.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://wi.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://tw.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ft.shxzskj.cn

[T16] Swift：Hello World
来源：http://ho.wgjwhj.cn

print("Hello")
来源：http://sd.szsharing.cn

[T17] Swift：变量与常量
来源：http://aj.shxzukj.cn

var a = 1;  let b = 2
来源：http://qf.szsharing.cn

[T18] Swift：字符串插值
来源：http://oc.hnjuh.cn

"值: \(b)"
来源：http://jx.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://su.wgjwhj.cn

if let n = opt { print(n) }
来源：http://zc.haigaiapp.cn

[T20] Swift：数组操作
来源：http://gm.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://go.jctech888.com.cn

[T21] Swift：遍历
来源：http://kp.521024.cn

for x in a { print(x) }
来源：http://ju.huixiangedu.cn

[T22] Swift：字典
来源：http://if.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://py.huixiangedu.cn

[T23] Swift：函数
来源：http://aa.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nn.9csxet.cn

[T24] Swift：闭包
来源：http://fl.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jd.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://xr.shtwfgs.cn

struct P { var x: Int }
来源：http://kw.nszjky.cn

[T26] Swift：类与重写
来源：http://dc.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://la.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://ln.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://ek.hahajie.cn

[T28] Swift：枚举
来源：http://il.shxzskj.cn

enum Color { case red, green }
来源：http://rc.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://nv.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ql.szsharing.cn

[T30] Swift：协议
来源：http://nx.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://kp.asd995.cn

[T31] Lua：Hello World
来源：http://xj.nszjky.cn

print("Hello")
来源：http://om.wgjwhj.cn

[T32] Lua：局部变量
来源：http://or.yuntaijiaju.cn

local a = 1
来源：http://wi.hahajie.cn

[T33] Lua：表（数组）
来源：http://ja.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cx.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://mf.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gc.nicolike.cn

[T35] Lua：字典表
来源：http://sc.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://fn.hnjuh.cn

[T36] Lua：函数
来源：http://ww.shxzukj.cn

function add(a, b) return a + b end
来源：http://hq.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://aj.bjjhwx.cn

"a" .. "b"
来源：http://ha.szxytkj.cn

[T38] Lua：条件
来源：http://ee.nicolike.cn

if x > 0 then print("正") end
来源：http://ru.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://cf.panjiajie.cn

string.find(s, "%d+")
来源：http://th.szxytkj.cn

[T40] Lua：元表
来源：http://mo.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://yo.bjjhwx.cn

[T41] Perl：Hello World
来源：http://jj.newstarts.cn

print "Hello\n";
来源：http://vd.lnxyls.cn

[T42] Perl：变量类型
来源：http://wt.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xw.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://jw.bookmarksfly.cn

"值: $a"
来源：http://vc.lnxyls.cn

[T44] Perl：条件
来源：http://ee.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://mx.gzmigu.cn

[T45] Perl：数组遍历
来源：http://rp.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://yg.huanxung.cn

[T46] Perl：哈希操作
来源：http://jc.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xr.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://to.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hw.huixiangedu.cn

[T48] Perl：正则替换
来源：http://hr.nicolike.cn

$s =~ s/old/new/g;
来源：http://cu.szxytkj.cn

[T49] Perl：函数
来源：http://ak.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ms.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://sh.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fh.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://zt.shxzskj.cn

[T51] Scala：Hello World
来源：http://ys.nicolike.cn

println("Hello")
来源：http://ho.haigaiapp.cn

[T52] Scala：变量
来源：http://bs.huixiangedu.cn

val a = 1;  var b = 2
来源：http://la.asd995.cn

[T53] Scala：字符串插值
来源：http://bn.asd995.cn

s"值: $b"
来源：http://aj.wgjwhj.cn

[T54] Scala：集合映射
来源：http://mf.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://gj.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://ht.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ac.wgjwhj.cn

[T56] Scala：样例类
来源：http://pe.hahajie.cn

case class User(name: String, age: Int)
来源：http://ky.hnjuh.cn

[T57] Scala：模式匹配
来源：http://zh.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gs.huixiangedu.cn

[T58] Scala：函数定义
来源：http://zm.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ve.gzmigu.cn

[T59] Scala：循环
来源：http://xm.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://pw.gzmigu.cn

[T60] Scala：折叠
来源：http://zy.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ld.huixinmuqiang.cn

================================================================================
来源：http://gg.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mm.nicolike.cn

================================================================================
来源：http://kk.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://da.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pl.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://et.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ih.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://bc.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gt.szsharing.cn

[U04] Py：变量调试打印
来源：http://gj.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eb.szsharing.cn

[U05] Py：列表去重且保序
来源：http://yp.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://pw.521024.cn

[U06] Py：合并两个字典
来源：http://at.gzmigu.cn

{**a, **b}
来源：http://nj.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://fa.hahajie.cn

{v: k for k, v in d.items()}
来源：http://nj.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://mi.shxzskj.cn

[y for x in nested for y in x]
来源：http://ud.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://xd.asd995.cn

max(d, key=d.get)
来源：http://we.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://sf.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yi.nszjky.cn

[U11] Py：生成器表达式
来源：http://av.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://dr.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ao.panjiajie.cn

Counter(arr).most_common(3)
来源：http://sr.521024.cn

[U13] Py：固定长度队列
来源：http://kx.colortex.cn

deque(maxlen=10)
来源：http://cm.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://ay.newstarts.cn

defaultdict(list)
来源：http://rm.hnjuh.cn

[U15] Py：高精度计时
来源：http://bd.lnxyls.cn

t = time.perf_counter()
来源：http://ie.521024.cn

[U16] Py：命令行参数解析
来源：http://wh.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pe.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://sl.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://fd.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://ln.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://iq.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://wt.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bd.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://ti.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://yh.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://rv.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://po.gzmigu.cn

[U22] Py：矩阵转置
来源：http://od.muxihuayi.cn

list(zip(*m))
来源：http://ti.szsharing.cn

[U23] Py：分块读取大文件
来源：http://un.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kn.jctech888.com.cn

[U24] Py：路径操作
来源：http://me.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ii.panjiajie.cn


<!-- 参考信息 -->