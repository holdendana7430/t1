代发 wailian999

int x; scanf("%d", &x);
来源：http://kk.nszjky.cn

[S04] C：字符串复制
来源：http://vd.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pv.szsharing.cn

[S05] C：字符串长度
来源：http://ix.huixiangedu.cn

strlen(s)
来源：http://rq.gzmigu.cn

[S06] C：字符串比较
来源：http://ss.shtwfgs.cn

strcmp(a, b) == 0
来源：http://he.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://rd.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bc.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://vy.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nq.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://pm.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dn.nicolike.cn

[S10] C：指针与解引用
来源：http://ok.9csxet.cn

int *p = &a;  *p = 5;
来源：http://ta.9csxet.cn

[S11] C：逐行读文件
来源：http://xp.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://as.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dq.huixiangedu.cn

fclose(f);
来源：http://cr.huanxung.cn

[S12] C：写文件
来源：http://wu.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pk.colortex.cn

[S13] C：宏定义
来源：http://rz.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fu.yuntaijiaju.cn

[S14] C：枚举
来源：http://px.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://wy.colortex.cn

[S15] C：类型转换
来源：http://gi.haigaiapp.cn

(double) a / b
来源：http://dt.asd995.cn

[S16] C：位操作置位
来源：http://ha.9csxet.cn

x |= (1 << 3);
来源：http://lu.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://tl.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tc.nszjky.cn

[S18] C：命令行参数
来源：http://vn.colortex.cn

int main(int argc, char **argv)
来源：http://tg.colortex.cn

[S19] C：快速排序
来源：http://wk.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eh.newstarts.cn

[S20] C：二分查找
来源：http://ds.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ku.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://qs.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ty.colortex.cn

[S22] C：字符串转数字
来源：http://hl.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://te.muxihuayi.cn

[S23] C：随机数
来源：http://su.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cg.szsharing.cn

[S24] C：获取本地时间
来源：http://mh.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fb.panjiajie.cn

[S25] C：内存拷贝
来源：http://xc.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://fi.newstarts.cn

[S26] C：内存清零
来源：http://ht.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://lo.yuexingan06.cn

[S27] C：定义常量
来源：http://fj.hahajie.cn

const double PI = 3.14159;
来源：http://ex.hnjuh.cn

[S28] C：静态变量
来源：http://ke.gzmigu.cn

static int counter = 0;
来源：http://by.newstarts.cn

[S29] C：变参函数
来源：http://yn.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bl.newstarts.cn

[S30] C：头文件保护
来源：http://du.jianghongdianzi.cn

#ifndef X_H
来源：http://mh.haigaiapp.cn

#define X_H
来源：http://ah.9csxet.cn

#endif
来源：http://gr.huanxung.cn

[S31] C++：Hello World
来源：http://nv.yuexingan06.cn

#include <iostream>
来源：http://wm.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://xn.huixiangedu.cn

[S32] C++：字符串
来源：http://nf.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://tm.9csxet.cn

[S33] C++：vector 增删
来源：http://jx.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eb.shxzskj.cn

[S34] C++：遍历 vector
来源：http://cy.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://in.jianghongdianzi.cn

[S35] C++：map
来源：http://ib.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cw.hahajie.cn

[S36] C++：unordered_map
来源：http://zl.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eo.panjiajie.cn

[S37] C++：set
来源：http://gi.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sn.muxihuayi.cn

[S38] C++：排序
来源：http://hr.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://nh.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://ig.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ll.bookmarksfly.cn

[S40] C++：查找元素
来源：http://yw.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pz.szsharing.cn

[S41] C++：类与构造函数
来源：http://bl.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xd.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://wo.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://cc.haigaiapp.cn

[S43] C++：智能指针
来源：http://lb.521024.cn

auto p = std::make_unique<int>(5);
来源：http://vm.bjjhwx.cn

[S44] C++：引用传参
来源：http://iw.asd995.cn

void inc(int &x) { ++x; }
来源：http://oz.huixinmuqiang.cn

[S45] C++：lambda
来源：http://kn.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://op.chemitech.net.cn

[S46] C++：函数模板
来源：http://tg.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zw.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://lw.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ex.lnxyls.cn

