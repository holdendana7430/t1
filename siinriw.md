代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nn.szxytkj.cn

[S13] C：宏定义
来源：http://fq.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bs.bjjhwx.cn

[S14] C：枚举
来源：http://hu.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://gt.huanxung.cn

[S15] C：类型转换
来源：http://lf.shtwfgs.cn

(double) a / b
来源：http://cb.chemitech.net.cn

[S16] C：位操作置位
来源：http://vn.hnjuh.cn

x |= (1 << 3);
来源：http://zd.colortex.cn

[S17] C：安全拼接字符串
来源：http://mb.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qt.haigaiapp.cn

[S18] C：命令行参数
来源：http://kk.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://dv.panjiajie.cn

[S19] C：快速排序
来源：http://rq.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ul.bookmarksfly.cn

[S20] C：二分查找
来源：http://mf.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fj.muxihuayi.cn

[S21] C：字符类别判断
来源：http://yb.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bx.gzmigu.cn

[S22] C：字符串转数字
来源：http://lj.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gi.gzmigu.cn

[S23] C：随机数
来源：http://rx.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ab.hahajie.cn

[S24] C：获取本地时间
来源：http://jm.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://he.asd995.cn

[S25] C：内存拷贝
来源：http://cq.huanxung.cn

memcpy(dst, src, n);
来源：http://mb.panjiajie.cn

[S26] C：内存清零
来源：http://dj.colortex.cn

memset(a, 0, sizeof a);
来源：http://of.bookmarksfly.cn

[S27] C：定义常量
来源：http://ny.colortex.cn

const double PI = 3.14159;
来源：http://to.newstarts.cn

[S28] C：静态变量
来源：http://ym.yuexingan06.cn

static int counter = 0;
来源：http://ff.yuexingan06.cn

[S29] C：变参函数
来源：http://bk.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://za.panjiajie.cn

[S30] C：头文件保护
来源：http://fc.huixinmuqiang.cn

#ifndef X_H
来源：http://jg.jctech888.com.cn

#define X_H
来源：http://ol.yuntaijiaju.cn

#endif
来源：http://mt.521024.cn

[S31] C++：Hello World
来源：http://jw.9csxet.cn

#include <iostream>
来源：http://fq.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fp.szsharing.cn

[S32] C++：字符串
来源：http://kp.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://bz.hnjuh.cn

[S33] C++：vector 增删
来源：http://do.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ex.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://ch.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://vs.hahajie.cn

[S35] C++：map
来源：http://ig.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mw.huixiangedu.cn

[S36] C++：unordered_map
来源：http://xy.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.huixiangedu.cn

[S37] C++：set
来源：http://mz.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mt.muxihuayi.cn

[S38] C++：排序
来源：http://wa.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://op.colortex.cn

[S39] C++：自定义比较器排序
来源：http://gz.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sl.panjiajie.cn

[S40] C++：查找元素
来源：http://cl.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vp.hnjuh.cn

[S41] C++：类与构造函数
来源：http://gf.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ko.nszjky.cn

[S42] C++：继承与虚函数
来源：http://nj.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://fh.jctech888.com.cn

[S43] C++：智能指针
来源：http://dx.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://vl.nicolike.cn

[S44] C++：引用传参
来源：http://jq.nszjky.cn

void inc(int &x) { ++x; }
来源：http://wi.yuntaijiaju.cn

[S45] C++：lambda
来源：http://tn.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://td.szsharing.cn

[S46] C++：函数模板
来源：http://db.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kl.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://ew.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ov.colortex.cn

[S48] C++：逐行读文件
来源：http://il.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zw.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://if.szxytkj.cn

[S49] C++：写文件
来源：http://vf.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hv.nicolike.cn

[S50] C++：格式化数字
来源：http://dw.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kr.hahajie.cn

[S51] C++：显式类型转换
来源：http://tc.lnxyls.cn

static_cast<double>(a) / b
来源：http://dt.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://my.521024.cn

int size() const noexcept { return n_; }
来源：http://sh.newstarts.cn

[S53] C++：移动语义
来源：http://wc.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://of.panjiajie.cn

[S54] C++：异常处理
来源：http://og.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ss.panjiajie.cn

[S55] C++：结构化绑定
来源：http://pr.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lo.9csxet.cn

[S56] C++：optional
来源：http://xi.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nf.colortex.cn

[S57] C++：编译期常量
来源：http://qk.colortex.cn

