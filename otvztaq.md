代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pi.shxzskj.cn

[S13] C：宏定义
来源：http://bm.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hm.shtwfgs.cn

[S14] C：枚举
来源：http://kg.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://fy.shxzskj.cn

[S15] C：类型转换
来源：http://ia.bjjhwx.cn

(double) a / b
来源：http://km.hahajie.cn

[S16] C：位操作置位
来源：http://qy.yuexingan06.cn

x |= (1 << 3);
来源：http://bo.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://qa.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yp.lnxyls.cn

[S18] C：命令行参数
来源：http://so.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://bh.bjjhwx.cn

[S19] C：快速排序
来源：http://wf.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zn.muxihuayi.cn

[S20] C：二分查找
来源：http://fq.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ej.chemitech.net.cn

[S21] C：字符类别判断
来源：http://dj.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zc.9csxet.cn

[S22] C：字符串转数字
来源：http://ng.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vd.yuexingan06.cn

[S23] C：随机数
来源：http://fs.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://br.shxzskj.cn

[S24] C：获取本地时间
来源：http://wm.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vl.asd995.cn

[S25] C：内存拷贝
来源：http://ue.jctech888.com.cn

memcpy(dst, src, n);
来源：http://lu.shxzukj.cn

[S26] C：内存清零
来源：http://sa.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://pg.huanxung.cn

[S27] C：定义常量
来源：http://pg.shxzskj.cn

const double PI = 3.14159;
来源：http://hs.colortex.cn

[S28] C：静态变量
来源：http://ah.bookmarksfly.cn

static int counter = 0;
来源：http://kd.hnjuh.cn

[S29] C：变参函数
来源：http://bg.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vr.chemitech.net.cn

[S30] C：头文件保护
来源：http://ca.chemitech.net.cn

#ifndef X_H
来源：http://be.newstarts.cn

#define X_H
来源：http://om.nszjky.cn

#endif
来源：http://sm.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://oq.newstarts.cn

#include <iostream>
来源：http://yc.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://pd.colortex.cn

[S32] C++：字符串
来源：http://vy.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://md.hahajie.cn

[S33] C++：vector 增删
来源：http://gs.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lb.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://zo.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://vk.shtwfgs.cn

[S35] C++：map
来源：http://of.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://at.muxihuayi.cn

[S36] C++：unordered_map
来源：http://si.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fu.wgjwhj.cn

[S37] C++：set
来源：http://dg.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hh.colortex.cn

[S38] C++：排序
来源：http://hr.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://eu.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://kd.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sh.jctech888.com.cn

[S40] C++：查找元素
来源：http://me.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://us.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://tk.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eu.asd995.cn

[S42] C++：继承与虚函数
来源：http://rn.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://wx.yuexingan06.cn

[S43] C++：智能指针
来源：http://mx.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://ym.hnjuh.cn

[S44] C++：引用传参
来源：http://lv.newstarts.cn

void inc(int &x) { ++x; }
来源：http://rx.bookmarksfly.cn

[S45] C++：lambda
来源：http://hh.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nt.bjjhwx.cn

[S46] C++：函数模板
来源：http://lu.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ek.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://oh.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gc.newstarts.cn

[S48] C++：逐行读文件
来源：http://gr.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://by.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://va.9csxet.cn

[S49] C++：写文件
来源：http://ml.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yt.panjiajie.cn

[S50] C++：格式化数字
来源：http://wq.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ng.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://lf.szsharing.cn

static_cast<double>(a) / b
来源：http://zd.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://im.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://qp.nicolike.cn

[S53] C++：移动语义
来源：http://aw.521024.cn

std::vector<int> w = std::move(v);
来源：http://nr.newstarts.cn

[S54] C++：异常处理
来源：http://jl.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ti.newstarts.cn

[S55] C++：结构化绑定
来源：http://cn.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wb.hnjuh.cn

[S56] C++：optional
来源：http://pv.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hd.yuexingan06.cn

[S57] C++：编译期常量
来源：http://gw.yuntaijiaju.cn

constexpr int N = 10;
来源：http://xc.nicolike.cn

[S58] C++：命名空间
来源：http://yg.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://ck.panjiajie.cn

[S59] C++：静态断言
来源：http://rv.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cu.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://ky.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yx.9csxet.cn

