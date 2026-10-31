代发 wailian999

[S39] C++：自定义比较器排序
来源：http://wv.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hh.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://xo.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ju.gzmigu.cn

[S41] C++：类与构造函数
来源：http://av.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nd.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://hh.521024.cn

class B : public Base { public: void f() override {} };
来源：http://am.huanxung.cn

[S43] C++：智能指针
来源：http://po.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://cz.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://rp.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://si.jianghongdianzi.cn

[S45] C++：lambda
来源：http://gj.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hq.bookmarksfly.cn

[S46] C++：函数模板
来源：http://gi.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lf.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://bl.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://av.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://fr.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bj.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://jp.muxihuayi.cn

[S49] C++：写文件
来源：http://ga.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zg.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://dw.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qc.newstarts.cn

[S51] C++：显式类型转换
来源：http://it.colortex.cn

static_cast<double>(a) / b
来源：http://pw.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://gf.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://km.szsharing.cn

[S53] C++：移动语义
来源：http://an.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://ni.nszjky.cn

[S54] C++：异常处理
来源：http://mm.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hm.521024.cn

[S55] C++：结构化绑定
来源：http://wv.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iq.huixiangedu.cn

[S56] C++：optional
来源：http://dl.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zx.lnxyls.cn

[S57] C++：编译期常量
来源：http://cz.lnxyls.cn

constexpr int N = 10;
来源：http://as.hahajie.cn

[S58] C++：命名空间
来源：http://gw.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://tu.huixiangedu.cn

[S59] C++：静态断言
来源：http://ch.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uv.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://dw.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jg.yuntaijiaju.cn

================================================================================
来源：http://zo.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lc.szxytkj.cn

================================================================================
来源：http://sb.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://bo.huanxung.cn

println("Hello")
来源：http://yz.haigaiapp.cn

[T02] Kotlin：变量
来源：http://yp.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qr.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://lo.yuntaijiaju.cn

"值: $b"
来源：http://iu.gzmigu.cn

[T04] Kotlin：空安全
来源：http://st.shxzskj.cn

val n: String? = null;  n?.length
来源：http://hu.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://db.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vb.szsharing.cn

[T06] Kotlin：集合映射
来源：http://sh.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zs.colortex.cn

[T07] Kotlin：集合过滤
来源：http://ai.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jy.shxzskj.cn

[T08] Kotlin：数据类
来源：http://dd.521024.cn

data class User(val name: String, val age: Int)
来源：http://oj.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://vp.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://ic.9csxet.cn

[T10] Kotlin：默认参数
来源：http://yn.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://it.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://dk.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wt.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://sa.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ae.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://vq.colortex.cn

val m = mapOf("a" to 1)
来源：http://io.chemitech.net.cn

[T14] Kotlin：循环
来源：http://ac.colortex.cn

for (i in 1..10) println(i)
来源：http://xc.hahajie.cn

[T15] Kotlin：接口
来源：http://ek.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://nh.jctech888.com.cn

[T16] Swift：Hello World
来源：http://le.gzmigu.cn

print("Hello")
来源：http://yv.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ty.hahajie.cn

var a = 1;  let b = 2
来源：http://ir.szsharing.cn

[T18] Swift：字符串插值
来源：http://zo.colortex.cn

"值: \(b)"
来源：http://xf.hahajie.cn

[T19] Swift：可选绑定
来源：http://qh.jctech888.com.cn

if let n = opt { print(n) }
来源：http://lu.hnjuh.cn

[T20] Swift：数组操作
来源：http://wk.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://eg.panjiajie.cn

[T21] Swift：遍历
来源：http://kf.jianghongdianzi.cn

for x in a { print(x) }
来源：http://lc.yuntaijiaju.cn

[T22] Swift：字典
来源：http://ev.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://he.colortex.cn

[T23] Swift：函数
来源：http://cf.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fc.hahajie.cn

[T24] Swift：闭包
来源：http://yk.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vx.szxytkj.cn

[T25] Swift：结构体
来源：http://ko.nszjky.cn

struct P { var x: Int }
来源：http://gk.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://gr.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://fs.panjiajie.cn

[T27] Swift：错误处理
来源：http://ql.asd995.cn

