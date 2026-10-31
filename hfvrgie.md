代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://xr.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://fy.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://fz.asd995.cn

[S03] C：读入整数
来源：http://xb.nszjky.cn

int x; scanf("%d", &x);
来源：http://nt.yuexingan06.cn

[S04] C：字符串复制
来源：http://lm.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rw.bjjhwx.cn

[S05] C：字符串长度
来源：http://qm.521024.cn

strlen(s)
来源：http://nb.wgjwhj.cn

[S06] C：字符串比较
来源：http://zx.shxzskj.cn

strcmp(a, b) == 0
来源：http://iv.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://mo.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lg.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://iq.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yq.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://ux.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ro.shxzukj.cn

[S10] C：指针与解引用
来源：http://jl.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://fi.wgjwhj.cn

[S11] C：逐行读文件
来源：http://xo.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://ax.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oa.shxzukj.cn

fclose(f);
来源：http://fi.shxzukj.cn

[S12] C：写文件
来源：http://ig.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bc.bookmarksfly.cn

[S13] C：宏定义
来源：http://op.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rt.nszjky.cn

[S14] C：枚举
来源：http://be.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://lm.panjiajie.cn

[S15] C：类型转换
来源：http://co.chemitech.net.cn

(double) a / b
来源：http://be.bjjhwx.cn

[S16] C：位操作置位
来源：http://io.nszjky.cn

x |= (1 << 3);
来源：http://uk.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://yf.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fs.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://bg.huanxung.cn

int main(int argc, char **argv)
来源：http://uz.szxytkj.cn

[S19] C：快速排序
来源：http://ld.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xi.gzmigu.cn

[S20] C：二分查找
来源：http://gw.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oy.haigaiapp.cn

[S21] C：字符类别判断
来源：http://vo.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ey.colortex.cn

[S22] C：字符串转数字
来源：http://ts.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tz.huixinmuqiang.cn

[S23] C：随机数
来源：http://fn.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oj.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://wc.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ut.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://qz.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ra.huanxung.cn

[S26] C：内存清零
来源：http://kn.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://kv.panjiajie.cn

[S27] C：定义常量
来源：http://lf.hahajie.cn

const double PI = 3.14159;
来源：http://yf.nicolike.cn

[S28] C：静态变量
来源：http://ci.shxzukj.cn

static int counter = 0;
来源：http://vv.hnjuh.cn

[S29] C：变参函数
来源：http://wu.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lw.yuexingan06.cn

[S30] C：头文件保护
来源：http://yy.521024.cn

#ifndef X_H
来源：http://ti.521024.cn

#define X_H
来源：http://qc.yuexingan06.cn

#endif
来源：http://ug.521024.cn

[S31] C++：Hello World
来源：http://or.szsharing.cn

#include <iostream>
来源：http://vc.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://hq.nicolike.cn

[S32] C++：字符串
来源：http://wx.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://gi.newstarts.cn

[S33] C++：vector 增删
来源：http://gi.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xk.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://mk.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://vb.bookmarksfly.cn

[S35] C++：map
来源：http://dk.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://us.huanxung.cn

[S36] C++：unordered_map
来源：http://fw.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.jctech888.com.cn

[S37] C++：set
来源：http://ou.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oi.bjjhwx.cn

[S38] C++：排序
来源：http://fr.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://hp.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://qo.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://is.huanxung.cn

[S40] C++：查找元素
来源：http://xn.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ey.lnxyls.cn

[S41] C++：类与构造函数
来源：http://in.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://me.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://rd.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://np.haigaiapp.cn

[S43] C++：智能指针
来源：http://mx.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://rf.hahajie.cn

[S44] C++：引用传参
来源：http://rj.huanxung.cn

void inc(int &x) { ++x; }
来源：http://nm.huixiangedu.cn

[S45] C++：lambda
来源：http://jn.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rh.shtwfgs.cn

[S46] C++：函数模板
来源：http://vl.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lp.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://pc.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ha.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://db.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://it.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://pn.gzmigu.cn

[S49] C++：写文件
来源：http://qe.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ug.huanxung.cn

[S50] C++：格式化数字
来源：http://gr.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ij.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://qg.521024.cn

