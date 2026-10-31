代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://os.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://wd.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://wf.9csxet.cn

[S03] C：读入整数
来源：http://mp.lnxyls.cn

int x; scanf("%d", &x);
来源：http://em.nicolike.cn

[S04] C：字符串复制
来源：http://oa.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ib.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://co.asd995.cn

strlen(s)
来源：http://fp.hnjuh.cn

[S06] C：字符串比较
来源：http://js.haigaiapp.cn

strcmp(a, b) == 0
来源：http://be.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://fg.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://df.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://fm.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rc.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://xw.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zw.muxihuayi.cn

[S10] C：指针与解引用
来源：http://mg.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://ah.szxytkj.cn

[S11] C：逐行读文件
来源：http://ol.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://vl.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ji.lnxyls.cn

fclose(f);
来源：http://wp.bookmarksfly.cn

[S12] C：写文件
来源：http://xb.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bp.newstarts.cn

[S13] C：宏定义
来源：http://dj.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sh.chemitech.net.cn

[S14] C：枚举
来源：http://wj.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://wu.bjjhwx.cn

[S15] C：类型转换
来源：http://yq.muxihuayi.cn

(double) a / b
来源：http://fl.muxihuayi.cn

[S16] C：位操作置位
来源：http://sh.9csxet.cn

x |= (1 << 3);
来源：http://ku.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://pd.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ap.newstarts.cn

[S18] C：命令行参数
来源：http://af.shtwfgs.cn

int main(int argc, char **argv)
来源：http://cs.szxytkj.cn

[S19] C：快速排序
来源：http://mv.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qx.hnjuh.cn

[S20] C：二分查找
来源：http://gf.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cu.huanxung.cn

[S21] C：字符类别判断
来源：http://pl.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gn.wgjwhj.cn

[S22] C：字符串转数字
来源：http://vq.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oa.panjiajie.cn

[S23] C：随机数
来源：http://ma.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tm.gzmigu.cn

[S24] C：获取本地时间
来源：http://ho.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jj.huixiangedu.cn

[S25] C：内存拷贝
来源：http://xm.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://xi.bookmarksfly.cn

[S26] C：内存清零
来源：http://wh.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://xr.szsharing.cn

[S27] C：定义常量
来源：http://nc.colortex.cn

const double PI = 3.14159;
来源：http://qz.shtwfgs.cn

[S28] C：静态变量
来源：http://jp.huanxung.cn

static int counter = 0;
来源：http://tp.wgjwhj.cn

[S29] C：变参函数
来源：http://xm.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ny.panjiajie.cn

[S30] C：头文件保护
来源：http://bn.panjiajie.cn

#ifndef X_H
来源：http://ad.bookmarksfly.cn

#define X_H
来源：http://im.newstarts.cn

#endif
来源：http://de.haigaiapp.cn

[S31] C++：Hello World
来源：http://qq.yuexingan06.cn

#include <iostream>
来源：http://kh.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://lw.muxihuayi.cn

[S32] C++：字符串
来源：http://fp.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://fl.colortex.cn

[S33] C++：vector 增删
来源：http://zk.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qr.nicolike.cn

[S34] C++：遍历 vector
来源：http://vt.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://zn.lnxyls.cn

[S35] C++：map
来源：http://cy.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wy.huanxung.cn

[S36] C++：unordered_map
来源：http://wr.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pu.shtwfgs.cn

[S37] C++：set
来源：http://yo.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ma.lnxyls.cn

[S38] C++：排序
来源：http://oz.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://yy.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://zh.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mm.jctech888.com.cn

[S40] C++：查找元素
来源：http://pp.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qm.szsharing.cn

[S41] C++：类与构造函数
来源：http://jr.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xy.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://ha.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://mu.nszjky.cn

[S43] C++：智能指针
来源：http://gw.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ww.huixiangedu.cn

[S44] C++：引用传参
来源：http://ps.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://lp.hnjuh.cn

[S45] C++：lambda
来源：http://bc.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vf.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ux.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sz.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://to.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rr.szsharing.cn

[S48] C++：逐行读文件
来源：http://ao.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wk.newstarts.cn