do { try f() } catch { print(error) }
来源：http://ba.wgjwhj.cn

[T28] Swift：枚举
来源：http://ye.hahajie.cn

enum Color { case red, green }
来源：http://ga.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://wc.asd995.cn

guard let x = opt else { return }
来源：http://pc.yuntaijiaju.cn

[T30] Swift：协议
来源：http://tc.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://ud.hnjuh.cn

[T31] Lua：Hello World
来源：http://oa.huixinmuqiang.cn

print("Hello")
来源：http://so.nszjky.cn

[T32] Lua：局部变量
来源：http://wr.shtwfgs.cn

local a = 1
来源：http://yn.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://ft.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ax.nicolike.cn

[T34] Lua：遍历表
来源：http://qs.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xu.shxzukj.cn

[T35] Lua：字典表
来源：http://yr.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://xr.shxzskj.cn

[T36] Lua：函数
来源：http://tc.haigaiapp.cn

function add(a, b) return a + b end
来源：http://cq.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://mm.huanxung.cn

"a" .. "b"
来源：http://vj.asd995.cn

[T38] Lua：条件
来源：http://fu.haigaiapp.cn

if x > 0 then print("正") end
来源：http://zb.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://dy.panjiajie.cn

string.find(s, "%d+")
来源：http://il.szxytkj.cn

[T40] Lua：元表
来源：http://xr.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://tq.szsharing.cn

[T41] Perl：Hello World
来源：http://oo.hahajie.cn

print "Hello\n";
来源：http://ms.lnxyls.cn

[T42] Perl：变量类型
来源：http://sq.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://im.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://ir.shxzskj.cn

"值: $a"
来源：http://uk.bookmarksfly.cn

[T44] Perl：条件
来源：http://kq.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://kt.panjiajie.cn

[T45] Perl：数组遍历
来源：http://ws.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://rq.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://wn.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nt.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://wh.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ov.gzmigu.cn

[T48] Perl：正则替换
来源：http://mp.nszjky.cn

$s =~ s/old/new/g;
来源：http://dn.shtwfgs.cn

[T49] Perl：函数
来源：http://fh.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ib.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://gx.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bs.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://mc.9csxet.cn

[T51] Scala：Hello World
来源：http://qk.hahajie.cn

println("Hello")
来源：http://tc.bjjhwx.cn

[T52] Scala：变量
来源：http://gd.521024.cn

val a = 1;  var b = 2
来源：http://le.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://kh.colortex.cn

s"值: $b"
来源：http://pu.wgjwhj.cn

[T54] Scala：集合映射
来源：http://qk.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://rc.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://ze.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rg.lnxyls.cn

[T56] Scala：样例类
来源：http://yn.colortex.cn

case class User(name: String, age: Int)
来源：http://gl.newstarts.cn

[T57] Scala：模式匹配
来源：http://ki.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pe.huixiangedu.cn

[T58] Scala：函数定义
来源：http://nc.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://df.wgjwhj.cn

[T59] Scala：循环
来源：http://ds.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://cv.521024.cn

[T60] Scala：折叠
来源：http://ha.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ei.szxytkj.cn

================================================================================
来源：http://fg.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rr.szsharing.cn

================================================================================
来源：http://qs.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://mv.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mp.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://nf.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qy.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://es.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ff.hnjuh.cn

[U04] Py：变量调试打印
来源：http://tc.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ll.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://ya.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://ow.9csxet.cn

[U06] Py：合并两个字典
来源：http://gg.panjiajie.cn

{**a, **b}
来源：http://jf.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://lw.nszjky.cn

{v: k for k, v in d.items()}
来源：http://om.newstarts.cn

[U08] Py：展平二维列表
来源：http://wh.szxytkj.cn

[y for x in nested for y in x]
来源：http://mm.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://cb.nszjky.cn

max(d, key=d.get)
来源：http://wa.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://bk.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ph.521024.cn

[U11] Py：生成器表达式
来源：http://wu.shtwfgs.cn

(x * 2 for x in arr)
来源：http://xo.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rw.521024.cn

Counter(arr).most_common(3)
来源：http://rx.hahajie.cn

[U13] Py：固定长度队列
来源：http://gy.521024.cn

