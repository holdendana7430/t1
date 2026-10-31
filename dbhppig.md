代发 wailian999

static int counter = 0;
来源：http://ep.szsharing.cn

[S29] C：变参函数
来源：http://gz.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sm.shtwfgs.cn

[S30] C：头文件保护
来源：http://za.nicolike.cn

#ifndef X_H
来源：http://gy.nszjky.cn

#define X_H
来源：http://su.asd995.cn

#endif
来源：http://we.panjiajie.cn

[S31] C++：Hello World
来源：http://zl.shxzskj.cn

#include <iostream>
来源：http://wv.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://bg.gzmigu.cn

[S32] C++：字符串
来源：http://uu.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ju.yuexingan06.cn

[S33] C++：vector 增删
来源：http://kv.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tn.shxzukj.cn

[S34] C++：遍历 vector
来源：http://kv.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://lp.chemitech.net.cn

[S35] C++：map
来源：http://sm.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://es.newstarts.cn

[S36] C++：unordered_map
来源：http://di.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fd.haigaiapp.cn

[S37] C++：set
来源：http://eq.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qd.gzmigu.cn

[S38] C++：排序
来源：http://ju.asd995.cn

std::sort(v.begin(), v.end());
来源：http://no.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ie.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://am.chemitech.net.cn

[S40] C++：查找元素
来源：http://qt.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uj.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://fg.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rh.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://mw.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://wg.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://zq.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://bs.521024.cn

[S44] C++：引用传参
来源：http://hn.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://dz.huixinmuqiang.cn

[S45] C++：lambda
来源：http://eu.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mk.szxytkj.cn

[S46] C++：函数模板
来源：http://az.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ac.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://if.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fa.hnjuh.cn

[S48] C++：逐行读文件
来源：http://xz.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rm.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://tg.haigaiapp.cn

[S49] C++：写文件
来源：http://hw.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nt.asd995.cn

[S50] C++：格式化数字
来源：http://ek.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yh.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ka.hahajie.cn

static_cast<double>(a) / b
来源：http://ln.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://lf.nszjky.cn

int size() const noexcept { return n_; }
来源：http://bs.wgjwhj.cn

[S53] C++：移动语义
来源：http://fb.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://lu.jctech888.com.cn

[S54] C++：异常处理
来源：http://ek.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sx.panjiajie.cn

[S55] C++：结构化绑定
来源：http://lv.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kk.shxzskj.cn

[S56] C++：optional
来源：http://nl.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gc.shtwfgs.cn

[S57] C++：编译期常量
来源：http://pi.lnxyls.cn

constexpr int N = 10;
来源：http://dj.nicolike.cn

[S58] C++：命名空间
来源：http://pr.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://qf.panjiajie.cn

[S59] C++：静态断言
来源：http://lu.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bq.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://af.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xs.nicolike.cn

================================================================================
来源：http://qq.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://go.gzmigu.cn

================================================================================
来源：http://bf.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://zi.shxzukj.cn

println("Hello")
来源：http://cb.hnjuh.cn

[T02] Kotlin：变量
来源：http://tk.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://et.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://vt.huixinmuqiang.cn

"值: $b"
来源：http://oc.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://rm.szxytkj.cn

val n: String? = null;  n?.length
来源：http://ts.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://vv.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ol.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://px.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ui.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://jw.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gh.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://ye.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://yz.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://wz.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://kx.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://hj.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kp.haigaiapp.cn

[T11] Kotlin：协程
来源：http://wz.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ph.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://pi.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://cv.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://es.521024.cn

val m = mapOf("a" to 1)
来源：http://vh.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://ni.521024.cn

for (i in 1..10) println(i)
来源：http://pe.chemitech.net.cn

[T15] Kotlin：接口
来源：http://vh.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://rg.yuexingan06.cn

[T16] Swift：Hello World
来源：http://lc.asd995.cn

print("Hello")
来源：http://vo.shxzukj.cn

[T17] Swift：变量与常量
来源：http://fz.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ah.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://js.9csxet.cn

"值: \(b)"
来源：http://pu.hahajie.cn

[T19] Swift：可选绑定
来源：http://wh.jctech888.com.cn

if let n = opt { print(n) }
来源：http://ig.szxytkj.cn

