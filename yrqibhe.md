代发 wailian999

static int counter = 0;
来源：http://ac.shxzukj.cn

[S29] C：变参函数
来源：http://ko.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zd.szsharing.cn

[S30] C：头文件保护
来源：http://hx.jctech888.com.cn

#ifndef X_H
来源：http://pi.colortex.cn

#define X_H
来源：http://ik.wgjwhj.cn

#endif
来源：http://kw.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://sh.jctech888.com.cn

#include <iostream>
来源：http://ym.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://zh.huixiangedu.cn

[S32] C++：字符串
来源：http://fj.colortex.cn

std::string s = "hi";  s += "!";
来源：http://is.asd995.cn

[S33] C++：vector 增删
来源：http://ef.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iy.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ra.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wx.lnxyls.cn

[S35] C++：map
来源：http://eb.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kv.huanxung.cn

[S36] C++：unordered_map
来源：http://zj.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ye.yuntaijiaju.cn

[S37] C++：set
来源：http://uy.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zl.asd995.cn

[S38] C++：排序
来源：http://mb.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://gu.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://bp.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gc.huanxung.cn

[S40] C++：查找元素
来源：http://mu.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mf.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://vh.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zw.521024.cn

[S42] C++：继承与虚函数
来源：http://cd.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://mn.hnjuh.cn

[S43] C++：智能指针
来源：http://vd.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://ex.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://mn.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://cy.jctech888.com.cn

[S45] C++：lambda
来源：http://tx.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zn.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ec.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uo.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://la.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yt.colortex.cn

[S48] C++：逐行读文件
来源：http://pu.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bo.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://sd.9csxet.cn

[S49] C++：写文件
来源：http://pj.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xj.szxytkj.cn

[S50] C++：格式化数字
来源：http://li.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ux.gzmigu.cn

[S51] C++：显式类型转换
来源：http://hq.panjiajie.cn

static_cast<double>(a) / b
来源：http://te.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://sg.newstarts.cn

int size() const noexcept { return n_; }
来源：http://oc.nszjky.cn

[S53] C++：移动语义
来源：http://la.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://rf.nicolike.cn

[S54] C++：异常处理
来源：http://oe.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bw.asd995.cn

[S55] C++：结构化绑定
来源：http://zf.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vq.9csxet.cn

[S56] C++：optional
来源：http://fq.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vj.huixiangedu.cn

[S57] C++：编译期常量
来源：http://fe.chemitech.net.cn

constexpr int N = 10;
来源：http://br.haigaiapp.cn

[S58] C++：命名空间
来源：http://py.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://yv.bookmarksfly.cn

[S59] C++：静态断言
来源：http://dw.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uz.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://vh.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mp.asd995.cn

================================================================================
来源：http://ck.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mt.bjjhwx.cn

================================================================================
来源：http://up.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://uw.huixiangedu.cn

println("Hello")
来源：http://ll.shxzukj.cn

[T02] Kotlin：变量
来源：http://vz.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://au.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://jk.colortex.cn

"值: $b"
来源：http://ll.huanxung.cn

[T04] Kotlin：空安全
来源：http://se.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ie.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://sv.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qm.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://wx.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fu.colortex.cn

[T07] Kotlin：集合过滤
来源：http://kz.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jg.521024.cn

[T08] Kotlin：数据类
来源：http://mh.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://fh.asd995.cn

[T09] Kotlin：扩展函数
来源：http://dc.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://vy.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://zd.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ax.gzmigu.cn

[T11] Kotlin：协程
来源：http://kq.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ip.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://to.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://od.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://lc.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://zl.colortex.cn

[T14] Kotlin：循环
来源：http://rv.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://kp.shxzskj.cn

[T15] Kotlin：接口
来源：http://sx.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://pt.9csxet.cn

[T16] Swift：Hello World
来源：http://in.asd995.cn

print("Hello")
来源：http://mf.szxytkj.cn

[T17] Swift：变量与常量
来源：http://jy.shtwfgs.cn

var a = 1;  let b = 2
来源：http://rg.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://mt.szsharing.cn

"值: \(b)"
来源：http://hx.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://wl.521024.cn

