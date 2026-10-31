代发 wailian999

int x; scanf("%d", &x);
来源：http://sf.jctech888.com.cn

[S04] C：字符串复制
来源：http://ub.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tx.bookmarksfly.cn

[S05] C：字符串长度
来源：http://io.shxzukj.cn

strlen(s)
来源：http://vb.shxzukj.cn

[S06] C：字符串比较
来源：http://ym.asd995.cn

strcmp(a, b) == 0
来源：http://jc.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://tx.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bh.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://xt.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tq.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://kr.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://je.chemitech.net.cn

[S10] C：指针与解引用
来源：http://qx.huanxung.cn

int *p = &a;  *p = 5;
来源：http://qv.wgjwhj.cn

[S11] C：逐行读文件
来源：http://db.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://nl.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sr.jianghongdianzi.cn

fclose(f);
来源：http://ka.jianghongdianzi.cn

[S12] C：写文件
来源：http://lt.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lr.newstarts.cn

[S13] C：宏定义
来源：http://ji.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gv.nszjky.cn

[S14] C：枚举
来源：http://yj.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://ju.yuntaijiaju.cn

[S15] C：类型转换
来源：http://im.shtwfgs.cn

(double) a / b
来源：http://vt.haigaiapp.cn

[S16] C：位操作置位
来源：http://qi.wgjwhj.cn

x |= (1 << 3);
来源：http://fs.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://mq.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ra.nicolike.cn

[S18] C：命令行参数
来源：http://pn.bjjhwx.cn

int main(int argc, char **argv)
来源：http://hi.jctech888.com.cn

[S19] C：快速排序
来源：http://am.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xu.bookmarksfly.cn

[S20] C：二分查找
来源：http://wg.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uy.newstarts.cn

[S21] C：字符类别判断
来源：http://je.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ef.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://az.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ol.wgjwhj.cn

[S23] C：随机数
来源：http://xo.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kw.huixiangedu.cn

[S24] C：获取本地时间
来源：http://fr.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ke.bjjhwx.cn

[S25] C：内存拷贝
来源：http://yy.9csxet.cn

memcpy(dst, src, n);
来源：http://gi.yuexingan06.cn

[S26] C：内存清零
来源：http://hu.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://zy.hnjuh.cn

[S27] C：定义常量
来源：http://cj.huixiangedu.cn

const double PI = 3.14159;
来源：http://gx.muxihuayi.cn

[S28] C：静态变量
来源：http://eo.huixinmuqiang.cn

static int counter = 0;
来源：http://ae.chemitech.net.cn

[S29] C：变参函数
来源：http://gd.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://us.szxytkj.cn

[S30] C：头文件保护
来源：http://pg.jctech888.com.cn

#ifndef X_H
来源：http://uk.shtwfgs.cn

#define X_H
来源：http://un.jctech888.com.cn

#endif
来源：http://ma.9csxet.cn

[S31] C++：Hello World
来源：http://uw.chemitech.net.cn

#include <iostream>
来源：http://gf.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://us.huanxung.cn

[S32] C++：字符串
来源：http://uh.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://ia.nicolike.cn

[S33] C++：vector 增删
来源：http://fp.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rg.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://si.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://wy.asd995.cn

[S35] C++：map
来源：http://on.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lj.huixiangedu.cn

[S36] C++：unordered_map
来源：http://wo.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ot.huanxung.cn

[S37] C++：set
来源：http://ne.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wt.newstarts.cn

[S38] C++：排序
来源：http://ak.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://sl.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://mj.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://em.newstarts.cn

[S40] C++：查找元素
来源：http://zt.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qs.shxzukj.cn

[S41] C++：类与构造函数
来源：http://jb.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tq.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://wl.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://jp.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://vc.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://ka.wgjwhj.cn

[S44] C++：引用传参
来源：http://mq.hahajie.cn

void inc(int &x) { ++x; }
来源：http://rq.shxzukj.cn

[S45] C++：lambda
来源：http://nd.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ny.asd995.cn

[S46] C++：函数模板
来源：http://dk.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lc.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://lz.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fs.szsharing.cn

[S48] C++：逐行读文件
来源：http://fu.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://re.9csxet.cn

