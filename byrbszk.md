代发 wailian999

[S39] C++：自定义比较器排序
来源：http://oe.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ny.jctech888.com.cn

[S40] C++：查找元素
来源：http://iw.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lz.nszjky.cn

[S41] C++：类与构造函数
来源：http://ba.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rx.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://os.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://qz.chemitech.net.cn

[S43] C++：智能指针
来源：http://rh.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://pp.hnjuh.cn

[S44] C++：引用传参
来源：http://ms.521024.cn

void inc(int &x) { ++x; }
来源：http://hz.yuntaijiaju.cn

[S45] C++：lambda
来源：http://gz.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vf.jctech888.com.cn

[S46] C++：函数模板
来源：http://mq.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xa.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://ok.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oc.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://yb.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xz.szsharing.cn

while (std::getline(in, line)) { }
来源：http://em.asd995.cn

[S49] C++：写文件
来源：http://xl.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jq.asd995.cn

[S50] C++：格式化数字
来源：http://xw.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ha.hnjuh.cn

[S51] C++：显式类型转换
来源：http://bp.nicolike.cn

static_cast<double>(a) / b
来源：http://jj.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://fg.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://vs.hahajie.cn

[S53] C++：移动语义
来源：http://zf.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://go.lnxyls.cn

[S54] C++：异常处理
来源：http://ya.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kx.gzmigu.cn

[S55] C++：结构化绑定
来源：http://pb.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ir.huixiangedu.cn

[S56] C++：optional
来源：http://bn.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ki.shxzukj.cn

[S57] C++：编译期常量
来源：http://vl.hahajie.cn

constexpr int N = 10;
来源：http://rn.bookmarksfly.cn

[S58] C++：命名空间
来源：http://wx.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://ew.9csxet.cn

[S59] C++：静态断言
来源：http://yg.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rj.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://jj.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qy.panjiajie.cn

================================================================================
来源：http://ev.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gl.gzmigu.cn

================================================================================
来源：http://up.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://fa.szsharing.cn

println("Hello")
来源：http://ch.9csxet.cn

[T02] Kotlin：变量
来源：http://yi.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mv.colortex.cn

[T03] Kotlin：字符串模板
来源：http://yg.szsharing.cn

"值: $b"
来源：http://ps.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://gr.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://sw.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://jh.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xc.colortex.cn

[T06] Kotlin：集合映射
来源：http://on.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mv.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://kx.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://df.lnxyls.cn

[T08] Kotlin：数据类
来源：http://pd.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://dv.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://zm.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://cu.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ar.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kr.shxzskj.cn

[T11] Kotlin：协程
来源：http://kc.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bw.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://hb.521024.cn

val (a, b) = Pair(1, 2)
来源：http://gt.asd995.cn

[T13] Kotlin：只读 Map
来源：http://fo.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://wm.shxzskj.cn

[T14] Kotlin：循环
来源：http://dy.asd995.cn

for (i in 1..10) println(i)
来源：http://nn.szsharing.cn

[T15] Kotlin：接口
来源：http://fy.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://rr.bjjhwx.cn

[T16] Swift：Hello World
来源：http://sl.panjiajie.cn

print("Hello")
来源：http://ga.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://eo.hnjuh.cn

var a = 1;  let b = 2
来源：http://kz.gzmigu.cn

[T18] Swift：字符串插值
来源：http://li.haigaiapp.cn

"值: \(b)"
来源：http://fo.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://cu.szxytkj.cn

if let n = opt { print(n) }
来源：http://ko.bjjhwx.cn

[T20] Swift：数组操作
来源：http://pn.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qc.yuexingan06.cn

[T21] Swift：遍历
来源：http://yn.szsharing.cn

for x in a { print(x) }
来源：http://mo.chemitech.net.cn

[T22] Swift：字典
来源：http://dd.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vy.shtwfgs.cn

[T23] Swift：函数
来源：http://jm.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tr.muxihuayi.cn

[T24] Swift：闭包
来源：http://el.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fr.szxytkj.cn

[T25] Swift：结构体
来源：http://rm.shxzskj.cn

struct P { var x: Int }
来源：http://nl.hahajie.cn

[T26] Swift：类与重写
来源：http://yh.asd995.cn

class A: Base { override func f() {} }
来源：http://bv.szsharing.cn

