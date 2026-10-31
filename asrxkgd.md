代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://xw.nicolike.cn

[S15] C：类型转换
来源：http://sa.jctech888.com.cn

(double) a / b
来源：http://qy.shxzukj.cn

[S16] C：位操作置位
来源：http://av.hahajie.cn

x |= (1 << 3);
来源：http://nn.521024.cn

[S17] C：安全拼接字符串
来源：http://be.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xm.asd995.cn

[S18] C：命令行参数
来源：http://lj.nszjky.cn

int main(int argc, char **argv)
来源：http://vn.hnjuh.cn

[S19] C：快速排序
来源：http://rw.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jr.nszjky.cn

[S20] C：二分查找
来源：http://zi.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wf.szsharing.cn

[S21] C：字符类别判断
来源：http://mk.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ih.haigaiapp.cn

[S22] C：字符串转数字
来源：http://eo.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tu.shxzskj.cn

[S23] C：随机数
来源：http://sj.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bv.hnjuh.cn

[S24] C：获取本地时间
来源：http://bj.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fg.lnxyls.cn

[S25] C：内存拷贝
来源：http://sj.jctech888.com.cn

memcpy(dst, src, n);
来源：http://gp.9csxet.cn

[S26] C：内存清零
来源：http://tu.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://oi.jctech888.com.cn

[S27] C：定义常量
来源：http://tj.jctech888.com.cn

const double PI = 3.14159;
来源：http://vm.huanxung.cn

[S28] C：静态变量
来源：http://yy.hahajie.cn

static int counter = 0;
来源：http://zf.wgjwhj.cn

[S29] C：变参函数
来源：http://iz.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bz.shxzukj.cn

[S30] C：头文件保护
来源：http://nn.nszjky.cn

#ifndef X_H
来源：http://yd.gzmigu.cn

#define X_H
来源：http://bg.shtwfgs.cn

#endif
来源：http://ar.yuexingan06.cn

[S31] C++：Hello World
来源：http://oc.bookmarksfly.cn

#include <iostream>
来源：http://mg.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ru.521024.cn

[S32] C++：字符串
来源：http://tw.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://zp.asd995.cn

[S33] C++：vector 增删
来源：http://wn.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qw.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://mb.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://km.gzmigu.cn

[S35] C++：map
来源：http://kg.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wv.asd995.cn

[S36] C++：unordered_map
来源：http://bg.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qh.panjiajie.cn

[S37] C++：set
来源：http://qo.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nz.huanxung.cn

[S38] C++：排序
来源：http://hp.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://bt.colortex.cn

[S39] C++：自定义比较器排序
来源：http://ki.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ri.hahajie.cn

[S40] C++：查找元素
来源：http://dk.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://na.nicolike.cn

[S41] C++：类与构造函数
来源：http://ow.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iv.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://gl.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://wz.wgjwhj.cn

[S43] C++：智能指针
来源：http://mv.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://kg.wgjwhj.cn

[S44] C++：引用传参
来源：http://xo.asd995.cn

void inc(int &x) { ++x; }
来源：http://lc.shxzskj.cn

[S45] C++：lambda
来源：http://cu.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mf.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://cq.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ga.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://hg.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://td.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://io.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nr.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://go.lnxyls.cn

[S49] C++：写文件
来源：http://pp.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yw.hnjuh.cn

[S50] C++：格式化数字
来源：http://os.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ns.asd995.cn

[S51] C++：显式类型转换
来源：http://gj.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://rs.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://ng.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://dx.9csxet.cn

[S53] C++：移动语义
来源：http://iu.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://fa.szxytkj.cn

[S54] C++：异常处理
来源：http://uj.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nc.521024.cn

[S55] C++：结构化绑定
来源：http://ek.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wt.jctech888.com.cn

[S56] C++：optional
来源：http://fs.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hl.asd995.cn

[S57] C++：编译期常量
来源：http://xs.yuntaijiaju.cn

constexpr int N = 10;
来源：http://ls.lnxyls.cn

[S58] C++：命名空间
来源：http://el.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://xy.huixiangedu.cn

[S59] C++：静态断言
来源：http://hp.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ja.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://bc.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ct.gzmigu.cn

================================================================================
来源：http://mp.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jq.gzmigu.cn

