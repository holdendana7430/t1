代发 wailian999

x |= (1 << 3);
来源：http://rk.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://qp.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fa.muxihuayi.cn

[S18] C：命令行参数
来源：http://ex.wgjwhj.cn

int main(int argc, char **argv)
来源：http://tb.newstarts.cn

[S19] C：快速排序
来源：http://wj.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ar.nszjky.cn

[S20] C：二分查找
来源：http://mv.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://of.gzmigu.cn

[S21] C：字符类别判断
来源：http://ub.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vr.521024.cn

[S22] C：字符串转数字
来源：http://mp.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gc.yuntaijiaju.cn

[S23] C：随机数
来源：http://pt.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yb.szxytkj.cn

[S24] C：获取本地时间
来源：http://tf.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bd.521024.cn

[S25] C：内存拷贝
来源：http://bl.lnxyls.cn

memcpy(dst, src, n);
来源：http://ek.gzmigu.cn

[S26] C：内存清零
来源：http://lu.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://ov.9csxet.cn

[S27] C：定义常量
来源：http://de.shxzskj.cn

const double PI = 3.14159;
来源：http://su.shxzskj.cn

[S28] C：静态变量
来源：http://am.huixinmuqiang.cn

static int counter = 0;
来源：http://hh.jctech888.com.cn

[S29] C：变参函数
来源：http://uv.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jd.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ko.colortex.cn

#ifndef X_H
来源：http://yy.yuntaijiaju.cn

#define X_H
来源：http://mr.bjjhwx.cn

#endif
来源：http://gb.jctech888.com.cn

[S31] C++：Hello World
来源：http://ho.hnjuh.cn

#include <iostream>
来源：http://sm.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://va.9csxet.cn

[S32] C++：字符串
来源：http://hu.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://as.jctech888.com.cn

[S33] C++：vector 增删
来源：http://sv.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gi.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://rp.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://sv.shtwfgs.cn

[S35] C++：map
来源：http://dd.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yq.huanxung.cn

[S36] C++：unordered_map
来源：http://jt.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bn.9csxet.cn

[S37] C++：set
来源：http://um.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sr.lnxyls.cn

[S38] C++：排序
来源：http://ul.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://og.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://ec.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ll.jctech888.com.cn

[S40] C++：查找元素
来源：http://zy.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bp.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ov.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uo.szsharing.cn

[S42] C++：继承与虚函数
来源：http://xw.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://gr.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://pl.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://hr.shtwfgs.cn

[S44] C++：引用传参
来源：http://so.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://td.haigaiapp.cn

[S45] C++：lambda
来源：http://oa.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yb.gzmigu.cn

[S46] C++：函数模板
来源：http://sj.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vn.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://ku.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ob.hnjuh.cn

[S48] C++：逐行读文件
来源：http://bo.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gb.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://lr.lnxyls.cn

[S49] C++：写文件
来源：http://lv.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://te.hahajie.cn

[S50] C++：格式化数字
来源：http://xx.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iv.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://te.nszjky.cn

static_cast<double>(a) / b
来源：http://wh.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://gc.huanxung.cn

int size() const noexcept { return n_; }
来源：http://td.yuexingan06.cn

[S53] C++：移动语义
来源：http://fz.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://nb.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://ap.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jt.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://fm.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sm.huixinmuqiang.cn

[S56] C++：optional
来源：http://hm.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ut.jctech888.com.cn

[S57] C++：编译期常量
来源：http://cl.wgjwhj.cn

constexpr int N = 10;
来源：http://ja.shtwfgs.cn

[S58] C++：命名空间
来源：http://bo.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://mz.nicolike.cn

[S59] C++：静态断言
来源：http://bf.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bp.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://dh.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bp.hnjuh.cn

================================================================================
来源：http://ok.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dp.szsharing.cn

================================================================================
来源：http://tv.hahajie.cn

[T01] Kotlin：Hello World
来源：http://na.szsharing.cn

println("Hello")
来源：http://ld.muxihuayi.cn

[T02] Kotlin：变量
来源：http://fw.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lg.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://nf.huixinmuqiang.cn

"值: $b"
来源：http://ja.asd995.cn

