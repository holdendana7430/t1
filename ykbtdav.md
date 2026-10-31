代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ie.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ig.521024.cn

fclose(f);
来源：http://ht.9csxet.cn

[S12] C：写文件
来源：http://ut.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yn.nicolike.cn

[S13] C：宏定义
来源：http://ut.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kx.szxytkj.cn

[S14] C：枚举
来源：http://mb.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://cp.chemitech.net.cn

[S15] C：类型转换
来源：http://mb.hahajie.cn

(double) a / b
来源：http://gr.szsharing.cn

[S16] C：位操作置位
来源：http://pk.hahajie.cn

x |= (1 << 3);
来源：http://fe.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://va.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vp.yuexingan06.cn

[S18] C：命令行参数
来源：http://at.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://af.shtwfgs.cn

[S19] C：快速排序
来源：http://xd.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aw.huixinmuqiang.cn

[S20] C：二分查找
来源：http://dm.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mz.521024.cn

[S21] C：字符类别判断
来源：http://gm.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ns.gzmigu.cn

[S22] C：字符串转数字
来源：http://nz.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iy.yuntaijiaju.cn

[S23] C：随机数
来源：http://gy.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xv.muxihuayi.cn

[S24] C：获取本地时间
来源：http://iz.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dl.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://si.9csxet.cn

memcpy(dst, src, n);
来源：http://pf.bjjhwx.cn

[S26] C：内存清零
来源：http://hs.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ba.muxihuayi.cn

[S27] C：定义常量
来源：http://de.bookmarksfly.cn

const double PI = 3.14159;
来源：http://ns.chemitech.net.cn

[S28] C：静态变量
来源：http://di.muxihuayi.cn

static int counter = 0;
来源：http://to.hahajie.cn

[S29] C：变参函数
来源：http://fi.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fs.bjjhwx.cn

[S30] C：头文件保护
来源：http://gb.lnxyls.cn

#ifndef X_H
来源：http://yh.bjjhwx.cn

#define X_H
来源：http://wn.gzmigu.cn

#endif
来源：http://gh.gzmigu.cn

[S31] C++：Hello World
来源：http://mz.yuntaijiaju.cn

#include <iostream>
来源：http://sl.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://hu.newstarts.cn

[S32] C++：字符串
来源：http://iy.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://ek.shtwfgs.cn

[S33] C++：vector 增删
来源：http://gj.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gx.shxzskj.cn

[S34] C++：遍历 vector
来源：http://ii.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://nf.chemitech.net.cn

[S35] C++：map
来源：http://ji.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ce.hnjuh.cn

[S36] C++：unordered_map
来源：http://ct.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yq.shtwfgs.cn

[S37] C++：set
来源：http://zw.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ci.shtwfgs.cn

[S38] C++：排序
来源：http://oq.colortex.cn

std::sort(v.begin(), v.end());
来源：http://lh.521024.cn

[S39] C++：自定义比较器排序
来源：http://gt.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vv.gzmigu.cn

[S40] C++：查找元素
来源：http://kj.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xb.szsharing.cn

[S41] C++：类与构造函数
来源：http://ay.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bn.9csxet.cn

[S42] C++：继承与虚函数
来源：http://bl.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://cb.asd995.cn

[S43] C++：智能指针
来源：http://sj.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://fc.panjiajie.cn

[S44] C++：引用传参
来源：http://mv.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://uz.nicolike.cn

[S45] C++：lambda
来源：http://je.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yo.asd995.cn

[S46] C++：函数模板
来源：http://xf.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://so.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://vb.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iq.asd995.cn

[S48] C++：逐行读文件
来源：http://tu.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ou.asd995.cn

while (std::getline(in, line)) { }
来源：http://nk.hnjuh.cn

[S49] C++：写文件
来源：http://tt.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uz.szsharing.cn

[S50] C++：格式化数字
来源：http://kr.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fc.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://ww.muxihuayi.cn

static_cast<double>(a) / b
来源：http://qi.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://jq.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://li.nicolike.cn

[S53] C++：移动语义
来源：http://cf.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://jg.colortex.cn

[S54] C++：异常处理
来源：http://qr.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lm.shxzskj.cn

[S55] C++：结构化绑定
来源：http://sz.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fv.hnjuh.cn

[S56] C++：optional
来源：http://mn.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gl.9csxet.cn

[S57] C++：编译期常量
来源：http://bh.muxihuayi.cn

