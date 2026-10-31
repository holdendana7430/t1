代发 wailian999

x |= (1 << 3);
来源：http://on.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://ap.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zs.wgjwhj.cn

[S18] C：命令行参数
来源：http://nb.lnxyls.cn

int main(int argc, char **argv)
来源：http://vo.lnxyls.cn

[S19] C：快速排序
来源：http://bf.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://id.lnxyls.cn

[S20] C：二分查找
来源：http://bh.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gv.nicolike.cn

[S21] C：字符类别判断
来源：http://ga.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pl.newstarts.cn

[S22] C：字符串转数字
来源：http://ho.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vs.wgjwhj.cn

[S23] C：随机数
来源：http://kl.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kt.panjiajie.cn

[S24] C：获取本地时间
来源：http://zz.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ki.521024.cn

[S25] C：内存拷贝
来源：http://oi.jctech888.com.cn

memcpy(dst, src, n);
来源：http://jt.hahajie.cn

[S26] C：内存清零
来源：http://ok.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://hi.chemitech.net.cn

[S27] C：定义常量
来源：http://vb.shxzskj.cn

const double PI = 3.14159;
来源：http://cz.huixinmuqiang.cn

[S28] C：静态变量
来源：http://qd.chemitech.net.cn

static int counter = 0;
来源：http://aw.haigaiapp.cn

[S29] C：变参函数
来源：http://dd.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hn.shxzukj.cn

[S30] C：头文件保护
来源：http://vg.bookmarksfly.cn

#ifndef X_H
来源：http://fl.hahajie.cn

#define X_H
来源：http://bx.lnxyls.cn

#endif
来源：http://dj.szxytkj.cn

[S31] C++：Hello World
来源：http://wk.yuexingan06.cn

#include <iostream>
来源：http://hy.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://dc.szsharing.cn

[S32] C++：字符串
来源：http://yw.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://if.szsharing.cn

[S33] C++：vector 增删
来源：http://ox.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pe.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://af.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://bh.hahajie.cn

[S35] C++：map
来源：http://eg.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mc.muxihuayi.cn

[S36] C++：unordered_map
来源：http://rr.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wh.shxzukj.cn

[S37] C++：set
来源：http://vy.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yh.gzmigu.cn

[S38] C++：排序
来源：http://dp.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://sa.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://qa.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yn.panjiajie.cn

[S40] C++：查找元素
来源：http://ud.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lk.hahajie.cn

[S41] C++：类与构造函数
来源：http://dp.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pz.521024.cn

[S42] C++：继承与虚函数
来源：http://ld.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://kr.shtwfgs.cn

[S43] C++：智能指针
来源：http://eq.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://tv.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://jc.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ne.shxzskj.cn

[S45] C++：lambda
来源：http://xj.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ld.asd995.cn

[S46] C++：函数模板
来源：http://ov.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://km.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://en.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sx.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://qa.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://np.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://vi.newstarts.cn

[S49] C++：写文件
来源：http://xj.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ch.9csxet.cn

[S50] C++：格式化数字
来源：http://pb.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nh.nicolike.cn

[S51] C++：显式类型转换
来源：http://ml.shxzukj.cn

static_cast<double>(a) / b
来源：http://hl.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://zo.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://ui.hahajie.cn

[S53] C++：移动语义
来源：http://bn.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://go.chemitech.net.cn

[S54] C++：异常处理
来源：http://wh.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ko.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://dm.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ci.yuntaijiaju.cn

[S56] C++：optional
来源：http://oi.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lr.shxzskj.cn

[S57] C++：编译期常量
来源：http://ay.huixinmuqiang.cn

constexpr int N = 10;
来源：http://af.szxytkj.cn

[S58] C++：命名空间
来源：http://az.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://cf.wgjwhj.cn

[S59] C++：静态断言
来源：http://bf.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zi.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://dv.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vr.bjjhwx.cn

================================================================================
来源：http://qy.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xm.wgjwhj.cn

================================================================================
来源：http://ls.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://mb.jctech888.com.cn

println("Hello")
来源：http://vd.jctech888.com.cn

[T02] Kotlin：变量
来源：http://cv.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fg.521024.cn