[T04] Kotlin：空安全
来源：http://yv.9csxet.cn

val n: String? = null;  n?.length
来源：http://ph.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://ps.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bj.huanxung.cn

[T06] Kotlin：集合映射
来源：http://cb.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://av.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://md.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vy.panjiajie.cn

[T08] Kotlin：数据类
来源：http://on.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://px.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://wv.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://yk.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://oy.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gl.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ti.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://me.asd995.cn

[T12] Kotlin：解构声明
来源：http://lw.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://se.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://ge.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://qp.haigaiapp.cn

[T14] Kotlin：循环
来源：http://um.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://of.gzmigu.cn

[T15] Kotlin：接口
来源：http://gb.9csxet.cn

interface Shape { fun area(): Double }
来源：http://je.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://xc.wgjwhj.cn

print("Hello")
来源：http://cb.huanxung.cn

[T17] Swift：变量与常量
来源：http://aj.newstarts.cn

var a = 1;  let b = 2
来源：http://ag.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://eq.huanxung.cn

"值: \(b)"
来源：http://hl.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://le.shxzukj.cn

if let n = opt { print(n) }
来源：http://zm.szsharing.cn

[T20] Swift：数组操作
来源：http://nv.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hg.hahajie.cn

[T21] Swift：遍历
来源：http://la.nszjky.cn

for x in a { print(x) }
来源：http://lv.hahajie.cn

[T22] Swift：字典
来源：http://pi.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tc.yuexingan06.cn

[T23] Swift：函数
来源：http://yv.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ru.jctech888.com.cn

[T24] Swift：闭包
来源：http://rv.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kg.newstarts.cn

[T25] Swift：结构体
来源：http://th.nicolike.cn

struct P { var x: Int }
来源：http://ki.shxzskj.cn

[T26] Swift：类与重写
来源：http://tu.szsharing.cn

class A: Base { override func f() {} }
来源：http://jp.hahajie.cn

[T27] Swift：错误处理
来源：http://eb.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://np.bookmarksfly.cn

[T28] Swift：枚举
来源：http://nd.yuexingan06.cn

enum Color { case red, green }
来源：http://uu.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://sn.jctech888.com.cn

guard let x = opt else { return }
来源：http://jg.newstarts.cn

[T30] Swift：协议
来源：http://fo.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://ze.bjjhwx.cn

[T31] Lua：Hello World
来源：http://ny.nszjky.cn

print("Hello")
来源：http://sw.huanxung.cn

[T32] Lua：局部变量
来源：http://zw.gzmigu.cn

local a = 1
来源：http://nt.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://ts.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pb.newstarts.cn

[T34] Lua：遍历表
来源：http://ie.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uu.nicolike.cn

[T35] Lua：字典表
来源：http://rf.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://zh.szsharing.cn

[T36] Lua：函数
来源：http://ou.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ja.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://su.chemitech.net.cn

"a" .. "b"
来源：http://sa.panjiajie.cn

[T38] Lua：条件
来源：http://sw.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://ir.szsharing.cn

[T39] Lua：模式匹配
来源：http://xm.newstarts.cn

string.find(s, "%d+")
来源：http://ig.bookmarksfly.cn

[T40] Lua：元表
来源：http://na.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://om.gzmigu.cn

[T41] Perl：Hello World
来源：http://ze.hahajie.cn

print "Hello\n";
来源：http://jw.szsharing.cn

[T42] Perl：变量类型
来源：http://gl.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://be.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://zo.nszjky.cn

"值: $a"
来源：http://cc.huixiangedu.cn

[T44] Perl：条件
来源：http://hu.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://ot.shxzukj.cn

[T45] Perl：数组遍历
来源：http://hr.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://xz.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://kp.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ih.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://wd.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ro.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://km.nszjky.cn

$s =~ s/old/new/g;
来源：http://xl.colortex.cn

[T49] Perl：函数
来源：http://ay.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pg.nicolike.cn

[T50] Perl：逐行读文件
来源：http://ej.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ft.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://jq.colortex.cn

[T51] Scala：Hello World
来源：http://uw.521024.cn