================================================================================
来源：http://nm.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://pd.szxytkj.cn

println("Hello")
来源：http://eb.shtwfgs.cn

[T02] Kotlin：变量
来源：http://hb.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sg.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ki.huanxung.cn

"值: $b"
来源：http://uz.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://im.nicolike.cn

val n: String? = null;  n?.length
来源：http://rr.asd995.cn

[T05] Kotlin：when 表达式
来源：http://vi.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tn.colortex.cn

[T06] Kotlin：集合映射
来源：http://nv.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vg.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ox.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ac.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://nm.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ys.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://el.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ki.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://qu.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ex.huixiangedu.cn

[T11] Kotlin：协程
来源：http://el.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qk.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://gd.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://bf.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://zg.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://wz.wgjwhj.cn

[T14] Kotlin：循环
来源：http://er.newstarts.cn

for (i in 1..10) println(i)
来源：http://lk.haigaiapp.cn

[T15] Kotlin：接口
来源：http://xy.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://bi.huanxung.cn

[T16] Swift：Hello World
来源：http://cu.hnjuh.cn

print("Hello")
来源：http://ub.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://ke.huixiangedu.cn

var a = 1;  let b = 2
来源：http://du.hnjuh.cn

[T18] Swift：字符串插值
来源：http://fz.shtwfgs.cn

"值: \(b)"
来源：http://kt.lnxyls.cn

[T19] Swift：可选绑定
来源：http://lr.shxzukj.cn

if let n = opt { print(n) }
来源：http://vw.hahajie.cn

[T20] Swift：数组操作
来源：http://mn.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zp.shxzukj.cn

[T21] Swift：遍历
来源：http://jw.huixiangedu.cn

for x in a { print(x) }
来源：http://yp.wgjwhj.cn

[T22] Swift：字典
来源：http://ng.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xw.muxihuayi.cn

[T23] Swift：函数
来源：http://rs.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cb.wgjwhj.cn

[T24] Swift：闭包
来源：http://pd.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ng.gzmigu.cn

[T25] Swift：结构体
来源：http://ok.chemitech.net.cn

struct P { var x: Int }
来源：http://jg.huixiangedu.cn

[T26] Swift：类与重写
来源：http://fn.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://mz.521024.cn

[T27] Swift：错误处理
来源：http://hd.521024.cn

do { try f() } catch { print(error) }
来源：http://wm.shtwfgs.cn

[T28] Swift：枚举
来源：http://ec.colortex.cn

enum Color { case red, green }
来源：http://ao.521024.cn

[T29] Swift：guard 提前返回
来源：http://xu.szxytkj.cn

guard let x = opt else { return }
来源：http://av.huanxung.cn

[T30] Swift：协议
来源：http://oe.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://vr.jctech888.com.cn

[T31] Lua：Hello World
来源：http://mh.jctech888.com.cn

print("Hello")
来源：http://gc.shtwfgs.cn

[T32] Lua：局部变量
来源：http://vs.9csxet.cn

local a = 1
来源：http://og.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://fy.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sj.haigaiapp.cn

[T34] Lua：遍历表
来源：http://zj.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yd.newstarts.cn

[T35] Lua：字典表
来源：http://cu.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://yd.chemitech.net.cn

[T36] Lua：函数
来源：http://xp.521024.cn

function add(a, b) return a + b end
来源：http://cy.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://bo.hnjuh.cn

"a" .. "b"
来源：http://ay.wgjwhj.cn

[T38] Lua：条件
来源：http://rq.bjjhwx.cn

if x > 0 then print("正") end
来源：http://cq.hahajie.cn

[T39] Lua：模式匹配
来源：http://dv.haigaiapp.cn

string.find(s, "%d+")
来源：http://we.hahajie.cn

[T40] Lua：元表
来源：http://qp.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://cd.shxzukj.cn

[T41] Perl：Hello World
来源：http://uo.shtwfgs.cn

print "Hello\n";
来源：http://rt.muxihuayi.cn

[T42] Perl：变量类型
来源：http://ht.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hm.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://qz.huanxung.cn

"值: $a"
来源：http://lk.9csxet.cn

[T44] Perl：条件
来源：http://hj.asd995.cn

if ($a > 0) { print "正"; }
来源：http://cp.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://uv.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://tk.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://an.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qf.newstarts.cn