while (std::getline(in, line)) { }
来源：http://zg.huixiangedu.cn

[S49] C++：写文件
来源：http://va.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wg.hahajie.cn

[S50] C++：格式化数字
来源：http://oj.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qg.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://iz.muxihuayi.cn

static_cast<double>(a) / b
来源：http://dq.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://wu.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://qx.szsharing.cn

[S53] C++：移动语义
来源：http://eh.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://tw.colortex.cn

[S54] C++：异常处理
来源：http://qq.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zu.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://kl.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://si.bookmarksfly.cn

[S56] C++：optional
来源：http://ut.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yt.panjiajie.cn

[S57] C++：编译期常量
来源：http://zc.shxzskj.cn

constexpr int N = 10;
来源：http://nx.shxzskj.cn

[S58] C++：命名空间
来源：http://ej.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://gj.muxihuayi.cn

[S59] C++：静态断言
来源：http://yb.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mc.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://ig.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wz.huanxung.cn

================================================================================
来源：http://yc.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jk.colortex.cn

================================================================================
来源：http://to.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://qf.newstarts.cn

println("Hello")
来源：http://gs.szxytkj.cn

[T02] Kotlin：变量
来源：http://sf.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jm.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://iu.szsharing.cn

"值: $b"
来源：http://mu.panjiajie.cn

[T04] Kotlin：空安全
来源：http://ow.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://kf.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://hb.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vu.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://fo.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dv.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://hu.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lh.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://ue.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://rp.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://fh.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://av.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://nm.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://au.haigaiapp.cn

[T11] Kotlin：协程
来源：http://wr.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tf.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://wx.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://wv.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://jq.521024.cn

val m = mapOf("a" to 1)
来源：http://xo.haigaiapp.cn

[T14] Kotlin：循环
来源：http://gv.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://fl.huanxung.cn

[T15] Kotlin：接口
来源：http://dg.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://ct.muxihuayi.cn

[T16] Swift：Hello World
来源：http://xe.huixiangedu.cn

print("Hello")
来源：http://la.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://pk.shtwfgs.cn

var a = 1;  let b = 2
来源：http://mo.szxytkj.cn

[T18] Swift：字符串插值
来源：http://wv.521024.cn

"值: \(b)"
来源：http://ro.nszjky.cn

[T19] Swift：可选绑定
来源：http://ar.shxzskj.cn

if let n = opt { print(n) }
来源：http://dp.yuexingan06.cn

[T20] Swift：数组操作
来源：http://kp.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kp.colortex.cn

[T21] Swift：遍历
来源：http://wd.wgjwhj.cn

for x in a { print(x) }
来源：http://fs.nszjky.cn

[T22] Swift：字典
来源：http://lm.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gb.nszjky.cn

[T23] Swift：函数
来源：http://gf.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ff.lnxyls.cn

[T24] Swift：闭包
来源：http://yb.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ds.yuexingan06.cn

[T25] Swift：结构体
来源：http://nx.panjiajie.cn

struct P { var x: Int }
来源：http://jy.nszjky.cn

[T26] Swift：类与重写
来源：http://kz.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://zx.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://sp.nicolike.cn

do { try f() } catch { print(error) }
来源：http://qh.9csxet.cn

[T28] Swift：枚举
来源：http://ez.szsharing.cn

enum Color { case red, green }
来源：http://ep.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://px.hahajie.cn

guard let x = opt else { return }
来源：http://pa.nicolike.cn

[T30] Swift：协议
来源：http://nv.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://mf.nszjky.cn

[T31] Lua：Hello World
来源：http://um.nszjky.cn

print("Hello")
来源：http://nh.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://te.huixiangedu.cn

local a = 1
来源：http://kw.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://ah.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nj.nszjky.cn

[T34] Lua：遍历表
来源：http://gy.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fg.521024.cn

[T35] Lua：字典表
来源：http://gb.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://zk.bookmarksfly.cn

[T36] Lua：函数
来源：http://dm.szxytkj.cn

function add(a, b) return a + b end
来源：http://vb.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://jh.jctech888.com.cn

"a" .. "b"
来源：http://mm.bookmarksfly.cn

[T38] Lua：条件
来源：http://mh.9csxet.cn

