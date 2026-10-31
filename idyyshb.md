代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yz.haigaiapp.cn

[S25] C：内存拷贝
来源：http://bv.hnjuh.cn

memcpy(dst, src, n);
来源：http://ma.nicolike.cn

[S26] C：内存清零
来源：http://ff.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://dk.chemitech.net.cn

[S27] C：定义常量
来源：http://jj.nicolike.cn

const double PI = 3.14159;
来源：http://jg.szsharing.cn

[S28] C：静态变量
来源：http://vl.nicolike.cn

static int counter = 0;
来源：http://bc.nszjky.cn

[S29] C：变参函数
来源：http://ho.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://se.bjjhwx.cn

[S30] C：头文件保护
来源：http://ei.shxzukj.cn

#ifndef X_H
来源：http://sw.hahajie.cn

#define X_H
来源：http://ye.hahajie.cn

#endif
来源：http://lx.szsharing.cn

[S31] C++：Hello World
来源：http://yj.chemitech.net.cn

#include <iostream>
来源：http://ts.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://dc.hahajie.cn

[S32] C++：字符串
来源：http://pi.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://na.muxihuayi.cn

[S33] C++：vector 增删
来源：http://bv.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ya.nszjky.cn

[S34] C++：遍历 vector
来源：http://vl.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://eq.bjjhwx.cn

[S35] C++：map
来源：http://wg.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ju.newstarts.cn

[S36] C++：unordered_map
来源：http://lf.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oj.huixiangedu.cn

[S37] C++：set
来源：http://wt.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mc.shxzskj.cn

[S38] C++：排序
来源：http://bp.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://ki.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://eq.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aw.szxytkj.cn

[S40] C++：查找元素
来源：http://wv.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nx.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://hz.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sd.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://yr.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://gu.huixiangedu.cn

[S43] C++：智能指针
来源：http://eo.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://ej.wgjwhj.cn

[S44] C++：引用传参
来源：http://bo.nicolike.cn

void inc(int &x) { ++x; }
来源：http://yg.521024.cn

[S45] C++：lambda
来源：http://dx.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fv.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ee.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pt.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://qy.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qw.szxytkj.cn

[S48] C++：逐行读文件
来源：http://yj.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jd.colortex.cn

while (std::getline(in, line)) { }
来源：http://er.huanxung.cn

[S49] C++：写文件
来源：http://kz.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xu.jctech888.com.cn

[S50] C++：格式化数字
来源：http://jw.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xt.asd995.cn

[S51] C++：显式类型转换
来源：http://hb.wgjwhj.cn

static_cast<double>(a) / b
来源：http://kb.521024.cn

[S52] C++：const 与 noexcept
来源：http://pn.huanxung.cn

int size() const noexcept { return n_; }
来源：http://ej.nicolike.cn

[S53] C++：移动语义
来源：http://zr.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://pb.muxihuayi.cn

[S54] C++：异常处理
来源：http://cl.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ld.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://ao.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cw.shxzukj.cn

[S56] C++：optional
来源：http://gm.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wn.hnjuh.cn

[S57] C++：编译期常量
来源：http://ys.nszjky.cn

constexpr int N = 10;
来源：http://qi.shxzskj.cn

[S58] C++：命名空间
来源：http://al.521024.cn

namespace ns { int f() { return 1; } }
来源：http://cx.wgjwhj.cn

[S59] C++：静态断言
来源：http://xk.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wl.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ce.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ti.bookmarksfly.cn

================================================================================
来源：http://fm.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ks.chemitech.net.cn

================================================================================
来源：http://cw.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://ft.chemitech.net.cn

println("Hello")
来源：http://xl.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://dl.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fn.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://eo.shxzukj.cn

"值: $b"
来源：http://tr.shxzskj.cn

[T04] Kotlin：空安全
来源：http://fr.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://eb.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://fi.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kq.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://hn.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gg.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://rz.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ti.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ry.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://lr.asd995.cn

[T09] Kotlin：扩展函数
来源：http://nn.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://pl.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://gs.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wx.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ra.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nc.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://oh.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://ka.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://kn.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://rl.9csxet.cn

[T14] Kotlin：循环
来源：http://fc.szxytkj.cn

for (i in 1..10) println(i)
来源：http://tm.shxzskj.cn

[T15] Kotlin：接口
来源：http://ak.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://pg.shtwfgs.cn