static_cast<double>(a) / b
来源：http://ew.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://tm.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://hs.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://cj.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://lj.colortex.cn

[S54] C++：异常处理
来源：http://yy.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yg.panjiajie.cn

[S55] C++：结构化绑定
来源：http://hh.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://im.9csxet.cn

[S56] C++：optional
来源：http://lv.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jm.nszjky.cn

[S57] C++：编译期常量
来源：http://wp.lnxyls.cn

constexpr int N = 10;
来源：http://jh.panjiajie.cn

[S58] C++：命名空间
来源：http://ac.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://sc.huixiangedu.cn

[S59] C++：静态断言
来源：http://kv.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jh.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://sb.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ci.huanxung.cn

================================================================================
来源：http://ht.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bd.panjiajie.cn

================================================================================
来源：http://wi.nicolike.cn

[T01] Kotlin：Hello World
来源：http://bf.huanxung.cn

println("Hello")
来源：http://kq.szxytkj.cn

[T02] Kotlin：变量
来源：http://ts.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cb.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://yd.haigaiapp.cn

"值: $b"
来源：http://az.asd995.cn

[T04] Kotlin：空安全
来源：http://ms.nszjky.cn

val n: String? = null;  n?.length
来源：http://tf.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://pi.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bj.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://to.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rr.colortex.cn

[T07] Kotlin：集合过滤
来源：http://dk.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fm.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://vm.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://vy.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://uu.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://sl.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://sc.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jk.bjjhwx.cn

[T11] Kotlin：协程
来源：http://qw.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fk.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://te.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://fm.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://br.huanxung.cn

val m = mapOf("a" to 1)
来源：http://bs.nszjky.cn

[T14] Kotlin：循环
来源：http://kc.nszjky.cn

for (i in 1..10) println(i)
来源：http://rv.hahajie.cn

[T15] Kotlin：接口
来源：http://ro.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://wi.521024.cn

[T16] Swift：Hello World
来源：http://ex.9csxet.cn

print("Hello")
来源：http://fe.shxzukj.cn

[T17] Swift：变量与常量
来源：http://qs.hahajie.cn

var a = 1;  let b = 2
来源：http://sb.lnxyls.cn

[T18] Swift：字符串插值
来源：http://fe.huixinmuqiang.cn

"值: \(b)"
来源：http://hr.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://jh.hahajie.cn

if let n = opt { print(n) }
来源：http://rt.shxzukj.cn

[T20] Swift：数组操作
来源：http://dl.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gs.wgjwhj.cn

[T21] Swift：遍历
来源：http://yj.bjjhwx.cn

for x in a { print(x) }
来源：http://ig.hahajie.cn

[T22] Swift：字典
来源：http://vb.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rn.asd995.cn

[T23] Swift：函数
来源：http://ao.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mg.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://tk.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xs.colortex.cn

[T25] Swift：结构体
来源：http://gh.shtwfgs.cn

struct P { var x: Int }
来源：http://ll.lnxyls.cn

[T26] Swift：类与重写
来源：http://cl.huanxung.cn

class A: Base { override func f() {} }
来源：http://nf.nicolike.cn

[T27] Swift：错误处理
来源：http://lu.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://fy.huanxung.cn

[T28] Swift：枚举
来源：http://sp.hnjuh.cn

enum Color { case red, green }
来源：http://dd.asd995.cn

[T29] Swift：guard 提前返回
来源：http://kp.lnxyls.cn

guard let x = opt else { return }
来源：http://xt.nszjky.cn

[T30] Swift：协议
来源：http://mn.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://ic.haigaiapp.cn

[T31] Lua：Hello World
来源：http://vf.yuntaijiaju.cn

print("Hello")
来源：http://vj.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://wu.asd995.cn

local a = 1
来源：http://rp.asd995.cn

[T33] Lua：表（数组）
来源：http://xp.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oy.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ge.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jg.521024.cn

[T35] Lua：字典表
来源：http://mc.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://ay.nszjky.cn

[T36] Lua：函数
来源：http://ho.huanxung.cn

function add(a, b) return a + b end
来源：http://fi.nicolike.cn

