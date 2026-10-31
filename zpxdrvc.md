代发 wailian999

[S37] C++：set
来源：http://ks.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iv.szxytkj.cn

[S38] C++：排序
来源：http://aw.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://nv.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://vb.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://do.yuexingan06.cn

[S40] C++：查找元素
来源：http://zi.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mb.shxzukj.cn

[S41] C++：类与构造函数
来源：http://sc.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pi.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://mh.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://uq.yuexingan06.cn

[S43] C++：智能指针
来源：http://me.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://je.lnxyls.cn

[S44] C++：引用传参
来源：http://wl.hahajie.cn

void inc(int &x) { ++x; }
来源：http://zf.szsharing.cn

[S45] C++：lambda
来源：http://md.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://av.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://yx.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pm.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://bv.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xv.shxzukj.cn

[S48] C++：逐行读文件
来源：http://qq.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ki.colortex.cn

while (std::getline(in, line)) { }
来源：http://ig.yuntaijiaju.cn

[S49] C++：写文件
来源：http://jk.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://du.szsharing.cn

[S50] C++：格式化数字
来源：http://dc.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ib.9csxet.cn

[S51] C++：显式类型转换
来源：http://uc.jctech888.com.cn

static_cast<double>(a) / b
来源：http://qq.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://ly.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://hd.shtwfgs.cn

[S53] C++：移动语义
来源：http://cj.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://nl.lnxyls.cn

[S54] C++：异常处理
来源：http://fh.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bd.szxytkj.cn

[S55] C++：结构化绑定
来源：http://tl.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gh.muxihuayi.cn

[S56] C++：optional
来源：http://co.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nt.9csxet.cn

[S57] C++：编译期常量
来源：http://mc.huixinmuqiang.cn

constexpr int N = 10;
来源：http://tx.shxzukj.cn

[S58] C++：命名空间
来源：http://ut.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://oq.huixiangedu.cn

[S59] C++：静态断言
来源：http://sh.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gg.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://wc.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gt.panjiajie.cn

================================================================================
来源：http://rv.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ni.colortex.cn

================================================================================
来源：http://bb.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://ky.hnjuh.cn

println("Hello")
来源：http://sq.shxzskj.cn

[T02] Kotlin：变量
来源：http://eu.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pd.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://yj.huixiangedu.cn

"值: $b"
来源：http://rg.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://yt.9csxet.cn

val n: String? = null;  n?.length
来源：http://uh.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://zl.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://li.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://nq.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mc.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://og.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fq.lnxyls.cn

[T08] Kotlin：数据类
来源：http://re.colortex.cn

data class User(val name: String, val age: Int)
来源：http://yv.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://ym.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://oo.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://sd.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xl.gzmigu.cn

[T11] Kotlin：协程
来源：http://le.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vt.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://jm.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://it.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://rl.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://nu.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://kb.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://sl.szsharing.cn

[T15] Kotlin：接口
来源：http://he.9csxet.cn

interface Shape { fun area(): Double }
来源：http://do.wgjwhj.cn

[T16] Swift：Hello World
来源：http://xq.asd995.cn

print("Hello")
来源：http://nl.newstarts.cn

[T17] Swift：变量与常量
来源：http://by.9csxet.cn

var a = 1;  let b = 2
来源：http://pd.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://et.lnxyls.cn

"值: \(b)"
来源：http://be.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://qp.asd995.cn

if let n = opt { print(n) }
来源：http://ue.panjiajie.cn

[T20] Swift：数组操作
来源：http://mb.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wa.shxzukj.cn

[T21] Swift：遍历
来源：http://yr.shtwfgs.cn

for x in a { print(x) }
来源：http://oe.chemitech.net.cn

[T22] Swift：字典
来源：http://nw.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ye.szsharing.cn

[T23] Swift：函数
来源：http://ea.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tk.shxzukj.cn

[T24] Swift：闭包
来源：http://we.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cv.shxzskj.cn

[T25] Swift：结构体
来源：http://ce.hahajie.cn

struct P { var x: Int }
来源：http://vn.jctech888.com.cn

[T26] Swift：类与重写
来源：http://yz.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://hp.hnjuh.cn

[T27] Swift：错误处理
来源：http://cf.nicolike.cn