[T03] Kotlin：字符串模板
来源：http://gm.hahajie.cn

"值: $b"
来源：http://bk.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://de.shxzskj.cn

val n: String? = null;  n?.length
来源：http://lf.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://dj.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cq.szsharing.cn

[T06] Kotlin：集合映射
来源：http://ct.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ym.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://lu.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mq.521024.cn

[T08] Kotlin：数据类
来源：http://yp.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://un.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://uc.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://ak.huanxung.cn

[T10] Kotlin：默认参数
来源：http://yr.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ik.nicolike.cn

[T11] Kotlin：协程
来源：http://ei.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fq.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://yz.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://nd.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://ql.asd995.cn

val m = mapOf("a" to 1)
来源：http://vr.asd995.cn

[T14] Kotlin：循环
来源：http://bl.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://es.panjiajie.cn

[T15] Kotlin：接口
来源：http://pg.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://va.shxzskj.cn

[T16] Swift：Hello World
来源：http://io.hnjuh.cn

print("Hello")
来源：http://xt.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://at.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://le.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://zs.nszjky.cn

"值: \(b)"
来源：http://li.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://tw.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://ln.asd995.cn

[T20] Swift：数组操作
来源：http://uh.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sy.haigaiapp.cn

[T21] Swift：遍历
来源：http://eq.bjjhwx.cn

for x in a { print(x) }
来源：http://jl.haigaiapp.cn

[T22] Swift：字典
来源：http://oq.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xf.9csxet.cn

[T23] Swift：函数
来源：http://kv.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zz.9csxet.cn

[T24] Swift：闭包
来源：http://ev.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tm.asd995.cn

[T25] Swift：结构体
来源：http://pb.asd995.cn

struct P { var x: Int }
来源：http://rd.shtwfgs.cn

[T26] Swift：类与重写
来源：http://ts.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://xg.muxihuayi.cn

[T27] Swift：错误处理
来源：http://lk.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://qk.szxytkj.cn

[T28] Swift：枚举
来源：http://az.jctech888.com.cn

enum Color { case red, green }
来源：http://uu.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://fa.bjjhwx.cn

guard let x = opt else { return }
来源：http://sq.haigaiapp.cn

[T30] Swift：协议
来源：http://up.asd995.cn

protocol Shape { func area() -> Double }
来源：http://qr.shtwfgs.cn

[T31] Lua：Hello World
来源：http://fq.asd995.cn

print("Hello")
来源：http://qa.shtwfgs.cn

[T32] Lua：局部变量
来源：http://ci.muxihuayi.cn

local a = 1
来源：http://da.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://qt.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fn.bjjhwx.cn

[T34] Lua：遍历表
来源：http://wf.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jy.hahajie.cn

[T35] Lua：字典表
来源：http://js.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://up.szxytkj.cn

[T36] Lua：函数
来源：http://en.chemitech.net.cn

function add(a, b) return a + b end
来源：http://wv.szsharing.cn

[T37] Lua：字符串拼接
来源：http://kt.chemitech.net.cn

"a" .. "b"
来源：http://tv.jianghongdianzi.cn

[T38] Lua：条件
来源：http://ya.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://zq.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://ac.asd995.cn

string.find(s, "%d+")
来源：http://os.hahajie.cn

[T40] Lua：元表
来源：http://ha.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://gn.lnxyls.cn

[T41] Perl：Hello World
来源：http://vk.bjjhwx.cn

print "Hello\n";
来源：http://mm.colortex.cn

[T42] Perl：变量类型
来源：http://ea.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yi.huanxung.cn

[T43] Perl：字符串插值
来源：http://um.jianghongdianzi.cn

"值: $a"
来源：http://ia.newstarts.cn

[T44] Perl：条件
来源：http://vh.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://sb.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://bq.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://zu.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://xw.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lu.nicolike.cn

[T47] Perl：正则捕获
来源：http://rv.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pr.lnxyls.cn

[T48] Perl：正则替换
来源：http://gq.asd995.cn

$s =~ s/old/new/g;
来源：http://te.chemitech.net.cn

[T49] Perl：函数
来源：http://jo.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vp.nszjky.cn