[T37] Lua：字符串拼接
来源：http://qs.bjjhwx.cn

"a" .. "b"
来源：http://pq.nszjky.cn

[T38] Lua：条件
来源：http://nm.shtwfgs.cn

if x > 0 then print("正") end
来源：http://wm.colortex.cn

[T39] Lua：模式匹配
来源：http://vj.bjjhwx.cn

string.find(s, "%d+")
来源：http://io.hnjuh.cn

[T40] Lua：元表
来源：http://xm.asd995.cn

setmetatable({}, { __index = base })
来源：http://iy.haigaiapp.cn

[T41] Perl：Hello World
来源：http://az.szsharing.cn

print "Hello\n";
来源：http://eo.muxihuayi.cn

[T42] Perl：变量类型
来源：http://ev.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hw.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://zm.huixinmuqiang.cn

"值: $a"
来源：http://bk.colortex.cn

[T44] Perl：条件
来源：http://pd.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://vm.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://wt.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://ej.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://eo.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uf.huanxung.cn

[T47] Perl：正则捕获
来源：http://mr.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gk.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://ma.521024.cn

$s =~ s/old/new/g;
来源：http://ph.huanxung.cn

[T49] Perl：函数
来源：http://hn.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xo.hahajie.cn

[T50] Perl：逐行读文件
来源：http://fz.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wf.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://cu.colortex.cn

[T51] Scala：Hello World
来源：http://ci.colortex.cn

println("Hello")
来源：http://qm.nicolike.cn

[T52] Scala：变量
来源：http://xh.newstarts.cn

val a = 1;  var b = 2
来源：http://gw.colortex.cn

[T53] Scala：字符串插值
来源：http://ot.jianghongdianzi.cn

s"值: $b"
来源：http://gq.yuexingan06.cn

[T54] Scala：集合映射
来源：http://ls.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://oe.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://uk.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kf.bookmarksfly.cn

[T56] Scala：样例类
来源：http://rl.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://mc.asd995.cn

[T57] Scala：模式匹配
来源：http://jz.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cs.hahajie.cn

[T58] Scala：函数定义
来源：http://ci.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://la.shxzskj.cn

[T59] Scala：循环
来源：http://he.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://ze.jctech888.com.cn

[T60] Scala：折叠
来源：http://yb.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kv.newstarts.cn

================================================================================
来源：http://td.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jt.shtwfgs.cn

================================================================================
来源：http://cp.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://ns.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qh.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://cj.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vm.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://ex.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yx.shxzukj.cn

[U04] Py：变量调试打印
来源：http://ex.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ju.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://sy.asd995.cn

list(dict.fromkeys(arr))
来源：http://wh.hahajie.cn

[U06] Py：合并两个字典
来源：http://he.huanxung.cn

{**a, **b}
来源：http://ko.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://qf.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://sc.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://xa.521024.cn

[y for x in nested for y in x]
来源：http://dr.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://qb.nszjky.cn

max(d, key=d.get)
来源：http://lm.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://xu.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://io.nszjky.cn

[U11] Py：生成器表达式
来源：http://pi.jctech888.com.cn

(x * 2 for x in arr)
来源：http://ph.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gr.newstarts.cn

Counter(arr).most_common(3)
来源：http://sd.nicolike.cn

[U13] Py：固定长度队列
来源：http://gj.szxytkj.cn

deque(maxlen=10)
来源：http://ep.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://gp.521024.cn

defaultdict(list)
来源：http://tu.nszjky.cn

[U15] Py：高精度计时
来源：http://ko.asd995.cn

t = time.perf_counter()
来源：http://dj.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://yp.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wb.nszjky.cn

[U17] Py：初始化日志
来源：http://iv.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://yt.chemitech.net.cn

[U18] Py：预编译正则
来源：http://rw.colortex.cn

pat = re.compile(r"\d+")
来源：http://kr.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://az.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://al.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://uz.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://af.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://au.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://wu.colortex.cn

[U22] Py：矩阵转置
来源：http://xr.hahajie.cn

list(zip(*m))
来源：http://vy.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://lc.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vo.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://sv.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yh.shtwfgs.cn


<!-- 参考信息 -->