[T20] Swift：数组操作
来源：http://st.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pd.gzmigu.cn

[T21] Swift：遍历
来源：http://ig.panjiajie.cn

for x in a { print(x) }
来源：http://ki.asd995.cn

[T22] Swift：字典
来源：http://ep.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://se.chemitech.net.cn

[T23] Swift：函数
来源：http://jn.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nm.hahajie.cn

[T24] Swift：闭包
来源：http://fk.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wi.bookmarksfly.cn

[T25] Swift：结构体
来源：http://lv.huanxung.cn

struct P { var x: Int }
来源：http://lt.newstarts.cn

[T26] Swift：类与重写
来源：http://ss.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://qj.shtwfgs.cn

[T27] Swift：错误处理
来源：http://tr.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://kf.panjiajie.cn

[T28] Swift：枚举
来源：http://uw.huixiangedu.cn

enum Color { case red, green }
来源：http://gq.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://ji.colortex.cn

guard let x = opt else { return }
来源：http://fy.gzmigu.cn

[T30] Swift：协议
来源：http://hg.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://sl.panjiajie.cn

[T31] Lua：Hello World
来源：http://di.huixinmuqiang.cn

print("Hello")
来源：http://qv.gzmigu.cn

[T32] Lua：局部变量
来源：http://jo.szxytkj.cn

local a = 1
来源：http://ex.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://bk.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gj.9csxet.cn

[T34] Lua：遍历表
来源：http://fv.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nn.lnxyls.cn

[T35] Lua：字典表
来源：http://dd.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://is.yuexingan06.cn

[T36] Lua：函数
来源：http://jj.shxzukj.cn

function add(a, b) return a + b end
来源：http://lc.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://rp.szsharing.cn

"a" .. "b"
来源：http://ac.muxihuayi.cn

[T38] Lua：条件
来源：http://ga.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://jg.colortex.cn

[T39] Lua：模式匹配
来源：http://az.nszjky.cn

string.find(s, "%d+")
来源：http://nc.colortex.cn

[T40] Lua：元表
来源：http://xn.huanxung.cn

setmetatable({}, { __index = base })
来源：http://lc.shtwfgs.cn

[T41] Perl：Hello World
来源：http://cs.hahajie.cn

print "Hello\n";
来源：http://ln.gzmigu.cn

[T42] Perl：变量类型
来源：http://qg.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://va.nszjky.cn

[T43] Perl：字符串插值
来源：http://je.huixinmuqiang.cn

"值: $a"
来源：http://lw.yuexingan06.cn

[T44] Perl：条件
来源：http://ou.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://hx.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://qb.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://oa.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://qy.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ba.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://ug.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gm.gzmigu.cn

[T48] Perl：正则替换
来源：http://as.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://ws.panjiajie.cn

[T49] Perl：函数
来源：http://jk.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kw.newstarts.cn

[T50] Perl：逐行读文件
来源：http://mx.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jk.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://yh.shtwfgs.cn

[T51] Scala：Hello World
来源：http://sj.haigaiapp.cn

println("Hello")
来源：http://ib.gzmigu.cn

[T52] Scala：变量
来源：http://px.lnxyls.cn

val a = 1;  var b = 2
来源：http://in.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://ib.huanxung.cn

s"值: $b"
来源：http://je.haigaiapp.cn

[T54] Scala：集合映射
来源：http://nl.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://ry.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://fy.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eg.jctech888.com.cn

[T56] Scala：样例类
来源：http://ke.newstarts.cn

case class User(name: String, age: Int)
来源：http://vn.shxzskj.cn

[T57] Scala：模式匹配
来源：http://ak.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://af.newstarts.cn

[T58] Scala：函数定义
来源：http://my.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wr.yuntaijiaju.cn

[T59] Scala：循环
来源：http://hi.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://xt.wgjwhj.cn

[T60] Scala：折叠
来源：http://vq.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eo.jctech888.com.cn

================================================================================
来源：http://sd.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bh.9csxet.cn

================================================================================
来源：http://oz.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://mj.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ls.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ny.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jh.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://by.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lh.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://za.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yn.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://zv.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://ne.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ol.shxzskj.cn

