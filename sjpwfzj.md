代发 wailian999

[S39] C++：自定义比较器排序
来源：http://by.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mg.haigaiapp.cn

[S40] C++：查找元素
来源：http://ii.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cg.newstarts.cn

[S41] C++：类与构造函数
来源：http://fn.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tn.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://vw.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://cs.colortex.cn

[S43] C++：智能指针
来源：http://mn.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://vz.yuexingan06.cn

[S44] C++：引用传参
来源：http://zv.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://dw.haigaiapp.cn

[S45] C++：lambda
来源：http://kk.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zz.hnjuh.cn

[S46] C++：函数模板
来源：http://gy.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cg.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://xk.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://al.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://xg.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jx.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://vf.jctech888.com.cn

[S49] C++：写文件
来源：http://gg.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pl.colortex.cn

[S50] C++：格式化数字
来源：http://jd.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kp.gzmigu.cn

[S51] C++：显式类型转换
来源：http://tg.yuexingan06.cn

static_cast<double>(a) / b
来源：http://dv.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://nb.521024.cn

int size() const noexcept { return n_; }
来源：http://xa.jctech888.com.cn

[S53] C++：移动语义
来源：http://dc.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fh.hahajie.cn

[S54] C++：异常处理
来源：http://lc.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jc.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://pa.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xw.shtwfgs.cn

[S56] C++：optional
来源：http://yt.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vh.szxytkj.cn

[S57] C++：编译期常量
来源：http://pw.haigaiapp.cn

constexpr int N = 10;
来源：http://gk.muxihuayi.cn

[S58] C++：命名空间
来源：http://ox.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://py.521024.cn

[S59] C++：静态断言
来源：http://ji.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jd.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://uy.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://az.haigaiapp.cn

================================================================================
来源：http://nu.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ih.hnjuh.cn

================================================================================
来源：http://hj.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://od.nicolike.cn

println("Hello")
来源：http://nh.colortex.cn

[T02] Kotlin：变量
来源：http://wm.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bo.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://kh.hahajie.cn

"值: $b"
来源：http://cn.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://jg.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://yz.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://so.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xw.asd995.cn

[T06] Kotlin：集合映射
来源：http://gb.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://py.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://ox.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bs.nszjky.cn

[T08] Kotlin：数据类
来源：http://lk.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://nr.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://yc.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://sy.nszjky.cn

[T10] Kotlin：默认参数
来源：http://jt.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nn.shtwfgs.cn

[T11] Kotlin：协程
来源：http://uj.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ne.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://fn.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://kp.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://ub.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://te.gzmigu.cn

[T14] Kotlin：循环
来源：http://rp.hnjuh.cn

for (i in 1..10) println(i)
来源：http://kq.shxzukj.cn

[T15] Kotlin：接口
来源：http://pw.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://qf.nszjky.cn

[T16] Swift：Hello World
来源：http://mb.jctech888.com.cn

print("Hello")
来源：http://li.lnxyls.cn

[T17] Swift：变量与常量
来源：http://lu.huanxung.cn

var a = 1;  let b = 2
来源：http://gs.hnjuh.cn

[T18] Swift：字符串插值
来源：http://mr.haigaiapp.cn

"值: \(b)"
来源：http://dz.panjiajie.cn

[T19] Swift：可选绑定
来源：http://lj.szsharing.cn

if let n = opt { print(n) }
来源：http://im.shtwfgs.cn

[T20] Swift：数组操作
来源：http://dr.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hp.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://eg.szxytkj.cn

for x in a { print(x) }
来源：http://vz.panjiajie.cn

[T22] Swift：字典
来源：http://ji.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bw.hahajie.cn

[T23] Swift：函数
来源：http://vs.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cd.chemitech.net.cn

[T24] Swift：闭包
来源：http://pu.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://de.asd995.cn

[T25] Swift：结构体
来源：http://cz.muxihuayi.cn

struct P { var x: Int }
来源：http://uw.colortex.cn

[T26] Swift：类与重写
来源：http://ln.shxzukj.cn

class A: Base { override func f() {} }
来源：http://pa.jctech888.com.cn

[T27] Swift：错误处理
来源：http://mz.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://cz.panjiajie.cn