[S48] C++：逐行读文件
来源：http://wq.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hw.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://bg.hahajie.cn

[S49] C++：写文件
来源：http://za.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fz.bjjhwx.cn

[S50] C++：格式化数字
来源：http://sl.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eb.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://on.wgjwhj.cn

static_cast<double>(a) / b
来源：http://ap.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://vd.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://yl.521024.cn

[S53] C++：移动语义
来源：http://ea.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ir.jctech888.com.cn

[S54] C++：异常处理
来源：http://yn.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://he.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ta.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://no.bjjhwx.cn

[S56] C++：optional
来源：http://mc.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yb.newstarts.cn

[S57] C++：编译期常量
来源：http://lq.nicolike.cn

constexpr int N = 10;
来源：http://vn.hnjuh.cn

[S58] C++：命名空间
来源：http://cn.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://hx.nicolike.cn

[S59] C++：静态断言
来源：http://tu.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yd.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://dv.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bj.shtwfgs.cn

================================================================================
来源：http://pq.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ok.bjjhwx.cn

================================================================================
来源：http://cj.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://il.gzmigu.cn

println("Hello")
来源：http://nx.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://sf.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://we.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://ll.9csxet.cn

"值: $b"
来源：http://zg.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://ep.gzmigu.cn

val n: String? = null;  n?.length
来源：http://fy.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://no.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zt.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://js.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tc.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://ou.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nn.asd995.cn

[T08] Kotlin：数据类
来源：http://is.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://xt.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://ne.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://wo.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://ut.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wk.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ui.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://py.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://ab.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://tx.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://ne.colortex.cn

val m = mapOf("a" to 1)
来源：http://vj.9csxet.cn

[T14] Kotlin：循环
来源：http://cm.nicolike.cn

for (i in 1..10) println(i)
来源：http://nu.hahajie.cn

[T15] Kotlin：接口
来源：http://ki.szsharing.cn

interface Shape { fun area(): Double }
来源：http://sh.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://sv.hnjuh.cn

print("Hello")
来源：http://sh.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://dk.bjjhwx.cn

var a = 1;  let b = 2
来源：http://yh.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://xx.yuexingan06.cn

"值: \(b)"
来源：http://ze.panjiajie.cn

[T19] Swift：可选绑定
来源：http://ja.shtwfgs.cn

if let n = opt { print(n) }
来源：http://yb.haigaiapp.cn

[T20] Swift：数组操作
来源：http://tf.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://px.huanxung.cn

[T21] Swift：遍历
来源：http://xg.chemitech.net.cn

for x in a { print(x) }
来源：http://na.hnjuh.cn

[T22] Swift：字典
来源：http://yw.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ny.hahajie.cn

[T23] Swift：函数
来源：http://ij.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ak.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://uc.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wp.gzmigu.cn

[T25] Swift：结构体
来源：http://mu.jianghongdianzi.cn

struct P { var x: Int }
来源：http://bn.colortex.cn

[T26] Swift：类与重写
来源：http://fl.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://qh.jctech888.com.cn

[T27] Swift：错误处理
来源：http://ex.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://uz.colortex.cn

[T28] Swift：枚举
来源：http://wg.hahajie.cn

enum Color { case red, green }
来源：http://iu.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://ak.nszjky.cn

guard let x = opt else { return }
来源：http://gw.521024.cn

[T30] Swift：协议
来源：http://lm.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://bt.colortex.cn

[T31] Lua：Hello World
来源：http://hz.lnxyls.cn

print("Hello")
来源：http://ic.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://rs.lnxyls.cn

local a = 1
来源：http://lv.shxzukj.cn

[T33] Lua：表（数组）
来源：http://fy.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sg.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://ib.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wgjwhj.cn

[T35] Lua：字典表
来源：http://tq.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://cs.haigaiapp.cn

[T36] Lua：函数
来源：http://iu.nszjky.cn

function add(a, b) return a + b end
来源：http://en.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://ic.huixiangedu.cn

"a" .. "b"
来源：http://me.chemitech.net.cn

[T38] Lua：条件
来源：http://ct.521024.cn

if x > 0 then print("正") end
来源：http://dc.asd995.cn

