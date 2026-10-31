代发 wailian999

static int counter = 0;
来源：http://jz.gzmigu.cn

[S29] C：变参函数
来源：http://fi.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ok.hnjuh.cn

[S30] C：头文件保护
来源：http://db.bjjhwx.cn

#ifndef X_H
来源：http://uf.gzmigu.cn

#define X_H
来源：http://fn.haigaiapp.cn

#endif
来源：http://hx.gzmigu.cn

[S31] C++：Hello World
来源：http://nt.huanxung.cn

#include <iostream>
来源：http://nn.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://po.szxytkj.cn

[S32] C++：字符串
来源：http://nv.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://rr.panjiajie.cn

[S33] C++：vector 增删
来源：http://kt.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pz.huanxung.cn

[S34] C++：遍历 vector
来源：http://kc.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://js.hahajie.cn

[S35] C++：map
来源：http://lw.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oj.asd995.cn

[S36] C++：unordered_map
来源：http://qb.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xa.szxytkj.cn

[S37] C++：set
来源：http://vr.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yd.colortex.cn

[S38] C++：排序
来源：http://zm.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://iy.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://pn.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qb.panjiajie.cn

[S40] C++：查找元素
来源：http://op.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vz.shxzukj.cn

[S41] C++：类与构造函数
来源：http://le.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://is.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ro.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://ym.colortex.cn

[S43] C++：智能指针
来源：http://hv.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://eh.jctech888.com.cn

[S44] C++：引用传参
来源：http://aw.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ta.nszjky.cn

[S45] C++：lambda
来源：http://wz.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pr.jctech888.com.cn

[S46] C++：函数模板
来源：http://fw.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://va.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://gq.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cc.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ol.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qa.asd995.cn

while (std::getline(in, line)) { }
来源：http://vt.jianghongdianzi.cn

[S49] C++：写文件
来源：http://oy.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nf.szxytkj.cn

[S50] C++：格式化数字
来源：http://cj.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sf.9csxet.cn

[S51] C++：显式类型转换
来源：http://ds.hahajie.cn

static_cast<double>(a) / b
来源：http://np.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://cj.colortex.cn

int size() const noexcept { return n_; }
来源：http://wx.bookmarksfly.cn

[S53] C++：移动语义
来源：http://gp.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://nu.colortex.cn

[S54] C++：异常处理
来源：http://uo.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rz.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://zu.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jp.bookmarksfly.cn

[S56] C++：optional
来源：http://nz.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gs.chemitech.net.cn

[S57] C++：编译期常量
来源：http://ec.shtwfgs.cn

constexpr int N = 10;
来源：http://ch.muxihuayi.cn

[S58] C++：命名空间
来源：http://pe.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://he.szsharing.cn

[S59] C++：静态断言
来源：http://er.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hq.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://at.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ay.lnxyls.cn

================================================================================
来源：http://ot.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jp.bookmarksfly.cn

================================================================================
来源：http://pl.521024.cn

[T01] Kotlin：Hello World
来源：http://zn.shxzukj.cn

println("Hello")
来源：http://zu.bjjhwx.cn

[T02] Kotlin：变量
来源：http://ne.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lf.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://mh.shxzukj.cn

"值: $b"
来源：http://kh.shxzskj.cn

[T04] Kotlin：空安全
来源：http://at.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://vz.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://xj.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fy.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://wh.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bm.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://vk.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hi.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://pj.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://zy.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://gb.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://yv.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://cg.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gy.newstarts.cn

[T11] Kotlin：协程
来源：http://zh.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zm.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://yx.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://wb.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://id.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://xu.haigaiapp.cn

[T14] Kotlin：循环
来源：http://qr.nszjky.cn

for (i in 1..10) println(i)
来源：http://jv.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://mw.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://lg.panjiajie.cn

[T16] Swift：Hello World
来源：http://vb.szsharing.cn

print("Hello")
来源：http://rr.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://vi.bjjhwx.cn

var a = 1;  let b = 2
来源：http://qr.9csxet.cn

[T18] Swift：字符串插值
来源：http://yk.bookmarksfly.cn

