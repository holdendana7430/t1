代发 wailian999

[S37] C++：set
来源：http://tr.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cv.szxytkj.cn

[S38] C++：排序
来源：http://xk.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://lo.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://mw.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qt.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://br.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bh.colortex.cn

[S41] C++：类与构造函数
来源：http://hz.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yf.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://lp.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://bo.bookmarksfly.cn

[S43] C++：智能指针
来源：http://xw.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://po.szxytkj.cn

[S44] C++：引用传参
来源：http://cr.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://en.newstarts.cn

[S45] C++：lambda
来源：http://mw.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ye.panjiajie.cn

[S46] C++：函数模板
来源：http://np.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xz.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://jy.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bx.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://wd.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ck.szsharing.cn

while (std::getline(in, line)) { }
来源：http://wd.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ja.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sv.muxihuayi.cn

[S50] C++：格式化数字
来源：http://fb.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qn.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://vy.haigaiapp.cn

static_cast<double>(a) / b
来源：http://vm.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://nr.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://ud.szxytkj.cn

[S53] C++：移动语义
来源：http://eq.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://kt.521024.cn

[S54] C++：异常处理
来源：http://uw.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qa.nicolike.cn

[S55] C++：结构化绑定
来源：http://gn.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kd.huixiangedu.cn

[S56] C++：optional
来源：http://ee.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ac.gzmigu.cn

[S57] C++：编译期常量
来源：http://qo.hahajie.cn

constexpr int N = 10;
来源：http://lr.hahajie.cn

[S58] C++：命名空间
来源：http://nk.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://xt.szsharing.cn

[S59] C++：静态断言
来源：http://ph.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vm.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ge.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cb.jianghongdianzi.cn

================================================================================
来源：http://my.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.521024.cn

================================================================================
来源：http://tr.newstarts.cn

[T01] Kotlin：Hello World
来源：http://hy.nicolike.cn

println("Hello")
来源：http://xq.haigaiapp.cn

[T02] Kotlin：变量
来源：http://so.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ny.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://mr.nszjky.cn

"值: $b"
来源：http://me.asd995.cn

[T04] Kotlin：空安全
来源：http://jo.shxzukj.cn

val n: String? = null;  n?.length
来源：http://mg.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://fu.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qd.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://ww.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hn.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://xu.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pa.panjiajie.cn

[T08] Kotlin：数据类
来源：http://jn.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://ti.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://eb.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://qo.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://uf.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yl.newstarts.cn

[T11] Kotlin：协程
来源：http://hu.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dz.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://ta.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://gp.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://pe.521024.cn

val m = mapOf("a" to 1)
来源：http://vs.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://jc.colortex.cn

for (i in 1..10) println(i)
来源：http://cq.hnjuh.cn

[T15] Kotlin：接口
来源：http://ox.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://py.huixiangedu.cn

[T16] Swift：Hello World
来源：http://wy.hnjuh.cn

print("Hello")
来源：http://st.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://dx.panjiajie.cn

var a = 1;  let b = 2
来源：http://gd.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://ph.asd995.cn

"值: \(b)"
来源：http://xo.nszjky.cn

[T19] Swift：可选绑定
来源：http://mt.yuexingan06.cn

if let n = opt { print(n) }
来源：http://tj.jctech888.com.cn

[T20] Swift：数组操作
来源：http://sj.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dd.jctech888.com.cn

[T21] Swift：遍历
来源：http://gu.gzmigu.cn

for x in a { print(x) }
来源：http://gm.nicolike.cn

[T22] Swift：字典
来源：http://pk.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fg.szsharing.cn

[T23] Swift：函数
来源：http://tg.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ea.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ep.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fa.newstarts.cn

[T25] Swift：结构体
来源：http://vg.huanxung.cn

struct P { var x: Int }
来源：http://ud.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://gr.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://oy.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://sg.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://jh.newstarts.cn

[T28] Swift：枚举
来源：http://od.nicolike.cn

enum Color { case red, green }
来源：http://ss.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://bh.szsharing.cn

