代发 wailian999

memset(a, 0, sizeof a);
来源：http://nd.9csxet.cn

[S27] C：定义常量
来源：http://tm.shxzukj.cn

const double PI = 3.14159;
来源：http://wx.bookmarksfly.cn

[S28] C：静态变量
来源：http://vf.gzmigu.cn

static int counter = 0;
来源：http://ic.nszjky.cn

[S29] C：变参函数
来源：http://pz.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lc.bookmarksfly.cn

[S30] C：头文件保护
来源：http://pb.521024.cn

#ifndef X_H
来源：http://ye.shxzukj.cn

#define X_H
来源：http://hc.bjjhwx.cn

#endif
来源：http://gm.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://tw.shtwfgs.cn

#include <iostream>
来源：http://yr.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ok.hahajie.cn

[S32] C++：字符串
来源：http://up.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://jy.lnxyls.cn

[S33] C++：vector 增删
来源：http://yh.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mk.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://oc.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://br.bjjhwx.cn

[S35] C++：map
来源：http://ct.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nh.huixiangedu.cn

[S36] C++：unordered_map
来源：http://nq.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ut.szxytkj.cn

[S37] C++：set
来源：http://yq.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://il.szsharing.cn

[S38] C++：排序
来源：http://cg.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://et.521024.cn

[S39] C++：自定义比较器排序
来源：http://ye.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://su.muxihuayi.cn

[S40] C++：查找元素
来源：http://ly.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wj.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://gw.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mt.nszjky.cn

[S42] C++：继承与虚函数
来源：http://mo.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://um.lnxyls.cn

[S43] C++：智能指针
来源：http://to.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://bu.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://vw.hahajie.cn

void inc(int &x) { ++x; }
来源：http://gg.bookmarksfly.cn

[S45] C++：lambda
来源：http://bm.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mo.szxytkj.cn

[S46] C++：函数模板
来源：http://vz.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://df.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://yw.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kw.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://rb.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ei.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://pr.nszjky.cn

[S49] C++：写文件
来源：http://bj.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uf.panjiajie.cn

[S50] C++：格式化数字
来源：http://uw.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vt.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://gc.nicolike.cn

static_cast<double>(a) / b
来源：http://uj.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ad.huanxung.cn

int size() const noexcept { return n_; }
来源：http://tv.shxzskj.cn

[S53] C++：移动语义
来源：http://ob.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://qj.huixiangedu.cn

[S54] C++：异常处理
来源：http://kw.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gg.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://tl.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ts.jctech888.com.cn

[S56] C++：optional
来源：http://sr.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mq.hahajie.cn

[S57] C++：编译期常量
来源：http://vi.haigaiapp.cn

constexpr int N = 10;
来源：http://cs.haigaiapp.cn

[S58] C++：命名空间
来源：http://pw.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://wj.panjiajie.cn

[S59] C++：静态断言
来源：http://su.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jj.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://mw.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lw.shtwfgs.cn

================================================================================
来源：http://og.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ye.shxzukj.cn

================================================================================
来源：http://yz.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://wp.shtwfgs.cn

println("Hello")
来源：http://hk.wgjwhj.cn

[T02] Kotlin：变量
来源：http://bo.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://go.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://ag.shtwfgs.cn

"值: $b"
来源：http://gf.shxzukj.cn

[T04] Kotlin：空安全
来源：http://wx.panjiajie.cn

val n: String? = null;  n?.length
来源：http://lk.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://md.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ks.hahajie.cn

[T06] Kotlin：集合映射
来源：http://qy.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://je.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://lq.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bf.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://bf.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://lr.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://gh.colortex.cn

fun String.exclaim() = this + "!"
来源：http://yd.nszjky.cn

[T10] Kotlin：默认参数
来源：http://es.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://by.gzmigu.cn

[T11] Kotlin：协程
来源：http://wq.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hs.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://wg.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://cc.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://si.nicolike.cn

val m = mapOf("a" to 1)
来源：http://ts.panjiajie.cn

[T14] Kotlin：循环
来源：http://al.lnxyls.cn

for (i in 1..10) println(i)
来源：http://lf.newstarts.cn

[T15] Kotlin：接口
来源：http://ff.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://md.huixiangedu.cn

[T16] Swift：Hello World
来源：http://go.lnxyls.cn

print("Hello")
来源：http://vq.szxytkj.cn

