代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hl.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fp.chemitech.net.cn

fclose(f);
来源：http://sh.bjjhwx.cn

[S12] C：写文件
来源：http://sa.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://be.hahajie.cn

[S13] C：宏定义
来源：http://ze.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fa.colortex.cn

[S14] C：枚举
来源：http://jo.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://vw.521024.cn

[S15] C：类型转换
来源：http://mn.shxzskj.cn

(double) a / b
来源：http://xg.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://oq.panjiajie.cn

x |= (1 << 3);
来源：http://gn.521024.cn

[S17] C：安全拼接字符串
来源：http://ow.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hm.hahajie.cn

[S18] C：命令行参数
来源：http://yi.gzmigu.cn

int main(int argc, char **argv)
来源：http://rx.lnxyls.cn

[S19] C：快速排序
来源：http://xr.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://se.lnxyls.cn

[S20] C：二分查找
来源：http://yr.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nl.yuexingan06.cn

[S21] C：字符类别判断
来源：http://mw.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cw.521024.cn

[S22] C：字符串转数字
来源：http://ho.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fx.yuntaijiaju.cn

[S23] C：随机数
来源：http://xa.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sy.yuexingan06.cn

[S24] C：获取本地时间
来源：http://fv.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pi.lnxyls.cn

[S25] C：内存拷贝
来源：http://ms.bjjhwx.cn

memcpy(dst, src, n);
来源：http://bi.bjjhwx.cn

[S26] C：内存清零
来源：http://mh.9csxet.cn

memset(a, 0, sizeof a);
来源：http://zw.nicolike.cn

[S27] C：定义常量
来源：http://wt.wgjwhj.cn

const double PI = 3.14159;
来源：http://rm.asd995.cn

[S28] C：静态变量
来源：http://be.szsharing.cn

static int counter = 0;
来源：http://gl.newstarts.cn

[S29] C：变参函数
来源：http://kh.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wc.hnjuh.cn

[S30] C：头文件保护
来源：http://nr.szsharing.cn

#ifndef X_H
来源：http://bs.szxytkj.cn

#define X_H
来源：http://hi.gzmigu.cn

#endif
来源：http://fk.bjjhwx.cn

[S31] C++：Hello World
来源：http://ao.yuntaijiaju.cn

#include <iostream>
来源：http://tt.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://fx.9csxet.cn

[S32] C++：字符串
来源：http://ct.colortex.cn

std::string s = "hi";  s += "!";
来源：http://lv.shxzskj.cn

[S33] C++：vector 增删
来源：http://ss.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://av.szxytkj.cn

[S34] C++：遍历 vector
来源：http://mc.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://cf.shxzukj.cn

[S35] C++：map
来源：http://xg.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wi.hahajie.cn

[S36] C++：unordered_map
来源：http://hc.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ni.jianghongdianzi.cn

[S37] C++：set
来源：http://xt.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bb.9csxet.cn

[S38] C++：排序
来源：http://zc.521024.cn

std::sort(v.begin(), v.end());
来源：http://rm.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://zw.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oz.shxzukj.cn

[S40] C++：查找元素
来源：http://uj.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gy.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://eg.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lu.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://lo.521024.cn

class B : public Base { public: void f() override {} };
来源：http://ow.haigaiapp.cn

[S43] C++：智能指针
来源：http://nf.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://xl.huanxung.cn

[S44] C++：引用传参
来源：http://kk.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://vh.bookmarksfly.cn

[S45] C++：lambda
来源：http://oj.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dc.lnxyls.cn

[S46] C++：函数模板
来源：http://av.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gs.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://yy.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vx.huanxung.cn

[S48] C++：逐行读文件
来源：http://ax.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wi.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://xx.hnjuh.cn

[S49] C++：写文件
来源：http://if.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eh.hnjuh.cn

[S50] C++：格式化数字
来源：http://kp.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bk.szsharing.cn

[S51] C++：显式类型转换
来源：http://cu.haigaiapp.cn

static_cast<double>(a) / b
来源：http://yq.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://nc.nszjky.cn

int size() const noexcept { return n_; }
来源：http://cs.gzmigu.cn

[S53] C++：移动语义
来源：http://qi.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://ok.nicolike.cn

[S54] C++：异常处理
来源：http://yf.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ae.hahajie.cn

