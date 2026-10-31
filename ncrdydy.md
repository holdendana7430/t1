代发 wailian999

x |= (1 << 3);
来源：http://ax.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://lf.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://an.jctech888.com.cn

[S18] C：命令行参数
来源：http://wz.bjjhwx.cn

int main(int argc, char **argv)
来源：http://aw.bjjhwx.cn

[S19] C：快速排序
来源：http://ew.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xn.hahajie.cn

[S20] C：二分查找
来源：http://zs.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kt.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://rc.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xb.muxihuayi.cn

[S22] C：字符串转数字
来源：http://nm.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oy.huanxung.cn

[S23] C：随机数
来源：http://nz.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ub.huanxung.cn

[S24] C：获取本地时间
来源：http://cp.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kp.gzmigu.cn

[S25] C：内存拷贝
来源：http://hk.shxzskj.cn

memcpy(dst, src, n);
来源：http://re.muxihuayi.cn

[S26] C：内存清零
来源：http://fx.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://xv.shxzukj.cn

[S27] C：定义常量
来源：http://qm.shxzskj.cn

const double PI = 3.14159;
来源：http://pw.521024.cn

[S28] C：静态变量
来源：http://kp.huixiangedu.cn

static int counter = 0;
来源：http://xc.shtwfgs.cn

[S29] C：变参函数
来源：http://no.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ic.shxzukj.cn

[S30] C：头文件保护
来源：http://zy.panjiajie.cn

#ifndef X_H
来源：http://tx.nszjky.cn

#define X_H
来源：http://rt.szxytkj.cn

#endif
来源：http://lo.shxzskj.cn

[S31] C++：Hello World
来源：http://cz.gzmigu.cn

#include <iostream>
来源：http://qv.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://cb.nicolike.cn

[S32] C++：字符串
来源：http://ey.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://km.nszjky.cn

[S33] C++：vector 增删
来源：http://ip.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hi.szsharing.cn

[S34] C++：遍历 vector
来源：http://dl.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://nk.shtwfgs.cn

[S35] C++：map
来源：http://vr.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fz.panjiajie.cn

[S36] C++：unordered_map
来源：http://cv.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://di.yuexingan06.cn

[S37] C++：set
来源：http://ns.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uc.hahajie.cn

[S38] C++：排序
来源：http://vh.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://wp.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://cl.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vb.bookmarksfly.cn

[S40] C++：查找元素
来源：http://ue.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zb.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://yr.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yd.colortex.cn

[S42] C++：继承与虚函数
来源：http://ld.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://tw.muxihuayi.cn

[S43] C++：智能指针
来源：http://qp.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ot.panjiajie.cn

[S44] C++：引用传参
来源：http://lk.newstarts.cn

void inc(int &x) { ++x; }
来源：http://ea.bjjhwx.cn

[S45] C++：lambda
来源：http://yt.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vb.hahajie.cn

[S46] C++：函数模板
来源：http://wn.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fx.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://wh.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://or.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://pq.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eb.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ab.jianghongdianzi.cn

[S49] C++：写文件
来源：http://lj.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://li.lnxyls.cn

[S50] C++：格式化数字
来源：http://ic.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cn.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://yj.hnjuh.cn

static_cast<double>(a) / b
来源：http://gu.asd995.cn

[S52] C++：const 与 noexcept
来源：http://wl.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://lh.asd995.cn

[S53] C++：移动语义
来源：http://nq.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://bp.wgjwhj.cn

[S54] C++：异常处理
来源：http://to.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gh.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://be.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bo.newstarts.cn

[S56] C++：optional
来源：http://xp.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fb.panjiajie.cn

[S57] C++：编译期常量
来源：http://kk.hahajie.cn

constexpr int N = 10;
来源：http://da.wgjwhj.cn

[S58] C++：命名空间
来源：http://iw.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://gt.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://jt.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xk.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ot.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://go.yuexingan06.cn

================================================================================
来源：http://fp.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://td.szsharing.cn

================================================================================
来源：http://ob.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://xf.asd995.cn

println("Hello")
来源：http://jr.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://yk.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ka.asd995.cn

[T03] Kotlin：字符串模板
来源：http://nj.jianghongdianzi.cn

"值: $b"
来源：http://tf.colortex.cn

