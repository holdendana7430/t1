代发 wailian999

x |= (1 << 3);
来源：http://es.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://rl.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://db.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://pl.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://oi.gzmigu.cn

[S19] C：快速排序
来源：http://fv.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kt.bjjhwx.cn

[S20] C：二分查找
来源：http://sv.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mh.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://iz.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cr.shxzukj.cn

[S22] C：字符串转数字
来源：http://rz.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://os.szsharing.cn

[S23] C：随机数
来源：http://bi.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mk.szsharing.cn

[S24] C：获取本地时间
来源：http://vv.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fi.szsharing.cn

[S25] C：内存拷贝
来源：http://gk.asd995.cn

memcpy(dst, src, n);
来源：http://de.nszjky.cn

[S26] C：内存清零
来源：http://ni.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://tt.9csxet.cn

[S27] C：定义常量
来源：http://ph.9csxet.cn

const double PI = 3.14159;
来源：http://gw.newstarts.cn

[S28] C：静态变量
来源：http://jj.huixinmuqiang.cn

static int counter = 0;
来源：http://be.wgjwhj.cn

[S29] C：变参函数
来源：http://ll.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yc.shxzskj.cn

[S30] C：头文件保护
来源：http://wr.huanxung.cn

#ifndef X_H
来源：http://id.wgjwhj.cn

#define X_H
来源：http://vq.yuntaijiaju.cn

#endif
来源：http://sp.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://mi.hnjuh.cn

#include <iostream>
来源：http://lc.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://th.shxzukj.cn

[S32] C++：字符串
来源：http://wp.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://os.chemitech.net.cn

[S33] C++：vector 增删
来源：http://qq.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ow.shxzukj.cn

[S34] C++：遍历 vector
来源：http://kl.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://do.colortex.cn

[S35] C++：map
来源：http://dz.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fy.shxzskj.cn

[S36] C++：unordered_map
来源：http://jm.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vp.huanxung.cn

[S37] C++：set
来源：http://xw.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ie.shxzskj.cn

[S38] C++：排序
来源：http://bh.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://gy.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://fz.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ys.nszjky.cn

[S40] C++：查找元素
来源：http://ni.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qg.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ej.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cg.521024.cn

[S42] C++：继承与虚函数
来源：http://wf.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://ku.gzmigu.cn

[S43] C++：智能指针
来源：http://ne.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://uw.asd995.cn

[S44] C++：引用传参
来源：http://ew.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://at.panjiajie.cn

[S45] C++：lambda
来源：http://vm.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gq.huanxung.cn

[S46] C++：函数模板
来源：http://bu.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mb.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://jo.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gk.huanxung.cn

[S48] C++：逐行读文件
来源：http://lr.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gv.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://pu.colortex.cn

[S49] C++：写文件
来源：http://ke.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hu.muxihuayi.cn

[S50] C++：格式化数字
来源：http://au.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://si.colortex.cn

[S51] C++：显式类型转换
来源：http://lr.szxytkj.cn

static_cast<double>(a) / b
来源：http://lg.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://rq.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://dn.asd995.cn

[S53] C++：移动语义
来源：http://ro.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://xs.jctech888.com.cn

[S54] C++：异常处理
来源：http://vz.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zj.nszjky.cn

[S55] C++：结构化绑定
来源：http://uf.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://td.jctech888.com.cn

[S56] C++：optional
来源：http://xx.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gz.lnxyls.cn

[S57] C++：编译期常量
来源：http://wf.yuntaijiaju.cn

constexpr int N = 10;
来源：http://mf.hahajie.cn

[S58] C++：命名空间
来源：http://rk.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://kz.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://sm.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://td.521024.cn

[S60] C++：遍历并删除元素
来源：http://ko.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vw.huixiangedu.cn

================================================================================
来源：http://md.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zj.bookmarksfly.cn

================================================================================
来源：http://zj.huanxung.cn

[T01] Kotlin：Hello World
来源：http://dp.hnjuh.cn

println("Hello")
来源：http://fh.lnxyls.cn

[T02] Kotlin：变量
来源：http://mo.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://is.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://mq.szsharing.cn

