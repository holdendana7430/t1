代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://sy.9csxet.cn

[S23] C：随机数
来源：http://mt.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hj.9csxet.cn

[S24] C：获取本地时间
来源：http://dp.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://km.asd995.cn

[S25] C：内存拷贝
来源：http://sz.nicolike.cn

memcpy(dst, src, n);
来源：http://eh.nszjky.cn

[S26] C：内存清零
来源：http://lq.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://zu.yuexingan06.cn

[S27] C：定义常量
来源：http://nv.jctech888.com.cn

const double PI = 3.14159;
来源：http://nb.jianghongdianzi.cn

[S28] C：静态变量
来源：http://vj.yuntaijiaju.cn

static int counter = 0;
来源：http://eo.asd995.cn

[S29] C：变参函数
来源：http://bp.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://si.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://fz.nicolike.cn

#ifndef X_H
来源：http://sm.jianghongdianzi.cn

#define X_H
来源：http://kx.jianghongdianzi.cn

#endif
来源：http://vt.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ht.9csxet.cn

#include <iostream>
来源：http://yz.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ch.jctech888.com.cn

[S32] C++：字符串
来源：http://xn.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://gr.wgjwhj.cn

[S33] C++：vector 增删
来源：http://js.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gk.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://hv.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ue.huixiangedu.cn

[S35] C++：map
来源：http://gi.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wp.muxihuayi.cn

[S36] C++：unordered_map
来源：http://oy.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jf.521024.cn

[S37] C++：set
来源：http://sr.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iq.jctech888.com.cn

[S38] C++：排序
来源：http://is.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://vb.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://va.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tb.yuexingan06.cn

[S40] C++：查找元素
来源：http://as.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mp.hahajie.cn

[S41] C++：类与构造函数
来源：http://av.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wl.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://lc.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://tu.newstarts.cn

[S43] C++：智能指针
来源：http://jp.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ez.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://fe.nszjky.cn

void inc(int &x) { ++x; }
来源：http://ag.newstarts.cn

[S45] C++：lambda
来源：http://wa.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gf.bookmarksfly.cn

[S46] C++：函数模板
来源：http://oo.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zy.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ko.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uq.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://hz.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dc.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://fv.huanxung.cn

[S49] C++：写文件
来源：http://kt.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://md.hahajie.cn

[S50] C++：格式化数字
来源：http://ko.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bg.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://up.shtwfgs.cn

static_cast<double>(a) / b
来源：http://nu.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://ry.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://hg.chemitech.net.cn

[S53] C++：移动语义
来源：http://hl.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://us.hahajie.cn

[S54] C++：异常处理
来源：http://uz.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://co.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://mi.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kx.wgjwhj.cn

[S56] C++：optional
来源：http://ue.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cr.gzmigu.cn

[S57] C++：编译期常量
来源：http://pj.chemitech.net.cn

constexpr int N = 10;
来源：http://dx.521024.cn

[S58] C++：命名空间
来源：http://ja.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://sc.shxzskj.cn

[S59] C++：静态断言
来源：http://hi.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ms.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://xs.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tg.hnjuh.cn

================================================================================
来源：http://ru.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rj.asd995.cn

================================================================================
来源：http://pd.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://nj.hahajie.cn

println("Hello")
来源：http://wj.chemitech.net.cn

[T02] Kotlin：变量
来源：http://sd.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qr.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://mv.yuntaijiaju.cn

"值: $b"
来源：http://dy.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://bn.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://zj.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://kg.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ke.521024.cn

[T06] Kotlin：集合映射
来源：http://ob.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jy.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://js.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hq.hnjuh.cn

[T08] Kotlin：数据类
来源：http://aq.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://vq.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://qh.521024.cn

fun String.exclaim() = this + "!"
来源：http://wk.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://vu.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://em.9csxet.cn

[T11] Kotlin：协程
来源：http://ht.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://px.521024.cn

[T12] Kotlin：解构声明
来源：http://wa.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://td.colortex.cn

[T13] Kotlin：只读 Map
来源：http://pd.szsharing.cn