[T27] Swift：错误处理
来源：http://rv.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://vo.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://lx.521024.cn

enum Color { case red, green }
来源：http://gb.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://bx.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://qx.haigaiapp.cn

[T30] Swift：协议
来源：http://cj.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://mf.nszjky.cn

[T31] Lua：Hello World
来源：http://vl.jctech888.com.cn

print("Hello")
来源：http://fo.colortex.cn

[T32] Lua：局部变量
来源：http://ra.yuexingan06.cn

local a = 1
来源：http://kc.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://wt.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rr.szxytkj.cn

[T34] Lua：遍历表
来源：http://jp.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lu.wgjwhj.cn

[T35] Lua：字典表
来源：http://fh.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://wk.panjiajie.cn

[T36] Lua：函数
来源：http://sc.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ad.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://bn.hnjuh.cn

"a" .. "b"
来源：http://lu.chemitech.net.cn

[T38] Lua：条件
来源：http://ds.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ug.szsharing.cn

[T39] Lua：模式匹配
来源：http://fr.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://gq.wgjwhj.cn

[T40] Lua：元表
来源：http://bq.nicolike.cn

setmetatable({}, { __index = base })
来源：http://ln.shxzskj.cn

[T41] Perl：Hello World
来源：http://gn.yuexingan06.cn

print "Hello\n";
来源：http://br.shxzukj.cn

[T42] Perl：变量类型
来源：http://yi.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ea.newstarts.cn

[T43] Perl：字符串插值
来源：http://ca.newstarts.cn

"值: $a"
来源：http://fd.nszjky.cn

[T44] Perl：条件
来源：http://hg.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://si.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://vv.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://to.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://ry.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hv.shxzskj.cn

[T47] Perl：正则捕获
来源：http://tu.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oc.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ru.shxzskj.cn

$s =~ s/old/new/g;
来源：http://ra.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ih.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tw.newstarts.cn

[T50] Perl：逐行读文件
来源：http://mo.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sy.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://pv.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://gk.jctech888.com.cn

println("Hello")
来源：http://gz.wgjwhj.cn

[T52] Scala：变量
来源：http://lk.panjiajie.cn

val a = 1;  var b = 2
来源：http://qt.szxytkj.cn

[T53] Scala：字符串插值
来源：http://dy.hahajie.cn

s"值: $b"
来源：http://ia.shxzskj.cn

[T54] Scala：集合映射
来源：http://tx.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ta.9csxet.cn

[T55] Scala：集合过滤
来源：http://yj.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ot.hahajie.cn

[T56] Scala：样例类
来源：http://dq.newstarts.cn

case class User(name: String, age: Int)
来源：http://xu.panjiajie.cn

[T57] Scala：模式匹配
来源：http://mw.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fu.huanxung.cn

[T58] Scala：函数定义
来源：http://pc.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ga.bookmarksfly.cn

[T59] Scala：循环
来源：http://cw.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://ao.asd995.cn

[T60] Scala：折叠
来源：http://xf.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xb.jianghongdianzi.cn

================================================================================
来源：http://mp.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zv.chemitech.net.cn

================================================================================
来源：http://kb.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://nz.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mw.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://ce.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mj.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://va.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fl.asd995.cn

[U04] Py：变量调试打印
来源：http://xs.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oo.newstarts.cn

[U05] Py：列表去重且保序
来源：http://zz.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://gr.hnjuh.cn

[U06] Py：合并两个字典
来源：http://fz.shxzukj.cn

{**a, **b}
来源：http://kg.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://bz.newstarts.cn

{v: k for k, v in d.items()}
来源：http://wb.hnjuh.cn

[U08] Py：展平二维列表
来源：http://mo.huixiangedu.cn

[y for x in nested for y in x]
来源：http://we.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://nk.newstarts.cn

max(d, key=d.get)
来源：http://sd.521024.cn

[U10] Py：按值排序字典
来源：http://lw.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wl.521024.cn

[U11] Py：生成器表达式
来源：http://mq.nszjky.cn

(x * 2 for x in arr)
来源：http://ry.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mm.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://vt.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://rk.shtwfgs.cn

deque(maxlen=10)
来源：http://lw.newstarts.cn

[U14] Py：分组收集到列表
来源：http://ve.haigaiapp.cn