[T47] Perl：正则捕获
来源：http://qr.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://or.nicolike.cn

[T48] Perl：正则替换
来源：http://pj.asd995.cn

$s =~ s/old/new/g;
来源：http://oc.jianghongdianzi.cn

[T49] Perl：函数
来源：http://sj.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tu.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ec.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jr.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://eo.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://nu.yuexingan06.cn

println("Hello")
来源：http://yw.bjjhwx.cn

[T52] Scala：变量
来源：http://ts.asd995.cn

val a = 1;  var b = 2
来源：http://nl.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://jg.asd995.cn

s"值: $b"
来源：http://vi.nicolike.cn

[T54] Scala：集合映射
来源：http://pb.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://la.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://wm.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uf.gzmigu.cn

[T56] Scala：样例类
来源：http://vx.szxytkj.cn

case class User(name: String, age: Int)
来源：http://md.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://mq.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ae.nszjky.cn

[T58] Scala：函数定义
来源：http://oe.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eo.muxihuayi.cn

[T59] Scala：循环
来源：http://tz.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://rh.9csxet.cn

[T60] Scala：折叠
来源：http://vm.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wc.shtwfgs.cn

================================================================================
来源：http://bp.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yk.haigaiapp.cn

================================================================================
来源：http://yv.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://zs.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zc.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://xp.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pq.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://we.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ko.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://tj.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://be.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://fu.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://yy.panjiajie.cn

[U06] Py：合并两个字典
来源：http://al.nicolike.cn

{**a, **b}
来源：http://zj.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://wl.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://bz.lnxyls.cn

[U08] Py：展平二维列表
来源：http://yu.huanxung.cn

[y for x in nested for y in x]
来源：http://wa.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://oc.szxytkj.cn

max(d, key=d.get)
来源：http://ds.colortex.cn

[U10] Py：按值排序字典
来源：http://ul.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ad.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ik.panjiajie.cn

(x * 2 for x in arr)
来源：http://zo.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ni.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ow.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://wx.nicolike.cn

deque(maxlen=10)
来源：http://ff.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://ou.huixinmuqiang.cn

defaultdict(list)
来源：http://uv.jctech888.com.cn

[U15] Py：高精度计时
来源：http://xb.chemitech.net.cn

t = time.perf_counter()
来源：http://tw.szsharing.cn

[U16] Py：命令行参数解析
来源：http://xt.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jg.bjjhwx.cn

[U17] Py：初始化日志
来源：http://au.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://zw.szxytkj.cn

[U18] Py：预编译正则
来源：http://ys.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://pb.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://my.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bl.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://sw.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://ps.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://ey.521024.cn

@contextlib.contextmanager
来源：http://bk.newstarts.cn

[U22] Py：矩阵转置
来源：http://ke.lnxyls.cn

list(zip(*m))
来源：http://xa.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://om.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://so.huixiangedu.cn

[U24] Py：路径操作
来源：http://vp.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ok.colortex.cn

[U25] Py：CSV 按字典读
来源：http://yx.yuexingan06.cn

csv.DictReader(f)
来源：http://xp.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://nv.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dv.nszjky.cn

[U27] Py：异步 HTTP
来源：http://ym.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://fv.shxzukj.cn

[U28] Py：类型别名
来源：http://dv.nszjky.cn

UserId = int
来源：http://za.szsharing.cn

[U29] Py：属性校验
来源：http://no.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://np.newstarts.cn

[U30] Py：数据类
来源：http://ky.chemitech.net.cn

@dataclass(slots=True)
来源：http://qg.chemitech.net.cn

[U31] Py：单测
来源：http://im.huixiangedu.cn

python -m pytest -q
来源：http://sj.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://go.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://ej.huixiangedu.cn

[U33] Py：打包发布
来源：http://vi.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://ed.bookmarksfly.cn

[U34] Py：判断编码
来源：http://xn.shxzskj.cn

chardet.detect(raw)
来源：http://tl.shtwfgs.cn

[U35] Py：发送邮件
来源：http://gu.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vs.muxihuayi.cn

[U36] Py：定时任务
来源：http://aa.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ui.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://tz.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cr.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ex.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://mx.panjiajie.cn


<!-- 参考信息 -->