val m = mapOf("a" to 1)
来源：http://kj.asd995.cn

[T14] Kotlin：循环
来源：http://ed.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://na.wgjwhj.cn

[T15] Kotlin：接口
来源：http://cx.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://nl.szsharing.cn

[T16] Swift：Hello World
来源：http://po.shxzukj.cn

print("Hello")
来源：http://go.shxzskj.cn

[T17] Swift：变量与常量
来源：http://xt.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://cu.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://kc.wgjwhj.cn

"值: \(b)"
来源：http://rl.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://gn.shxzskj.cn

if let n = opt { print(n) }
来源：http://jz.chemitech.net.cn

[T20] Swift：数组操作
来源：http://oi.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nq.jctech888.com.cn

[T21] Swift：遍历
来源：http://py.shxzskj.cn

for x in a { print(x) }
来源：http://yi.yuexingan06.cn

[T22] Swift：字典
来源：http://uv.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sg.szxytkj.cn

[T23] Swift：函数
来源：http://jk.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nq.colortex.cn

[T24] Swift：闭包
来源：http://gh.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bq.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://zw.haigaiapp.cn

struct P { var x: Int }
来源：http://ur.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://mu.huanxung.cn

class A: Base { override func f() {} }
来源：http://gi.colortex.cn

[T27] Swift：错误处理
来源：http://je.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://qm.gzmigu.cn

[T28] Swift：枚举
来源：http://wh.huanxung.cn

enum Color { case red, green }
来源：http://mg.asd995.cn

[T29] Swift：guard 提前返回
来源：http://pz.newstarts.cn

guard let x = opt else { return }
来源：http://rz.bookmarksfly.cn

[T30] Swift：协议
来源：http://hk.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://wj.521024.cn

[T31] Lua：Hello World
来源：http://ek.521024.cn

print("Hello")
来源：http://et.szxytkj.cn

[T32] Lua：局部变量
来源：http://rx.lnxyls.cn

local a = 1
来源：http://zv.szxytkj.cn

[T33] Lua：表（数组）
来源：http://ri.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lp.jctech888.com.cn

[T34] Lua：遍历表
来源：http://am.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rc.lnxyls.cn

[T35] Lua：字典表
来源：http://cj.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://tq.gzmigu.cn

[T36] Lua：函数
来源：http://ux.nszjky.cn

function add(a, b) return a + b end
来源：http://dm.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://ra.haigaiapp.cn

"a" .. "b"
来源：http://hb.newstarts.cn

[T38] Lua：条件
来源：http://dm.huanxung.cn

if x > 0 then print("正") end
来源：http://nm.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://zb.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://vx.chemitech.net.cn

[T40] Lua：元表
来源：http://hk.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://li.shxzukj.cn

[T41] Perl：Hello World
来源：http://ps.shxzskj.cn

print "Hello\n";
来源：http://ww.huanxung.cn

[T42] Perl：变量类型
来源：http://bl.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bn.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://wi.521024.cn

"值: $a"
来源：http://gr.newstarts.cn

[T44] Perl：条件
来源：http://uv.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://ee.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://ju.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://yx.hnjuh.cn

[T46] Perl：哈希操作
来源：http://fy.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://se.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ka.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tu.nszjky.cn

[T48] Perl：正则替换
来源：http://ph.newstarts.cn

$s =~ s/old/new/g;
来源：http://xw.huixinmuqiang.cn

[T49] Perl：函数
来源：http://mz.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ln.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://kc.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://to.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ik.lnxyls.cn

[T51] Scala：Hello World
来源：http://sg.bjjhwx.cn

println("Hello")
来源：http://yn.hahajie.cn

[T52] Scala：变量
来源：http://df.huixiangedu.cn

val a = 1;  var b = 2
来源：http://ad.9csxet.cn

[T53] Scala：字符串插值
来源：http://pl.haigaiapp.cn

s"值: $b"
来源：http://ma.shtwfgs.cn

[T54] Scala：集合映射
来源：http://zd.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://dt.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://ga.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xm.shtwfgs.cn

[T56] Scala：样例类
来源：http://yt.nicolike.cn