guard let x = opt else { return }
来源：http://gm.yuexingan06.cn

[T30] Swift：协议
来源：http://or.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://ei.jctech888.com.cn

[T31] Lua：Hello World
来源：http://gw.newstarts.cn

print("Hello")
来源：http://ga.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://ex.nicolike.cn

local a = 1
来源：http://po.panjiajie.cn

[T33] Lua：表（数组）
来源：http://qh.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ro.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ca.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://it.shxzukj.cn

[T35] Lua：字典表
来源：http://yj.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://pk.muxihuayi.cn

[T36] Lua：函数
来源：http://qc.szsharing.cn

function add(a, b) return a + b end
来源：http://jh.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://cs.jctech888.com.cn

"a" .. "b"
来源：http://zg.bookmarksfly.cn

[T38] Lua：条件
来源：http://uf.hahajie.cn

if x > 0 then print("正") end
来源：http://uq.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://xr.colortex.cn

string.find(s, "%d+")
来源：http://wd.szxytkj.cn

[T40] Lua：元表
来源：http://bj.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://xa.wgjwhj.cn

[T41] Perl：Hello World
来源：http://bs.nszjky.cn

print "Hello\n";
来源：http://gd.nicolike.cn

[T42] Perl：变量类型
来源：http://wu.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oc.szsharing.cn

[T43] Perl：字符串插值
来源：http://cp.wgjwhj.cn

"值: $a"
来源：http://ey.newstarts.cn

[T44] Perl：条件
来源：http://ds.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://jj.gzmigu.cn

[T45] Perl：数组遍历
来源：http://op.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://mg.shxzskj.cn

[T46] Perl：哈希操作
来源：http://ox.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pn.szxytkj.cn

[T47] Perl：正则捕获
来源：http://lp.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cy.asd995.cn

[T48] Perl：正则替换
来源：http://gj.nicolike.cn

$s =~ s/old/new/g;
来源：http://yi.shtwfgs.cn

[T49] Perl：函数
来源：http://dn.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xg.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://kw.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ss.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ig.hnjuh.cn

[T51] Scala：Hello World
来源：http://re.9csxet.cn

println("Hello")
来源：http://ts.chemitech.net.cn

[T52] Scala：变量
来源：http://ip.shxzukj.cn

val a = 1;  var b = 2
来源：http://zl.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://yn.9csxet.cn

s"值: $b"
来源：http://gt.9csxet.cn

[T54] Scala：集合映射
来源：http://qo.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://pc.panjiajie.cn

[T55] Scala：集合过滤
来源：http://mk.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ik.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://zg.nicolike.cn

case class User(name: String, age: Int)
来源：http://mq.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://tg.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lo.newstarts.cn

[T58] Scala：函数定义
来源：http://rz.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hx.chemitech.net.cn

[T59] Scala：循环
来源：http://pa.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://im.shtwfgs.cn

[T60] Scala：折叠
来源：http://gn.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pr.asd995.cn

================================================================================
来源：http://my.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ur.hahajie.cn

================================================================================
来源：http://wy.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://wx.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mg.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://zj.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zx.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://bj.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://av.shxzskj.cn

[U04] Py：变量调试打印
来源：http://af.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ac.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://sn.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://cm.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ny.huixiangedu.cn

{**a, **b}
来源：http://ju.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://at.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://gq.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://np.lnxyls.cn

[y for x in nested for y in x]
来源：http://ki.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://is.yuntaijiaju.cn

max(d, key=d.get)
来源：http://iw.9csxet.cn

[U10] Py：按值排序字典
来源：http://fg.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wj.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://hk.521024.cn

(x * 2 for x in arr)
来源：http://pr.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dv.lnxyls.cn

Counter(arr).most_common(3)
来源：http://sn.szsharing.cn

[U13] Py：固定长度队列
来源：http://qf.bjjhwx.cn

deque(maxlen=10)
来源：http://pu.newstarts.cn

[U14] Py：分组收集到列表
来源：http://lt.9csxet.cn

defaultdict(list)
来源：http://fh.shxzskj.cn