constexpr int N = 10;
来源：http://hw.gzmigu.cn

[S58] C++：命名空间
来源：http://sh.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://wb.haigaiapp.cn

[S59] C++：静态断言
来源：http://ep.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vz.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://ki.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qv.yuexingan06.cn

================================================================================
来源：http://he.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ay.shxzskj.cn

================================================================================
来源：http://oa.521024.cn

[T01] Kotlin：Hello World
来源：http://qn.shtwfgs.cn

println("Hello")
来源：http://tn.chemitech.net.cn

[T02] Kotlin：变量
来源：http://on.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zd.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://mk.jctech888.com.cn

"值: $b"
来源：http://ti.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://gx.colortex.cn

val n: String? = null;  n?.length
来源：http://ww.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://vn.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bh.colortex.cn

[T06] Kotlin：集合映射
来源：http://lx.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hh.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://lo.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ip.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://ix.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://gm.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://pb.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://zz.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://mv.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qo.hnjuh.cn

[T11] Kotlin：协程
来源：http://ba.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ef.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://qk.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://fj.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://wc.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://bh.huanxung.cn

[T14] Kotlin：循环
来源：http://wb.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://fl.szxytkj.cn

[T15] Kotlin：接口
来源：http://qw.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://wh.huixiangedu.cn

[T16] Swift：Hello World
来源：http://na.bookmarksfly.cn

print("Hello")
来源：http://sv.panjiajie.cn

[T17] Swift：变量与常量
来源：http://ds.521024.cn

var a = 1;  let b = 2
来源：http://fo.521024.cn

[T18] Swift：字符串插值
来源：http://kw.wgjwhj.cn

"值: \(b)"
来源：http://hv.shxzskj.cn

[T19] Swift：可选绑定
来源：http://nl.9csxet.cn

if let n = opt { print(n) }
来源：http://zy.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://db.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vb.shxzukj.cn

[T21] Swift：遍历
来源：http://pr.szsharing.cn

for x in a { print(x) }
来源：http://vc.huanxung.cn

[T22] Swift：字典
来源：http://bp.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cq.huixiangedu.cn

[T23] Swift：函数
来源：http://jt.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://md.jctech888.com.cn

[T24] Swift：闭包
来源：http://nh.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tl.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://af.yuntaijiaju.cn

struct P { var x: Int }
来源：http://mt.szxytkj.cn

[T26] Swift：类与重写
来源：http://yp.9csxet.cn

class A: Base { override func f() {} }
来源：http://lz.shxzskj.cn

[T27] Swift：错误处理
来源：http://wu.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://fs.huixiangedu.cn

[T28] Swift：枚举
来源：http://kt.hnjuh.cn

enum Color { case red, green }
来源：http://ri.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://hc.yuexingan06.cn

guard let x = opt else { return }
来源：http://qs.hnjuh.cn

[T30] Swift：协议
来源：http://rq.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://pa.szxytkj.cn

[T31] Lua：Hello World
来源：http://ev.yuexingan06.cn

print("Hello")
来源：http://qo.jctech888.com.cn

[T32] Lua：局部变量
来源：http://tq.nszjky.cn

local a = 1
来源：http://zl.colortex.cn

[T33] Lua：表（数组）
来源：http://pt.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ks.szxytkj.cn

[T34] Lua：遍历表
来源：http://ng.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mf.chemitech.net.cn

[T35] Lua：字典表
来源：http://dj.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://cd.shxzukj.cn

[T36] Lua：函数
来源：http://ga.panjiajie.cn

function add(a, b) return a + b end
来源：http://nz.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://ky.haigaiapp.cn

"a" .. "b"
来源：http://gi.panjiajie.cn

[T38] Lua：条件
来源：http://ej.colortex.cn

if x > 0 then print("正") end
来源：http://gy.shxzskj.cn

[T39] Lua：模式匹配
来源：http://zz.shxzukj.cn

string.find(s, "%d+")
来源：http://ea.shxzskj.cn

[T40] Lua：元表
来源：http://zz.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://mz.lnxyls.cn

[T41] Perl：Hello World
来源：http://rf.chemitech.net.cn

print "Hello\n";
来源：http://mr.shxzukj.cn

[T42] Perl：变量类型
来源：http://ds.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nz.panjiajie.cn

[T43] Perl：字符串插值
来源：http://rv.shtwfgs.cn