[T16] Swift：Hello World
来源：http://zw.shxzskj.cn

print("Hello")
来源：http://yu.newstarts.cn

[T17] Swift：变量与常量
来源：http://fq.bjjhwx.cn

var a = 1;  let b = 2
来源：http://em.nicolike.cn

[T18] Swift：字符串插值
来源：http://ic.nicolike.cn

"值: \(b)"
来源：http://vo.hnjuh.cn

[T19] Swift：可选绑定
来源：http://yv.jctech888.com.cn

if let n = opt { print(n) }
来源：http://nf.chemitech.net.cn

[T20] Swift：数组操作
来源：http://xc.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ei.huanxung.cn

[T21] Swift：遍历
来源：http://oh.haigaiapp.cn

for x in a { print(x) }
来源：http://fu.muxihuayi.cn

[T22] Swift：字典
来源：http://yh.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bh.9csxet.cn

[T23] Swift：函数
来源：http://sn.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vm.shxzskj.cn

[T24] Swift：闭包
来源：http://ra.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://is.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://tr.hahajie.cn

struct P { var x: Int }
来源：http://ic.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://cf.szxytkj.cn

class A: Base { override func f() {} }
来源：http://mg.bjjhwx.cn

[T27] Swift：错误处理
来源：http://po.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://if.muxihuayi.cn

[T28] Swift：枚举
来源：http://jj.shxzukj.cn

enum Color { case red, green }
来源：http://bw.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://gx.hahajie.cn

guard let x = opt else { return }
来源：http://dk.yuexingan06.cn

[T30] Swift：协议
来源：http://iv.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://wi.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://nu.huixiangedu.cn

print("Hello")
来源：http://hi.haigaiapp.cn

[T32] Lua：局部变量
来源：http://hw.yuexingan06.cn

local a = 1
来源：http://cf.szsharing.cn

[T33] Lua：表（数组）
来源：http://ul.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bz.shxzukj.cn

[T34] Lua：遍历表
来源：http://av.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rx.521024.cn

[T35] Lua：字典表
来源：http://iw.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://eu.muxihuayi.cn

[T36] Lua：函数
来源：http://sl.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://el.9csxet.cn

[T37] Lua：字符串拼接
来源：http://hm.nszjky.cn

"a" .. "b"
来源：http://fz.muxihuayi.cn

[T38] Lua：条件
来源：http://sx.nicolike.cn

if x > 0 then print("正") end
来源：http://ry.hnjuh.cn

[T39] Lua：模式匹配
来源：http://vb.colortex.cn

string.find(s, "%d+")
来源：http://eq.shxzskj.cn

[T40] Lua：元表
来源：http://xq.9csxet.cn

setmetatable({}, { __index = base })
来源：http://nv.shxzskj.cn

[T41] Perl：Hello World
来源：http://kn.jctech888.com.cn

print "Hello\n";
来源：http://uk.shtwfgs.cn

[T42] Perl：变量类型
来源：http://or.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hc.nszjky.cn

[T43] Perl：字符串插值
来源：http://eu.szsharing.cn

"值: $a"
来源：http://fv.bookmarksfly.cn

[T44] Perl：条件
来源：http://to.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://gg.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ve.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://ev.panjiajie.cn

[T46] Perl：哈希操作
来源：http://oa.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wk.521024.cn

[T47] Perl：正则捕获
来源：http://gv.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uj.shxzukj.cn

[T48] Perl：正则替换
来源：http://es.asd995.cn

$s =~ s/old/new/g;
来源：http://ln.nszjky.cn

[T49] Perl：函数
来源：http://wh.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xs.szsharing.cn

[T50] Perl：逐行读文件
来源：http://ad.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://an.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://pj.nicolike.cn

[T51] Scala：Hello World
来源：http://zt.asd995.cn

println("Hello")
来源：http://mg.hnjuh.cn

[T52] Scala：变量
来源：http://ex.hnjuh.cn

val a = 1;  var b = 2
来源：http://qn.szxytkj.cn

[T53] Scala：字符串插值
来源：http://ty.szsharing.cn

s"值: $b"
来源：http://ee.muxihuayi.cn

[T54] Scala：集合映射
来源：http://mv.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://dg.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ra.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sx.huixiangedu.cn

[T56] Scala：样例类
来源：http://vd.nszjky.cn

case class User(name: String, age: Int)
来源：http://ot.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://jb.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ai.haigaiapp.cn

