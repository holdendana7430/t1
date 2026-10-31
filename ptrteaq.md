代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iq.yuntaijiaju.cn

[S13] C：宏定义
来源：http://zv.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ux.wgjwhj.cn

[S14] C：枚举
来源：http://va.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://rk.nszjky.cn

[S15] C：类型转换
来源：http://go.asd995.cn

(double) a / b
来源：http://yw.newstarts.cn

[S16] C：位操作置位
来源：http://hn.colortex.cn

x |= (1 << 3);
来源：http://sp.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://ha.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fw.newstarts.cn

[S18] C：命令行参数
来源：http://ht.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://nx.521024.cn

[S19] C：快速排序
来源：http://ah.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xv.panjiajie.cn

[S20] C：二分查找
来源：http://um.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ma.shtwfgs.cn

[S21] C：字符类别判断
来源：http://by.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ei.shxzskj.cn

[S22] C：字符串转数字
来源：http://qw.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lo.yuntaijiaju.cn

[S23] C：随机数
来源：http://fm.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fi.jctech888.com.cn

[S24] C：获取本地时间
来源：http://nc.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lx.nszjky.cn

[S25] C：内存拷贝
来源：http://hc.hnjuh.cn

memcpy(dst, src, n);
来源：http://tj.chemitech.net.cn

[S26] C：内存清零
来源：http://ro.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://gb.yuntaijiaju.cn

[S27] C：定义常量
来源：http://np.shxzskj.cn

const double PI = 3.14159;
来源：http://dx.chemitech.net.cn

[S28] C：静态变量
来源：http://jy.newstarts.cn

static int counter = 0;
来源：http://si.gzmigu.cn

[S29] C：变参函数
来源：http://mw.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hs.huixiangedu.cn

[S30] C：头文件保护
来源：http://vf.nicolike.cn

#ifndef X_H
来源：http://bd.521024.cn

#define X_H
来源：http://dg.yuntaijiaju.cn

#endif
来源：http://oc.wgjwhj.cn

[S31] C++：Hello World
来源：http://jo.panjiajie.cn

#include <iostream>
来源：http://fd.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://pl.shxzukj.cn

[S32] C++：字符串
来源：http://by.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://zs.nicolike.cn

[S33] C++：vector 增删
来源：http://ze.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dv.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://kq.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://xc.shtwfgs.cn

[S35] C++：map
来源：http://ex.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lr.szxytkj.cn

[S36] C++：unordered_map
来源：http://ss.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gz.bookmarksfly.cn

[S37] C++：set
来源：http://jy.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kx.hahajie.cn

[S38] C++：排序
来源：http://ys.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://cn.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://hj.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tq.shtwfgs.cn

[S40] C++：查找元素
来源：http://kl.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fl.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://gj.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bf.colortex.cn

[S42] C++：继承与虚函数
来源：http://fs.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://za.chemitech.net.cn

[S43] C++：智能指针
来源：http://ap.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://ge.szsharing.cn

[S44] C++：引用传参
来源：http://rv.huanxung.cn

void inc(int &x) { ++x; }
来源：http://xn.hahajie.cn

[S45] C++：lambda
来源：http://jp.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vb.bjjhwx.cn

[S46] C++：函数模板
来源：http://jd.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cx.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ox.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eh.gzmigu.cn

[S48] C++：逐行读文件
来源：http://lq.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ux.9csxet.cn

while (std::getline(in, line)) { }
来源：http://mt.szsharing.cn

[S49] C++：写文件
来源：http://cd.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://du.huixiangedu.cn

[S50] C++：格式化数字
来源：http://cz.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jf.colortex.cn

[S51] C++：显式类型转换
来源：http://yr.szxytkj.cn

static_cast<double>(a) / b
来源：http://hh.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://kd.nszjky.cn

int size() const noexcept { return n_; }
来源：http://wy.panjiajie.cn

[S53] C++：移动语义
来源：http://yj.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://xq.nszjky.cn

[S54] C++：异常处理
来源：http://xe.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gj.9csxet.cn

[S55] C++：结构化绑定
来源：http://kw.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qf.bjjhwx.cn

[S56] C++：optional
来源：http://ed.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yu.hahajie.cn

[S57] C++：编译期常量
来源：http://nn.jctech888.com.cn

constexpr int N = 10;
来源：http://tr.nszjky.cn

[S58] C++：命名空间
来源：http://th.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://oa.huanxung.cn