[T50] Perl：逐行读文件
来源：http://lo.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mt.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://cv.newstarts.cn

[T51] Scala：Hello World
来源：http://lu.asd995.cn

println("Hello")
来源：http://qn.nszjky.cn

[T52] Scala：变量
来源：http://zj.colortex.cn

val a = 1;  var b = 2
来源：http://wf.hahajie.cn

[T53] Scala：字符串插值
来源：http://ym.jctech888.com.cn

s"值: $b"
来源：http://nx.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://hn.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://ba.colortex.cn

[T55] Scala：集合过滤
来源：http://wx.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vt.wgjwhj.cn

[T56] Scala：样例类
来源：http://rd.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://tn.shxzskj.cn

[T57] Scala：模式匹配
来源：http://se.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://td.wgjwhj.cn

[T58] Scala：函数定义
来源：http://ad.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ge.bookmarksfly.cn

[T59] Scala：循环
来源：http://wz.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://fq.szxytkj.cn

[T60] Scala：折叠
来源：http://uy.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hh.huixiangedu.cn

================================================================================
来源：http://tm.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qc.yuntaijiaju.cn

================================================================================
来源：http://hp.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://kq.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://is.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://iv.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://im.colortex.cn

[U03] Py：加载 .env 配置
来源：http://cr.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://df.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://ww.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rw.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://ux.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://aj.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://iz.bjjhwx.cn

{**a, **b}
来源：http://tu.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://zo.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://rl.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://hg.nicolike.cn

[y for x in nested for y in x]
来源：http://qp.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://hd.9csxet.cn

max(d, key=d.get)
来源：http://kn.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://af.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uu.nszjky.cn

[U11] Py：生成器表达式
来源：http://ov.nszjky.cn

(x * 2 for x in arr)
来源：http://jp.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tc.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://lw.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://wf.shtwfgs.cn

deque(maxlen=10)
来源：http://be.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://ca.gzmigu.cn

defaultdict(list)
来源：http://fx.hnjuh.cn

[U15] Py：高精度计时
来源：http://ow.shxzukj.cn

t = time.perf_counter()
来源：http://yx.szsharing.cn

[U16] Py：命令行参数解析
来源：http://sr.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://md.hnjuh.cn

[U17] Py：初始化日志
来源：http://tj.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://mh.shtwfgs.cn

[U18] Py：预编译正则
来源：http://bh.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://oh.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ci.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://oa.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://dg.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://br.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://kv.nszjky.cn

[U22] Py：矩阵转置
来源：http://dr.huanxung.cn

list(zip(*m))
来源：http://fr.asd995.cn

[U23] Py：分块读取大文件
来源：http://xo.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ss.yuexingan06.cn

[U24] Py：路径操作
来源：http://in.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vv.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://md.nszjky.cn

csv.DictReader(f)
来源：http://nu.hnjuh.cn

[U26] Py：并发下载
来源：http://rj.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ah.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://fu.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://pl.newstarts.cn

[U28] Py：类型别名
来源：http://ja.nicolike.cn

UserId = int
来源：http://ld.chemitech.net.cn

[U29] Py：属性校验
来源：http://nz.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://ds.shxzukj.cn

[U30] Py：数据类
来源：http://gk.shtwfgs.cn

@dataclass(slots=True)
来源：http://kz.gzmigu.cn

[U31] Py：单测
来源：http://tt.9csxet.cn

python -m pytest -q
来源：http://bm.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://dq.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://fl.chemitech.net.cn

[U33] Py：打包发布
来源：http://xe.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://jz.haigaiapp.cn

[U34] Py：判断编码
来源：http://nj.huanxung.cn

chardet.detect(raw)
来源：http://ls.shxzskj.cn

[U35] Py：发送邮件
来源：http://pv.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qw.newstarts.cn

[U36] Py：定时任务
来源：http://lp.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://pl.gzmigu.cn

[U37] Py：读写 Excel
来源：http://xb.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uo.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://lw.shxzukj.cn

Path(__file__).resolve().parent
来源：http://nv.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://ax.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ys.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://jm.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://gf.gzmigu.cn


<!-- 参考信息 -->