[T58] Scala：函数定义
来源：http://rf.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wm.jianghongdianzi.cn

[T59] Scala：循环
来源：http://tm.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://ze.haigaiapp.cn

[T60] Scala：折叠
来源：http://sq.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bg.wgjwhj.cn

================================================================================
来源：http://wh.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tw.newstarts.cn

================================================================================
来源：http://jr.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://za.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vu.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://fb.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xf.colortex.cn

[U03] Py：加载 .env 配置
来源：http://cs.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ql.panjiajie.cn

[U04] Py：变量调试打印
来源：http://gv.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ws.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://lr.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://ak.huanxung.cn

[U06] Py：合并两个字典
来源：http://rh.gzmigu.cn

{**a, **b}
来源：http://jz.colortex.cn

[U07] Py：反转字典键值
来源：http://zj.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://ji.nicolike.cn

[U08] Py：展平二维列表
来源：http://gx.lnxyls.cn

[y for x in nested for y in x]
来源：http://ix.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://na.bookmarksfly.cn

max(d, key=d.get)
来源：http://fd.panjiajie.cn

[U10] Py：按值排序字典
来源：http://qa.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fs.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://lw.wgjwhj.cn

(x * 2 for x in arr)
来源：http://kp.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yc.nszjky.cn

Counter(arr).most_common(3)
来源：http://zl.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://gp.szsharing.cn

deque(maxlen=10)
来源：http://kq.szsharing.cn

[U14] Py：分组收集到列表
来源：http://qv.newstarts.cn

defaultdict(list)
来源：http://xs.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://zm.9csxet.cn

t = time.perf_counter()
来源：http://vb.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://fw.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yv.colortex.cn

[U17] Py：初始化日志
来源：http://pk.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://lp.nicolike.cn

[U18] Py：预编译正则
来源：http://ij.asd995.cn

pat = re.compile(r"\d+")
来源：http://rf.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://fu.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ta.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ra.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://kr.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://oj.panjiajie.cn

@contextlib.contextmanager
来源：http://am.nszjky.cn

[U22] Py：矩阵转置
来源：http://lg.hnjuh.cn

list(zip(*m))
来源：http://lk.nszjky.cn

[U23] Py：分块读取大文件
来源：http://ii.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vv.lnxyls.cn

[U24] Py：路径操作
来源：http://br.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tg.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://pj.panjiajie.cn

csv.DictReader(f)
来源：http://fv.yuexingan06.cn

[U26] Py：并发下载
来源：http://zx.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yv.521024.cn

[U27] Py：异步 HTTP
来源：http://uh.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uq.9csxet.cn

[U28] Py：类型别名
来源：http://bx.panjiajie.cn

UserId = int
来源：http://nx.nszjky.cn

[U29] Py：属性校验
来源：http://ca.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://gw.szsharing.cn

[U30] Py：数据类
来源：http://ka.asd995.cn

@dataclass(slots=True)
来源：http://ax.hnjuh.cn

[U31] Py：单测
来源：http://fl.newstarts.cn

python -m pytest -q
来源：http://va.asd995.cn

[U32] Py：代码格式化
来源：http://xx.colortex.cn

ruff format . && ruff check --fix .
来源：http://zl.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://cl.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://ou.colortex.cn

[U34] Py：判断编码
来源：http://qq.521024.cn

chardet.detect(raw)
来源：http://jp.bjjhwx.cn

[U35] Py：发送邮件
来源：http://ii.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mp.szsharing.cn

[U36] Py：定时任务
来源：http://it.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://oc.panjiajie.cn

[U37] Py：读写 Excel
来源：http://pl.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vl.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://th.nszjky.cn

Path(__file__).resolve().parent
来源：http://xr.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://ut.muxihuayi.cn

sys.stdout.isatty()
来源：http://kr.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://kq.szxytkj.cn

print("err", file=sys.stderr)
来源：http://cp.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://ha.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ng.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://pq.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ak.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://oo.bookmarksfly.cn

namespace App\Http;
来源：http://jt.9csxet.cn

[U44] PHP：开启严格类型
来源：http://ed.colortex.cn

declare(strict_types=1);
来源：http://xd.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://us.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lf.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://ey.jctech888.com.cn

?string $name = null
来源：http://ky.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://pa.shxzskj.cn

int|string $id
来源：http://sz.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://lw.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ta.yuexingan06.cn


<!-- 参考信息 -->