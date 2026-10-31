代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://yx.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://yu.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ft.huixiangedu.cn

[S03] C：读入整数
来源：http://iu.shxzukj.cn

int x; scanf("%d", &x);
来源：http://ag.nicolike.cn

[S04] C：字符串复制
来源：http://hz.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://on.muxihuayi.cn

[S05] C：字符串长度
来源：http://ge.huanxung.cn

strlen(s)
来源：http://kl.chemitech.net.cn

[S06] C：字符串比较
来源：http://cf.shtwfgs.cn

strcmp(a, b) == 0
来源：http://jb.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://zj.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vp.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://vz.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ib.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://af.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lw.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://ml.hahajie.cn

int *p = &a;  *p = 5;
来源：http://db.huanxung.cn

[S11] C：逐行读文件
来源：http://gs.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://nq.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://et.9csxet.cn

fclose(f);
来源：http://ok.shxzskj.cn

[S12] C：写文件
来源：http://ex.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oi.hnjuh.cn

[S13] C：宏定义
来源：http://mp.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kk.521024.cn

[S14] C：枚举
来源：http://xz.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://mc.wgjwhj.cn

[S15] C：类型转换
来源：http://qz.szsharing.cn

(double) a / b
来源：http://yq.wgjwhj.cn

[S16] C：位操作置位
来源：http://bz.nszjky.cn

x |= (1 << 3);
来源：http://ax.521024.cn

[S17] C：安全拼接字符串
来源：http://cr.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rt.gzmigu.cn

[S18] C：命令行参数
来源：http://tc.szsharing.cn

int main(int argc, char **argv)
来源：http://pi.szxytkj.cn

[S19] C：快速排序
来源：http://ew.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gi.521024.cn

[S20] C：二分查找
来源：http://li.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ct.hnjuh.cn

[S21] C：字符类别判断
来源：http://qe.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sp.muxihuayi.cn

[S22] C：字符串转数字
来源：http://qt.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yk.chemitech.net.cn

[S23] C：随机数
来源：http://wb.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tg.huanxung.cn

[S24] C：获取本地时间
来源：http://wv.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pn.haigaiapp.cn

[S25] C：内存拷贝
来源：http://hi.shxzskj.cn

memcpy(dst, src, n);
来源：http://xo.colortex.cn

[S26] C：内存清零
来源：http://le.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://hz.yuexingan06.cn

[S27] C：定义常量
来源：http://pz.colortex.cn

const double PI = 3.14159;
来源：http://jn.shxzukj.cn

[S28] C：静态变量
来源：http://vz.haigaiapp.cn

static int counter = 0;
来源：http://dn.lnxyls.cn

[S29] C：变参函数
来源：http://ol.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ei.nszjky.cn

[S30] C：头文件保护
来源：http://rr.huanxung.cn

#ifndef X_H
来源：http://lq.hahajie.cn

#define X_H
来源：http://td.hnjuh.cn

#endif
来源：http://vr.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://ch.colortex.cn

#include <iostream>
来源：http://bn.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://pn.nszjky.cn

[S32] C++：字符串
来源：http://zw.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://ae.szsharing.cn

[S33] C++：vector 增删
来源：http://fr.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mn.szsharing.cn

[S34] C++：遍历 vector
来源：http://tu.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://gf.lnxyls.cn

[S35] C++：map
来源：http://df.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ik.huixiangedu.cn

[S36] C++：unordered_map
来源：http://ys.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kv.huixinmuqiang.cn

[S37] C++：set
来源：http://ys.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qz.haigaiapp.cn

[S38] C++：排序
来源：http://is.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://am.colortex.cn

[S39] C++：自定义比较器排序
来源：http://xn.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zf.hahajie.cn

[S40] C++：查找元素
来源：http://fv.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://an.hnjuh.cn

[S41] C++：类与构造函数
来源：http://yt.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mu.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://lk.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://jd.shtwfgs.cn

[S43] C++：智能指针
来源：http://eq.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://io.asd995.cn

[S44] C++：引用传参
来源：http://os.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ka.huanxung.cn

