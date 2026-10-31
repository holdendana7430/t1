代发 wailian999

[S37] C++：set
来源：http://we.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ti.hahajie.cn

[S38] C++：排序
来源：http://dn.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://gi.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://ol.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oh.szsharing.cn

[S40] C++：查找元素
来源：http://mv.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yg.gzmigu.cn

[S41] C++：类与构造函数
来源：http://qd.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fj.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://cu.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://ri.huanxung.cn

[S43] C++：智能指针
来源：http://ct.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://to.muxihuayi.cn

[S44] C++：引用传参
来源：http://jo.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://yp.bookmarksfly.cn

[S45] C++：lambda
来源：http://ep.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tg.gzmigu.cn

[S46] C++：函数模板
来源：http://hm.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kp.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://us.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gf.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://ll.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rb.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://dv.huanxung.cn

[S49] C++：写文件
来源：http://ix.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://om.panjiajie.cn

[S50] C++：格式化数字
来源：http://nn.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ah.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://co.shtwfgs.cn

static_cast<double>(a) / b
来源：http://vr.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://mb.nicolike.cn

int size() const noexcept { return n_; }
来源：http://hx.bjjhwx.cn

[S53] C++：移动语义
来源：http://ao.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://sv.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://pd.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iz.521024.cn

[S55] C++：结构化绑定
来源：http://lr.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fz.muxihuayi.cn

[S56] C++：optional
来源：http://xp.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gg.panjiajie.cn

[S57] C++：编译期常量
来源：http://ji.shxzukj.cn

constexpr int N = 10;
来源：http://ua.jctech888.com.cn

[S58] C++：命名空间
来源：http://wp.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://oe.muxihuayi.cn

[S59] C++：静态断言
来源：http://wl.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qb.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://uq.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zo.hahajie.cn

================================================================================
来源：http://zj.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xh.bjjhwx.cn

================================================================================
来源：http://ca.hahajie.cn

[T01] Kotlin：Hello World
来源：http://hr.shxzukj.cn

println("Hello")
来源：http://lc.hnjuh.cn

[T02] Kotlin：变量
来源：http://pq.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ve.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://hm.hahajie.cn

"值: $b"
来源：http://qt.newstarts.cn

[T04] Kotlin：空安全
来源：http://sl.hahajie.cn

val n: String? = null;  n?.length
来源：http://sv.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://vo.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xm.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://bv.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ph.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://sw.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xk.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://cy.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://gv.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://df.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://fs.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://cb.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kh.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://xq.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gg.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://em.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://lr.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://dk.9csxet.cn

val m = mapOf("a" to 1)
来源：http://ob.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://kw.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://mo.hahajie.cn

[T15] Kotlin：接口
来源：http://lx.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://zf.bjjhwx.cn

[T16] Swift：Hello World
来源：http://ey.muxihuayi.cn

print("Hello")
来源：http://on.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://ov.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://gx.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://sf.huixinmuqiang.cn

"值: \(b)"
来源：http://gt.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://eb.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://cm.huanxung.cn

[T20] Swift：数组操作
来源：http://sq.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ag.huanxung.cn

[T21] Swift：遍历
来源：http://iw.yuexingan06.cn

for x in a { print(x) }
来源：http://wb.huixinmuqiang.cn

[T22] Swift：字典
来源：http://mg.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yr.9csxet.cn

[T23] Swift：函数
来源：http://wl.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nv.muxihuayi.cn

[T24] Swift：闭包
来源：http://ao.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://in.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://pr.jianghongdianzi.cn

struct P { var x: Int }
来源：http://bt.shtwfgs.cn

[T26] Swift：类与重写
来源：http://mw.szxytkj.cn

class A: Base { override func f() {} }
来源：http://vm.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://fd.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://fq.chemitech.net.cn

[T28] Swift：枚举
来源：http://ay.wgjwhj.cn

enum Color { case red, green }
来源：http://nr.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://gf.hahajie.cn