[T28] Swift：枚举
来源：http://zh.lnxyls.cn

enum Color { case red, green }
来源：http://hv.colortex.cn

[T29] Swift：guard 提前返回
来源：http://rd.shxzskj.cn

guard let x = opt else { return }
来源：http://bn.yuexingan06.cn

[T30] Swift：协议
来源：http://vz.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://nc.nszjky.cn

[T31] Lua：Hello World
来源：http://ts.nicolike.cn

print("Hello")
来源：http://lg.shxzukj.cn

[T32] Lua：局部变量
来源：http://qp.jianghongdianzi.cn

local a = 1
来源：http://ja.colortex.cn

[T33] Lua：表（数组）
来源：http://pq.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jp.asd995.cn

[T34] Lua：遍历表
来源：http://rs.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rw.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://ji.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://qj.shtwfgs.cn

[T36] Lua：函数
来源：http://ia.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ax.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://ge.panjiajie.cn

"a" .. "b"
来源：http://bk.wgjwhj.cn

[T38] Lua：条件
来源：http://lu.szsharing.cn

if x > 0 then print("正") end
来源：http://kl.newstarts.cn

[T39] Lua：模式匹配
来源：http://io.chemitech.net.cn

string.find(s, "%d+")
来源：http://yu.hnjuh.cn

[T40] Lua：元表
来源：http://yt.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://rf.muxihuayi.cn

[T41] Perl：Hello World
来源：http://xf.shxzukj.cn

print "Hello\n";
来源：http://sk.shxzskj.cn

[T42] Perl：变量类型
来源：http://wu.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wd.huanxung.cn

[T43] Perl：字符串插值
来源：http://as.yuexingan06.cn

"值: $a"
来源：http://fx.nicolike.cn

[T44] Perl：条件
来源：http://jr.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://zf.shxzskj.cn

[T45] Perl：数组遍历
来源：http://pp.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://el.nszjky.cn

[T46] Perl：哈希操作
来源：http://bv.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nu.hahajie.cn

[T47] Perl：正则捕获
来源：http://tq.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jq.9csxet.cn

[T48] Perl：正则替换
来源：http://au.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://jq.bookmarksfly.cn

[T49] Perl：函数
来源：http://hn.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://me.521024.cn

[T50] Perl：逐行读文件
来源：http://eq.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tb.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://wf.yuexingan06.cn

[T51] Scala：Hello World
来源：http://rf.huanxung.cn

println("Hello")
来源：http://kb.asd995.cn

[T52] Scala：变量
来源：http://dz.nszjky.cn

val a = 1;  var b = 2
来源：http://cu.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://ty.nszjky.cn

s"值: $b"
来源：http://ga.huanxung.cn

[T54] Scala：集合映射
来源：http://kd.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://lq.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://zj.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bk.9csxet.cn

[T56] Scala：样例类
来源：http://pc.hnjuh.cn

case class User(name: String, age: Int)
来源：http://lq.9csxet.cn

[T57] Scala：模式匹配
来源：http://vt.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mk.shtwfgs.cn

[T58] Scala：函数定义
来源：http://il.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wc.muxihuayi.cn

[T59] Scala：循环
来源：http://sx.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://ov.newstarts.cn

[T60] Scala：折叠
来源：http://qm.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ha.panjiajie.cn

================================================================================
来源：http://mb.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bp.newstarts.cn

================================================================================
来源：http://jn.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://pp.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cy.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://ca.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sl.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://mf.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ah.nicolike.cn

[U04] Py：变量调试打印
来源：http://bz.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dy.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ty.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://ez.hahajie.cn

[U06] Py：合并两个字典
来源：http://uz.lnxyls.cn

{**a, **b}
来源：http://sa.nszjky.cn

[U07] Py：反转字典键值
来源：http://lu.nicolike.cn

{v: k for k, v in d.items()}
来源：http://xk.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://do.gzmigu.cn

[y for x in nested for y in x]
来源：http://nc.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://sc.szsharing.cn

max(d, key=d.get)
来源：http://dl.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://tj.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sz.newstarts.cn

[U11] Py：生成器表达式
来源：http://xq.nicolike.cn

