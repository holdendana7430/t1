代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bo.panjiajie.cn

[S10] C：指针与解引用
来源：http://zv.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://zc.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://of.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://zy.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gt.szxytkj.cn

fclose(f);
来源：http://pc.shxzukj.cn

[S12] C：写文件
来源：http://fu.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ha.yuntaijiaju.cn

[S13] C：宏定义
来源：http://qb.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fl.521024.cn

[S14] C：枚举
来源：http://ys.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://su.newstarts.cn

[S15] C：类型转换
来源：http://gc.newstarts.cn

(double) a / b
来源：http://uw.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://yt.shxzskj.cn

x |= (1 << 3);
来源：http://bk.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://vv.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://no.nszjky.cn

[S18] C：命令行参数
来源：http://yg.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://me.shtwfgs.cn

[S19] C：快速排序
来源：http://rw.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oz.yuexingan06.cn

[S20] C：二分查找
来源：http://zz.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ld.panjiajie.cn

[S21] C：字符类别判断
来源：http://bc.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hu.panjiajie.cn

[S22] C：字符串转数字
来源：http://bc.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ma.asd995.cn

[S23] C：随机数
来源：http://zb.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wx.huanxung.cn

[S24] C：获取本地时间
来源：http://db.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aj.jctech888.com.cn

[S25] C：内存拷贝
来源：http://ea.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://ek.huanxung.cn

[S26] C：内存清零
来源：http://pf.huanxung.cn

memset(a, 0, sizeof a);
来源：http://ul.9csxet.cn

[S27] C：定义常量
来源：http://wl.colortex.cn

const double PI = 3.14159;
来源：http://lp.lnxyls.cn

[S28] C：静态变量
来源：http://ag.shxzukj.cn

static int counter = 0;
来源：http://sr.wgjwhj.cn

[S29] C：变参函数
来源：http://kr.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gb.asd995.cn

[S30] C：头文件保护
来源：http://eh.huixinmuqiang.cn

#ifndef X_H
来源：http://ac.huanxung.cn

#define X_H
来源：http://cn.nszjky.cn

#endif
来源：http://db.yuexingan06.cn

[S31] C++：Hello World
来源：http://nc.huanxung.cn

#include <iostream>
来源：http://ji.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://yy.nicolike.cn

[S32] C++：字符串
来源：http://jy.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://zm.chemitech.net.cn

[S33] C++：vector 增删
来源：http://rt.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jx.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://mr.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ub.hahajie.cn

[S35] C++：map
来源：http://fj.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eu.bjjhwx.cn

[S36] C++：unordered_map
来源：http://kz.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://et.muxihuayi.cn

[S37] C++：set
来源：http://dp.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hv.newstarts.cn

[S38] C++：排序
来源：http://nq.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://ws.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ed.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xj.wgjwhj.cn

[S40] C++：查找元素
来源：http://gr.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nj.hahajie.cn

[S41] C++：类与构造函数
来源：http://pu.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://me.hahajie.cn

[S42] C++：继承与虚函数
来源：http://xb.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ss.yuexingan06.cn

[S43] C++：智能指针
来源：http://qz.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://xa.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://it.colortex.cn

void inc(int &x) { ++x; }
来源：http://gc.yuexingan06.cn

[S45] C++：lambda
来源：http://cn.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rc.chemitech.net.cn

[S46] C++：函数模板
来源：http://xt.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ew.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://vu.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cg.lnxyls.cn

[S48] C++：逐行读文件
来源：http://zf.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kr.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://vi.panjiajie.cn

[S49] C++：写文件
来源：http://tk.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ep.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://fd.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dn.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://ht.huanxung.cn

static_cast<double>(a) / b
来源：http://yk.colortex.cn

[S52] C++：const 与 noexcept
来源：http://iw.hahajie.cn

int size() const noexcept { return n_; }
来源：http://dd.shtwfgs.cn

[S53] C++：移动语义
来源：http://va.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://gr.hnjuh.cn

[S54] C++：异常处理
来源：http://vi.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qy.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ga.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gd.szsharing.cn

[S56] C++：optional
来源：http://if.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pg.9csxet.cn

[S57] C++：编译期常量
来源：http://fy.huanxung.cn

constexpr int N = 10;
来源：http://jg.hnjuh.cn