"值: $b"
来源：http://li.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://cb.nicolike.cn

val n: String? = null;  n?.length
来源：http://fv.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://tx.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sj.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://pt.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yy.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://og.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kl.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://wc.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://lc.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ns.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://kf.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://mb.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ig.muxihuayi.cn

[T11] Kotlin：协程
来源：http://eo.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bx.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://md.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://ny.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://ie.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://lh.bjjhwx.cn

[T14] Kotlin：循环
来源：http://hw.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://qa.yuexingan06.cn

[T15] Kotlin：接口
来源：http://mx.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://bx.panjiajie.cn

[T16] Swift：Hello World
来源：http://rm.chemitech.net.cn

print("Hello")
来源：http://cq.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://vj.asd995.cn

var a = 1;  let b = 2
来源：http://mn.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://fn.9csxet.cn

"值: \(b)"
来源：http://hx.szxytkj.cn

[T19] Swift：可选绑定
来源：http://gn.panjiajie.cn

if let n = opt { print(n) }
来源：http://ht.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://zf.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bc.colortex.cn

[T21] Swift：遍历
来源：http://pn.asd995.cn

for x in a { print(x) }
来源：http://qd.shxzukj.cn

[T22] Swift：字典
来源：http://at.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://do.szsharing.cn

[T23] Swift：函数
来源：http://ie.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eg.shxzskj.cn

[T24] Swift：闭包
来源：http://cz.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kb.jctech888.com.cn

[T25] Swift：结构体
来源：http://yy.521024.cn

struct P { var x: Int }
来源：http://ef.colortex.cn

[T26] Swift：类与重写
来源：http://hb.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://dz.muxihuayi.cn

[T27] Swift：错误处理
来源：http://yw.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://nk.newstarts.cn

[T28] Swift：枚举
来源：http://fs.9csxet.cn

enum Color { case red, green }
来源：http://on.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://yp.szsharing.cn

guard let x = opt else { return }
来源：http://pn.newstarts.cn

[T30] Swift：协议
来源：http://zn.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://gy.muxihuayi.cn

[T31] Lua：Hello World
来源：http://io.bookmarksfly.cn

print("Hello")
来源：http://if.asd995.cn

[T32] Lua：局部变量
来源：http://fj.panjiajie.cn

local a = 1
来源：http://wp.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://zy.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mb.nicolike.cn

[T34] Lua：遍历表
来源：http://al.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://me.bjjhwx.cn

[T35] Lua：字典表
来源：http://ng.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://di.panjiajie.cn

[T36] Lua：函数
来源：http://dq.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://ss.huanxung.cn

[T37] Lua：字符串拼接
来源：http://jp.nszjky.cn

"a" .. "b"
来源：http://qd.asd995.cn

[T38] Lua：条件
来源：http://ik.hnjuh.cn

if x > 0 then print("正") end
来源：http://zm.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://hr.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://cr.yuntaijiaju.cn

[T40] Lua：元表
来源：http://dw.newstarts.cn

setmetatable({}, { __index = base })
来源：http://yw.521024.cn

[T41] Perl：Hello World
来源：http://uu.nicolike.cn

print "Hello\n";
来源：http://jx.hahajie.cn

[T42] Perl：变量类型
来源：http://uq.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xu.hnjuh.cn

[T43] Perl：字符串插值
来源：http://hw.haigaiapp.cn

"值: $a"
来源：http://au.bookmarksfly.cn

[T44] Perl：条件
来源：http://ii.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ov.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://ch.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://my.hahajie.cn

[T46] Perl：哈希操作
来源：http://rh.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wt.hahajie.cn

[T47] Perl：正则捕获
来源：http://yr.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vq.haigaiapp.cn

[T48] Perl：正则替换
来源：http://ca.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://ia.nszjky.cn

[T49] Perl：函数
来源：http://rx.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qw.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://nr.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://th.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://hw.jctech888.com.cn

[T51] Scala：Hello World
来源：http://qe.lnxyls.cn

println("Hello")
来源：http://iq.yuntaijiaju.cn

