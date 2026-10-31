代发 wailian999

memset(a, 0, sizeof a);
来源：http://xq.wgjwhj.cn

[S27] C：定义常量
来源：http://fh.lnxyls.cn

const double PI = 3.14159;
来源：http://wj.nicolike.cn

[S28] C：静态变量
来源：http://zw.shxzukj.cn

static int counter = 0;
来源：http://bu.huixinmuqiang.cn

[S29] C：变参函数
来源：http://rj.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hq.colortex.cn

[S30] C：头文件保护
来源：http://wp.shtwfgs.cn

#ifndef X_H
来源：http://ok.yuexingan06.cn

#define X_H
来源：http://td.shxzskj.cn

#endif
来源：http://bx.hnjuh.cn

[S31] C++：Hello World
来源：http://hp.yuntaijiaju.cn

#include <iostream>
来源：http://fg.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://hv.bjjhwx.cn

[S32] C++：字符串
来源：http://cn.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://la.asd995.cn

[S33] C++：vector 增删
来源：http://tm.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ms.szsharing.cn

[S34] C++：遍历 vector
来源：http://pa.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ee.bjjhwx.cn

[S35] C++：map
来源：http://ph.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://my.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://dc.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wx.shxzukj.cn

[S37] C++：set
来源：http://wo.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mf.szsharing.cn

[S38] C++：排序
来源：http://wm.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://vk.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://tb.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ss.huixiangedu.cn

[S40] C++：查找元素
来源：http://ta.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jh.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://ud.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gc.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://yx.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://px.9csxet.cn

[S43] C++：智能指针
来源：http://ne.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://ap.9csxet.cn

[S44] C++：引用传参
来源：http://go.colortex.cn

void inc(int &x) { ++x; }
来源：http://hq.chemitech.net.cn

[S45] C++：lambda
来源：http://zn.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qn.huanxung.cn

[S46] C++：函数模板
来源：http://ta.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uo.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://dg.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xv.521024.cn

[S48] C++：逐行读文件
来源：http://sv.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ah.hahajie.cn

while (std::getline(in, line)) { }
来源：http://fn.asd995.cn

[S49] C++：写文件
来源：http://zt.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yj.gzmigu.cn

[S50] C++：格式化数字
来源：http://ya.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yb.huanxung.cn

[S51] C++：显式类型转换
来源：http://ux.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://il.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://iu.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ha.newstarts.cn

[S53] C++：移动语义
来源：http://xo.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://cm.huanxung.cn

[S54] C++：异常处理
来源：http://ud.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ru.lnxyls.cn

[S55] C++：结构化绑定
来源：http://ra.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rs.nszjky.cn

[S56] C++：optional
来源：http://uz.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ug.9csxet.cn

[S57] C++：编译期常量
来源：http://rq.shxzskj.cn

constexpr int N = 10;
来源：http://gh.muxihuayi.cn

[S58] C++：命名空间
来源：http://mb.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://sj.hnjuh.cn

[S59] C++：静态断言
来源：http://lb.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ch.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://fg.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hp.bjjhwx.cn

================================================================================
来源：http://ew.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wg.hahajie.cn

================================================================================
来源：http://jv.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://ly.huixiangedu.cn

println("Hello")
来源：http://yl.hahajie.cn

[T02] Kotlin：变量
来源：http://qx.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fw.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://zu.9csxet.cn

"值: $b"
来源：http://jo.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://nw.asd995.cn

val n: String? = null;  n?.length
来源：http://le.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://td.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qq.newstarts.cn

[T06] Kotlin：集合映射
来源：http://bj.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ts.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://gz.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wj.521024.cn

[T08] Kotlin：数据类
来源：http://so.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://rm.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://vz.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://hl.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://yn.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gb.shtwfgs.cn

[T11] Kotlin：协程
来源：http://lq.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qi.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://xj.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://zb.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ts.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ux.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://jr.521024.cn

for (i in 1..10) println(i)
来源：http://mk.nicolike.cn

[T15] Kotlin：接口
来源：http://wf.hahajie.cn

interface Shape { fun area(): Double }
来源：http://wo.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://fq.shtwfgs.cn