(x * 2 for x in arr)
来源：http://py.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dr.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://dq.lnxyls.cn

[U13] Py：固定长度队列
来源：http://pz.szsharing.cn

deque(maxlen=10)
来源：http://bo.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ou.lnxyls.cn

defaultdict(list)
来源：http://ku.huixiangedu.cn

[U15] Py：高精度计时
来源：http://hh.521024.cn

t = time.perf_counter()
来源：http://cg.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://pp.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ea.jctech888.com.cn

[U17] Py：初始化日志
来源：http://uu.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://uw.newstarts.cn

[U18] Py：预编译正则
来源：http://zs.nszjky.cn

pat = re.compile(r"\d+")
来源：http://lr.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://yg.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ov.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://ex.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ek.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://jb.9csxet.cn

@contextlib.contextmanager
来源：http://mo.9csxet.cn

[U22] Py：矩阵转置
来源：http://gg.lnxyls.cn

list(zip(*m))
来源：http://nq.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ii.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yy.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://sw.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pn.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://ju.jctech888.com.cn

csv.DictReader(f)
来源：http://bm.nicolike.cn

[U26] Py：并发下载
来源：http://zt.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eg.asd995.cn

[U27] Py：异步 HTTP
来源：http://it.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://sk.lnxyls.cn

[U28] Py：类型别名
来源：http://il.9csxet.cn

UserId = int
来源：http://xi.nszjky.cn

[U29] Py：属性校验
来源：http://hn.nicolike.cn

@property 与 @x.setter 配合
来源：http://ys.wgjwhj.cn

[U30] Py：数据类
来源：http://ia.gzmigu.cn

@dataclass(slots=True)
来源：http://di.colortex.cn

[U31] Py：单测
来源：http://lk.shtwfgs.cn

python -m pytest -q
来源：http://kt.wgjwhj.cn

[U32] Py：代码格式化
来源：http://qh.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://zb.hnjuh.cn

[U33] Py：打包发布
来源：http://pu.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://vh.huanxung.cn

[U34] Py：判断编码
来源：http://ke.521024.cn

chardet.detect(raw)
来源：http://mx.wgjwhj.cn

[U35] Py：发送邮件
来源：http://de.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rj.huixiangedu.cn

[U36] Py：定时任务
来源：http://ow.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://bh.panjiajie.cn

[U37] Py：读写 Excel
来源：http://bj.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://in.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://uk.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://mv.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://oj.szxytkj.cn

sys.stdout.isatty()
来源：http://db.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://lh.newstarts.cn

print("err", file=sys.stderr)
来源：http://jd.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://is.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tl.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://kf.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tf.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://ui.hahajie.cn

namespace App\Http;
来源：http://lp.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://ol.muxihuayi.cn

declare(strict_types=1);
来源：http://zt.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://to.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.shxzskj.cn

[U46] PHP：可空类型
来源：http://qd.shtwfgs.cn

?string $name = null
来源：http://jf.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://nz.521024.cn

int|string $id
来源：http://td.nicolike.cn

[U48] PHP：纯枚举
来源：http://ds.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rq.hahajie.cn

[U49] PHP：只读属性
来源：http://nb.bjjhwx.cn

public readonly string $name
来源：http://am.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://xz.nicolike.cn

public function __construct(private int $id) {}
来源：http://ii.shxzukj.cn

[U51] PHP：数组解构
来源：http://xo.bjjhwx.cn

[$a, $b] = $arr;
来源：http://mr.shxzskj.cn

[U52] PHP：箭头函数
来源：http://de.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://tz.nszjky.cn

[U53] PHP：空合并运算符
来源：http://nf.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://xx.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://tj.gzmigu.cn

$obj?->method()
来源：http://vw.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://gl.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://px.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://og.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://xf.521024.cn

[U57] PHP：字符串插值
来源：http://cp.panjiajie.cn

"值: {$a}"
来源：http://as.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://ro.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pm.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://rq.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ms.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://eu.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://go.huanxung.cn

[U61] PHP：正则
来源：http://eb.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://da.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://jg.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uf.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ge.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ia.szxytkj.cn

[U64] PHP：目录遍历
来源：http://sf.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ui.lnxyls.cn


<!-- 参考信息 -->