if let n = opt { print(n) }
来源：http://oo.hahajie.cn

[T20] Swift：数组操作
来源：http://yh.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gs.hnjuh.cn

[T21] Swift：遍历
来源：http://sd.yuexingan06.cn

for x in a { print(x) }
来源：http://wt.colortex.cn

[T22] Swift：字典
来源：http://gh.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rx.szxytkj.cn

[T23] Swift：函数
来源：http://lc.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ig.huanxung.cn

[T24] Swift：闭包
来源：http://tc.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zb.jctech888.com.cn

[T25] Swift：结构体
来源：http://ff.lnxyls.cn

struct P { var x: Int }
来源：http://ac.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://mr.newstarts.cn

class A: Base { override func f() {} }
来源：http://me.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://cz.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://tw.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://gc.shtwfgs.cn

enum Color { case red, green }
来源：http://mc.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://of.asd995.cn

guard let x = opt else { return }
来源：http://ey.wgjwhj.cn

[T30] Swift：协议
来源：http://vw.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://pe.hnjuh.cn

[T31] Lua：Hello World
来源：http://wl.yuntaijiaju.cn

print("Hello")
来源：http://rp.newstarts.cn

[T32] Lua：局部变量
来源：http://ds.yuntaijiaju.cn

local a = 1
来源：http://cs.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://ad.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tg.szsharing.cn

[T34] Lua：遍历表
来源：http://tr.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tg.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://nk.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://pc.wgjwhj.cn

[T36] Lua：函数
来源：http://ka.bjjhwx.cn

function add(a, b) return a + b end
来源：http://ds.9csxet.cn

[T37] Lua：字符串拼接
来源：http://yz.jianghongdianzi.cn

"a" .. "b"
来源：http://lk.huixiangedu.cn

[T38] Lua：条件
来源：http://bo.szsharing.cn

if x > 0 then print("正") end
来源：http://tw.nicolike.cn

[T39] Lua：模式匹配
来源：http://ry.lnxyls.cn

string.find(s, "%d+")
来源：http://og.wgjwhj.cn

[T40] Lua：元表
来源：http://oa.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://gk.shxzskj.cn

[T41] Perl：Hello World
来源：http://sg.huixinmuqiang.cn

print "Hello\n";
来源：http://dy.szsharing.cn

[T42] Perl：变量类型
来源：http://ws.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uz.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://gy.hahajie.cn

"值: $a"
来源：http://uh.gzmigu.cn

[T44] Perl：条件
来源：http://xe.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ci.panjiajie.cn

[T45] Perl：数组遍历
来源：http://od.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://xh.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://cp.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nw.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://tv.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wn.yuexingan06.cn

[T48] Perl：正则替换
来源：http://xr.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://tz.asd995.cn

[T49] Perl：函数
来源：http://uj.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mz.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://gt.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://to.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://qn.9csxet.cn

[T51] Scala：Hello World
来源：http://ti.huanxung.cn

println("Hello")
来源：http://mi.colortex.cn

[T52] Scala：变量
来源：http://vd.bjjhwx.cn

val a = 1;  var b = 2
来源：http://ow.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://au.huixinmuqiang.cn

s"值: $b"
来源：http://xb.521024.cn

[T54] Scala：集合映射
来源：http://ni.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://kc.9csxet.cn

[T55] Scala：集合过滤
来源：http://yj.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nz.huixiangedu.cn

[T56] Scala：样例类
来源：http://sk.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://dl.nszjky.cn

[T57] Scala：模式匹配
来源：http://hz.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://js.shtwfgs.cn

[T58] Scala：函数定义
来源：http://tg.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sc.yuexingan06.cn

[T59] Scala：循环
来源：http://ya.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://hn.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://kj.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bo.colortex.cn

================================================================================
来源：http://ia.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fn.huanxung.cn

================================================================================
来源：http://ip.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://pl.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zr.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://kr.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ek.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://zu.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ei.hnjuh.cn

[U04] Py：变量调试打印
来源：http://xy.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pu.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://gg.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://rf.shxzukj.cn

[U06] Py：合并两个字典
来源：http://js.szsharing.cn