defaultdict(list)
来源：http://ki.huanxung.cn

[U15] Py：高精度计时
来源：http://ld.nicolike.cn

t = time.perf_counter()
来源：http://ix.newstarts.cn

[U16] Py：命令行参数解析
来源：http://us.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fz.gzmigu.cn

[U17] Py：初始化日志
来源：http://tn.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://yi.lnxyls.cn

[U18] Py：预编译正则
来源：http://yo.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://fm.9csxet.cn

[U19] Py：正则替换带回调
来源：http://va.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xj.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ki.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://zg.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://la.yuexingan06.cn

@contextlib.contextmanager
来源：http://nl.panjiajie.cn

[U22] Py：矩阵转置
来源：http://hy.yuntaijiaju.cn

list(zip(*m))
来源：http://kh.newstarts.cn

[U23] Py：分块读取大文件
来源：http://hh.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ir.yuexingan06.cn

[U24] Py：路径操作
来源：http://le.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://od.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://jt.shxzskj.cn

csv.DictReader(f)
来源：http://kw.panjiajie.cn

[U26] Py：并发下载
来源：http://fh.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ud.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://xy.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://dg.huanxung.cn

[U28] Py：类型别名
来源：http://li.521024.cn

UserId = int
来源：http://ub.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://ar.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://eu.wgjwhj.cn

[U30] Py：数据类
来源：http://at.shxzukj.cn

@dataclass(slots=True)
来源：http://lf.newstarts.cn

[U31] Py：单测
来源：http://wm.yuntaijiaju.cn

python -m pytest -q
来源：http://mn.huixiangedu.cn

[U32] Py：代码格式化
来源：http://td.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://qi.huanxung.cn

[U33] Py：打包发布
来源：http://ul.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://pd.hahajie.cn

[U34] Py：判断编码
来源：http://yw.jctech888.com.cn

chardet.detect(raw)
来源：http://ia.nszjky.cn

[U35] Py：发送邮件
来源：http://rd.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ta.shxzukj.cn

[U36] Py：定时任务
来源：http://vv.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://ur.nszjky.cn

[U37] Py：读写 Excel
来源：http://nm.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ga.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://ja.newstarts.cn

Path(__file__).resolve().parent
来源：http://gm.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://gp.muxihuayi.cn

sys.stdout.isatty()
来源：http://oh.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://bd.hnjuh.cn

print("err", file=sys.stderr)
来源：http://lh.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ku.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lk.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://qw.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jk.nicolike.cn

[U43] PHP：声明命名空间
来源：http://kv.chemitech.net.cn

namespace App\Http;
来源：http://ye.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://yi.huanxung.cn

declare(strict_types=1);
来源：http://ca.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://ya.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gy.521024.cn

[U46] PHP：可空类型
来源：http://gg.nszjky.cn

?string $name = null
来源：http://vm.szsharing.cn

[U47] PHP：联合类型
来源：http://nr.szsharing.cn

int|string $id
来源：http://vd.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://ol.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qw.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://to.nszjky.cn

public readonly string $name
来源：http://nj.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://kw.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://hp.bjjhwx.cn

[U51] PHP：数组解构
来源：http://iq.nszjky.cn

[$a, $b] = $arr;
来源：http://aj.9csxet.cn

[U52] PHP：箭头函数
来源：http://lz.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://ja.szsharing.cn

[U53] PHP：空合并运算符
来源：http://uz.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://nd.colortex.cn

[U54] PHP：空安全调用
来源：http://vj.yuntaijiaju.cn

$obj?->method()
来源：http://ep.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://lw.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vg.gzmigu.cn

[U56] PHP：命名参数
来源：http://fu.gzmigu.cn

f(a: 1, b: 2)
来源：http://so.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://ce.yuexingan06.cn

"值: {$a}"
来源：http://oo.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://vp.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sp.hnjuh.cn

[U59] PHP：自定义排序
来源：http://nv.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fq.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://fs.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fp.nicolike.cn

[U61] PHP：正则
来源：http://vs.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kl.9csxet.cn

[U62] PHP：日期对象
来源：http://an.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kg.yuexingan06.cn

[U63] PHP：文件读写
来源：http://hx.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://un.521024.cn

[U64] PHP：目录遍历
来源：http://vi.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://sq.hnjuh.cn


<!-- 参考信息 -->