[S45] C++：lambda
来源：http://qq.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mg.gzmigu.cn

[S46] C++：函数模板
来源：http://rg.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cw.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://sn.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bs.shxzukj.cn

[S48] C++：逐行读文件
来源：http://ba.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://um.nszjky.cn

while (std::getline(in, line)) { }
来源：http://al.colortex.cn

[S49] C++：写文件
来源：http://qz.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dp.hnjuh.cn

[S50] C++：格式化数字
来源：http://lc.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kk.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://vr.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://qc.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://bt.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://xs.bookmarksfly.cn

[S53] C++：移动语义
来源：http://cx.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://cf.shtwfgs.cn

[S54] C++：异常处理
来源：http://tw.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ml.panjiajie.cn

[S55] C++：结构化绑定
来源：http://mx.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fs.huanxung.cn

[S56] C++：optional
来源：http://jt.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ug.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://pm.shtwfgs.cn

constexpr int N = 10;
来源：http://me.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://hn.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://yv.panjiajie.cn

[S59] C++：静态断言
来源：http://fo.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://st.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://lq.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zy.panjiajie.cn

================================================================================
来源：http://ev.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://po.panjiajie.cn

================================================================================
来源：http://ab.newstarts.cn

[T01] Kotlin：Hello World
来源：http://dt.szxytkj.cn

println("Hello")
来源：http://pf.gzmigu.cn

[T02] Kotlin：变量
来源：http://wg.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kf.521024.cn

[T03] Kotlin：字符串模板
来源：http://tk.newstarts.cn

"值: $b"
来源：http://wx.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://eu.szxytkj.cn

val n: String? = null;  n?.length
来源：http://kw.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://dg.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jl.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://uh.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hb.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://mk.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pq.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://mw.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://sg.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://ju.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://sj.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://rt.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jz.panjiajie.cn

[T11] Kotlin：协程
来源：http://wz.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rf.colortex.cn

[T12] Kotlin：解构声明
来源：http://gf.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://ry.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://nt.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://tk.asd995.cn

[T14] Kotlin：循环
来源：http://kc.szxytkj.cn

for (i in 1..10) println(i)
来源：http://fw.hnjuh.cn

[T15] Kotlin：接口
来源：http://ql.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://lj.521024.cn

[T16] Swift：Hello World
来源：http://qv.haigaiapp.cn

print("Hello")
来源：http://ot.szsharing.cn

[T17] Swift：变量与常量
来源：http://du.shxzukj.cn

var a = 1;  let b = 2
来源：http://bz.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ow.shxzskj.cn

"值: \(b)"
来源：http://ie.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://yy.huanxung.cn

if let n = opt { print(n) }
来源：http://le.hnjuh.cn

[T20] Swift：数组操作
来源：http://kv.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gs.chemitech.net.cn

[T21] Swift：遍历
来源：http://wc.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ge.szsharing.cn

[T22] Swift：字典
来源：http://ao.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ic.haigaiapp.cn

[T23] Swift：函数
来源：http://hg.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://la.nicolike.cn

[T24] Swift：闭包
来源：http://et.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://or.asd995.cn

[T25] Swift：结构体
来源：http://hd.bookmarksfly.cn

struct P { var x: Int }
来源：http://oa.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://sy.newstarts.cn

class A: Base { override func f() {} }
来源：http://xc.newstarts.cn

[T27] Swift：错误处理
来源：http://hw.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://lg.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://xw.gzmigu.cn

enum Color { case red, green }
来源：http://qj.colortex.cn

[T29] Swift：guard 提前返回
来源：http://is.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://nw.shtwfgs.cn

[T30] Swift：协议
来源：http://wn.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://bz.gzmigu.cn

[T31] Lua：Hello World
来源：http://ii.colortex.cn

print("Hello")
来源：http://du.yuexingan06.cn

[T32] Lua：局部变量
来源：http://gw.huixiangedu.cn

local a = 1
来源：http://sp.szsharing.cn

[T33] Lua：表（数组）
来源：http://gh.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hu.huixiangedu.cn