"值: $a"
来源：http://js.9csxet.cn

[T44] Perl：条件
来源：http://ql.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://zd.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://wx.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://dq.521024.cn

[T46] Perl：哈希操作
来源：http://ze.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fq.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://wc.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ii.hahajie.cn

[T48] Perl：正则替换
来源：http://vv.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://nc.muxihuayi.cn

[T49] Perl：函数
来源：http://iq.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hn.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://si.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ck.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://ll.nszjky.cn

[T51] Scala：Hello World
来源：http://ar.jianghongdianzi.cn

println("Hello")
来源：http://yb.nicolike.cn

[T52] Scala：变量
来源：http://ms.colortex.cn

val a = 1;  var b = 2
来源：http://bc.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://kt.panjiajie.cn

s"值: $b"
来源：http://js.521024.cn

[T54] Scala：集合映射
来源：http://md.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://yd.szsharing.cn

[T55] Scala：集合过滤
来源：http://ep.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://je.muxihuayi.cn

[T56] Scala：样例类
来源：http://pm.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://ek.asd995.cn

[T57] Scala：模式匹配
来源：http://fw.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ft.jctech888.com.cn

[T58] Scala：函数定义
来源：http://op.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wr.shxzskj.cn

[T59] Scala：循环
来源：http://rr.521024.cn

for (i <- 1 to 10) println(i)
来源：http://pw.szxytkj.cn

[T60] Scala：折叠
来源：http://yw.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pm.jctech888.com.cn

================================================================================
来源：http://ba.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nr.shxzskj.cn

================================================================================
来源：http://nu.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://mc.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jf.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://cd.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zr.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://lg.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bx.hahajie.cn

[U04] Py：变量调试打印
来源：http://ra.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://in.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://gl.521024.cn

list(dict.fromkeys(arr))
来源：http://ox.521024.cn

[U06] Py：合并两个字典
来源：http://ek.hahajie.cn

{**a, **b}
来源：http://na.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://sv.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://nj.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://tb.hnjuh.cn

[y for x in nested for y in x]
来源：http://qm.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://bq.huanxung.cn

max(d, key=d.get)
来源：http://sy.521024.cn

[U10] Py：按值排序字典
来源：http://ft.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wm.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ew.shxzukj.cn

(x * 2 for x in arr)
来源：http://mh.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wl.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://gk.colortex.cn

[U13] Py：固定长度队列
来源：http://sx.nicolike.cn

deque(maxlen=10)
来源：http://qg.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://je.lnxyls.cn

defaultdict(list)
来源：http://uk.hnjuh.cn

[U15] Py：高精度计时
来源：http://ht.huixinmuqiang.cn

t = time.perf_counter()
来源：http://sd.521024.cn

[U16] Py：命令行参数解析
来源：http://my.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bp.nszjky.cn

[U17] Py：初始化日志
来源：http://dj.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://br.jctech888.com.cn

[U18] Py：预编译正则
来源：http://yj.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://ep.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://bz.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ja.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://ws.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://rk.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://sf.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://ov.asd995.cn

[U22] Py：矩阵转置
来源：http://es.shxzukj.cn

list(zip(*m))
来源：http://yv.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://ju.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fr.9csxet.cn

[U24] Py：路径操作
来源：http://hl.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ne.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://nj.lnxyls.cn

csv.DictReader(f)
来源：http://lx.hahajie.cn

[U26] Py：并发下载
来源：http://ad.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yl.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://hf.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ho.colortex.cn

[U28] Py：类型别名
来源：http://ef.gzmigu.cn

UserId = int
来源：http://yl.yuexingan06.cn

[U29] Py：属性校验
来源：http://ut.nszjky.cn

@property 与 @x.setter 配合
来源：http://cw.hnjuh.cn

[U30] Py：数据类
来源：http://cv.muxihuayi.cn

@dataclass(slots=True)
来源：http://dw.muxihuayi.cn

[U31] Py：单测
来源：http://bu.bjjhwx.cn

python -m pytest -q
来源：http://wj.haigaiapp.cn

[U32] Py：代码格式化
来源：http://gl.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://yl.asd995.cn

[U33] Py：打包发布
来源：http://ik.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://jp.9csxet.cn

[U34] Py：判断编码
来源：http://hj.521024.cn

chardet.detect(raw)
来源：http://le.lnxyls.cn


<!-- 参考信息 -->