[S58] C++：命名空间
来源：http://vc.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://en.newstarts.cn

[S59] C++：静态断言
来源：http://qr.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ik.colortex.cn

[S60] C++：遍历并删除元素
来源：http://fq.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hc.bookmarksfly.cn

================================================================================
来源：http://ww.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ps.huixiangedu.cn

================================================================================
来源：http://wd.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://xa.hahajie.cn

println("Hello")
来源：http://cl.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://yi.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wz.521024.cn

[T03] Kotlin：字符串模板
来源：http://oe.huixinmuqiang.cn

"值: $b"
来源：http://tm.hahajie.cn

[T04] Kotlin：空安全
来源：http://za.colortex.cn

val n: String? = null;  n?.length
来源：http://ii.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://ib.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ow.nszjky.cn

[T06] Kotlin：集合映射
来源：http://sd.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://su.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://nj.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wj.gzmigu.cn

[T08] Kotlin：数据类
来源：http://kn.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://pi.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://js.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://fy.colortex.cn

[T10] Kotlin：默认参数
来源：http://tp.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sc.huanxung.cn

[T11] Kotlin：协程
来源：http://tl.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ot.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://oa.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://qi.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://tj.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://fs.hnjuh.cn

[T14] Kotlin：循环
来源：http://fo.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://sq.huanxung.cn

[T15] Kotlin：接口
来源：http://of.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://sl.szsharing.cn

[T16] Swift：Hello World
来源：http://le.colortex.cn

print("Hello")
来源：http://ja.shxzskj.cn

[T17] Swift：变量与常量
来源：http://pf.jctech888.com.cn

var a = 1;  let b = 2
来源：http://ge.colortex.cn

[T18] Swift：字符串插值
来源：http://xy.nszjky.cn

"值: \(b)"
来源：http://gm.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://ss.nicolike.cn

if let n = opt { print(n) }
来源：http://yj.szsharing.cn

[T20] Swift：数组操作
来源：http://ju.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hx.asd995.cn

[T21] Swift：遍历
来源：http://rf.panjiajie.cn

for x in a { print(x) }
来源：http://lz.chemitech.net.cn

[T22] Swift：字典
来源：http://pb.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ej.yuntaijiaju.cn

[T23] Swift：函数
来源：http://mm.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fl.shxzukj.cn

[T24] Swift：闭包
来源：http://dv.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zd.9csxet.cn

[T25] Swift：结构体
来源：http://oe.jctech888.com.cn

struct P { var x: Int }
来源：http://hb.lnxyls.cn

[T26] Swift：类与重写
来源：http://ua.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ky.gzmigu.cn

[T27] Swift：错误处理
来源：http://ga.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://bu.9csxet.cn

[T28] Swift：枚举
来源：http://va.huanxung.cn

enum Color { case red, green }
来源：http://mq.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://nr.bookmarksfly.cn

guard let x = opt else { return }
来源：http://mh.szxytkj.cn

[T30] Swift：协议
来源：http://mx.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://la.chemitech.net.cn

[T31] Lua：Hello World
来源：http://ug.hahajie.cn

print("Hello")
来源：http://rp.huanxung.cn

[T32] Lua：局部变量
来源：http://xi.haigaiapp.cn

local a = 1
来源：http://kp.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://fn.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lf.shxzukj.cn

[T34] Lua：遍历表
来源：http://qs.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ot.hahajie.cn

[T35] Lua：字典表
来源：http://hb.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://wb.shxzukj.cn

[T36] Lua：函数
来源：http://ya.shtwfgs.cn

function add(a, b) return a + b end
来源：http://lu.colortex.cn

[T37] Lua：字符串拼接
来源：http://ll.lnxyls.cn

"a" .. "b"
来源：http://ln.shxzskj.cn

[T38] Lua：条件
来源：http://nh.nszjky.cn

if x > 0 then print("正") end
来源：http://en.panjiajie.cn

[T39] Lua：模式匹配
来源：http://gc.haigaiapp.cn

string.find(s, "%d+")
来源：http://je.nszjky.cn

[T40] Lua：元表
来源：http://cs.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://pa.huanxung.cn

[T41] Perl：Hello World
来源：http://ff.yuntaijiaju.cn

print "Hello\n";
来源：http://os.haigaiapp.cn