do { try f() } catch { print(error) }
来源：http://on.9csxet.cn

[T28] Swift：枚举
来源：http://da.muxihuayi.cn

enum Color { case red, green }
来源：http://mr.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://am.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://us.gzmigu.cn

[T30] Swift：协议
来源：http://ft.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://aw.colortex.cn

[T31] Lua：Hello World
来源：http://sf.panjiajie.cn

print("Hello")
来源：http://ib.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://vc.newstarts.cn

local a = 1
来源：http://dl.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://uy.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://di.nszjky.cn

[T34] Lua：遍历表
来源：http://dj.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xs.szsharing.cn

[T35] Lua：字典表
来源：http://lr.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://fk.asd995.cn

[T36] Lua：函数
来源：http://qs.szsharing.cn

function add(a, b) return a + b end
来源：http://lv.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://yf.colortex.cn

"a" .. "b"
来源：http://zl.jctech888.com.cn

[T38] Lua：条件
来源：http://jg.szsharing.cn

if x > 0 then print("正") end
来源：http://bm.lnxyls.cn

[T39] Lua：模式匹配
来源：http://fq.chemitech.net.cn

string.find(s, "%d+")
来源：http://qi.yuexingan06.cn

[T40] Lua：元表
来源：http://vr.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://zz.asd995.cn

[T41] Perl：Hello World
来源：http://xc.yuntaijiaju.cn

print "Hello\n";
来源：http://ua.yuexingan06.cn

[T42] Perl：变量类型
来源：http://ts.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ue.panjiajie.cn

[T43] Perl：字符串插值
来源：http://xp.wgjwhj.cn

"值: $a"
来源：http://st.wgjwhj.cn

[T44] Perl：条件
来源：http://pz.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://fb.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://hh.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://su.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://fa.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ce.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://er.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vv.shxzskj.cn

[T48] Perl：正则替换
来源：http://dc.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://yp.bjjhwx.cn

[T49] Perl：函数
来源：http://ns.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://os.9csxet.cn

[T50] Perl：逐行读文件
来源：http://op.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pj.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ta.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://he.newstarts.cn

println("Hello")
来源：http://xo.wgjwhj.cn

[T52] Scala：变量
来源：http://mi.nszjky.cn

val a = 1;  var b = 2
来源：http://ue.lnxyls.cn

[T53] Scala：字符串插值
来源：http://xu.bookmarksfly.cn

s"值: $b"
来源：http://ry.haigaiapp.cn

[T54] Scala：集合映射
来源：http://po.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://fy.hnjuh.cn

[T55] Scala：集合过滤
来源：http://hr.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ey.9csxet.cn

[T56] Scala：样例类
来源：http://pg.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://ic.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://ay.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ub.newstarts.cn

[T58] Scala：函数定义
来源：http://mb.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://py.yuexingan06.cn

[T59] Scala：循环
来源：http://le.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://gl.hnjuh.cn

[T60] Scala：折叠
来源：http://ya.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://up.szxytkj.cn

================================================================================
来源：http://oi.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fu.shtwfgs.cn

================================================================================
来源：http://mo.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://pz.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ch.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://yt.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oa.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://kt.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ew.newstarts.cn

[U04] Py：变量调试打印
来源：http://oa.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rc.hahajie.cn

[U05] Py：列表去重且保序
来源：http://zn.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://xj.szxytkj.cn

[U06] Py：合并两个字典
来源：http://hi.hahajie.cn

{**a, **b}
来源：http://sd.szsharing.cn

[U07] Py：反转字典键值
来源：http://nn.huanxung.cn

{v: k for k, v in d.items()}
来源：http://pz.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://hl.chemitech.net.cn

[y for x in nested for y in x]
来源：http://qx.521024.cn

[U09] Py：字典取最大值的键
来源：http://hu.haigaiapp.cn

max(d, key=d.get)
来源：http://ld.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://uy.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ud.huanxung.cn

[U11] Py：生成器表达式
来源：http://zx.shtwfgs.cn

(x * 2 for x in arr)
来源：http://dm.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xt.newstarts.cn

Counter(arr).most_common(3)
来源：http://nk.gzmigu.cn