{**a, **b}
来源：http://jh.nszjky.cn

[U07] Py：反转字典键值
来源：http://ae.newstarts.cn

{v: k for k, v in d.items()}
来源：http://gw.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://ek.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://cr.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://oy.nicolike.cn

max(d, key=d.get)
来源：http://wx.shxzskj.cn

[U10] Py：按值排序字典
来源：http://cv.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ib.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://iw.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://am.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hu.szsharing.cn

Counter(arr).most_common(3)
来源：http://rn.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://pk.wgjwhj.cn

deque(maxlen=10)
来源：http://cy.nszjky.cn

[U14] Py：分组收集到列表
来源：http://sa.huanxung.cn

defaultdict(list)
来源：http://um.9csxet.cn

[U15] Py：高精度计时
来源：http://wg.huixiangedu.cn

t = time.perf_counter()
来源：http://yi.colortex.cn

[U16] Py：命令行参数解析
来源：http://jw.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rp.shxzskj.cn

[U17] Py：初始化日志
来源：http://ny.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://sx.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ih.nicolike.cn

pat = re.compile(r"\d+")
来源：http://vg.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://dz.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://op.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://ft.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://ye.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://hj.newstarts.cn

@contextlib.contextmanager
来源：http://js.asd995.cn

[U22] Py：矩阵转置
来源：http://ld.lnxyls.cn

list(zip(*m))
来源：http://te.colortex.cn

[U23] Py：分块读取大文件
来源：http://xt.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ru.colortex.cn

[U24] Py：路径操作
来源：http://fa.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yh.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://kf.gzmigu.cn

csv.DictReader(f)
来源：http://oo.shxzukj.cn

[U26] Py：并发下载
来源：http://we.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qb.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://fq.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://px.szxytkj.cn

[U28] Py：类型别名
来源：http://he.jctech888.com.cn

UserId = int
来源：http://pq.jctech888.com.cn

[U29] Py：属性校验
来源：http://yx.hnjuh.cn

@property 与 @x.setter 配合
来源：http://kc.lnxyls.cn

[U30] Py：数据类
来源：http://wo.jctech888.com.cn

@dataclass(slots=True)
来源：http://tz.huixinmuqiang.cn

[U31] Py：单测
来源：http://eu.jctech888.com.cn

python -m pytest -q
来源：http://wu.chemitech.net.cn

[U32] Py：代码格式化
来源：http://pm.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://ks.521024.cn

[U33] Py：打包发布
来源：http://ma.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://cz.newstarts.cn

[U34] Py：判断编码
来源：http://hr.hnjuh.cn

chardet.detect(raw)
来源：http://vr.colortex.cn

[U35] Py：发送邮件
来源：http://yf.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jz.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://ml.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://nu.gzmigu.cn

[U37] Py：读写 Excel
来源：http://ld.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iw.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://mo.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://cc.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://dq.haigaiapp.cn

sys.stdout.isatty()
来源：http://lo.521024.cn

[U40] Py：打印到标准错误
来源：http://me.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://iw.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://tz.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ud.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://mb.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ac.nszjky.cn

[U43] PHP：声明命名空间
来源：http://ck.chemitech.net.cn

namespace App\Http;
来源：http://yp.huanxung.cn

[U44] PHP：开启严格类型
来源：http://gr.9csxet.cn

declare(strict_types=1);
来源：http://dp.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://yc.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iz.huanxung.cn

[U46] PHP：可空类型
来源：http://gh.lnxyls.cn

?string $name = null
来源：http://tr.nicolike.cn

[U47] PHP：联合类型
来源：http://oc.huixinmuqiang.cn

int|string $id
来源：http://yv.shxzskj.cn

[U48] PHP：纯枚举
来源：http://rs.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jh.gzmigu.cn

[U49] PHP：只读属性
来源：http://if.asd995.cn

public readonly string $name
来源：http://ms.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://cl.szsharing.cn

public function __construct(private int $id) {}
来源：http://cy.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://er.shxzukj.cn

[$a, $b] = $arr;
来源：http://uc.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://oh.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://nv.muxihuayi.cn


<!-- 参考信息 -->