[T52] Scala：变量
来源：http://cx.shtwfgs.cn

val a = 1;  var b = 2
来源：http://lq.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://sr.muxihuayi.cn

s"值: $b"
来源：http://rv.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://ne.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ep.hahajie.cn

[T55] Scala：集合过滤
来源：http://ao.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wq.nicolike.cn

[T56] Scala：样例类
来源：http://vs.szxytkj.cn

case class User(name: String, age: Int)
来源：http://bu.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://ja.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ys.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://sg.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zp.bookmarksfly.cn

[T59] Scala：循环
来源：http://jo.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://dv.haigaiapp.cn

[T60] Scala：折叠
来源：http://yq.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://da.bjjhwx.cn

================================================================================
来源：http://bo.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zu.bookmarksfly.cn

================================================================================
来源：http://tu.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://cz.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://el.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://rx.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cz.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://cm.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zs.521024.cn

[U04] Py：变量调试打印
来源：http://dl.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gh.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://uv.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://vf.huanxung.cn

[U06] Py：合并两个字典
来源：http://eu.bookmarksfly.cn

{**a, **b}
来源：http://ld.huanxung.cn

[U07] Py：反转字典键值
来源：http://jr.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://av.hahajie.cn

[U08] Py：展平二维列表
来源：http://hb.huanxung.cn

[y for x in nested for y in x]
来源：http://cv.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://qh.hnjuh.cn

max(d, key=d.get)
来源：http://st.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://gh.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aq.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://uq.asd995.cn

(x * 2 for x in arr)
来源：http://vb.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dg.521024.cn

Counter(arr).most_common(3)
来源：http://vl.hnjuh.cn

[U13] Py：固定长度队列
来源：http://dm.lnxyls.cn

deque(maxlen=10)
来源：http://sy.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://nw.gzmigu.cn

defaultdict(list)
来源：http://bk.muxihuayi.cn

[U15] Py：高精度计时
来源：http://jg.muxihuayi.cn

t = time.perf_counter()
来源：http://dk.nicolike.cn

[U16] Py：命令行参数解析
来源：http://by.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ml.nicolike.cn

[U17] Py：初始化日志
来源：http://at.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ju.newstarts.cn

[U18] Py：预编译正则
来源：http://yd.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://bl.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://sd.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lz.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://dn.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://mf.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://cy.haigaiapp.cn

@contextlib.contextmanager
来源：http://ee.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://rs.jctech888.com.cn

list(zip(*m))
来源：http://db.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://ue.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ln.9csxet.cn

[U24] Py：路径操作
来源：http://ot.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ty.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://nr.haigaiapp.cn

csv.DictReader(f)
来源：http://av.haigaiapp.cn

[U26] Py：并发下载
来源：http://rf.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://km.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://yr.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://ym.yuexingan06.cn

[U28] Py：类型别名
来源：http://ao.hahajie.cn

UserId = int
来源：http://vx.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://za.nicolike.cn

@property 与 @x.setter 配合
来源：http://us.asd995.cn

[U30] Py：数据类
来源：http://xz.huixiangedu.cn

@dataclass(slots=True)
来源：http://yb.newstarts.cn

[U31] Py：单测
来源：http://xh.shxzskj.cn

python -m pytest -q
来源：http://oe.lnxyls.cn

[U32] Py：代码格式化
来源：http://hj.hahajie.cn

ruff format . && ruff check --fix .
来源：http://wz.hnjuh.cn

[U33] Py：打包发布
来源：http://vz.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://dq.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://yv.chemitech.net.cn

chardet.detect(raw)
来源：http://po.jctech888.com.cn

[U35] Py：发送邮件
来源：http://ii.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mn.lnxyls.cn

[U36] Py：定时任务
来源：http://du.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://rm.asd995.cn

[U37] Py：读写 Excel
来源：http://po.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wp.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://fp.panjiajie.cn

Path(__file__).resolve().parent
来源：http://as.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://zp.hahajie.cn

sys.stdout.isatty()
来源：http://cu.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://bs.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://dg.szxytkj.cn


<!-- 参考信息 -->