[T04] Kotlin：空安全
来源：http://io.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://no.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://tx.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uh.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://lw.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dp.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://iw.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sf.colortex.cn

[T08] Kotlin：数据类
来源：http://tk.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://ak.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://tb.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://mb.hahajie.cn

[T10] Kotlin：默认参数
来源：http://fq.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wz.wgjwhj.cn

[T11] Kotlin：协程
来源：http://az.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yr.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://eg.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://po.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://lz.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://dn.newstarts.cn

[T14] Kotlin：循环
来源：http://jb.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://bh.huixiangedu.cn

[T15] Kotlin：接口
来源：http://kg.nicolike.cn

interface Shape { fun area(): Double }
来源：http://ay.nicolike.cn

[T16] Swift：Hello World
来源：http://nk.yuntaijiaju.cn

print("Hello")
来源：http://fn.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://yh.jctech888.com.cn

var a = 1;  let b = 2
来源：http://ku.hahajie.cn

[T18] Swift：字符串插值
来源：http://gt.yuntaijiaju.cn

"值: \(b)"
来源：http://pn.huanxung.cn

[T19] Swift：可选绑定
来源：http://iy.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://uy.jctech888.com.cn

[T20] Swift：数组操作
来源：http://je.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fe.szsharing.cn

[T21] Swift：遍历
来源：http://jk.haigaiapp.cn

for x in a { print(x) }
来源：http://nb.asd995.cn

[T22] Swift：字典
来源：http://fe.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vm.jctech888.com.cn

[T23] Swift：函数
来源：http://pg.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fw.wgjwhj.cn

[T24] Swift：闭包
来源：http://ye.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ps.yuexingan06.cn

[T25] Swift：结构体
来源：http://jt.lnxyls.cn

struct P { var x: Int }
来源：http://ns.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://fn.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://xd.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://na.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://am.nszjky.cn

[T28] Swift：枚举
来源：http://qk.huixiangedu.cn

enum Color { case red, green }
来源：http://ce.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://hc.yuexingan06.cn

guard let x = opt else { return }
来源：http://ws.hahajie.cn

[T30] Swift：协议
来源：http://ny.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://lt.panjiajie.cn

[T31] Lua：Hello World
来源：http://uk.jianghongdianzi.cn

print("Hello")
来源：http://at.newstarts.cn

[T32] Lua：局部变量
来源：http://ll.haigaiapp.cn

local a = 1
来源：http://bd.gzmigu.cn

[T33] Lua：表（数组）
来源：http://nd.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ai.shxzskj.cn

[T34] Lua：遍历表
来源：http://aj.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vg.panjiajie.cn

[T35] Lua：字典表
来源：http://uu.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://uo.shxzskj.cn

[T36] Lua：函数
来源：http://ty.asd995.cn

function add(a, b) return a + b end
来源：http://ar.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://pr.szsharing.cn

"a" .. "b"
来源：http://nb.szsharing.cn

[T38] Lua：条件
来源：http://we.gzmigu.cn

if x > 0 then print("正") end
来源：http://nb.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ge.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://xn.9csxet.cn

[T40] Lua：元表
来源：http://cy.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://yi.newstarts.cn

[T41] Perl：Hello World
来源：http://tj.haigaiapp.cn

print "Hello\n";
来源：http://gc.wgjwhj.cn

[T42] Perl：变量类型
来源：http://aj.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wq.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://hs.gzmigu.cn

"值: $a"
来源：http://kh.lnxyls.cn

[T44] Perl：条件
来源：http://nt.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://jz.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://xn.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://xy.panjiajie.cn

[T46] Perl：哈希操作
来源：http://zk.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ph.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://ha.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wq.bjjhwx.cn

[T48] Perl：正则替换
来源：http://xz.huanxung.cn

$s =~ s/old/new/g;
来源：http://hm.shxzskj.cn

[T49] Perl：函数
来源：http://wx.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ws.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://ev.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xq.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://um.hnjuh.cn

[T51] Scala：Hello World
来源：http://po.chemitech.net.cn

println("Hello")
来源：http://bo.yuexingan06.cn

[T52] Scala：变量
来源：http://jn.hahajie.cn

val a = 1;  var b = 2
来源：http://zq.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://ko.yuntaijiaju.cn