[S59] C++：静态断言
来源：http://xd.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gp.521024.cn

[S60] C++：遍历并删除元素
来源：http://rm.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mq.wgjwhj.cn

================================================================================
来源：http://vv.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tr.huixinmuqiang.cn

================================================================================
来源：http://sf.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://ce.gzmigu.cn

println("Hello")
来源：http://iy.asd995.cn

[T02] Kotlin：变量
来源：http://wn.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://au.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://fl.nicolike.cn

"值: $b"
来源：http://qt.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://wu.asd995.cn

val n: String? = null;  n?.length
来源：http://ni.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://ua.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pi.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://oj.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bq.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://rw.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dn.hnjuh.cn

[T08] Kotlin：数据类
来源：http://hi.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://cv.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://ih.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://lj.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://vt.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bw.jctech888.com.cn

[T11] Kotlin：协程
来源：http://mg.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hr.huanxung.cn

[T12] Kotlin：解构声明
来源：http://ka.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://me.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://fo.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://ha.huixiangedu.cn

[T14] Kotlin：循环
来源：http://gg.hnjuh.cn

for (i in 1..10) println(i)
来源：http://vq.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://xk.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://yt.lnxyls.cn

[T16] Swift：Hello World
来源：http://sr.nicolike.cn

print("Hello")
来源：http://xv.shxzukj.cn

[T17] Swift：变量与常量
来源：http://xw.wgjwhj.cn

var a = 1;  let b = 2
来源：http://mw.hnjuh.cn

[T18] Swift：字符串插值
来源：http://vc.shxzukj.cn

"值: \(b)"
来源：http://tc.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ur.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://ot.huanxung.cn

[T20] Swift：数组操作
来源：http://po.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pv.lnxyls.cn

[T21] Swift：遍历
来源：http://vu.huixiangedu.cn

for x in a { print(x) }
来源：http://xf.521024.cn

[T22] Swift：字典
来源：http://fc.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nn.huixiangedu.cn

[T23] Swift：函数
来源：http://zd.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mv.9csxet.cn

[T24] Swift：闭包
来源：http://mr.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lc.yuexingan06.cn

[T25] Swift：结构体
来源：http://lp.521024.cn

struct P { var x: Int }
来源：http://lu.jctech888.com.cn

[T26] Swift：类与重写
来源：http://dd.nszjky.cn

class A: Base { override func f() {} }
来源：http://qq.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://iz.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://nz.wgjwhj.cn

[T28] Swift：枚举
来源：http://ny.newstarts.cn

enum Color { case red, green }
来源：http://vp.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://ug.gzmigu.cn

guard let x = opt else { return }
来源：http://pe.nszjky.cn

[T30] Swift：协议
来源：http://ir.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://kg.huanxung.cn

[T31] Lua：Hello World
来源：http://yx.521024.cn

print("Hello")
来源：http://oo.panjiajie.cn

[T32] Lua：局部变量
来源：http://fs.yuexingan06.cn

local a = 1
来源：http://jz.colortex.cn

[T33] Lua：表（数组）
来源：http://tx.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qd.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://zo.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ry.huixiangedu.cn

[T35] Lua：字典表
来源：http://th.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://qf.newstarts.cn

[T36] Lua：函数
来源：http://wq.9csxet.cn

function add(a, b) return a + b end
来源：http://lx.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://bf.9csxet.cn

"a" .. "b"
来源：http://pw.jctech888.com.cn

[T38] Lua：条件
来源：http://lk.huixiangedu.cn

if x > 0 then print("正") end
来源：http://ef.szxytkj.cn

[T39] Lua：模式匹配
来源：http://gl.asd995.cn

string.find(s, "%d+")
来源：http://ew.hnjuh.cn

[T40] Lua：元表
来源：http://jh.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ot.panjiajie.cn

[T41] Perl：Hello World
来源：http://eh.lnxyls.cn

print "Hello\n";
来源：http://si.chemitech.net.cn

[T42] Perl：变量类型
来源：http://wl.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nq.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://fl.huanxung.cn

"值: $a"
来源：http://td.panjiajie.cn

[T44] Perl：条件
来源：http://dj.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://mq.gzmigu.cn

[T45] Perl：数组遍历
来源：http://hw.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://nr.asd995.cn

[T46] Perl：哈希操作
来源：http://uw.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ve.asd995.cn

[T47] Perl：正则捕获
来源：http://cb.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bd.szsharing.cn