constexpr int N = 10;
来源：http://pu.gzmigu.cn

[S58] C++：命名空间
来源：http://yv.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://ym.nicolike.cn

[S59] C++：静态断言
来源：http://ad.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ou.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://ak.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://je.bjjhwx.cn

================================================================================
来源：http://cl.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mx.nicolike.cn

================================================================================
来源：http://qx.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://hy.hahajie.cn

println("Hello")
来源：http://io.yuexingan06.cn

[T02] Kotlin：变量
来源：http://dn.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fw.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://hf.panjiajie.cn

"值: $b"
来源：http://hi.shxzskj.cn

[T04] Kotlin：空安全
来源：http://ta.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://da.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://na.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ju.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://qc.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://at.colortex.cn

[T07] Kotlin：集合过滤
来源：http://yu.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ru.szxytkj.cn

[T08] Kotlin：数据类
来源：http://tf.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://xl.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://ml.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ld.szsharing.cn

[T10] Kotlin：默认参数
来源：http://cj.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ly.bjjhwx.cn

[T11] Kotlin：协程
来源：http://vr.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://va.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://yb.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://df.asd995.cn

[T13] Kotlin：只读 Map
来源：http://tg.asd995.cn

val m = mapOf("a" to 1)
来源：http://bc.shxzskj.cn

[T14] Kotlin：循环
来源：http://ol.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://rr.wgjwhj.cn

[T15] Kotlin：接口
来源：http://sa.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://rw.yuexingan06.cn

[T16] Swift：Hello World
来源：http://wz.yuexingan06.cn

print("Hello")
来源：http://ek.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://ht.colortex.cn

var a = 1;  let b = 2
来源：http://wm.szxytkj.cn

[T18] Swift：字符串插值
来源：http://an.haigaiapp.cn

"值: \(b)"
来源：http://vp.szxytkj.cn

[T19] Swift：可选绑定
来源：http://qb.huanxung.cn

if let n = opt { print(n) }
来源：http://dr.huanxung.cn

[T20] Swift：数组操作
来源：http://ma.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gp.shxzskj.cn

[T21] Swift：遍历
来源：http://qe.521024.cn

for x in a { print(x) }
来源：http://hf.hahajie.cn

[T22] Swift：字典
来源：http://jn.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dr.jctech888.com.cn

[T23] Swift：函数
来源：http://kq.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uw.shxzskj.cn

[T24] Swift：闭包
来源：http://wq.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cj.9csxet.cn

[T25] Swift：结构体
来源：http://pa.hnjuh.cn

struct P { var x: Int }
来源：http://ou.9csxet.cn

[T26] Swift：类与重写
来源：http://lo.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://pt.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://qq.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://sj.521024.cn

[T28] Swift：枚举
来源：http://vt.asd995.cn

enum Color { case red, green }
来源：http://ui.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://cy.shxzukj.cn

guard let x = opt else { return }
来源：http://ry.shxzukj.cn

[T30] Swift：协议
来源：http://pi.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ix.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://no.asd995.cn

print("Hello")
来源：http://qf.hahajie.cn

[T32] Lua：局部变量
来源：http://th.jctech888.com.cn

local a = 1
来源：http://tg.gzmigu.cn

[T33] Lua：表（数组）
来源：http://dk.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ve.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ca.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ih.hahajie.cn

[T35] Lua：字典表
来源：http://it.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://pj.huixinmuqiang.cn

[T36] Lua：函数
来源：http://rm.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://vf.521024.cn

[T37] Lua：字符串拼接
来源：http://ga.yuexingan06.cn

"a" .. "b"
来源：http://ui.asd995.cn

[T38] Lua：条件
来源：http://zn.jctech888.com.cn

if x > 0 then print("正") end
来源：http://dz.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://al.huixiangedu.cn

string.find(s, "%d+")
来源：http://ok.szsharing.cn

[T40] Lua：元表
来源：http://iq.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://np.521024.cn

[T41] Perl：Hello World
来源：http://uh.yuntaijiaju.cn

print "Hello\n";
来源：http://jf.lnxyls.cn

[T42] Perl：变量类型
来源：http://fm.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kv.9csxet.cn

[T43] Perl：字符串插值
来源：http://sy.nszjky.cn

"值: $a"
来源：http://ed.9csxet.cn

[T44] Perl：条件
来源：http://nw.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://cw.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://zi.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://ph.lnxyls.cn

[T46] Perl：哈希操作
来源：http://cz.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ct.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://xj.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jq.lnxyls.cn