if x > 0 then print("正") end
来源：http://tg.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://ey.yuexingan06.cn

string.find(s, "%d+")
来源：http://dq.hahajie.cn

[T40] Lua：元表
来源：http://fh.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://ax.wgjwhj.cn

[T41] Perl：Hello World
来源：http://sx.521024.cn

print "Hello\n";
来源：http://vz.lnxyls.cn

[T42] Perl：变量类型
来源：http://pf.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wu.nszjky.cn

[T43] Perl：字符串插值
来源：http://kx.lnxyls.cn

"值: $a"
来源：http://ug.shxzskj.cn

[T44] Perl：条件
来源：http://mu.521024.cn

if ($a > 0) { print "正"; }
来源：http://ov.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://sl.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ik.nszjky.cn

[T46] Perl：哈希操作
来源：http://gk.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yn.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://sp.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xj.jctech888.com.cn

[T48] Perl：正则替换
来源：http://qy.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://jy.jctech888.com.cn

[T49] Perl：函数
来源：http://zr.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ib.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://eb.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://da.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://vq.9csxet.cn

[T51] Scala：Hello World
来源：http://rq.521024.cn

println("Hello")
来源：http://vg.haigaiapp.cn

[T52] Scala：变量
来源：http://dp.huanxung.cn

val a = 1;  var b = 2
来源：http://jv.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://tr.newstarts.cn

s"值: $b"
来源：http://nh.chemitech.net.cn

[T54] Scala：集合映射
来源：http://qy.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://mb.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://bi.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kj.wgjwhj.cn

[T56] Scala：样例类
来源：http://te.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://vg.panjiajie.cn

[T57] Scala：模式匹配
来源：http://qv.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gn.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://zb.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zn.gzmigu.cn

[T59] Scala：循环
来源：http://ho.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://jc.szxytkj.cn

[T60] Scala：折叠
来源：http://cw.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dx.muxihuayi.cn

================================================================================
来源：http://nb.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zx.muxihuayi.cn

================================================================================
来源：http://pf.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://ut.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://df.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://nq.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ma.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://pm.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yq.nszjky.cn

[U04] Py：变量调试打印
来源：http://gx.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yk.szsharing.cn

[U05] Py：列表去重且保序
来源：http://fq.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://cj.hahajie.cn

[U06] Py：合并两个字典
来源：http://uh.wgjwhj.cn

{**a, **b}
来源：http://nl.gzmigu.cn

[U07] Py：反转字典键值
来源：http://yu.asd995.cn

{v: k for k, v in d.items()}
来源：http://of.gzmigu.cn

[U08] Py：展平二维列表
来源：http://bj.nicolike.cn

[y for x in nested for y in x]
来源：http://ir.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://yh.wgjwhj.cn

max(d, key=d.get)
来源：http://cx.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://xa.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xq.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://sy.colortex.cn

(x * 2 for x in arr)
来源：http://wa.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fj.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://vt.9csxet.cn

[U13] Py：固定长度队列
来源：http://mm.huanxung.cn

deque(maxlen=10)
来源：http://bi.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://me.yuntaijiaju.cn

defaultdict(list)
来源：http://iv.muxihuayi.cn

[U15] Py：高精度计时
来源：http://vi.yuntaijiaju.cn

t = time.perf_counter()
来源：http://yp.521024.cn

[U16] Py：命令行参数解析
来源：http://zx.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cv.asd995.cn

[U17] Py：初始化日志
来源：http://gw.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ld.asd995.cn

[U18] Py：预编译正则
来源：http://nl.hahajie.cn

pat = re.compile(r"\d+")
来源：http://qh.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ec.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cq.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://ux.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://dx.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://ki.wgjwhj.cn

@contextlib.contextmanager
来源：http://ri.colortex.cn

[U22] Py：矩阵转置
来源：http://aa.shtwfgs.cn

list(zip(*m))
来源：http://nn.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://di.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ys.shxzskj.cn

[U24] Py：路径操作
来源：http://yy.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gd.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://ob.shtwfgs.cn

csv.DictReader(f)
来源：http://au.huanxung.cn

[U26] Py：并发下载
来源：http://qe.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kt.hnjuh.cn


<!-- 参考信息 -->