print("Hello")
来源：http://nm.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://lm.wgjwhj.cn

var a = 1;  let b = 2
来源：http://ln.huanxung.cn

[T18] Swift：字符串插值
来源：http://tc.hahajie.cn

"值: \(b)"
来源：http://ba.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://uk.shxzskj.cn

if let n = opt { print(n) }
来源：http://jl.shtwfgs.cn

[T20] Swift：数组操作
来源：http://ds.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xa.hahajie.cn

[T21] Swift：遍历
来源：http://um.szxytkj.cn

for x in a { print(x) }
来源：http://ov.nicolike.cn

[T22] Swift：字典
来源：http://zx.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ky.muxihuayi.cn

[T23] Swift：函数
来源：http://bs.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cg.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://wz.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nz.panjiajie.cn

[T25] Swift：结构体
来源：http://wh.hahajie.cn

struct P { var x: Int }
来源：http://sh.panjiajie.cn

[T26] Swift：类与重写
来源：http://mz.9csxet.cn

class A: Base { override func f() {} }
来源：http://rd.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ra.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://mh.hnjuh.cn

[T28] Swift：枚举
来源：http://qh.szxytkj.cn

enum Color { case red, green }
来源：http://kj.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://bj.asd995.cn

guard let x = opt else { return }
来源：http://ec.huixiangedu.cn

[T30] Swift：协议
来源：http://us.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://en.szsharing.cn

[T31] Lua：Hello World
来源：http://eu.yuntaijiaju.cn

print("Hello")
来源：http://yv.wgjwhj.cn

[T32] Lua：局部变量
来源：http://lp.9csxet.cn

local a = 1
来源：http://fb.shxzukj.cn

[T33] Lua：表（数组）
来源：http://zl.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uw.panjiajie.cn

[T34] Lua：遍历表
来源：http://qs.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dz.newstarts.cn

[T35] Lua：字典表
来源：http://em.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ls.huanxung.cn

[T36] Lua：函数
来源：http://ha.panjiajie.cn

function add(a, b) return a + b end
来源：http://uy.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://qh.hahajie.cn

"a" .. "b"
来源：http://of.haigaiapp.cn

[T38] Lua：条件
来源：http://ku.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://yz.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://oa.colortex.cn

string.find(s, "%d+")
来源：http://rp.yuntaijiaju.cn

[T40] Lua：元表
来源：http://gl.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://am.gzmigu.cn

[T41] Perl：Hello World
来源：http://as.chemitech.net.cn

print "Hello\n";
来源：http://zu.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://ka.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ks.nszjky.cn

[T43] Perl：字符串插值
来源：http://ge.9csxet.cn

"值: $a"
来源：http://ur.hahajie.cn

[T44] Perl：条件
来源：http://vo.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://sn.hahajie.cn

[T45] Perl：数组遍历
来源：http://ly.521024.cn

for my $x (@arr) { print $x; }
来源：http://oo.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://il.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ji.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://zg.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ut.hnjuh.cn

[T48] Perl：正则替换
来源：http://ea.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://ld.nszjky.cn

[T49] Perl：函数
来源：http://ny.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hq.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ys.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ts.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://bd.shxzukj.cn

[T51] Scala：Hello World
来源：http://rr.gzmigu.cn

println("Hello")
来源：http://es.hahajie.cn

[T52] Scala：变量
来源：http://fa.szxytkj.cn

val a = 1;  var b = 2
来源：http://he.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ba.jianghongdianzi.cn

s"值: $b"
来源：http://bj.wgjwhj.cn

[T54] Scala：集合映射
来源：http://pv.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://wi.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://kk.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dz.panjiajie.cn

[T56] Scala：样例类
来源：http://it.9csxet.cn

case class User(name: String, age: Int)
来源：http://br.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://qu.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ah.shtwfgs.cn

[T58] Scala：函数定义
来源：http://wk.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vn.jctech888.com.cn

[T59] Scala：循环
来源：http://db.521024.cn

for (i <- 1 to 10) println(i)
来源：http://ey.jctech888.com.cn

[T60] Scala：折叠
来源：http://oy.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wp.newstarts.cn

================================================================================
来源：http://mz.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gt.9csxet.cn