[T34] Lua：遍历表
来源：http://sr.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dv.shxzukj.cn

[T35] Lua：字典表
来源：http://rf.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://mf.chemitech.net.cn

[T36] Lua：函数
来源：http://hh.asd995.cn

function add(a, b) return a + b end
来源：http://av.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://sp.521024.cn

"a" .. "b"
来源：http://md.yuexingan06.cn

[T38] Lua：条件
来源：http://ld.wgjwhj.cn

if x > 0 then print("正") end
来源：http://ae.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://sn.huanxung.cn

string.find(s, "%d+")
来源：http://fo.jctech888.com.cn

[T40] Lua：元表
来源：http://ue.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://fa.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://fv.panjiajie.cn

print "Hello\n";
来源：http://cz.nszjky.cn

[T42] Perl：变量类型
来源：http://kh.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uz.nicolike.cn

[T43] Perl：字符串插值
来源：http://ij.panjiajie.cn

"值: $a"
来源：http://oz.huixinmuqiang.cn

[T44] Perl：条件
来源：http://sa.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://ug.gzmigu.cn

[T45] Perl：数组遍历
来源：http://te.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://xg.shxzskj.cn

[T46] Perl：哈希操作
来源：http://fk.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cc.newstarts.cn

[T47] Perl：正则捕获
来源：http://rx.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ki.yuexingan06.cn

[T48] Perl：正则替换
来源：http://hy.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://zk.shtwfgs.cn

[T49] Perl：函数
来源：http://ar.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wu.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://bi.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ti.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ac.hahajie.cn

[T51] Scala：Hello World
来源：http://vb.lnxyls.cn

println("Hello")
来源：http://uw.szsharing.cn

[T52] Scala：变量
来源：http://vy.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://de.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://tu.yuntaijiaju.cn

s"值: $b"
来源：http://ed.9csxet.cn

[T54] Scala：集合映射
来源：http://fm.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://cr.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://lx.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://da.nszjky.cn

[T56] Scala：样例类
来源：http://pe.gzmigu.cn

case class User(name: String, age: Int)
来源：http://xp.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://rb.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bj.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://af.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ky.bookmarksfly.cn

[T59] Scala：循环
来源：http://jq.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://ul.huanxung.cn

[T60] Scala：折叠
来源：http://ia.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lp.wgjwhj.cn

================================================================================
来源：http://xh.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uy.bjjhwx.cn

================================================================================
来源：http://nm.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://zs.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tc.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://mq.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wl.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://xg.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ig.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://zy.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hi.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://bm.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://ix.gzmigu.cn

[U06] Py：合并两个字典
来源：http://tl.szxytkj.cn

{**a, **b}
来源：http://lz.hahajie.cn

[U07] Py：反转字典键值
来源：http://kx.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://li.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://gy.panjiajie.cn

[y for x in nested for y in x]
来源：http://to.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://ew.szsharing.cn

max(d, key=d.get)
来源：http://mb.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://rp.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gn.colortex.cn

[U11] Py：生成器表达式
来源：http://ps.521024.cn

(x * 2 for x in arr)
来源：http://at.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rs.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://vc.panjiajie.cn

[U13] Py：固定长度队列
来源：http://gg.hnjuh.cn

deque(maxlen=10)
来源：http://am.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://ma.szsharing.cn

defaultdict(list)
来源：http://ip.shtwfgs.cn

[U15] Py：高精度计时
来源：http://gj.wgjwhj.cn

t = time.perf_counter()
来源：http://ej.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://wz.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kx.nicolike.cn

[U17] Py：初始化日志
来源：http://hx.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://vc.szxytkj.cn

[U18] Py：预编译正则
来源：http://de.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://qi.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://pl.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ou.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://sr.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://hh.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://gc.huixiangedu.cn

@contextlib.contextmanager
来源：http://ji.521024.cn

[U22] Py：矩阵转置
来源：http://ca.jctech888.com.cn

list(zip(*m))
来源：http://ka.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://es.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vi.chemitech.net.cn

[U24] Py：路径操作
来源：http://si.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vy.newstarts.cn


<!-- 参考信息 -->