[T48] Perl：正则替换
来源：http://or.asd995.cn

$s =~ s/old/new/g;
来源：http://fm.haigaiapp.cn

[T49] Perl：函数
来源：http://qk.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lu.newstarts.cn

[T50] Perl：逐行读文件
来源：http://nt.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mk.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://nk.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ka.bookmarksfly.cn

println("Hello")
来源：http://pe.asd995.cn

[T52] Scala：变量
来源：http://fq.shtwfgs.cn

val a = 1;  var b = 2
来源：http://zv.hahajie.cn

[T53] Scala：字符串插值
来源：http://sx.9csxet.cn

s"值: $b"
来源：http://rj.hnjuh.cn

[T54] Scala：集合映射
来源：http://nn.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://yc.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://vq.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://od.lnxyls.cn

[T56] Scala：样例类
来源：http://bf.hahajie.cn

case class User(name: String, age: Int)
来源：http://kg.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ec.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bf.colortex.cn

[T58] Scala：函数定义
来源：http://xy.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bn.shtwfgs.cn

[T59] Scala：循环
来源：http://ja.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://ok.muxihuayi.cn

[T60] Scala：折叠
来源：http://pi.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jm.bookmarksfly.cn

================================================================================
来源：http://lk.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dl.gzmigu.cn

================================================================================
来源：http://iy.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://kf.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xe.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://zj.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fn.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://fv.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xj.shxzukj.cn

[U04] Py：变量调试打印
来源：http://xq.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.521024.cn

[U05] Py：列表去重且保序
来源：http://hg.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://vt.colortex.cn

[U06] Py：合并两个字典
来源：http://rh.huixiangedu.cn

{**a, **b}
来源：http://kx.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://pc.9csxet.cn

{v: k for k, v in d.items()}
来源：http://yz.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://kf.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://wk.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://jy.szsharing.cn

max(d, key=d.get)
来源：http://cs.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://lf.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cz.521024.cn

[U11] Py：生成器表达式
来源：http://uo.newstarts.cn

(x * 2 for x in arr)
来源：http://px.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lh.huanxung.cn

Counter(arr).most_common(3)
来源：http://le.hahajie.cn

[U13] Py：固定长度队列
来源：http://bk.521024.cn

deque(maxlen=10)
来源：http://qp.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://tu.muxihuayi.cn

defaultdict(list)
来源：http://qd.szxytkj.cn

[U15] Py：高精度计时
来源：http://yt.yuntaijiaju.cn

t = time.perf_counter()
来源：http://kh.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://pj.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cj.lnxyls.cn

[U17] Py：初始化日志
来源：http://ls.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://hp.shxzukj.cn

[U18] Py：预编译正则
来源：http://du.szsharing.cn

pat = re.compile(r"\d+")
来源：http://lf.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://tb.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pa.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://cq.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://kv.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://lp.asd995.cn

@contextlib.contextmanager
来源：http://mt.nszjky.cn

[U22] Py：矩阵转置
来源：http://sn.nicolike.cn

list(zip(*m))
来源：http://dt.521024.cn

[U23] Py：分块读取大文件
来源：http://se.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zz.szsharing.cn

[U24] Py：路径操作
来源：http://cv.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xi.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://ir.9csxet.cn

csv.DictReader(f)
来源：http://xp.huanxung.cn

[U26] Py：并发下载
来源：http://ie.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kv.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://tp.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://og.shxzukj.cn

[U28] Py：类型别名
来源：http://xi.nicolike.cn

UserId = int
来源：http://qr.huixiangedu.cn

[U29] Py：属性校验
来源：http://hc.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://ds.szsharing.cn

[U30] Py：数据类
来源：http://xk.panjiajie.cn

@dataclass(slots=True)
来源：http://xg.szsharing.cn

[U31] Py：单测
来源：http://on.newstarts.cn

python -m pytest -q
来源：http://zp.bjjhwx.cn

[U32] Py：代码格式化
来源：http://qm.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://pb.chemitech.net.cn

[U33] Py：打包发布
来源：http://ta.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ci.hahajie.cn

[U34] Py：判断编码
来源：http://ok.colortex.cn

chardet.detect(raw)
来源：http://im.shxzskj.cn

[U35] Py：发送邮件
来源：http://kj.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fc.yuexingan06.cn

[U36] Py：定时任务
来源：http://re.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://cs.9csxet.cn


<!-- 参考信息 -->