"值: \(b)"
来源：http://fc.gzmigu.cn

[T19] Swift：可选绑定
来源：http://ts.shxzukj.cn

if let n = opt { print(n) }
来源：http://kj.szsharing.cn

[T20] Swift：数组操作
来源：http://ri.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kf.jctech888.com.cn

[T21] Swift：遍历
来源：http://uj.wgjwhj.cn

for x in a { print(x) }
来源：http://ug.huixinmuqiang.cn

[T22] Swift：字典
来源：http://qv.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fz.shxzskj.cn

[T23] Swift：函数
来源：http://pi.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tz.shxzskj.cn

[T24] Swift：闭包
来源：http://zh.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ea.gzmigu.cn

[T25] Swift：结构体
来源：http://ta.huixinmuqiang.cn

struct P { var x: Int }
来源：http://ts.9csxet.cn

[T26] Swift：类与重写
来源：http://ia.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://er.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://gh.colortex.cn

do { try f() } catch { print(error) }
来源：http://zc.szsharing.cn

[T28] Swift：枚举
来源：http://jy.nszjky.cn

enum Color { case red, green }
来源：http://ld.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://xw.wgjwhj.cn

guard let x = opt else { return }
来源：http://rn.gzmigu.cn

[T30] Swift：协议
来源：http://ua.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://rv.jctech888.com.cn

[T31] Lua：Hello World
来源：http://kr.jianghongdianzi.cn

print("Hello")
来源：http://ew.lnxyls.cn

[T32] Lua：局部变量
来源：http://gf.huanxung.cn

local a = 1
来源：http://fb.hahajie.cn

[T33] Lua：表（数组）
来源：http://uh.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ni.wgjwhj.cn

[T34] Lua：遍历表
来源：http://pa.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cc.bjjhwx.cn

[T35] Lua：字典表
来源：http://ua.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://mb.shxzskj.cn

[T36] Lua：函数
来源：http://sa.huanxung.cn

function add(a, b) return a + b end
来源：http://vg.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://yn.nicolike.cn

"a" .. "b"
来源：http://sd.shxzskj.cn

[T38] Lua：条件
来源：http://wb.jctech888.com.cn

if x > 0 then print("正") end
来源：http://ot.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://wh.bookmarksfly.cn

string.find(s, "%d+")
来源：http://up.bookmarksfly.cn

[T40] Lua：元表
来源：http://rp.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://vn.shtwfgs.cn

[T41] Perl：Hello World
来源：http://vy.521024.cn

print "Hello\n";
来源：http://cl.szsharing.cn

[T42] Perl：变量类型
来源：http://rg.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kz.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://zc.yuntaijiaju.cn

"值: $a"
来源：http://da.hnjuh.cn

[T44] Perl：条件
来源：http://fv.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://ce.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://eo.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://yq.panjiajie.cn

[T46] Perl：哈希操作
来源：http://sr.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qg.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://bu.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xt.haigaiapp.cn

[T48] Perl：正则替换
来源：http://xs.hahajie.cn

$s =~ s/old/new/g;
来源：http://jq.lnxyls.cn

[T49] Perl：函数
来源：http://sm.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ei.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://jl.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yt.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://sd.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://qt.nicolike.cn

println("Hello")
来源：http://qt.jctech888.com.cn

[T52] Scala：变量
来源：http://cx.jctech888.com.cn

val a = 1;  var b = 2
来源：http://hc.szxytkj.cn

[T53] Scala：字符串插值
来源：http://xe.panjiajie.cn

s"值: $b"
来源：http://lk.huixiangedu.cn

[T54] Scala：集合映射
来源：http://wo.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://cw.asd995.cn

[T55] Scala：集合过滤
来源：http://hk.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wr.bjjhwx.cn

[T56] Scala：样例类
来源：http://ox.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://fy.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://eo.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ma.521024.cn

[T58] Scala：函数定义
来源：http://yg.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xp.muxihuayi.cn

[T59] Scala：循环
来源：http://mq.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://lw.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://bl.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qb.huixinmuqiang.cn

================================================================================
来源：http://yw.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://io.yuntaijiaju.cn