================================================================================
来源：http://wv.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cj.huanxung.cn

================================================================================
来源：http://du.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://sy.shxzskj.cn

println("Hello")
来源：http://ay.panjiajie.cn

[T02] Kotlin：变量
来源：http://ui.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://li.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://dh.huanxung.cn

"值: $b"
来源：http://ua.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://xt.gzmigu.cn

val n: String? = null;  n?.length
来源：http://hf.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://tx.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qh.nszjky.cn

[T06] Kotlin：集合映射
来源：http://bk.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yc.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://lc.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ra.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://bx.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://lh.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://lm.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://mo.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://fn.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sf.9csxet.cn

[T11] Kotlin：协程
来源：http://bx.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://si.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ie.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://nd.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://lk.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://wz.muxihuayi.cn

[T14] Kotlin：循环
来源：http://sy.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://jq.haigaiapp.cn

[T15] Kotlin：接口
来源：http://fm.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://bs.szsharing.cn

[T16] Swift：Hello World
来源：http://an.newstarts.cn

print("Hello")
来源：http://ip.hnjuh.cn

[T17] Swift：变量与常量
来源：http://ms.shxzskj.cn

var a = 1;  let b = 2
来源：http://qj.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://nz.chemitech.net.cn

"值: \(b)"
来源：http://hh.gzmigu.cn

[T19] Swift：可选绑定
来源：http://fy.yuexingan06.cn

if let n = opt { print(n) }
来源：http://vz.yuexingan06.cn

[T20] Swift：数组操作
来源：http://lc.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ld.huanxung.cn

[T21] Swift：遍历
来源：http://kt.nszjky.cn

for x in a { print(x) }
来源：http://ke.yuntaijiaju.cn

[T22] Swift：字典
来源：http://xl.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fx.chemitech.net.cn

[T23] Swift：函数
来源：http://st.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dw.gzmigu.cn

[T24] Swift：闭包
来源：http://be.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gv.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://ba.521024.cn

struct P { var x: Int }
来源：http://ul.muxihuayi.cn

[T26] Swift：类与重写
来源：http://kz.szsharing.cn

class A: Base { override func f() {} }
来源：http://ub.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://iy.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://fo.szxytkj.cn

[T28] Swift：枚举
来源：http://ih.jctech888.com.cn

enum Color { case red, green }
来源：http://xf.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://pd.gzmigu.cn

guard let x = opt else { return }
来源：http://mv.chemitech.net.cn

[T30] Swift：协议
来源：http://aa.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://fe.hahajie.cn

[T31] Lua：Hello World
来源：http://yl.szxytkj.cn

print("Hello")
来源：http://dx.nicolike.cn

[T32] Lua：局部变量
来源：http://ej.jctech888.com.cn

local a = 1
来源：http://ga.asd995.cn

[T33] Lua：表（数组）
来源：http://ji.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wz.panjiajie.cn

[T34] Lua：遍历表
来源：http://ir.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mi.colortex.cn

[T35] Lua：字典表
来源：http://ed.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://sb.huixiangedu.cn

[T36] Lua：函数
来源：http://rl.9csxet.cn

function add(a, b) return a + b end
来源：http://jf.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://bn.shxzskj.cn

"a" .. "b"
来源：http://hi.lnxyls.cn

[T38] Lua：条件
来源：http://dy.shxzskj.cn

if x > 0 then print("正") end
来源：http://fz.lnxyls.cn

[T39] Lua：模式匹配
来源：http://cr.nszjky.cn

string.find(s, "%d+")
来源：http://qb.newstarts.cn

[T40] Lua：元表
来源：http://ty.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://bq.chemitech.net.cn

[T41] Perl：Hello World
来源：http://zy.521024.cn

print "Hello\n";
来源：http://iw.521024.cn

[T42] Perl：变量类型
来源：http://wa.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wh.lnxyls.cn

[T43] Perl：字符串插值
来源：http://kx.chemitech.net.cn

"值: $a"
来源：http://cr.521024.cn

[T44] Perl：条件
来源：http://nf.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://uh.shxzskj.cn

[T45] Perl：数组遍历
来源：http://oe.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://xl.huanxung.cn

[T46] Perl：哈希操作
来源：http://si.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kz.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://km.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wk.nicolike.cn

