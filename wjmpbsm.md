代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xy.shxzskj.cn

[S13] C：宏定义
来源：http://qu.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gh.asd995.cn

[S14] C：枚举
来源：http://gr.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://xi.asd995.cn

[S15] C：类型转换
来源：http://ef.huixiangedu.cn

(double) a / b
来源：http://oy.newstarts.cn

[S16] C：位操作置位
来源：http://cu.bjjhwx.cn

x |= (1 << 3);
来源：http://af.szsharing.cn

[S17] C：安全拼接字符串
来源：http://jk.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dz.9csxet.cn

[S18] C：命令行参数
来源：http://de.chemitech.net.cn

int main(int argc, char **argv)
来源：http://yg.gzmigu.cn

[S19] C：快速排序
来源：http://bg.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bf.jctech888.com.cn

[S20] C：二分查找
来源：http://pr.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gr.chemitech.net.cn

[S21] C：字符类别判断
来源：http://gl.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jn.nicolike.cn

[S22] C：字符串转数字
来源：http://ks.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fv.colortex.cn

[S23] C：随机数
来源：http://fe.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ue.shxzukj.cn

[S24] C：获取本地时间
来源：http://go.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cx.lnxyls.cn

[S25] C：内存拷贝
来源：http://jr.huixiangedu.cn

memcpy(dst, src, n);
来源：http://hc.asd995.cn

[S26] C：内存清零
来源：http://iv.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://yf.shxzukj.cn

[S27] C：定义常量
来源：http://sh.newstarts.cn

const double PI = 3.14159;
来源：http://lt.huixinmuqiang.cn

[S28] C：静态变量
来源：http://cs.521024.cn

static int counter = 0;
来源：http://kl.shxzukj.cn

[S29] C：变参函数
来源：http://ny.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hn.szsharing.cn

[S30] C：头文件保护
来源：http://xo.9csxet.cn

#ifndef X_H
来源：http://kc.chemitech.net.cn

#define X_H
来源：http://or.panjiajie.cn

#endif
来源：http://ke.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://bx.szsharing.cn

#include <iostream>
来源：http://yb.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ox.newstarts.cn

[S32] C++：字符串
来源：http://io.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://gh.shxzskj.cn

[S33] C++：vector 增删
来源：http://tq.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bj.huanxung.cn

[S34] C++：遍历 vector
来源：http://qd.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://jx.szsharing.cn

[S35] C++：map
来源：http://zk.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vl.lnxyls.cn

[S36] C++：unordered_map
来源：http://zw.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mn.colortex.cn

[S37] C++：set
来源：http://sb.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tg.colortex.cn

[S38] C++：排序
来源：http://pk.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://oh.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://gf.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rj.hnjuh.cn

[S40] C++：查找元素
来源：http://qs.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xt.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://af.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://en.asd995.cn

[S42] C++：继承与虚函数
来源：http://iv.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://wl.jctech888.com.cn

[S43] C++：智能指针
来源：http://hk.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://zq.haigaiapp.cn

[S44] C++：引用传参
来源：http://fo.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://cb.huanxung.cn

[S45] C++：lambda
来源：http://eo.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sj.521024.cn

[S46] C++：函数模板
来源：http://yj.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ap.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://qd.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ql.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://px.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ic.521024.cn

while (std::getline(in, line)) { }
来源：http://ie.haigaiapp.cn

[S49] C++：写文件
来源：http://li.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://se.haigaiapp.cn

[S50] C++：格式化数字
来源：http://kk.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oe.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://nz.lnxyls.cn

static_cast<double>(a) / b
来源：http://yq.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://tm.hahajie.cn

int size() const noexcept { return n_; }
来源：http://vj.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://wl.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://qk.newstarts.cn

[S54] C++：异常处理
来源：http://pt.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bg.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://lm.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hd.521024.cn

[S56] C++：optional
来源：http://oo.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mi.panjiajie.cn

[S57] C++：编译期常量
来源：http://ak.panjiajie.cn

constexpr int N = 10;
来源：http://hc.shtwfgs.cn

[S58] C++：命名空间
来源：http://cl.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://kz.szxytkj.cn

[S59] C++：静态断言
来源：http://ma.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dk.colortex.cn