guard let x = opt else { return }
来源：http://mz.huixiangedu.cn

[T30] Swift：协议
来源：http://ln.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://uu.521024.cn

[T31] Lua：Hello World
来源：http://nl.colortex.cn

print("Hello")
来源：http://wv.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://lx.newstarts.cn

local a = 1
来源：http://ol.shxzskj.cn

[T33] Lua：表（数组）
来源：http://ea.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bn.panjiajie.cn

[T34] Lua：遍历表
来源：http://zt.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dk.jctech888.com.cn

[T35] Lua：字典表
来源：http://ml.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://zs.nszjky.cn

[T36] Lua：函数
来源：http://ww.wgjwhj.cn

function add(a, b) return a + b end
来源：http://fx.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://pn.szxytkj.cn

"a" .. "b"
来源：http://ux.bookmarksfly.cn

[T38] Lua：条件
来源：http://ae.nicolike.cn

if x > 0 then print("正") end
来源：http://qd.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://ev.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://kx.chemitech.net.cn

[T40] Lua：元表
来源：http://gf.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://hr.muxihuayi.cn

[T41] Perl：Hello World
来源：http://um.shtwfgs.cn

print "Hello\n";
来源：http://xp.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://rx.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yi.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://io.521024.cn

"值: $a"
来源：http://ml.nszjky.cn

[T44] Perl：条件
来源：http://vt.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://ed.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://wl.colortex.cn

for my $x (@arr) { print $x; }
来源：http://us.panjiajie.cn

[T46] Perl：哈希操作
来源：http://ue.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bc.gzmigu.cn

[T47] Perl：正则捕获
来源：http://bg.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cp.muxihuayi.cn

[T48] Perl：正则替换
来源：http://ty.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://yf.asd995.cn

[T49] Perl：函数
来源：http://et.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bt.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://ug.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mh.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://sc.colortex.cn

[T51] Scala：Hello World
来源：http://sg.bjjhwx.cn

println("Hello")
来源：http://hd.haigaiapp.cn

[T52] Scala：变量
来源：http://hr.521024.cn

val a = 1;  var b = 2
来源：http://un.9csxet.cn

[T53] Scala：字符串插值
来源：http://xf.bjjhwx.cn

s"值: $b"
来源：http://op.yuexingan06.cn

[T54] Scala：集合映射
来源：http://lm.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://ri.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://rz.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sg.shxzskj.cn

[T56] Scala：样例类
来源：http://ov.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ix.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://fz.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cg.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://bl.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bu.haigaiapp.cn

[T59] Scala：循环
来源：http://nh.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://ds.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://ns.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xa.hahajie.cn

================================================================================
来源：http://bs.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tk.newstarts.cn

================================================================================
来源：http://eu.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://uv.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iy.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://ue.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kg.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://cn.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lx.szxytkj.cn

[U04] Py：变量调试打印
来源：http://tu.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tx.asd995.cn

[U05] Py：列表去重且保序
来源：http://ce.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://va.szxytkj.cn

[U06] Py：合并两个字典
来源：http://lq.haigaiapp.cn

{**a, **b}
来源：http://mw.521024.cn

[U07] Py：反转字典键值
来源：http://tq.newstarts.cn

{v: k for k, v in d.items()}
来源：http://fh.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://og.521024.cn

[y for x in nested for y in x]
来源：http://ee.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ux.shtwfgs.cn

max(d, key=d.get)
来源：http://uu.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://wa.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qp.shxzukj.cn

[U11] Py：生成器表达式
来源：http://mo.newstarts.cn

(x * 2 for x in arr)
来源：http://sh.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nc.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://mv.nszjky.cn

[U13] Py：固定长度队列
来源：http://ab.hahajie.cn

deque(maxlen=10)
来源：http://ph.huanxung.cn

[U14] Py：分组收集到列表
来源：http://kk.9csxet.cn

defaultdict(list)
来源：http://db.panjiajie.cn

[U15] Py：高精度计时
来源：http://ry.asd995.cn

