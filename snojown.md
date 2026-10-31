代发 wailian999

int main(int argc, char **argv)
来源：http://hv.hahajie.cn

[S19] C：快速排序
来源：http://mw.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sf.gzmigu.cn

[S20] C：二分查找
来源：http://cx.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vf.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://am.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sk.hahajie.cn

[S22] C：字符串转数字
来源：http://jo.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kf.yuntaijiaju.cn

[S23] C：随机数
来源：http://sm.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nn.panjiajie.cn

[S24] C：获取本地时间
来源：http://xz.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pf.szsharing.cn

[S25] C：内存拷贝
来源：http://qs.bjjhwx.cn

memcpy(dst, src, n);
来源：http://ft.hahajie.cn

[S26] C：内存清零
来源：http://oj.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://tb.yuntaijiaju.cn

[S27] C：定义常量
来源：http://gw.hnjuh.cn

const double PI = 3.14159;
来源：http://lj.hahajie.cn

[S28] C：静态变量
来源：http://al.yuntaijiaju.cn

static int counter = 0;
来源：http://gl.szxytkj.cn

[S29] C：变参函数
来源：http://eu.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jx.asd995.cn

[S30] C：头文件保护
来源：http://jk.szxytkj.cn

#ifndef X_H
来源：http://hy.asd995.cn

#define X_H
来源：http://qx.nszjky.cn

#endif
来源：http://mx.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://nw.huanxung.cn

#include <iostream>
来源：http://pp.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://by.huanxung.cn

[S32] C++：字符串
来源：http://we.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://iz.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://rm.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kp.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://fa.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ck.shxzskj.cn

[S35] C++：map
来源：http://li.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hj.jctech888.com.cn

[S36] C++：unordered_map
来源：http://cp.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://py.huanxung.cn

[S37] C++：set
来源：http://ci.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ih.chemitech.net.cn

[S38] C++：排序
来源：http://no.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://oh.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://tc.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://av.huixiangedu.cn

[S40] C++：查找元素
来源：http://zi.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xs.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://ag.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xi.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://dh.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://xa.wgjwhj.cn

[S43] C++：智能指针
来源：http://ay.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://iq.gzmigu.cn

[S44] C++：引用传参
来源：http://cl.9csxet.cn

void inc(int &x) { ++x; }
来源：http://gy.huanxung.cn

[S45] C++：lambda
来源：http://ha.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yb.szsharing.cn

[S46] C++：函数模板
来源：http://ev.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ck.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://zr.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ts.szxytkj.cn

[S48] C++：逐行读文件
来源：http://jb.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yy.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://dw.bjjhwx.cn

[S49] C++：写文件
来源：http://ey.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iy.nszjky.cn

[S50] C++：格式化数字
来源：http://fk.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pz.nszjky.cn

[S51] C++：显式类型转换
来源：http://ip.huixiangedu.cn

static_cast<double>(a) / b
来源：http://zp.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://iq.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://rk.panjiajie.cn

[S53] C++：移动语义
来源：http://mj.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://pu.asd995.cn

[S54] C++：异常处理
来源：http://ey.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oe.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://au.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gw.chemitech.net.cn

[S56] C++：optional
来源：http://iw.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ii.shxzukj.cn

[S57] C++：编译期常量
来源：http://vv.panjiajie.cn

constexpr int N = 10;
来源：http://vv.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://ci.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://sp.wgjwhj.cn

[S59] C++：静态断言
来源：http://hh.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nl.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://nf.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ci.521024.cn

================================================================================
来源：http://pi.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oh.szsharing.cn

================================================================================
来源：http://yp.nicolike.cn

[T01] Kotlin：Hello World
来源：http://iz.szxytkj.cn

println("Hello")
来源：http://gj.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://ub.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uz.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://fw.gzmigu.cn

"值: $b"
来源：http://ao.szxytkj.cn

[T04] Kotlin：空安全
来源：http://ih.newstarts.cn

val n: String? = null;  n?.length
来源：http://fh.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://bd.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yo.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://rd.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xm.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://rg.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rk.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ka.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://lf.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://fv.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://ch.nszjky.cn