[S60] C++：遍历并删除元素
来源：http://gp.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zk.shtwfgs.cn

================================================================================
来源：http://zy.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lb.haigaiapp.cn

================================================================================
来源：http://ap.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://uu.jianghongdianzi.cn

println("Hello")
来源：http://hj.panjiajie.cn

[T02] Kotlin：变量
来源：http://jd.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dj.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://bf.huanxung.cn

"值: $b"
来源：http://aj.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://yg.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://ho.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://lf.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mi.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://mx.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ni.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://iw.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xk.shxzukj.cn

[T08] Kotlin：数据类
来源：http://yt.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://jy.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://ii.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://fl.521024.cn

[T10] Kotlin：默认参数
来源：http://im.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yv.chemitech.net.cn

[T11] Kotlin：协程
来源：http://bl.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cs.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://vh.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://xm.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://fk.nicolike.cn

val m = mapOf("a" to 1)
来源：http://ga.newstarts.cn

[T14] Kotlin：循环
来源：http://qz.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://vm.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://fu.szsharing.cn

interface Shape { fun area(): Double }
来源：http://vd.hnjuh.cn

[T16] Swift：Hello World
来源：http://nn.lnxyls.cn

print("Hello")
来源：http://mm.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://zj.panjiajie.cn

var a = 1;  let b = 2
来源：http://mb.huanxung.cn

[T18] Swift：字符串插值
来源：http://nl.bjjhwx.cn

"值: \(b)"
来源：http://xy.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://vh.shxzskj.cn

if let n = opt { print(n) }
来源：http://eq.9csxet.cn

[T20] Swift：数组操作
来源：http://xf.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yh.szxytkj.cn

[T21] Swift：遍历
来源：http://ku.yuntaijiaju.cn

for x in a { print(x) }
来源：http://jq.9csxet.cn

[T22] Swift：字典
来源：http://ao.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gz.bookmarksfly.cn

[T23] Swift：函数
来源：http://hx.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gt.muxihuayi.cn

[T24] Swift：闭包
来源：http://ek.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eh.nszjky.cn

[T25] Swift：结构体
来源：http://ol.nszjky.cn

struct P { var x: Int }
来源：http://ms.huixiangedu.cn

[T26] Swift：类与重写
来源：http://at.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://ue.9csxet.cn

[T27] Swift：错误处理
来源：http://da.hahajie.cn

do { try f() } catch { print(error) }
来源：http://fo.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://fi.521024.cn

enum Color { case red, green }
来源：http://rm.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://vt.bookmarksfly.cn

guard let x = opt else { return }
来源：http://ks.muxihuayi.cn

[T30] Swift：协议
来源：http://bi.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://ck.szxytkj.cn

[T31] Lua：Hello World
来源：http://qy.szxytkj.cn

print("Hello")
来源：http://us.chemitech.net.cn

[T32] Lua：局部变量
来源：http://sk.asd995.cn

local a = 1
来源：http://ne.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://zn.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bn.haigaiapp.cn

[T34] Lua：遍历表
来源：http://cb.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://co.muxihuayi.cn

[T35] Lua：字典表
来源：http://yn.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://er.shxzskj.cn

[T36] Lua：函数
来源：http://wt.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://nn.9csxet.cn

[T37] Lua：字符串拼接
来源：http://qg.nszjky.cn

"a" .. "b"
来源：http://zf.yuexingan06.cn

[T38] Lua：条件
来源：http://os.bjjhwx.cn

if x > 0 then print("正") end
来源：http://sb.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://oy.bookmarksfly.cn

string.find(s, "%d+")
来源：http://wg.colortex.cn

[T40] Lua：元表
来源：http://ks.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://og.shxzukj.cn

[T41] Perl：Hello World
来源：http://nd.lnxyls.cn

print "Hello\n";
来源：http://iw.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://yk.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xn.newstarts.cn

[T43] Perl：字符串插值
来源：http://vy.haigaiapp.cn

"值: $a"
来源：http://os.hnjuh.cn

[T44] Perl：条件
来源：http://dc.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://ef.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://uc.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ja.shxzskj.cn

[T46] Perl：哈希操作
来源：http://il.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mo.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://xm.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dp.huanxung.cn

[T48] Perl：正则替换
来源：http://sy.521024.cn