[T17] Swift：变量与常量
来源：http://av.shxzskj.cn

var a = 1;  let b = 2
来源：http://aa.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://rn.521024.cn

"值: \(b)"
来源：http://ec.asd995.cn

[T19] Swift：可选绑定
来源：http://qf.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://iw.panjiajie.cn

[T20] Swift：数组操作
来源：http://lg.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://np.colortex.cn

[T21] Swift：遍历
来源：http://lk.muxihuayi.cn

for x in a { print(x) }
来源：http://yg.yuexingan06.cn

[T22] Swift：字典
来源：http://ay.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bj.hahajie.cn

[T23] Swift：函数
来源：http://es.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ti.newstarts.cn

[T24] Swift：闭包
来源：http://mj.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zy.haigaiapp.cn

[T25] Swift：结构体
来源：http://eq.hahajie.cn

struct P { var x: Int }
来源：http://aj.haigaiapp.cn

[T26] Swift：类与重写
来源：http://qc.521024.cn

class A: Base { override func f() {} }
来源：http://wa.9csxet.cn

[T27] Swift：错误处理
来源：http://dj.huanxung.cn

do { try f() } catch { print(error) }
来源：http://qg.hahajie.cn

[T28] Swift：枚举
来源：http://nm.lnxyls.cn

enum Color { case red, green }
来源：http://tb.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://to.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://nh.huixinmuqiang.cn

[T30] Swift：协议
来源：http://sh.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://fx.9csxet.cn

[T31] Lua：Hello World
来源：http://xb.haigaiapp.cn

print("Hello")
来源：http://zl.hahajie.cn

[T32] Lua：局部变量
来源：http://ea.bjjhwx.cn

local a = 1
来源：http://vz.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://bc.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mv.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://ht.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://df.haigaiapp.cn

[T35] Lua：字典表
来源：http://bv.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://ux.panjiajie.cn

[T36] Lua：函数
来源：http://yj.chemitech.net.cn

function add(a, b) return a + b end
来源：http://wr.asd995.cn

[T37] Lua：字符串拼接
来源：http://oj.jctech888.com.cn

"a" .. "b"
来源：http://og.nszjky.cn

[T38] Lua：条件
来源：http://ae.gzmigu.cn

if x > 0 then print("正") end
来源：http://qw.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://be.nszjky.cn

string.find(s, "%d+")
来源：http://xl.shtwfgs.cn

[T40] Lua：元表
来源：http://gg.9csxet.cn

setmetatable({}, { __index = base })
来源：http://zi.shtwfgs.cn

[T41] Perl：Hello World
来源：http://vw.asd995.cn

print "Hello\n";
来源：http://gh.nszjky.cn

[T42] Perl：变量类型
来源：http://ls.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oy.panjiajie.cn

[T43] Perl：字符串插值
来源：http://kd.panjiajie.cn

"值: $a"
来源：http://to.bookmarksfly.cn

[T44] Perl：条件
来源：http://yg.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://tz.shxzskj.cn

[T45] Perl：数组遍历
来源：http://np.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://ly.9csxet.cn

[T46] Perl：哈希操作
来源：http://td.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://az.asd995.cn

[T47] Perl：正则捕获
来源：http://hi.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nz.gzmigu.cn

[T48] Perl：正则替换
来源：http://ls.nszjky.cn

$s =~ s/old/new/g;
来源：http://si.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ro.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ee.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://aj.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jt.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ae.asd995.cn

[T51] Scala：Hello World
来源：http://dy.huanxung.cn

println("Hello")
来源：http://qk.gzmigu.cn

[T52] Scala：变量
来源：http://jg.wgjwhj.cn

val a = 1;  var b = 2
来源：http://aa.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://mk.shxzskj.cn

s"值: $b"
来源：http://zq.muxihuayi.cn

[T54] Scala：集合映射
来源：http://ch.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://jg.gzmigu.cn

[T55] Scala：集合过滤
来源：http://ke.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aq.gzmigu.cn

[T56] Scala：样例类
来源：http://yy.newstarts.cn

case class User(name: String, age: Int)
来源：http://nr.szsharing.cn

[T57] Scala：模式匹配
来源：http://id.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ok.jctech888.com.cn

[T58] Scala：函数定义
来源：http://jp.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ys.szsharing.cn

[T59] Scala：循环
来源：http://kv.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://cy.hahajie.cn