{**a, **b}
来源：http://kw.gzmigu.cn

[U07] Py：反转字典键值
来源：http://jh.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://lj.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://cf.szxytkj.cn

[y for x in nested for y in x]
来源：http://da.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://nw.gzmigu.cn

max(d, key=d.get)
来源：http://gs.panjiajie.cn

[U10] Py：按值排序字典
来源：http://gh.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cs.szxytkj.cn

[U11] Py：生成器表达式
来源：http://ii.szsharing.cn

(x * 2 for x in arr)
来源：http://er.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tq.szsharing.cn

Counter(arr).most_common(3)
来源：http://jr.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://di.jctech888.com.cn

deque(maxlen=10)
来源：http://eg.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://bo.chemitech.net.cn

defaultdict(list)
来源：http://aa.jctech888.com.cn

[U15] Py：高精度计时
来源：http://rr.nszjky.cn

t = time.perf_counter()
来源：http://nu.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://ps.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yw.shxzskj.cn

[U17] Py：初始化日志
来源：http://ns.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://wm.chemitech.net.cn

[U18] Py：预编译正则
来源：http://gf.colortex.cn

pat = re.compile(r"\d+")
来源：http://lg.newstarts.cn

[U19] Py：正则替换带回调
来源：http://uw.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hm.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://dp.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://xj.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ts.lnxyls.cn

@contextlib.contextmanager
来源：http://qw.9csxet.cn

[U22] Py：矩阵转置
来源：http://dl.yuexingan06.cn

list(zip(*m))
来源：http://vd.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://mx.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ur.panjiajie.cn

[U24] Py：路径操作
来源：http://hh.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zk.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://bo.yuexingan06.cn

csv.DictReader(f)
来源：http://cb.jctech888.com.cn

[U26] Py：并发下载
来源：http://wb.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://on.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ic.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://wo.shtwfgs.cn

[U28] Py：类型别名
来源：http://by.newstarts.cn

UserId = int
来源：http://oa.521024.cn

[U29] Py：属性校验
来源：http://qh.lnxyls.cn

@property 与 @x.setter 配合
来源：http://mo.colortex.cn

[U30] Py：数据类
来源：http://gp.yuexingan06.cn

@dataclass(slots=True)
来源：http://on.nszjky.cn

[U31] Py：单测
来源：http://dq.yuntaijiaju.cn

python -m pytest -q
来源：http://vw.shxzskj.cn

[U32] Py：代码格式化
来源：http://xy.9csxet.cn

ruff format . && ruff check --fix .
来源：http://pr.muxihuayi.cn

[U33] Py：打包发布
来源：http://wj.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://wb.shtwfgs.cn

[U34] Py：判断编码
来源：http://oq.yuntaijiaju.cn

chardet.detect(raw)
来源：http://us.nicolike.cn

[U35] Py：发送邮件
来源：http://ul.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yn.lnxyls.cn

[U36] Py：定时任务
来源：http://ko.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://lv.szxytkj.cn

[U37] Py：读写 Excel
来源：http://gp.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ox.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://ow.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://nj.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://xr.huixiangedu.cn

sys.stdout.isatty()
来源：http://lk.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://el.nicolike.cn

print("err", file=sys.stderr)
来源：http://js.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://ku.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vu.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://ox.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ir.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://zq.gzmigu.cn

namespace App\Http;
来源：http://fs.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://we.shtwfgs.cn

declare(strict_types=1);
来源：http://oj.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://mb.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.chemitech.net.cn

[U46] PHP：可空类型
来源：http://el.shxzskj.cn

?string $name = null
来源：http://bc.panjiajie.cn

[U47] PHP：联合类型
来源：http://bn.huixinmuqiang.cn

int|string $id
来源：http://yf.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://at.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://op.shxzukj.cn

[U49] PHP：只读属性
来源：http://gl.panjiajie.cn

public readonly string $name
来源：http://dw.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://io.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://wr.wgjwhj.cn

[U51] PHP：数组解构
来源：http://cj.yuexingan06.cn

[$a, $b] = $arr;
来源：http://sq.shxzukj.cn

[U52] PHP：箭头函数
来源：http://hk.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://jv.bookmarksfly.cn


<!-- 参考信息 -->