$s =~ s/old/new/g;
来源：http://xz.yuntaijiaju.cn

[T49] Perl：函数
来源：http://tj.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://de.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://je.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xm.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://uw.nicolike.cn

[T51] Scala：Hello World
来源：http://lh.chemitech.net.cn

println("Hello")
来源：http://cy.wgjwhj.cn

[T52] Scala：变量
来源：http://xi.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://hl.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://sq.shtwfgs.cn

s"值: $b"
来源：http://th.hnjuh.cn

[T54] Scala：集合映射
来源：http://ao.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xk.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://ud.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://km.chemitech.net.cn

[T56] Scala：样例类
来源：http://ul.nicolike.cn

case class User(name: String, age: Int)
来源：http://ny.huanxung.cn

[T57] Scala：模式匹配
来源：http://vn.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nr.huixiangedu.cn

[T58] Scala：函数定义
来源：http://vg.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kj.chemitech.net.cn

[T59] Scala：循环
来源：http://db.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://cv.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ik.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gk.bookmarksfly.cn

================================================================================
来源：http://bs.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iu.shxzukj.cn

================================================================================
来源：http://gs.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ir.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ca.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://sw.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ji.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://ew.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hp.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://qu.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ba.nszjky.cn

[U05] Py：列表去重且保序
来源：http://pu.newstarts.cn

list(dict.fromkeys(arr))
来源：http://jx.shxzukj.cn

[U06] Py：合并两个字典
来源：http://hs.asd995.cn

{**a, **b}
来源：http://ke.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://uj.521024.cn

{v: k for k, v in d.items()}
来源：http://hq.gzmigu.cn

[U08] Py：展平二维列表
来源：http://gi.shxzskj.cn

[y for x in nested for y in x]
来源：http://qf.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://mp.gzmigu.cn

max(d, key=d.get)
来源：http://bh.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://cc.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eu.lnxyls.cn

[U11] Py：生成器表达式
来源：http://ik.bjjhwx.cn

(x * 2 for x in arr)
来源：http://dj.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uo.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://to.521024.cn

[U13] Py：固定长度队列
来源：http://cv.bjjhwx.cn

deque(maxlen=10)
来源：http://dg.newstarts.cn

[U14] Py：分组收集到列表
来源：http://yf.yuexingan06.cn

defaultdict(list)
来源：http://pc.huanxung.cn

[U15] Py：高精度计时
来源：http://vd.huixinmuqiang.cn

t = time.perf_counter()
来源：http://me.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://fi.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hg.gzmigu.cn

[U17] Py：初始化日志
来源：http://fm.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://nj.hahajie.cn

[U18] Py：预编译正则
来源：http://rs.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ie.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://kb.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lx.colortex.cn

[U20] Py：缓存函数结果
来源：http://kb.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://bv.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://sv.hnjuh.cn

@contextlib.contextmanager
来源：http://wq.panjiajie.cn

[U22] Py：矩阵转置
来源：http://kr.asd995.cn

list(zip(*m))
来源：http://eq.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://xj.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ho.gzmigu.cn

[U24] Py：路径操作
来源：http://iy.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xw.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://sy.bookmarksfly.cn

csv.DictReader(f)
来源：http://js.jctech888.com.cn

[U26] Py：并发下载
来源：http://yr.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yi.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://su.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://nt.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://cz.521024.cn

UserId = int
来源：http://jo.huanxung.cn

[U29] Py：属性校验
来源：http://ef.gzmigu.cn

@property 与 @x.setter 配合
来源：http://vg.nicolike.cn

[U30] Py：数据类
来源：http://cx.chemitech.net.cn

@dataclass(slots=True)
来源：http://an.panjiajie.cn

[U31] Py：单测
来源：http://me.huixiangedu.cn

python -m pytest -q
来源：http://jd.nszjky.cn

[U32] Py：代码格式化
来源：http://sa.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://fv.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://yp.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ao.nicolike.cn

[U34] Py：判断编码
来源：http://ts.yuexingan06.cn

chardet.detect(raw)
来源：http://fa.chemitech.net.cn

[U35] Py：发送邮件
来源：http://gf.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rq.asd995.cn

[U36] Py：定时任务
来源：http://hk.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://pp.szsharing.cn


<!-- 参考信息 -->