case class User(name: String, age: Int)
来源：http://ab.hahajie.cn

[T57] Scala：模式匹配
来源：http://nd.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dq.szxytkj.cn

[T58] Scala：函数定义
来源：http://xa.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://do.jianghongdianzi.cn

[T59] Scala：循环
来源：http://wo.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://bd.yuexingan06.cn

[T60] Scala：折叠
来源：http://ag.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ml.muxihuayi.cn

================================================================================
来源：http://gz.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lk.9csxet.cn

================================================================================
来源：http://bu.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://kc.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qz.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://nl.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jb.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://zd.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wo.hahajie.cn

[U04] Py：变量调试打印
来源：http://vx.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mq.9csxet.cn

[U05] Py：列表去重且保序
来源：http://mo.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://uw.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://wd.huixiangedu.cn

{**a, **b}
来源：http://qt.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://jl.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://iy.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://kb.gzmigu.cn

[y for x in nested for y in x]
来源：http://qs.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://py.jianghongdianzi.cn

max(d, key=d.get)
来源：http://co.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://qa.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fy.shxzskj.cn

[U11] Py：生成器表达式
来源：http://mg.shxzukj.cn

(x * 2 for x in arr)
来源：http://ev.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yd.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://cv.9csxet.cn

[U13] Py：固定长度队列
来源：http://zd.huanxung.cn

deque(maxlen=10)
来源：http://im.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://cb.hnjuh.cn

defaultdict(list)
来源：http://kd.gzmigu.cn

[U15] Py：高精度计时
来源：http://gc.szxytkj.cn

t = time.perf_counter()
来源：http://it.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://tp.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mw.szsharing.cn

[U17] Py：初始化日志
来源：http://ma.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://wo.nicolike.cn

[U18] Py：预编译正则
来源：http://bn.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://gd.asd995.cn

[U19] Py：正则替换带回调
来源：http://bv.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xn.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://gj.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://py.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://cr.bjjhwx.cn

@contextlib.contextmanager
来源：http://ty.hnjuh.cn

[U22] Py：矩阵转置
来源：http://si.panjiajie.cn

list(zip(*m))
来源：http://dt.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://lz.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nb.haigaiapp.cn

[U24] Py：路径操作
来源：http://ml.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dl.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://wp.szxytkj.cn

csv.DictReader(f)
来源：http://gt.szsharing.cn

[U26] Py：并发下载
来源：http://pu.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bv.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://zc.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://pb.panjiajie.cn

[U28] Py：类型别名
来源：http://oi.muxihuayi.cn

UserId = int
来源：http://ov.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://ry.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://hq.521024.cn

[U30] Py：数据类
来源：http://xc.9csxet.cn

@dataclass(slots=True)
来源：http://dt.szsharing.cn

[U31] Py：单测
来源：http://ur.colortex.cn

python -m pytest -q
来源：http://td.wgjwhj.cn

[U32] Py：代码格式化
来源：http://ms.asd995.cn

ruff format . && ruff check --fix .
来源：http://qa.haigaiapp.cn

[U33] Py：打包发布
来源：http://qd.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://ie.shxzskj.cn

[U34] Py：判断编码
来源：http://uy.newstarts.cn

chardet.detect(raw)
来源：http://xx.shtwfgs.cn

[U35] Py：发送邮件
来源：http://fw.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ao.hnjuh.cn

[U36] Py：定时任务
来源：http://fz.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://xg.asd995.cn

[U37] Py：读写 Excel
来源：http://qa.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kg.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://fx.hahajie.cn

Path(__file__).resolve().parent
来源：http://te.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://zu.shxzukj.cn

sys.stdout.isatty()
来源：http://nf.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://xk.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://hz.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://vo.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fr.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://vn.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://er.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://yw.shxzskj.cn

namespace App\Http;
来源：http://wd.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://xz.jianghongdianzi.cn

declare(strict_types=1);
来源：http://dz.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://xl.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hh.nicolike.cn

[U46] PHP：可空类型
来源：http://ck.521024.cn

?string $name = null
来源：http://ox.gzmigu.cn


<!-- 参考信息 -->