[U15] Py：高精度计时
来源：http://jk.huixinmuqiang.cn

t = time.perf_counter()
来源：http://rq.asd995.cn

[U16] Py：命令行参数解析
来源：http://tz.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yq.9csxet.cn

[U17] Py：初始化日志
来源：http://cl.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://af.wgjwhj.cn

[U18] Py：预编译正则
来源：http://tn.szsharing.cn

pat = re.compile(r"\d+")
来源：http://av.nszjky.cn

[U19] Py：正则替换带回调
来源：http://pi.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mr.hahajie.cn

[U20] Py：缓存函数结果
来源：http://sa.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://fp.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://bk.shtwfgs.cn

@contextlib.contextmanager
来源：http://py.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://cq.yuexingan06.cn

list(zip(*m))
来源：http://pz.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://en.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zo.szsharing.cn

[U24] Py：路径操作
来源：http://do.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://af.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://dh.huixiangedu.cn

csv.DictReader(f)
来源：http://uk.panjiajie.cn

[U26] Py：并发下载
来源：http://zt.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vj.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://zq.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://tz.nszjky.cn

[U28] Py：类型别名
来源：http://bx.huixinmuqiang.cn

UserId = int
来源：http://mc.lnxyls.cn

[U29] Py：属性校验
来源：http://gp.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://ie.yuntaijiaju.cn

[U30] Py：数据类
来源：http://yn.szxytkj.cn

@dataclass(slots=True)
来源：http://ku.9csxet.cn

[U31] Py：单测
来源：http://du.panjiajie.cn

python -m pytest -q
来源：http://xt.chemitech.net.cn

[U32] Py：代码格式化
来源：http://my.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ba.shxzukj.cn

[U33] Py：打包发布
来源：http://jj.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://pa.nicolike.cn

[U34] Py：判断编码
来源：http://hs.huixiangedu.cn

chardet.detect(raw)
来源：http://tz.panjiajie.cn

[U35] Py：发送邮件
来源：http://zq.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qs.panjiajie.cn

[U36] Py：定时任务
来源：http://kq.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://jt.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://gu.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jx.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://uk.shxzukj.cn

Path(__file__).resolve().parent
来源：http://kj.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://hn.yuexingan06.cn

sys.stdout.isatty()
来源：http://lo.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://ze.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ih.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://vu.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nl.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://dd.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ms.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://ch.bookmarksfly.cn

namespace App\Http;
来源：http://qh.szsharing.cn

[U44] PHP：开启严格类型
来源：http://hs.yuexingan06.cn

declare(strict_types=1);
来源：http://ng.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://na.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jc.huanxung.cn

[U46] PHP：可空类型
来源：http://pn.jianghongdianzi.cn

?string $name = null
来源：http://cx.haigaiapp.cn

[U47] PHP：联合类型
来源：http://gm.yuntaijiaju.cn

int|string $id
来源：http://dk.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://zu.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qk.yuexingan06.cn

[U49] PHP：只读属性
来源：http://fd.huixiangedu.cn

public readonly string $name
来源：http://ww.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://dp.nicolike.cn

public function __construct(private int $id) {}
来源：http://gu.huanxung.cn

[U51] PHP：数组解构
来源：http://mf.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://vh.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://ca.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://rv.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://bd.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://sl.huanxung.cn

[U54] PHP：空安全调用
来源：http://va.lnxyls.cn

$obj?->method()
来源：http://fl.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://qc.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xx.asd995.cn

[U56] PHP：命名参数
来源：http://nw.szsharing.cn

f(a: 1, b: 2)
来源：http://de.shxzskj.cn

[U57] PHP：字符串插值
来源：http://qp.yuntaijiaju.cn

"值: {$a}"
来源：http://bv.colortex.cn

[U58] PHP：数组三件套
来源：http://bb.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://em.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://th.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wk.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://av.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ho.hahajie.cn

[U61] PHP：正则
来源：http://ki.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hr.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://ad.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xf.lnxyls.cn


<!-- 参考信息 -->