while (std::getline(in, line)) { }
来源：http://lq.yuexingan06.cn

[S49] C++：写文件
来源：http://qs.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jx.nicolike.cn

[S50] C++：格式化数字
来源：http://yc.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ml.huanxung.cn

[S51] C++：显式类型转换
来源：http://as.asd995.cn

static_cast<double>(a) / b
来源：http://xw.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://rl.szsharing.cn

int size() const noexcept { return n_; }
来源：http://yf.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://hl.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://hp.chemitech.net.cn

[S54] C++：异常处理
来源：http://hf.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eg.colortex.cn

[S55] C++：结构化绑定
来源：http://lw.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ye.yuntaijiaju.cn

[S56] C++：optional
来源：http://ky.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cr.huanxung.cn

[S57] C++：编译期常量
来源：http://kn.hnjuh.cn

constexpr int N = 10;
来源：http://my.muxihuayi.cn

[S58] C++：命名空间
来源：http://do.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://kb.huanxung.cn

[S59] C++：静态断言
来源：http://ws.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bh.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://xv.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tz.hnjuh.cn

================================================================================
来源：http://mj.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fb.wgjwhj.cn

================================================================================
来源：http://xt.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ko.nicolike.cn

println("Hello")
来源：http://te.gzmigu.cn

[T02] Kotlin：变量
来源：http://ol.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sj.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://ap.chemitech.net.cn

"值: $b"
来源：http://du.colortex.cn

[T04] Kotlin：空安全
来源：http://wy.shxzskj.cn

val n: String? = null;  n?.length
来源：http://vc.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://zu.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vs.nszjky.cn

[T06] Kotlin：集合映射
来源：http://uf.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sc.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://xg.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bl.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://vw.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://kf.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://ok.colortex.cn

fun String.exclaim() = this + "!"
来源：http://nh.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://pd.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xx.chemitech.net.cn

[T11] Kotlin：协程
来源：http://hl.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yv.colortex.cn

[T12] Kotlin：解构声明
来源：http://ng.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://qg.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://df.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://fk.szsharing.cn

[T14] Kotlin：循环
来源：http://sd.gzmigu.cn

for (i in 1..10) println(i)
来源：http://vt.jctech888.com.cn

[T15] Kotlin：接口
来源：http://dt.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ex.nicolike.cn

[T16] Swift：Hello World
来源：http://ya.gzmigu.cn

print("Hello")
来源：http://rg.hahajie.cn

[T17] Swift：变量与常量
来源：http://pl.asd995.cn

var a = 1;  let b = 2
来源：http://lb.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://qx.yuexingan06.cn

"值: \(b)"
来源：http://nq.gzmigu.cn

[T19] Swift：可选绑定
来源：http://ps.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ph.newstarts.cn

[T20] Swift：数组操作
来源：http://ga.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://me.chemitech.net.cn

[T21] Swift：遍历
来源：http://cv.lnxyls.cn

for x in a { print(x) }
来源：http://vn.hahajie.cn

[T22] Swift：字典
来源：http://gj.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vx.jianghongdianzi.cn

[T23] Swift：函数
来源：http://fz.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ua.szxytkj.cn

[T24] Swift：闭包
来源：http://tq.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://em.wgjwhj.cn

[T25] Swift：结构体
来源：http://gs.haigaiapp.cn

struct P { var x: Int }
来源：http://sb.9csxet.cn

[T26] Swift：类与重写
来源：http://rq.hnjuh.cn

class A: Base { override func f() {} }
来源：http://jn.huixiangedu.cn

[T27] Swift：错误处理
来源：http://xz.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://mx.shxzskj.cn

[T28] Swift：枚举
来源：http://nj.szxytkj.cn

enum Color { case red, green }
来源：http://kz.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://wz.asd995.cn

guard let x = opt else { return }
来源：http://zq.huixiangedu.cn

[T30] Swift：协议
来源：http://sy.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://fq.yuexingan06.cn

[T31] Lua：Hello World
来源：http://lj.hnjuh.cn

print("Hello")
来源：http://qc.521024.cn

[T32] Lua：局部变量
来源：http://yy.shxzskj.cn

local a = 1
来源：http://pu.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://kj.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://le.yuexingan06.cn