[T48] Perl：正则替换
来源：http://dq.newstarts.cn

$s =~ s/old/new/g;
来源：http://mm.newstarts.cn

[T49] Perl：函数
来源：http://nn.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ra.nszjky.cn

[T50] Perl：逐行读文件
来源：http://gu.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://du.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vc.gzmigu.cn

[T51] Scala：Hello World
来源：http://ez.szsharing.cn

println("Hello")
来源：http://ps.521024.cn

[T52] Scala：变量
来源：http://xq.shxzskj.cn

val a = 1;  var b = 2
来源：http://at.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://ep.yuexingan06.cn

s"值: $b"
来源：http://if.muxihuayi.cn

[T54] Scala：集合映射
来源：http://bb.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://vc.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://lj.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://va.bookmarksfly.cn

[T56] Scala：样例类
来源：http://wn.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ra.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://ad.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dg.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://do.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cp.521024.cn

[T59] Scala：循环
来源：http://of.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://dy.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://ql.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nx.9csxet.cn

================================================================================
来源：http://ma.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bd.jctech888.com.cn

================================================================================
来源：http://ca.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://er.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ra.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://vj.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xz.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://bt.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oi.colortex.cn

[U04] Py：变量调试打印
来源：http://lf.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rq.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://xf.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://hz.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://ih.gzmigu.cn

{**a, **b}
来源：http://pi.szsharing.cn

[U07] Py：反转字典键值
来源：http://wn.huanxung.cn

{v: k for k, v in d.items()}
来源：http://lf.newstarts.cn

[U08] Py：展平二维列表
来源：http://xv.muxihuayi.cn

[y for x in nested for y in x]
来源：http://pf.asd995.cn

[U09] Py：字典取最大值的键
来源：http://uc.asd995.cn

max(d, key=d.get)
来源：http://bv.huanxung.cn

[U10] Py：按值排序字典
来源：http://sf.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ey.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://xc.jctech888.com.cn

(x * 2 for x in arr)
来源：http://qh.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yo.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://oq.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://zf.jctech888.com.cn

deque(maxlen=10)
来源：http://of.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://ey.hahajie.cn

defaultdict(list)
来源：http://qy.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://rt.asd995.cn

t = time.perf_counter()
来源：http://rh.521024.cn

[U16] Py：命令行参数解析
来源：http://jj.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ar.chemitech.net.cn

[U17] Py：初始化日志
来源：http://rn.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://xg.shxzskj.cn

[U18] Py：预编译正则
来源：http://dm.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://zr.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://zf.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uo.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://hg.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://mw.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://cb.shxzukj.cn

@contextlib.contextmanager
来源：http://aw.colortex.cn

[U22] Py：矩阵转置
来源：http://gi.nicolike.cn

list(zip(*m))
来源：http://om.nszjky.cn

[U23] Py：分块读取大文件
来源：http://ik.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hx.bookmarksfly.cn

[U24] Py：路径操作
来源：http://la.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://il.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://ll.nszjky.cn

csv.DictReader(f)
来源：http://yf.hnjuh.cn

[U26] Py：并发下载
来源：http://qy.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ee.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://wc.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://fm.hnjuh.cn

[U28] Py：类型别名
来源：http://ye.chemitech.net.cn

UserId = int
来源：http://rn.shxzskj.cn

[U29] Py：属性校验
来源：http://qe.asd995.cn

@property 与 @x.setter 配合
来源：http://af.gzmigu.cn

[U30] Py：数据类
来源：http://dx.panjiajie.cn

@dataclass(slots=True)
来源：http://jn.hahajie.cn

[U31] Py：单测
来源：http://yr.nszjky.cn

python -m pytest -q
来源：http://sp.521024.cn

[U32] Py：代码格式化
来源：http://yz.nicolike.cn

ruff format . && ruff check --fix .
来源：http://wl.huixiangedu.cn

[U33] Py：打包发布
来源：http://wi.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://bv.gzmigu.cn

[U34] Py：判断编码
来源：http://sy.huixinmuqiang.cn

chardet.detect(raw)
来源：http://rv.521024.cn

[U35] Py：发送邮件
来源：http://jv.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dk.asd995.cn

[U36] Py：定时任务
来源：http://de.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://ys.jctech888.com.cn


<!-- 参考信息 -->