[T60] Scala：折叠
来源：http://fd.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nf.szsharing.cn

================================================================================
来源：http://wn.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gc.yuexingan06.cn

================================================================================
来源：http://je.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://nt.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jo.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://oz.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ro.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://vs.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gz.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://au.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uf.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://no.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://yd.hnjuh.cn

[U06] Py：合并两个字典
来源：http://ic.gzmigu.cn

{**a, **b}
来源：http://ru.hahajie.cn

[U07] Py：反转字典键值
来源：http://zy.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://nt.hnjuh.cn

[U08] Py：展平二维列表
来源：http://wo.wgjwhj.cn

[y for x in nested for y in x]
来源：http://hq.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://dk.shxzskj.cn

max(d, key=d.get)
来源：http://gd.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://mv.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dg.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://zy.colortex.cn

(x * 2 for x in arr)
来源：http://ub.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tq.hahajie.cn

Counter(arr).most_common(3)
来源：http://zk.nicolike.cn

[U13] Py：固定长度队列
来源：http://vx.shxzukj.cn

deque(maxlen=10)
来源：http://yu.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://ra.yuntaijiaju.cn

defaultdict(list)
来源：http://sn.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://eu.gzmigu.cn

t = time.perf_counter()
来源：http://bv.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://sq.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ac.newstarts.cn

[U17] Py：初始化日志
来源：http://dq.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fo.nicolike.cn

[U18] Py：预编译正则
来源：http://mw.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://ab.nicolike.cn

[U19] Py：正则替换带回调
来源：http://uz.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wk.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://vs.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://mz.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://pp.nszjky.cn

@contextlib.contextmanager
来源：http://oo.szxytkj.cn

[U22] Py：矩阵转置
来源：http://ez.nszjky.cn

list(zip(*m))
来源：http://vf.nszjky.cn

[U23] Py：分块读取大文件
来源：http://pf.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yb.bjjhwx.cn

[U24] Py：路径操作
来源：http://ao.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://an.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://tm.colortex.cn

csv.DictReader(f)
来源：http://wr.9csxet.cn

[U26] Py：并发下载
来源：http://tq.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pt.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://jl.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://nl.shtwfgs.cn

[U28] Py：类型别名
来源：http://di.shtwfgs.cn

UserId = int
来源：http://dc.chemitech.net.cn

[U29] Py：属性校验
来源：http://jp.shxzskj.cn

@property 与 @x.setter 配合
来源：http://ka.bjjhwx.cn

[U30] Py：数据类
来源：http://bo.yuexingan06.cn

@dataclass(slots=True)
来源：http://rx.gzmigu.cn

[U31] Py：单测
来源：http://tc.521024.cn

python -m pytest -q
来源：http://pl.lnxyls.cn

[U32] Py：代码格式化
来源：http://mm.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://nm.shtwfgs.cn

[U33] Py：打包发布
来源：http://br.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://yh.bjjhwx.cn

[U34] Py：判断编码
来源：http://um.chemitech.net.cn

chardet.detect(raw)
来源：http://vq.lnxyls.cn

[U35] Py：发送邮件
来源：http://ur.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gk.newstarts.cn

[U36] Py：定时任务
来源：http://kc.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://ny.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://yj.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nr.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://hz.hahajie.cn

Path(__file__).resolve().parent
来源：http://hz.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://ao.yuexingan06.cn

sys.stdout.isatty()
来源：http://kv.hahajie.cn

[U40] Py：打印到标准错误
来源：http://fz.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://iy.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://eg.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ea.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://az.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lx.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://ko.shtwfgs.cn

namespace App\Http;
来源：http://rw.szsharing.cn

[U44] PHP：开启严格类型
来源：http://pv.huixiangedu.cn

declare(strict_types=1);
来源：http://cq.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://fm.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ou.shtwfgs.cn

[U46] PHP：可空类型
来源：http://ug.nszjky.cn

?string $name = null
来源：http://da.lnxyls.cn

[U47] PHP：联合类型
来源：http://xl.haigaiapp.cn

int|string $id
来源：http://ps.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://km.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zi.shxzukj.cn

[U49] PHP：只读属性
来源：http://tm.nszjky.cn

public readonly string $name
来源：http://pr.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://jo.shxzukj.cn

public function __construct(private int $id) {}
来源：http://qf.hahajie.cn


<!-- 参考信息 -->