[T34] Lua：遍历表
来源：http://qc.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pq.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://lc.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://ji.colortex.cn

[T36] Lua：函数
来源：http://bm.szxytkj.cn

function add(a, b) return a + b end
来源：http://ze.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://xb.jianghongdianzi.cn

"a" .. "b"
来源：http://un.asd995.cn

[T38] Lua：条件
来源：http://su.jctech888.com.cn

if x > 0 then print("正") end
来源：http://iz.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://mj.asd995.cn

string.find(s, "%d+")
来源：http://ay.521024.cn

[T40] Lua：元表
来源：http://hu.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://bi.nszjky.cn

[T41] Perl：Hello World
来源：http://fu.chemitech.net.cn

print "Hello\n";
来源：http://rh.asd995.cn

[T42] Perl：变量类型
来源：http://xh.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rf.gzmigu.cn

[T43] Perl：字符串插值
来源：http://rv.bjjhwx.cn

"值: $a"
来源：http://ao.muxihuayi.cn

[T44] Perl：条件
来源：http://qc.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ks.hnjuh.cn

[T45] Perl：数组遍历
来源：http://ry.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://hc.newstarts.cn

[T46] Perl：哈希操作
来源：http://hw.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rn.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://du.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kr.panjiajie.cn

[T48] Perl：正则替换
来源：http://jk.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://hg.hnjuh.cn

[T49] Perl：函数
来源：http://ja.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wa.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://mz.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ru.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://qp.chemitech.net.cn

[T51] Scala：Hello World
来源：http://mo.bookmarksfly.cn

println("Hello")
来源：http://dq.gzmigu.cn

[T52] Scala：变量
来源：http://da.newstarts.cn

val a = 1;  var b = 2
来源：http://xp.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://oq.huixinmuqiang.cn

s"值: $b"
来源：http://zc.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://kz.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://yw.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://wk.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xm.chemitech.net.cn

[T56] Scala：样例类
来源：http://xb.asd995.cn

case class User(name: String, age: Int)
来源：http://hz.lnxyls.cn

[T57] Scala：模式匹配
来源：http://ok.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://si.gzmigu.cn

[T58] Scala：函数定义
来源：http://uc.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wb.wgjwhj.cn

[T59] Scala：循环
来源：http://gp.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://nv.wgjwhj.cn

[T60] Scala：折叠
来源：http://vd.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pv.jctech888.com.cn

================================================================================
来源：http://gc.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pu.asd995.cn

================================================================================
来源：http://st.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://zw.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qp.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ii.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hk.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://jv.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ix.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://sn.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mt.nszjky.cn

[U05] Py：列表去重且保序
来源：http://tx.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://nj.lnxyls.cn

[U06] Py：合并两个字典
来源：http://pa.newstarts.cn

{**a, **b}
来源：http://gw.hahajie.cn

[U07] Py：反转字典键值
来源：http://vo.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://qw.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://fw.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://rc.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://fh.huanxung.cn

max(d, key=d.get)
来源：http://pe.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://cj.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fx.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://la.panjiajie.cn

(x * 2 for x in arr)
来源：http://wp.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hj.colortex.cn

Counter(arr).most_common(3)
来源：http://vy.panjiajie.cn

[U13] Py：固定长度队列
来源：http://xa.shtwfgs.cn

deque(maxlen=10)
来源：http://vc.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://hd.huixinmuqiang.cn

defaultdict(list)
来源：http://ej.szxytkj.cn

[U15] Py：高精度计时
来源：http://wz.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ll.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://rv.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hg.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://op.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://bd.shxzukj.cn

[U18] Py：预编译正则
来源：http://hr.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://fj.521024.cn

[U19] Py：正则替换带回调
来源：http://fe.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zn.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://jk.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://qn.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://ah.shxzukj.cn

@contextlib.contextmanager
来源：http://hs.szxytkj.cn

[U22] Py：矩阵转置
来源：http://ot.szxytkj.cn

list(zip(*m))
来源：http://jl.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://jo.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lm.muxihuayi.cn

[U24] Py：路径操作
来源：http://if.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ew.nszjky.cn


<!-- 参考信息 -->