================================================================================
来源：http://um.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://bq.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fe.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://wj.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ma.colortex.cn

[U03] Py：加载 .env 配置
来源：http://ke.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://za.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://ut.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vv.9csxet.cn

[U05] Py：列表去重且保序
来源：http://hd.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://ss.hnjuh.cn

[U06] Py：合并两个字典
来源：http://fy.huixiangedu.cn

{**a, **b}
来源：http://sh.asd995.cn

[U07] Py：反转字典键值
来源：http://rg.nszjky.cn

{v: k for k, v in d.items()}
来源：http://zn.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://xr.muxihuayi.cn

[y for x in nested for y in x]
来源：http://sc.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://bk.shxzskj.cn

max(d, key=d.get)
来源：http://gb.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://dj.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ex.nicolike.cn

[U11] Py：生成器表达式
来源：http://ms.colortex.cn

(x * 2 for x in arr)
来源：http://vu.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zr.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://mv.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://xo.nicolike.cn

deque(maxlen=10)
来源：http://jb.asd995.cn

[U14] Py：分组收集到列表
来源：http://tc.bookmarksfly.cn

defaultdict(list)
来源：http://lz.hahajie.cn

[U15] Py：高精度计时
来源：http://yl.wgjwhj.cn

t = time.perf_counter()
来源：http://pz.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://fi.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ya.yuexingan06.cn

[U17] Py：初始化日志
来源：http://ff.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://tf.newstarts.cn

[U18] Py：预编译正则
来源：http://wi.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://wt.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://oy.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fn.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://ro.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://gi.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://np.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://jn.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://xb.bjjhwx.cn

list(zip(*m))
来源：http://ba.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://id.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uv.shxzukj.cn

[U24] Py：路径操作
来源：http://ps.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mq.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://pf.jianghongdianzi.cn

csv.DictReader(f)
来源：http://cy.gzmigu.cn

[U26] Py：并发下载
来源：http://yx.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ej.521024.cn

[U27] Py：异步 HTTP
来源：http://my.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://lx.newstarts.cn

[U28] Py：类型别名
来源：http://jr.bjjhwx.cn

UserId = int
来源：http://ni.colortex.cn

[U29] Py：属性校验
来源：http://hw.panjiajie.cn

@property 与 @x.setter 配合
来源：http://ud.colortex.cn

[U30] Py：数据类
来源：http://ki.9csxet.cn

@dataclass(slots=True)
来源：http://lv.huanxung.cn

[U31] Py：单测
来源：http://mp.huanxung.cn

python -m pytest -q
来源：http://zc.nicolike.cn

[U32] Py：代码格式化
来源：http://st.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://jn.newstarts.cn

[U33] Py：打包发布
来源：http://uh.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://lg.szxytkj.cn

[U34] Py：判断编码
来源：http://le.jianghongdianzi.cn

chardet.detect(raw)
来源：http://ux.huanxung.cn

[U35] Py：发送邮件
来源：http://bh.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xz.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ki.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://te.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://iq.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zw.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://va.lnxyls.cn

Path(__file__).resolve().parent
来源：http://lm.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://ji.newstarts.cn

sys.stdout.isatty()
来源：http://tf.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://xp.521024.cn

print("err", file=sys.stderr)
来源：http://yd.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://rp.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sx.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://om.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ko.nszjky.cn

[U43] PHP：声明命名空间
来源：http://wg.9csxet.cn

namespace App\Http;
来源：http://tu.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://wv.wgjwhj.cn

declare(strict_types=1);
来源：http://bm.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://at.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bs.huanxung.cn

[U46] PHP：可空类型
来源：http://cu.wgjwhj.cn

?string $name = null
来源：http://of.huanxung.cn

[U47] PHP：联合类型
来源：http://eb.wgjwhj.cn

int|string $id
来源：http://yq.szsharing.cn

[U48] PHP：纯枚举
来源：http://kh.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xj.colortex.cn

[U49] PHP：只读属性
来源：http://cs.yuntaijiaju.cn

public readonly string $name
来源：http://ln.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://ef.nicolike.cn

public function __construct(private int $id) {}
来源：http://rs.colortex.cn


<!-- 参考信息 -->