[S55] C++：结构化绑定
来源：http://vb.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fi.newstarts.cn

[S56] C++：optional
来源：http://qy.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mt.bjjhwx.cn

[S57] C++：编译期常量
来源：http://lh.yuntaijiaju.cn

constexpr int N = 10;
来源：http://tv.nicolike.cn

[S58] C++：命名空间
来源：http://ke.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://sn.nszjky.cn

[S59] C++：静态断言
来源：http://ud.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ub.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://dx.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cg.muxihuayi.cn

================================================================================
来源：http://jo.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jk.hnjuh.cn

================================================================================
来源：http://xt.521024.cn

[T01] Kotlin：Hello World
来源：http://xu.bookmarksfly.cn

println("Hello")
来源：http://fn.yuexingan06.cn

[T02] Kotlin：变量
来源：http://pa.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tg.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://lz.chemitech.net.cn

"值: $b"
来源：http://ak.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://ov.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://iw.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://ht.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hu.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://dg.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tr.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://rv.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eo.hahajie.cn

[T08] Kotlin：数据类
来源：http://ce.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://kr.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://xo.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://jz.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ud.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bs.bjjhwx.cn

[T11] Kotlin：协程
来源：http://iu.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vn.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://bt.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://xc.colortex.cn

[T13] Kotlin：只读 Map
来源：http://lz.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://vi.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://vz.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://zh.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://ls.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ec.huanxung.cn

[T16] Swift：Hello World
来源：http://gg.asd995.cn

print("Hello")
来源：http://ud.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://fv.nszjky.cn

var a = 1;  let b = 2
来源：http://sh.hahajie.cn

[T18] Swift：字符串插值
来源：http://rl.hahajie.cn

"值: \(b)"
来源：http://sr.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://bf.shxzskj.cn

if let n = opt { print(n) }
来源：http://oo.asd995.cn

[T20] Swift：数组操作
来源：http://ad.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yg.nicolike.cn

[T21] Swift：遍历
来源：http://qv.huanxung.cn

for x in a { print(x) }
来源：http://gz.panjiajie.cn

[T22] Swift：字典
来源：http://lx.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://no.colortex.cn

[T23] Swift：函数
来源：http://ky.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yt.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://bv.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ml.newstarts.cn

[T25] Swift：结构体
来源：http://ct.wgjwhj.cn

struct P { var x: Int }
来源：http://js.nicolike.cn

[T26] Swift：类与重写
来源：http://xi.hahajie.cn

class A: Base { override func f() {} }
来源：http://bl.panjiajie.cn

[T27] Swift：错误处理
来源：http://ar.newstarts.cn

do { try f() } catch { print(error) }
来源：http://lg.huanxung.cn

[T28] Swift：枚举
来源：http://cg.hnjuh.cn

enum Color { case red, green }
来源：http://pp.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://wh.nszjky.cn

guard let x = opt else { return }
来源：http://bh.haigaiapp.cn

[T30] Swift：协议
来源：http://fb.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://eq.wgjwhj.cn

[T31] Lua：Hello World
来源：http://xv.lnxyls.cn

print("Hello")
来源：http://ea.szsharing.cn

[T32] Lua：局部变量
来源：http://sb.muxihuayi.cn

local a = 1
来源：http://vg.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://oj.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lm.gzmigu.cn

[T34] Lua：遍历表
来源：http://jk.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xq.nszjky.cn

[T35] Lua：字典表
来源：http://ro.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://gm.huixinmuqiang.cn

[T36] Lua：函数
来源：http://hz.newstarts.cn

function add(a, b) return a + b end
来源：http://rb.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://zq.hnjuh.cn

"a" .. "b"
来源：http://ne.szxytkj.cn

[T38] Lua：条件
来源：http://qy.chemitech.net.cn

if x > 0 then print("正") end
来源：http://ht.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://qo.hahajie.cn

string.find(s, "%d+")
来源：http://tk.nicolike.cn

[T40] Lua：元表
来源：http://us.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://rq.bjjhwx.cn

[T41] Perl：Hello World
来源：http://ds.nicolike.cn

print "Hello\n";
来源：http://vg.asd995.cn

[T42] Perl：变量类型
来源：http://iu.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fr.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://dw.shtwfgs.cn