deque(maxlen=10)
来源：http://zi.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ix.shxzskj.cn

defaultdict(list)
来源：http://is.asd995.cn

[U15] Py：高精度计时
来源：http://ml.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ik.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://xy.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ug.nszjky.cn

[U17] Py：初始化日志
来源：http://va.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://gt.szxytkj.cn

[U18] Py：预编译正则
来源：http://pl.newstarts.cn

pat = re.compile(r"\d+")
来源：http://fm.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://fn.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ci.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://ie.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ou.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://th.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://zx.panjiajie.cn

[U22] Py：矩阵转置
来源：http://sn.shxzskj.cn

list(zip(*m))
来源：http://ul.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ae.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ud.colortex.cn

[U24] Py：路径操作
来源：http://dy.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kr.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://ov.nicolike.cn

csv.DictReader(f)
来源：http://ii.9csxet.cn

[U26] Py：并发下载
来源：http://oe.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://co.9csxet.cn

[U27] Py：异步 HTTP
来源：http://oz.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://li.panjiajie.cn

[U28] Py：类型别名
来源：http://cf.panjiajie.cn

UserId = int
来源：http://zu.asd995.cn

[U29] Py：属性校验
来源：http://ax.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://ya.jianghongdianzi.cn

[U30] Py：数据类
来源：http://yp.gzmigu.cn

@dataclass(slots=True)
来源：http://qg.nicolike.cn

[U31] Py：单测
来源：http://rc.huixinmuqiang.cn

python -m pytest -q
来源：http://mw.nicolike.cn

[U32] Py：代码格式化
来源：http://wm.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://sk.521024.cn

[U33] Py：打包发布
来源：http://bd.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://pz.wgjwhj.cn

[U34] Py：判断编码
来源：http://wr.panjiajie.cn

chardet.detect(raw)
来源：http://yg.lnxyls.cn

[U35] Py：发送邮件
来源：http://gd.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cc.bookmarksfly.cn

[U36] Py：定时任务
来源：http://vv.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ud.shxzskj.cn

[U37] Py：读写 Excel
来源：http://aj.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hs.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://bs.shxzukj.cn

Path(__file__).resolve().parent
来源：http://zs.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://bj.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://wz.szsharing.cn

[U40] Py：打印到标准错误
来源：http://pe.shxzukj.cn

print("err", file=sys.stderr)
来源：http://vd.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://xf.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cm.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ve.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hb.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://hb.wgjwhj.cn

namespace App\Http;
来源：http://tw.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://ib.hnjuh.cn

declare(strict_types=1);
来源：http://fk.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://yo.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rz.szxytkj.cn

[U46] PHP：可空类型
来源：http://ec.huixiangedu.cn

?string $name = null
来源：http://qu.nszjky.cn

[U47] PHP：联合类型
来源：http://cx.bjjhwx.cn

int|string $id
来源：http://nt.gzmigu.cn

[U48] PHP：纯枚举
来源：http://rp.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hr.jctech888.com.cn

[U49] PHP：只读属性
来源：http://bd.newstarts.cn

public readonly string $name
来源：http://ys.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://wk.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://er.huixiangedu.cn

[U51] PHP：数组解构
来源：http://bn.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://mj.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://ns.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ef.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://jd.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://bl.hnjuh.cn

[U54] PHP：空安全调用
来源：http://vq.muxihuayi.cn

$obj?->method()
来源：http://an.nicolike.cn

[U55] PHP：match 表达式
来源：http://tk.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wb.panjiajie.cn

[U56] PHP：命名参数
来源：http://al.hnjuh.cn

f(a: 1, b: 2)
来源：http://gf.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://pj.colortex.cn

"值: {$a}"
来源：http://bv.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ky.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qw.nicolike.cn

[U59] PHP：自定义排序
来源：http://jt.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pd.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://iz.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pp.521024.cn

[U61] PHP：正则
来源：http://sq.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mk.haigaiapp.cn

[U62] PHP：日期对象
来源：http://uh.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wu.521024.cn

[U63] PHP：文件读写
来源：http://cz.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ku.nicolike.cn

[U64] PHP：目录遍历
来源：http://bu.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://hj.jctech888.com.cn


<!-- 参考信息 -->