[U13] Py：固定长度队列
来源：http://qm.521024.cn

deque(maxlen=10)
来源：http://wn.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://ly.huixinmuqiang.cn

defaultdict(list)
来源：http://ve.panjiajie.cn

[U15] Py：高精度计时
来源：http://ta.yuexingan06.cn

t = time.perf_counter()
来源：http://ti.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://yr.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dl.shxzukj.cn

[U17] Py：初始化日志
来源：http://og.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://li.muxihuayi.cn

[U18] Py：预编译正则
来源：http://by.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://qw.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://il.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uu.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ev.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://le.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://py.hnjuh.cn

@contextlib.contextmanager
来源：http://by.asd995.cn

[U22] Py：矩阵转置
来源：http://nr.shxzskj.cn

list(zip(*m))
来源：http://uc.521024.cn

[U23] Py：分块读取大文件
来源：http://nv.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ve.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://qx.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zg.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://gs.jctech888.com.cn

csv.DictReader(f)
来源：http://wa.szsharing.cn

[U26] Py：并发下载
来源：http://ii.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gc.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://in.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://id.haigaiapp.cn

[U28] Py：类型别名
来源：http://zc.muxihuayi.cn

UserId = int
来源：http://cw.bookmarksfly.cn

[U29] Py：属性校验
来源：http://qn.gzmigu.cn

@property 与 @x.setter 配合
来源：http://vc.newstarts.cn

[U30] Py：数据类
来源：http://gq.lnxyls.cn

@dataclass(slots=True)
来源：http://qu.newstarts.cn

[U31] Py：单测
来源：http://tf.huanxung.cn

python -m pytest -q
来源：http://il.lnxyls.cn

[U32] Py：代码格式化
来源：http://li.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://hf.hahajie.cn

[U33] Py：打包发布
来源：http://rj.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://jt.szsharing.cn

[U34] Py：判断编码
来源：http://xz.hnjuh.cn

chardet.detect(raw)
来源：http://ul.newstarts.cn

[U35] Py：发送邮件
来源：http://cm.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wh.szsharing.cn

[U36] Py：定时任务
来源：http://oy.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://zd.colortex.cn

[U37] Py：读写 Excel
来源：http://qw.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uw.521024.cn

[U38] Py：获取脚本所在目录
来源：http://lg.gzmigu.cn

Path(__file__).resolve().parent
来源：http://yu.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://nl.asd995.cn

sys.stdout.isatty()
来源：http://au.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://xx.9csxet.cn

print("err", file=sys.stderr)
来源：http://lx.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ym.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zb.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://qd.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ke.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://qh.huixinmuqiang.cn

namespace App\Http;
来源：http://kt.szsharing.cn

[U44] PHP：开启严格类型
来源：http://qe.yuntaijiaju.cn

declare(strict_types=1);
来源：http://tt.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://hm.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nv.panjiajie.cn

[U46] PHP：可空类型
来源：http://us.huanxung.cn

?string $name = null
来源：http://ir.lnxyls.cn

[U47] PHP：联合类型
来源：http://jh.muxihuayi.cn

int|string $id
来源：http://yd.lnxyls.cn

[U48] PHP：纯枚举
来源：http://bj.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://td.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://po.szxytkj.cn

public readonly string $name
来源：http://iu.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://oa.9csxet.cn

public function __construct(private int $id) {}
来源：http://rs.9csxet.cn

[U51] PHP：数组解构
来源：http://kr.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://dj.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://yu.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://ns.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ku.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://yn.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://bw.huixinmuqiang.cn

$obj?->method()
来源：http://ou.nicolike.cn

[U55] PHP：match 表达式
来源：http://yr.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ni.huanxung.cn

[U56] PHP：命名参数
来源：http://gy.gzmigu.cn

f(a: 1, b: 2)
来源：http://ka.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://ck.jianghongdianzi.cn

"值: {$a}"
来源：http://bo.newstarts.cn

[U58] PHP：数组三件套
来源：http://wo.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rq.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://im.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ah.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://ke.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xp.szsharing.cn

[U61] PHP：正则
来源：http://jt.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hi.hahajie.cn

[U62] PHP：日期对象
来源：http://bm.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kr.haigaiapp.cn


<!-- 参考信息 -->