s"值: $b"
来源：http://ph.yuexingan06.cn

[T54] Scala：集合映射
来源：http://ep.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://pg.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://pb.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wk.szsharing.cn

[T56] Scala：样例类
来源：http://rt.asd995.cn

case class User(name: String, age: Int)
来源：http://ku.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://nm.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uj.shxzskj.cn

[T58] Scala：函数定义
来源：http://ph.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fv.521024.cn

[T59] Scala：循环
来源：http://se.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://jq.szxytkj.cn

[T60] Scala：折叠
来源：http://js.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tp.jianghongdianzi.cn

================================================================================
来源：http://eq.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://np.gzmigu.cn

================================================================================
来源：http://rz.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://yj.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cu.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://sy.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ol.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://us.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ns.gzmigu.cn

[U04] Py：变量调试打印
来源：http://lh.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kx.asd995.cn

[U05] Py：列表去重且保序
来源：http://ut.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ph.newstarts.cn

[U06] Py：合并两个字典
来源：http://xb.newstarts.cn

{**a, **b}
来源：http://kv.lnxyls.cn

[U07] Py：反转字典键值
来源：http://wi.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://ko.521024.cn

[U08] Py：展平二维列表
来源：http://ou.newstarts.cn

[y for x in nested for y in x]
来源：http://hl.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://ie.hahajie.cn

max(d, key=d.get)
来源：http://yk.szxytkj.cn

[U10] Py：按值排序字典
来源：http://wl.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iy.gzmigu.cn

[U11] Py：生成器表达式
来源：http://cd.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://wg.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xy.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://pi.hnjuh.cn

[U13] Py：固定长度队列
来源：http://mb.newstarts.cn

deque(maxlen=10)
来源：http://bq.szsharing.cn

[U14] Py：分组收集到列表
来源：http://od.haigaiapp.cn

defaultdict(list)
来源：http://ff.muxihuayi.cn

[U15] Py：高精度计时
来源：http://sv.huanxung.cn

t = time.perf_counter()
来源：http://et.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://xi.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jf.huixiangedu.cn

[U17] Py：初始化日志
来源：http://cg.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://hw.huixiangedu.cn

[U18] Py：预编译正则
来源：http://mk.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://ot.nicolike.cn

[U19] Py：正则替换带回调
来源：http://wz.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dj.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://jx.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://la.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://gh.521024.cn

@contextlib.contextmanager
来源：http://xf.szxytkj.cn

[U22] Py：矩阵转置
来源：http://iy.hahajie.cn

list(zip(*m))
来源：http://th.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://ou.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bb.huanxung.cn

[U24] Py：路径操作
来源：http://gy.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dk.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://co.huixinmuqiang.cn

csv.DictReader(f)
来源：http://lj.shxzskj.cn

[U26] Py：并发下载
来源：http://ya.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://de.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://oa.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://cc.yuexingan06.cn

[U28] Py：类型别名
来源：http://ti.huanxung.cn

UserId = int
来源：http://gx.panjiajie.cn

[U29] Py：属性校验
来源：http://wq.nszjky.cn

@property 与 @x.setter 配合
来源：http://nv.wgjwhj.cn

[U30] Py：数据类
来源：http://wu.jctech888.com.cn

@dataclass(slots=True)
来源：http://vr.muxihuayi.cn

[U31] Py：单测
来源：http://ai.shxzukj.cn

python -m pytest -q
来源：http://tv.szsharing.cn

[U32] Py：代码格式化
来源：http://oq.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://rb.bookmarksfly.cn

[U33] Py：打包发布
来源：http://on.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://ul.shxzskj.cn

[U34] Py：判断编码
来源：http://jr.szsharing.cn

chardet.detect(raw)
来源：http://ww.yuexingan06.cn

[U35] Py：发送邮件
来源：http://we.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eu.jctech888.com.cn

[U36] Py：定时任务
来源：http://sz.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://et.newstarts.cn

[U37] Py：读写 Excel
来源：http://so.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rx.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://vc.szxytkj.cn

Path(__file__).resolve().parent
来源：http://cg.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://nb.hahajie.cn

sys.stdout.isatty()
来源：http://qg.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ej.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://pz.chemitech.net.cn


<!-- 参考信息 -->