================================================================================
来源：http://xm.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://ex.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://at.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://em.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mj.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://gi.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gw.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://uw.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rq.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://hv.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://gz.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ot.shxzskj.cn

{**a, **b}
来源：http://fw.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://yp.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://eo.lnxyls.cn

[U08] Py：展平二维列表
来源：http://lo.lnxyls.cn

[y for x in nested for y in x]
来源：http://zl.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://so.nszjky.cn

max(d, key=d.get)
来源：http://gb.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://gx.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pz.shxzukj.cn

[U11] Py：生成器表达式
来源：http://gy.nicolike.cn

(x * 2 for x in arr)
来源：http://gt.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://um.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://kl.nszjky.cn

[U13] Py：固定长度队列
来源：http://dd.shxzukj.cn

deque(maxlen=10)
来源：http://lj.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://lh.huanxung.cn

defaultdict(list)
来源：http://ve.jctech888.com.cn

[U15] Py：高精度计时
来源：http://pc.hahajie.cn

t = time.perf_counter()
来源：http://mb.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://ze.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hm.shxzskj.cn

[U17] Py：初始化日志
来源：http://vg.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://au.asd995.cn

[U18] Py：预编译正则
来源：http://cr.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ba.szsharing.cn

[U19] Py：正则替换带回调
来源：http://wm.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jd.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://uv.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://iq.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://wo.muxihuayi.cn

@contextlib.contextmanager
来源：http://si.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://jv.shxzskj.cn

list(zip(*m))
来源：http://rh.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://pv.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yy.szsharing.cn

[U24] Py：路径操作
来源：http://yc.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://if.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://my.hahajie.cn

csv.DictReader(f)
来源：http://wa.szxytkj.cn

[U26] Py：并发下载
来源：http://li.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qt.colortex.cn

[U27] Py：异步 HTTP
来源：http://ri.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://pm.szsharing.cn

[U28] Py：类型别名
来源：http://fv.jctech888.com.cn

UserId = int
来源：http://oj.asd995.cn

[U29] Py：属性校验
来源：http://jq.nicolike.cn

@property 与 @x.setter 配合
来源：http://jv.bjjhwx.cn

[U30] Py：数据类
来源：http://uq.jctech888.com.cn

@dataclass(slots=True)
来源：http://pt.wgjwhj.cn

[U31] Py：单测
来源：http://kl.huixinmuqiang.cn

python -m pytest -q
来源：http://su.muxihuayi.cn

[U32] Py：代码格式化
来源：http://mc.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ee.newstarts.cn

[U33] Py：打包发布
来源：http://ha.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://ar.bookmarksfly.cn

[U34] Py：判断编码
来源：http://ym.shtwfgs.cn

chardet.detect(raw)
来源：http://un.shxzskj.cn

[U35] Py：发送邮件
来源：http://eh.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cr.521024.cn

[U36] Py：定时任务
来源：http://pn.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://ck.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://lq.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ms.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://il.huanxung.cn

Path(__file__).resolve().parent
来源：http://af.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://ld.hnjuh.cn

sys.stdout.isatty()
来源：http://dp.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://gp.szxytkj.cn

print("err", file=sys.stderr)
来源：http://dc.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://su.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ua.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://bk.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bj.huanxung.cn

[U43] PHP：声明命名空间
来源：http://jq.jianghongdianzi.cn

namespace App\Http;
来源：http://ia.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://nq.muxihuayi.cn

declare(strict_types=1);
来源：http://fm.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ao.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vk.newstarts.cn

[U46] PHP：可空类型
来源：http://nt.colortex.cn

?string $name = null
来源：http://go.asd995.cn

[U47] PHP：联合类型
来源：http://fz.huixiangedu.cn

int|string $id
来源：http://ox.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://fv.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nu.yuexingan06.cn

[U49] PHP：只读属性
来源：http://ed.nszjky.cn

public readonly string $name
来源：http://kb.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://xi.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://yl.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://do.shxzskj.cn

[$a, $b] = $arr;
来源：http://yk.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://bf.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://pu.gzmigu.cn


<!-- 参考信息 -->