t = time.perf_counter()
来源：http://yj.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://bf.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kq.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ly.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://sy.gzmigu.cn

[U18] Py：预编译正则
来源：http://cp.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://vd.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://wy.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uk.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://sr.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://ec.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://fm.panjiajie.cn

@contextlib.contextmanager
来源：http://ka.asd995.cn

[U22] Py：矩阵转置
来源：http://nx.bookmarksfly.cn

list(zip(*m))
来源：http://ws.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://yp.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gz.szsharing.cn

[U24] Py：路径操作
来源：http://ji.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hl.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://tj.muxihuayi.cn

csv.DictReader(f)
来源：http://hc.gzmigu.cn

[U26] Py：并发下载
来源：http://cw.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ih.colortex.cn

[U27] Py：异步 HTTP
来源：http://ak.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://bd.hahajie.cn

[U28] Py：类型别名
来源：http://zc.nicolike.cn

UserId = int
来源：http://pz.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://wn.nicolike.cn

@property 与 @x.setter 配合
来源：http://xt.chemitech.net.cn

[U30] Py：数据类
来源：http://qu.colortex.cn

@dataclass(slots=True)
来源：http://gm.yuexingan06.cn

[U31] Py：单测
来源：http://rc.hnjuh.cn

python -m pytest -q
来源：http://um.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://sk.asd995.cn

ruff format . && ruff check --fix .
来源：http://ye.9csxet.cn

[U33] Py：打包发布
来源：http://gd.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://yn.muxihuayi.cn

[U34] Py：判断编码
来源：http://yp.yuntaijiaju.cn

chardet.detect(raw)
来源：http://bt.wgjwhj.cn

[U35] Py：发送邮件
来源：http://vj.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rc.shtwfgs.cn

[U36] Py：定时任务
来源：http://jm.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://ti.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://zm.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sl.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://rp.szxytkj.cn

Path(__file__).resolve().parent
来源：http://gq.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://ao.chemitech.net.cn

sys.stdout.isatty()
来源：http://iy.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://om.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://qp.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ow.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://no.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://sz.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://il.newstarts.cn

[U43] PHP：声明命名空间
来源：http://rh.lnxyls.cn

namespace App\Http;
来源：http://gx.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://hm.newstarts.cn

declare(strict_types=1);
来源：http://bj.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://rl.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.nszjky.cn

[U46] PHP：可空类型
来源：http://ns.wgjwhj.cn

?string $name = null
来源：http://az.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ht.jctech888.com.cn

int|string $id
来源：http://aw.nszjky.cn

[U48] PHP：纯枚举
来源：http://ca.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eo.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://pn.huanxung.cn

public readonly string $name
来源：http://gk.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://mf.asd995.cn

public function __construct(private int $id) {}
来源：http://qp.muxihuayi.cn

[U51] PHP：数组解构
来源：http://pl.hnjuh.cn

[$a, $b] = $arr;
来源：http://ll.asd995.cn

[U52] PHP：箭头函数
来源：http://kz.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://ci.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://lu.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://no.lnxyls.cn

[U54] PHP：空安全调用
来源：http://yh.wgjwhj.cn

$obj?->method()
来源：http://gr.szxytkj.cn

[U55] PHP：match 表达式
来源：http://ab.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bq.asd995.cn

[U56] PHP：命名参数
来源：http://dj.9csxet.cn

f(a: 1, b: 2)
来源：http://aj.asd995.cn

[U57] PHP：字符串插值
来源：http://ta.chemitech.net.cn

"值: {$a}"
来源：http://qe.asd995.cn

[U58] PHP：数组三件套
来源：http://kf.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aa.shxzukj.cn

[U59] PHP：自定义排序
来源：http://lg.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pe.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://qi.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xv.yuexingan06.cn

[U61] PHP：正则
来源：http://ev.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sg.asd995.cn

[U62] PHP：日期对象
来源：http://br.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://je.bjjhwx.cn


<!-- 参考信息 -->