[T39] Lua：模式匹配
来源：http://zc.lnxyls.cn

string.find(s, "%d+")
来源：http://kw.shtwfgs.cn

[T40] Lua：元表
来源：http://no.szsharing.cn

setmetatable({}, { __index = base })
来源：http://wj.colortex.cn

[T41] Perl：Hello World
来源：http://er.muxihuayi.cn

print "Hello\n";
来源：http://wu.wgjwhj.cn

[T42] Perl：变量类型
来源：http://vl.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xi.huanxung.cn

[T43] Perl：字符串插值
来源：http://rx.bjjhwx.cn

"值: $a"
来源：http://xn.huanxung.cn

[T44] Perl：条件
来源：http://vh.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://mw.newstarts.cn

[T45] Perl：数组遍历
来源：http://cx.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://me.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ww.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ar.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://pb.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dg.9csxet.cn

[T48] Perl：正则替换
来源：http://hv.shxzskj.cn

$s =~ s/old/new/g;
来源：http://ti.colortex.cn

[T49] Perl：函数
来源：http://wb.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bw.colortex.cn

[T50] Perl：逐行读文件
来源：http://kb.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://np.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://hb.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://al.szxytkj.cn

println("Hello")
来源：http://ns.shxzukj.cn

[T52] Scala：变量
来源：http://kt.panjiajie.cn

val a = 1;  var b = 2
来源：http://jz.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ja.shxzskj.cn

s"值: $b"
来源：http://qx.asd995.cn

[T54] Scala：集合映射
来源：http://yf.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ug.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://vp.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cq.haigaiapp.cn

[T56] Scala：样例类
来源：http://rw.szsharing.cn

case class User(name: String, age: Int)
来源：http://kg.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://js.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wk.muxihuayi.cn

[T58] Scala：函数定义
来源：http://ss.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rs.asd995.cn

[T59] Scala：循环
来源：http://mb.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://qv.muxihuayi.cn

[T60] Scala：折叠
来源：http://lv.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sc.yuntaijiaju.cn

================================================================================
来源：http://or.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mw.shxzukj.cn

================================================================================
来源：http://pr.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://cs.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ob.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://wn.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nl.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://oc.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cf.hahajie.cn

[U04] Py：变量调试打印
来源：http://ry.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tq.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://ul.521024.cn

list(dict.fromkeys(arr))
来源：http://sd.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://vv.chemitech.net.cn

{**a, **b}
来源：http://ik.colortex.cn

[U07] Py：反转字典键值
来源：http://gs.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://qt.panjiajie.cn

[U08] Py：展平二维列表
来源：http://wn.huanxung.cn

[y for x in nested for y in x]
来源：http://ec.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://fe.yuexingan06.cn

max(d, key=d.get)
来源：http://ko.newstarts.cn

[U10] Py：按值排序字典
来源：http://nb.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ii.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://ps.newstarts.cn

(x * 2 for x in arr)
来源：http://we.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lg.nszjky.cn

Counter(arr).most_common(3)
来源：http://zd.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://fh.shtwfgs.cn

deque(maxlen=10)
来源：http://wx.szsharing.cn

[U14] Py：分组收集到列表
来源：http://ti.panjiajie.cn

defaultdict(list)
来源：http://bh.szxytkj.cn

[U15] Py：高精度计时
来源：http://zb.shxzskj.cn

t = time.perf_counter()
来源：http://qe.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://cn.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qj.szxytkj.cn

[U17] Py：初始化日志
来源：http://fn.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ze.szsharing.cn

[U18] Py：预编译正则
来源：http://ni.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://bf.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://me.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ur.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://zg.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://mj.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://nl.huanxung.cn

@contextlib.contextmanager
来源：http://gg.panjiajie.cn

[U22] Py：矩阵转置
来源：http://oo.nicolike.cn

list(zip(*m))
来源：http://rr.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://zj.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xf.nszjky.cn

[U24] Py：路径操作
来源：http://uf.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cn.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://vh.gzmigu.cn

csv.DictReader(f)
来源：http://rz.huixiangedu.cn

[U26] Py：并发下载
来源：http://hv.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ph.hahajie.cn


<!-- 参考信息 -->