println("Hello")
来源：http://vd.huixinmuqiang.cn

[T52] Scala：变量
来源：http://wo.newstarts.cn

val a = 1;  var b = 2
来源：http://ac.szsharing.cn

[T53] Scala：字符串插值
来源：http://mt.huixiangedu.cn

s"值: $b"
来源：http://vc.huixiangedu.cn

[T54] Scala：集合映射
来源：http://eu.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://fh.asd995.cn

[T55] Scala：集合过滤
来源：http://de.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://al.bjjhwx.cn

[T56] Scala：样例类
来源：http://lz.lnxyls.cn

case class User(name: String, age: Int)
来源：http://rg.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ma.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tg.shxzskj.cn

[T58] Scala：函数定义
来源：http://gb.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xa.panjiajie.cn

[T59] Scala：循环
来源：http://nc.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://ei.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://gj.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ng.wgjwhj.cn

================================================================================
来源：http://fq.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bp.yuntaijiaju.cn

================================================================================
来源：http://hh.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://km.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iz.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://hy.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yu.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://ak.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gr.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://db.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zz.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://js.szsharing.cn

list(dict.fromkeys(arr))
来源：http://uw.shxzskj.cn

[U06] Py：合并两个字典
来源：http://qk.gzmigu.cn

{**a, **b}
来源：http://ig.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ij.asd995.cn

{v: k for k, v in d.items()}
来源：http://uv.gzmigu.cn

[U08] Py：展平二维列表
来源：http://ty.haigaiapp.cn

[y for x in nested for y in x]
来源：http://pp.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://at.shxzukj.cn

max(d, key=d.get)
来源：http://sp.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://lm.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uv.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://ug.shxzskj.cn

(x * 2 for x in arr)
来源：http://bi.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ln.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://yi.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://lt.jctech888.com.cn

deque(maxlen=10)
来源：http://pz.szsharing.cn

[U14] Py：分组收集到列表
来源：http://ba.huixinmuqiang.cn

defaultdict(list)
来源：http://rh.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://pg.szxytkj.cn

t = time.perf_counter()
来源：http://zj.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://bv.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://th.panjiajie.cn

[U17] Py：初始化日志
来源：http://is.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://fh.huixiangedu.cn

[U18] Py：预编译正则
来源：http://dm.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://ha.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ds.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wt.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://rx.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://ko.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://ya.wgjwhj.cn

@contextlib.contextmanager
来源：http://lq.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://uz.muxihuayi.cn

list(zip(*m))
来源：http://rk.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://bf.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://om.wgjwhj.cn

[U24] Py：路径操作
来源：http://gx.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fy.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://el.panjiajie.cn

csv.DictReader(f)
来源：http://lf.asd995.cn

[U26] Py：并发下载
来源：http://fa.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lm.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://qs.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://fh.bookmarksfly.cn

[U28] Py：类型别名
来源：http://yf.newstarts.cn

UserId = int
来源：http://iu.szsharing.cn

[U29] Py：属性校验
来源：http://wd.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ja.jianghongdianzi.cn

[U30] Py：数据类
来源：http://ks.shxzskj.cn

@dataclass(slots=True)
来源：http://oo.haigaiapp.cn

[U31] Py：单测
来源：http://ji.nszjky.cn

python -m pytest -q
来源：http://wm.521024.cn

[U32] Py：代码格式化
来源：http://oa.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ci.nszjky.cn

[U33] Py：打包发布
来源：http://sd.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ny.lnxyls.cn

[U34] Py：判断编码
来源：http://qv.hahajie.cn

chardet.detect(raw)
来源：http://kr.nszjky.cn

[U35] Py：发送邮件
来源：http://ol.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ov.nicolike.cn

[U36] Py：定时任务
来源：http://zm.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://up.szsharing.cn

[U37] Py：读写 Excel
来源：http://fh.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pl.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://oy.szsharing.cn

Path(__file__).resolve().parent
来源：http://xm.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://gr.shxzskj.cn

sys.stdout.isatty()
来源：http://fg.nicolike.cn

[U40] Py：打印到标准错误
来源：http://aq.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://gi.jianghongdianzi.cn


<!-- 参考信息 -->