[T10] Kotlin：默认参数
来源：http://ik.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dt.nszjky.cn

[T11] Kotlin：协程
来源：http://lz.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sj.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://zw.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://fz.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://pg.521024.cn

val m = mapOf("a" to 1)
来源：http://hs.yuexingan06.cn

[T14] Kotlin：循环
来源：http://nv.shxzukj.cn

for (i in 1..10) println(i)
来源：http://jt.shtwfgs.cn

[T15] Kotlin：接口
来源：http://pr.nszjky.cn

interface Shape { fun area(): Double }
来源：http://ap.shxzukj.cn

[T16] Swift：Hello World
来源：http://ce.huixinmuqiang.cn

print("Hello")
来源：http://nf.hahajie.cn

[T17] Swift：变量与常量
来源：http://fj.yuexingan06.cn

var a = 1;  let b = 2
来源：http://me.gzmigu.cn

[T18] Swift：字符串插值
来源：http://ai.asd995.cn

"值: \(b)"
来源：http://mr.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://jd.yuexingan06.cn

if let n = opt { print(n) }
来源：http://ka.jctech888.com.cn

[T20] Swift：数组操作
来源：http://su.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vx.yuexingan06.cn

[T21] Swift：遍历
来源：http://zn.nszjky.cn

for x in a { print(x) }
来源：http://hx.shxzukj.cn

[T22] Swift：字典
来源：http://gh.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uw.szsharing.cn

[T23] Swift：函数
来源：http://yj.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://be.asd995.cn

[T24] Swift：闭包
来源：http://hi.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://al.shxzskj.cn

[T25] Swift：结构体
来源：http://ht.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ox.muxihuayi.cn

[T26] Swift：类与重写
来源：http://fz.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://bh.nicolike.cn

[T27] Swift：错误处理
来源：http://mu.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://rh.newstarts.cn

[T28] Swift：枚举
来源：http://eu.yuexingan06.cn

enum Color { case red, green }
来源：http://qk.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://sh.gzmigu.cn

guard let x = opt else { return }
来源：http://qp.panjiajie.cn

[T30] Swift：协议
来源：http://yp.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://pw.hahajie.cn

[T31] Lua：Hello World
来源：http://ji.shtwfgs.cn

print("Hello")
来源：http://pv.wgjwhj.cn

[T32] Lua：局部变量
来源：http://kk.szxytkj.cn

local a = 1
来源：http://xt.huanxung.cn

[T33] Lua：表（数组）
来源：http://cf.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bp.huixiangedu.cn

[T34] Lua：遍历表
来源：http://dp.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lg.521024.cn

[T35] Lua：字典表
来源：http://bv.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://vw.szxytkj.cn

[T36] Lua：函数
来源：http://ds.huanxung.cn

function add(a, b) return a + b end
来源：http://tx.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://rs.bjjhwx.cn

"a" .. "b"
来源：http://jm.huanxung.cn

[T38] Lua：条件
来源：http://wi.yuexingan06.cn

if x > 0 then print("正") end
来源：http://zk.panjiajie.cn

[T39] Lua：模式匹配
来源：http://wv.panjiajie.cn

string.find(s, "%d+")
来源：http://bv.gzmigu.cn

[T40] Lua：元表
来源：http://sd.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://lb.bjjhwx.cn

[T41] Perl：Hello World
来源：http://ec.hahajie.cn

print "Hello\n";
来源：http://sj.gzmigu.cn

[T42] Perl：变量类型
来源：http://mc.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nt.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://ep.shxzskj.cn

"值: $a"
来源：http://bm.gzmigu.cn

[T44] Perl：条件
来源：http://sh.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://tl.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://ib.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://af.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://yx.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fs.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://vz.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://my.hnjuh.cn

[T48] Perl：正则替换
来源：http://wn.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://cu.nszjky.cn

[T49] Perl：函数
来源：http://bj.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vc.nszjky.cn

[T50] Perl：逐行读文件
来源：http://jf.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gp.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://hw.521024.cn

[T51] Scala：Hello World
来源：http://vn.chemitech.net.cn

println("Hello")
来源：http://nu.yuexingan06.cn