[T48] Perl：正则替换
来源：http://hf.shxzskj.cn

$s =~ s/old/new/g;
来源：http://so.szxytkj.cn

[T49] Perl：函数
来源：http://tl.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wz.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://ej.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hr.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://uy.szxytkj.cn

[T51] Scala：Hello World
来源：http://mo.nicolike.cn

println("Hello")
来源：http://ei.muxihuayi.cn

[T52] Scala：变量
来源：http://qg.yuexingan06.cn

val a = 1;  var b = 2
来源：http://sg.lnxyls.cn

[T53] Scala：字符串插值
来源：http://yu.shxzskj.cn

s"值: $b"
来源：http://iy.wgjwhj.cn

[T54] Scala：集合映射
来源：http://sl.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://lp.shxzskj.cn

[T55] Scala：集合过滤
来源：http://dx.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tl.hnjuh.cn

[T56] Scala：样例类
来源：http://uf.hahajie.cn

case class User(name: String, age: Int)
来源：http://ac.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://xj.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cr.yuexingan06.cn

[T58] Scala：函数定义
来源：http://nx.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ye.shxzskj.cn

[T59] Scala：循环
来源：http://vb.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://jo.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://fh.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ut.colortex.cn

================================================================================
来源：http://ec.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tp.bookmarksfly.cn

================================================================================
来源：http://ld.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://au.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ua.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://zn.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yl.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://ui.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ys.hnjuh.cn

[U04] Py：变量调试打印
来源：http://jd.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pm.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://ak.asd995.cn

list(dict.fromkeys(arr))
来源：http://th.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://wx.yuntaijiaju.cn

{**a, **b}
来源：http://kl.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://vf.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://ew.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://oy.szsharing.cn

[y for x in nested for y in x]
来源：http://fp.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://da.huixinmuqiang.cn

max(d, key=d.get)
来源：http://cd.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://cc.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rf.szsharing.cn

[U11] Py：生成器表达式
来源：http://vo.asd995.cn

(x * 2 for x in arr)
来源：http://hn.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xn.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://xy.hahajie.cn

[U13] Py：固定长度队列
来源：http://ov.jctech888.com.cn

deque(maxlen=10)
来源：http://gv.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://ok.huanxung.cn

defaultdict(list)
来源：http://pe.shxzskj.cn

[U15] Py：高精度计时
来源：http://ye.haigaiapp.cn

t = time.perf_counter()
来源：http://bb.9csxet.cn

[U16] Py：命令行参数解析
来源：http://lq.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sa.nszjky.cn

[U17] Py：初始化日志
来源：http://rg.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ee.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://aj.hahajie.cn

pat = re.compile(r"\d+")
来源：http://xf.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://sb.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ys.521024.cn

[U20] Py：缓存函数结果
来源：http://qo.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ld.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://zv.hahajie.cn

@contextlib.contextmanager
来源：http://sp.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://cr.shxzskj.cn

list(zip(*m))
来源：http://eu.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://kc.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xx.yuexingan06.cn

[U24] Py：路径操作
来源：http://kl.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cu.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://tq.bjjhwx.cn

csv.DictReader(f)
来源：http://el.szxytkj.cn

[U26] Py：并发下载
来源：http://mc.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://df.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://az.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ap.jctech888.com.cn

[U28] Py：类型别名
来源：http://it.newstarts.cn

UserId = int
来源：http://at.haigaiapp.cn

[U29] Py：属性校验
来源：http://wf.asd995.cn

@property 与 @x.setter 配合
来源：http://cs.jianghongdianzi.cn

[U30] Py：数据类
来源：http://rr.huixiangedu.cn

@dataclass(slots=True)
来源：http://kq.huixinmuqiang.cn

[U31] Py：单测
来源：http://xq.shxzskj.cn

python -m pytest -q
来源：http://wi.huanxung.cn

[U32] Py：代码格式化
来源：http://hb.colortex.cn

ruff format . && ruff check --fix .
来源：http://to.gzmigu.cn

[U33] Py：打包发布
来源：http://gr.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://sc.hnjuh.cn

[U34] Py：判断编码
来源：http://gh.asd995.cn

chardet.detect(raw)
来源：http://md.shxzskj.cn

[U35] Py：发送邮件
来源：http://rx.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ji.panjiajie.cn

[U36] Py：定时任务
来源：http://wj.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://xb.chemitech.net.cn


<!-- 参考信息 -->