[T42] Perl：变量类型
来源：http://jj.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cx.nicolike.cn

[T43] Perl：字符串插值
来源：http://ua.lnxyls.cn

"值: $a"
来源：http://cg.asd995.cn

[T44] Perl：条件
来源：http://ji.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://dv.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://gu.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://ty.gzmigu.cn

[T46] Perl：哈希操作
来源：http://oe.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uq.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ms.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lw.hnjuh.cn

[T48] Perl：正则替换
来源：http://rz.shxzskj.cn

$s =~ s/old/new/g;
来源：http://fl.wgjwhj.cn

[T49] Perl：函数
来源：http://qb.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gd.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://jx.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zj.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://rk.wgjwhj.cn

[T51] Scala：Hello World
来源：http://yb.szsharing.cn

println("Hello")
来源：http://zb.asd995.cn

[T52] Scala：变量
来源：http://tn.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://il.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://sj.chemitech.net.cn

s"值: $b"
来源：http://yw.hahajie.cn

[T54] Scala：集合映射
来源：http://vl.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://ol.szxytkj.cn

[T55] Scala：集合过滤
来源：http://xd.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://az.panjiajie.cn

[T56] Scala：样例类
来源：http://dm.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://qu.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ec.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tg.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://ch.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qb.muxihuayi.cn

[T59] Scala：循环
来源：http://xe.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ql.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://sn.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ek.chemitech.net.cn

================================================================================
来源：http://og.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xx.shxzukj.cn

================================================================================
来源：http://al.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://wn.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ub.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://ob.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vb.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://yt.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://aw.9csxet.cn

[U04] Py：变量调试打印
来源：http://tl.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://md.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://xj.huanxung.cn

list(dict.fromkeys(arr))
来源：http://nu.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://bb.chemitech.net.cn

{**a, **b}
来源：http://nx.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://to.szsharing.cn

{v: k for k, v in d.items()}
来源：http://hk.panjiajie.cn

[U08] Py：展平二维列表
来源：http://uq.chemitech.net.cn

[y for x in nested for y in x]
来源：http://mi.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://rm.haigaiapp.cn

max(d, key=d.get)
来源：http://eb.shxzukj.cn

[U10] Py：按值排序字典
来源：http://ht.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kl.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://kr.haigaiapp.cn

(x * 2 for x in arr)
来源：http://us.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://il.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://oj.colortex.cn

[U13] Py：固定长度队列
来源：http://aa.haigaiapp.cn

deque(maxlen=10)
来源：http://rb.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://vi.bookmarksfly.cn

defaultdict(list)
来源：http://yh.hahajie.cn

[U15] Py：高精度计时
来源：http://uq.jctech888.com.cn

t = time.perf_counter()
来源：http://vc.hahajie.cn

[U16] Py：命令行参数解析
来源：http://il.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wj.yuexingan06.cn

[U17] Py：初始化日志
来源：http://vm.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://kq.szsharing.cn

[U18] Py：预编译正则
来源：http://ov.9csxet.cn

pat = re.compile(r"\d+")
来源：http://fj.521024.cn

[U19] Py：正则替换带回调
来源：http://qx.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zp.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://lq.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://bi.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://yg.hnjuh.cn

@contextlib.contextmanager
来源：http://qp.asd995.cn

[U22] Py：矩阵转置
来源：http://ko.gzmigu.cn

list(zip(*m))
来源：http://qi.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://mt.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bd.hahajie.cn

[U24] Py：路径操作
来源：http://ac.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://za.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://bh.muxihuayi.cn

csv.DictReader(f)
来源：http://zs.chemitech.net.cn

[U26] Py：并发下载
来源：http://rl.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dl.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://lc.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://aq.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://hj.yuexingan06.cn

UserId = int
来源：http://va.bjjhwx.cn

[U29] Py：属性校验
来源：http://dz.colortex.cn

@property 与 @x.setter 配合
来源：http://pk.521024.cn

[U30] Py：数据类
来源：http://ry.newstarts.cn

@dataclass(slots=True)
来源：http://hv.shxzukj.cn

[U31] Py：单测
来源：http://wq.muxihuayi.cn

python -m pytest -q
来源：http://gi.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ma.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://dl.szxytkj.cn


<!-- 参考信息 -->