[T52] Scala：变量
来源：http://wu.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ca.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://xw.asd995.cn

s"值: $b"
来源：http://mr.bjjhwx.cn

[T54] Scala：集合映射
来源：http://yk.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://qz.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://hu.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vg.9csxet.cn

[T56] Scala：样例类
来源：http://qy.colortex.cn

case class User(name: String, age: Int)
来源：http://pe.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://om.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wu.szsharing.cn

[T58] Scala：函数定义
来源：http://gb.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hs.bookmarksfly.cn

[T59] Scala：循环
来源：http://sf.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://jb.nicolike.cn

[T60] Scala：折叠
来源：http://fw.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jy.bookmarksfly.cn

================================================================================
来源：http://uk.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bg.hahajie.cn

================================================================================
来源：http://jl.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://db.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hn.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://aa.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mc.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://my.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dv.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://lh.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gp.szsharing.cn

[U05] Py：列表去重且保序
来源：http://li.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://tp.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://hu.521024.cn

{**a, **b}
来源：http://oo.9csxet.cn

[U07] Py：反转字典键值
来源：http://ip.nicolike.cn

{v: k for k, v in d.items()}
来源：http://vx.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://te.szsharing.cn

[y for x in nested for y in x]
来源：http://ss.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ie.haigaiapp.cn

max(d, key=d.get)
来源：http://kw.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://ja.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fl.lnxyls.cn

[U11] Py：生成器表达式
来源：http://ug.yuexingan06.cn

(x * 2 for x in arr)
来源：http://de.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uv.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://pg.shxzskj.cn

[U13] Py：固定长度队列
来源：http://an.lnxyls.cn

deque(maxlen=10)
来源：http://pq.nszjky.cn

[U14] Py：分组收集到列表
来源：http://kq.hahajie.cn

defaultdict(list)
来源：http://xb.521024.cn

[U15] Py：高精度计时
来源：http://mx.jctech888.com.cn

t = time.perf_counter()
来源：http://gj.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://cx.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aa.hnjuh.cn

[U17] Py：初始化日志
来源：http://st.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://su.shxzskj.cn

[U18] Py：预编译正则
来源：http://ac.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://av.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://ro.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fh.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://cq.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://fy.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://fk.haigaiapp.cn

@contextlib.contextmanager
来源：http://zq.newstarts.cn

[U22] Py：矩阵转置
来源：http://cr.newstarts.cn

list(zip(*m))
来源：http://on.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://ns.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ax.muxihuayi.cn

[U24] Py：路径操作
来源：http://lb.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ou.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://bh.bookmarksfly.cn

csv.DictReader(f)
来源：http://gh.asd995.cn

[U26] Py：并发下载
来源：http://at.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fk.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://ve.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://vg.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://ra.huixinmuqiang.cn

UserId = int
来源：http://ke.huanxung.cn

[U29] Py：属性校验
来源：http://fp.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://ct.huixiangedu.cn

[U30] Py：数据类
来源：http://gg.shtwfgs.cn

@dataclass(slots=True)
来源：http://dn.bookmarksfly.cn

[U31] Py：单测
来源：http://bt.newstarts.cn

python -m pytest -q
来源：http://cg.chemitech.net.cn

[U32] Py：代码格式化
来源：http://lu.newstarts.cn

ruff format . && ruff check --fix .
来源：http://jt.huixiangedu.cn

[U33] Py：打包发布
来源：http://up.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://tg.shtwfgs.cn

[U34] Py：判断编码
来源：http://el.szsharing.cn

chardet.detect(raw)
来源：http://jq.yuexingan06.cn

[U35] Py：发送邮件
来源：http://wy.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zh.jctech888.com.cn

[U36] Py：定时任务
来源：http://su.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://vg.newstarts.cn

[U37] Py：读写 Excel
来源：http://vm.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xm.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ru.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://zp.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://lb.chemitech.net.cn

sys.stdout.isatty()
来源：http://ey.szsharing.cn

[U40] Py：打印到标准错误
来源：http://gr.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://wv.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://rd.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fh.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://zi.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hq.szsharing.cn


<!-- 参考信息 -->