"值: $a"
来源：http://hm.shxzskj.cn

[T44] Perl：条件
来源：http://rz.colortex.cn

if ($a > 0) { print "正"; }
来源：http://fy.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://qg.521024.cn

for my $x (@arr) { print $x; }
来源：http://fq.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://lw.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://js.nicolike.cn

[T47] Perl：正则捕获
来源：http://zh.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zz.521024.cn

[T48] Perl：正则替换
来源：http://vr.gzmigu.cn

$s =~ s/old/new/g;
来源：http://ux.gzmigu.cn

[T49] Perl：函数
来源：http://cg.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rk.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://li.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ai.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ds.9csxet.cn

[T51] Scala：Hello World
来源：http://sq.haigaiapp.cn

println("Hello")
来源：http://sk.haigaiapp.cn

[T52] Scala：变量
来源：http://qj.521024.cn

val a = 1;  var b = 2
来源：http://fo.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://jb.shxzukj.cn

s"值: $b"
来源：http://gt.haigaiapp.cn

[T54] Scala：集合映射
来源：http://fn.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://uo.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://qn.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ah.panjiajie.cn

[T56] Scala：样例类
来源：http://cm.521024.cn

case class User(name: String, age: Int)
来源：http://ms.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://mg.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ux.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://jj.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ic.szsharing.cn

[T59] Scala：循环
来源：http://jb.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://uv.colortex.cn

[T60] Scala：折叠
来源：http://rx.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gy.chemitech.net.cn

================================================================================
来源：http://cl.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uy.bjjhwx.cn

================================================================================
来源：http://az.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://at.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://py.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://rd.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://id.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://cy.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ai.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://zc.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dd.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://jl.huanxung.cn

list(dict.fromkeys(arr))
来源：http://vu.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://ed.nicolike.cn

{**a, **b}
来源：http://dd.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://id.colortex.cn

{v: k for k, v in d.items()}
来源：http://ss.asd995.cn

[U08] Py：展平二维列表
来源：http://wc.shxzukj.cn

[y for x in nested for y in x]
来源：http://np.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://zr.521024.cn

max(d, key=d.get)
来源：http://ar.gzmigu.cn

[U10] Py：按值排序字典
来源：http://zj.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dj.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://ia.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://zr.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gs.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://az.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://xi.shxzskj.cn

deque(maxlen=10)
来源：http://sd.colortex.cn

[U14] Py：分组收集到列表
来源：http://tx.huixinmuqiang.cn

defaultdict(list)
来源：http://xt.nicolike.cn

[U15] Py：高精度计时
来源：http://nc.hnjuh.cn

t = time.perf_counter()
来源：http://dq.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://mc.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mi.bjjhwx.cn

[U17] Py：初始化日志
来源：http://lk.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://cp.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://lm.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://ze.nicolike.cn

[U19] Py：正则替换带回调
来源：http://tb.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bu.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://zk.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ph.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://ey.asd995.cn

@contextlib.contextmanager
来源：http://nn.9csxet.cn

[U22] Py：矩阵转置
来源：http://wn.yuexingan06.cn

list(zip(*m))
来源：http://hl.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://cq.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ht.szsharing.cn

[U24] Py：路径操作
来源：http://bl.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://he.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://un.newstarts.cn

csv.DictReader(f)
来源：http://oz.colortex.cn

[U26] Py：并发下载
来源：http://pw.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bf.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://rl.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qc.newstarts.cn

[U28] Py：类型别名
来源：http://sg.yuexingan06.cn

UserId = int
来源：http://ir.bjjhwx.cn

[U29] Py：属性校验
来源：http://ub.colortex.cn

@property 与 @x.setter 配合
来源：http://ew.lnxyls.cn

[U30] Py：数据类
来源：http://kf.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://ou.hnjuh.cn

[U31] Py：单测
来源：http://mc.colortex.cn

python -m pytest -q
来源：http://at.nszjky.cn

[U32] Py：代码格式化
来源：http://ne.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://aw.huixiangedu.cn

[U33] Py：打包发布
来源：http://pi.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://va.bookmarksfly.cn

[U34] Py：判断编码
来源：http://cd.newstarts.cn

chardet.detect(raw)
来源：http://kw.shxzskj.cn


<!-- 参考信息 -->