代发 wailian999

[S39] C++：自定义比较器排序
来源：http://tu.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jh.nicolike.cn

[S40] C++：查找元素
来源：http://du.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xy.hnjuh.cn

[S41] C++：类与构造函数
来源：http://kx.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ti.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://ge.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://dk.newstarts.cn

[S43] C++：智能指针
来源：http://ci.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://sv.jctech888.com.cn

[S44] C++：引用传参
来源：http://gp.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://ig.yuntaijiaju.cn

[S45] C++：lambda
来源：http://do.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cz.hahajie.cn

[S46] C++：函数模板
来源：http://vs.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://er.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://px.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lq.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://gk.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hj.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ai.szsharing.cn

[S49] C++：写文件
来源：http://ye.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ce.shtwfgs.cn

[S50] C++：格式化数字
来源：http://up.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://er.nicolike.cn

[S51] C++：显式类型转换
来源：http://ci.huixiangedu.cn

static_cast<double>(a) / b
来源：http://wm.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://ig.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://af.huanxung.cn

[S53] C++：移动语义
来源：http://or.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://jp.lnxyls.cn

[S54] C++：异常处理
来源：http://wf.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kf.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://bt.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oo.szxytkj.cn

[S56] C++：optional
来源：http://bq.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sv.lnxyls.cn

[S57] C++：编译期常量
来源：http://al.szsharing.cn

constexpr int N = 10;
来源：http://hu.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://ub.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://pn.bookmarksfly.cn

[S59] C++：静态断言
来源：http://pr.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pe.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://dd.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vq.yuexingan06.cn

================================================================================
来源：http://pf.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xx.huanxung.cn

================================================================================
来源：http://ae.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://vl.shxzskj.cn

println("Hello")
来源：http://ph.newstarts.cn

[T02] Kotlin：变量
来源：http://gz.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fe.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://wg.asd995.cn

"值: $b"
来源：http://tr.nicolike.cn

[T04] Kotlin：空安全
来源：http://rm.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://id.colortex.cn

[T05] Kotlin：when 表达式
来源：http://bk.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fr.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://yr.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fr.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ce.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yw.lnxyls.cn

[T08] Kotlin：数据类
来源：http://ra.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://yh.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://qm.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://ot.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ve.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://om.asd995.cn

[T11] Kotlin：协程
来源：http://ab.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zw.newstarts.cn

[T12] Kotlin：解构声明
来源：http://yu.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://gk.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ry.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://pb.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://xj.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://wu.muxihuayi.cn

[T15] Kotlin：接口
来源：http://tz.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://lp.szxytkj.cn

[T16] Swift：Hello World
来源：http://oo.hahajie.cn

print("Hello")
来源：http://xv.newstarts.cn

[T17] Swift：变量与常量
来源：http://is.jctech888.com.cn

var a = 1;  let b = 2
来源：http://xy.szsharing.cn

[T18] Swift：字符串插值
来源：http://yl.bookmarksfly.cn

"值: \(b)"
来源：http://kc.521024.cn

[T19] Swift：可选绑定
来源：http://ub.haigaiapp.cn

if let n = opt { print(n) }
来源：http://to.shtwfgs.cn

[T20] Swift：数组操作
来源：http://rh.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lj.yuexingan06.cn

[T21] Swift：遍历
来源：http://kk.haigaiapp.cn

for x in a { print(x) }
来源：http://ki.yuntaijiaju.cn

[T22] Swift：字典
来源：http://yw.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sl.bjjhwx.cn

[T23] Swift：函数
来源：http://tn.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ng.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://bh.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gr.muxihuayi.cn

[T25] Swift：结构体
来源：http://zx.szxytkj.cn

struct P { var x: Int }
来源：http://xc.huixiangedu.cn

[T26] Swift：类与重写
来源：http://gn.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://vj.panjiajie.cn

[T27] Swift：错误处理
来源：http://cp.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://pr.szsharing.cn

[T28] Swift：枚举
来源：http://ar.chemitech.net.cn

enum Color { case red, green }
来源：http://ur.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://lv.9csxet.cn

guard let x = opt else { return }
来源：http://ja.szsharing.cn

[T30] Swift：协议
来源：http://wm.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://vz.wgjwhj.cn

[T31] Lua：Hello World
来源：http://wc.huanxung.cn

print("Hello")
来源：http://ut.shxzskj.cn

[T32] Lua：局部变量
来源：http://vf.gzmigu.cn

local a = 1
来源：http://et.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://og.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ja.hahajie.cn

[T34] Lua：遍历表
来源：http://eb.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wl.hahajie.cn

[T35] Lua：字典表
来源：http://gz.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://ys.muxihuayi.cn

[T36] Lua：函数
来源：http://po.hnjuh.cn

function add(a, b) return a + b end
来源：http://op.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://xe.hahajie.cn

"a" .. "b"
来源：http://yx.shxzukj.cn

[T38] Lua：条件
来源：http://oq.wgjwhj.cn

if x > 0 then print("正") end
来源：http://ux.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://lx.huanxung.cn

string.find(s, "%d+")
来源：http://mo.9csxet.cn

[T40] Lua：元表
来源：http://fq.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://bh.szxytkj.cn

[T41] Perl：Hello World
来源：http://lf.9csxet.cn

print "Hello\n";
来源：http://jh.huanxung.cn

[T42] Perl：变量类型
来源：http://ok.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bu.panjiajie.cn

[T43] Perl：字符串插值
来源：http://ka.huixinmuqiang.cn

"值: $a"
来源：http://nt.yuntaijiaju.cn

[T44] Perl：条件
来源：http://qs.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://qf.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://mz.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://st.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://gf.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pe.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ol.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fw.lnxyls.cn

[T48] Perl：正则替换
来源：http://to.nicolike.cn

$s =~ s/old/new/g;
来源：http://ok.shtwfgs.cn

[T49] Perl：函数
来源：http://bx.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hc.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://ad.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tl.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://cd.chemitech.net.cn

[T51] Scala：Hello World
来源：http://dr.bookmarksfly.cn

println("Hello")
来源：http://sn.bjjhwx.cn

[T52] Scala：变量
来源：http://vd.lnxyls.cn

val a = 1;  var b = 2
来源：http://kl.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://yt.nicolike.cn

s"值: $b"
来源：http://to.nicolike.cn

[T54] Scala：集合映射
来源：http://yp.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://oe.hnjuh.cn

[T55] Scala：集合过滤
来源：http://dn.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://va.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://xs.szsharing.cn

case class User(name: String, age: Int)
来源：http://vv.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://ma.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dg.newstarts.cn

[T58] Scala：函数定义
来源：http://qa.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rk.yuexingan06.cn

[T59] Scala：循环
来源：http://mm.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ak.asd995.cn

[T60] Scala：折叠
来源：http://ie.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iw.bookmarksfly.cn

================================================================================
来源：http://os.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ot.yuntaijiaju.cn

================================================================================
来源：http://wi.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://hr.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ku.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://it.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vf.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://ly.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xg.panjiajie.cn

[U04] Py：变量调试打印
来源：http://ag.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bc.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://hd.521024.cn

list(dict.fromkeys(arr))
来源：http://yy.colortex.cn

[U06] Py：合并两个字典
来源：http://te.chemitech.net.cn

{**a, **b}
来源：http://po.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://nn.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://bk.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://xc.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://le.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://bc.shxzskj.cn

max(d, key=d.get)
来源：http://pl.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://au.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://id.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://uo.nicolike.cn

(x * 2 for x in arr)
来源：http://eg.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ee.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://lk.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ve.wgjwhj.cn

deque(maxlen=10)
来源：http://ik.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://bo.lnxyls.cn

defaultdict(list)
来源：http://vb.szxytkj.cn

[U15] Py：高精度计时
来源：http://dj.yuexingan06.cn

t = time.perf_counter()
来源：http://ha.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://no.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fn.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://ld.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://dj.hnjuh.cn

[U18] Py：预编译正则
来源：http://mo.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://xw.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://rh.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xv.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://lk.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://md.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://tv.panjiajie.cn

@contextlib.contextmanager
来源：http://fx.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://oq.haigaiapp.cn

list(zip(*m))
来源：http://om.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://qy.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lj.shxzukj.cn

[U24] Py：路径操作
来源：http://ec.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dh.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://wa.gzmigu.cn

csv.DictReader(f)
来源：http://oz.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://dl.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://so.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ec.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://hx.asd995.cn

[U28] Py：类型别名
来源：http://vh.szsharing.cn

UserId = int
来源：http://nc.bjjhwx.cn

[U29] Py：属性校验
来源：http://mb.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://na.chemitech.net.cn

[U30] Py：数据类
来源：http://rl.shxzukj.cn

@dataclass(slots=True)
来源：http://ez.jctech888.com.cn

[U31] Py：单测
来源：http://mu.9csxet.cn

python -m pytest -q
来源：http://ke.521024.cn

[U32] Py：代码格式化
来源：http://lr.asd995.cn

ruff format . && ruff check --fix .
来源：http://sv.szxytkj.cn

[U33] Py：打包发布
来源：http://eu.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://mj.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://tc.bjjhwx.cn

chardet.detect(raw)
来源：http://yy.521024.cn

[U35] Py：发送邮件
来源：http://ya.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sb.wgjwhj.cn

[U36] Py：定时任务
来源：http://rg.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://be.huanxung.cn

[U37] Py：读写 Excel
来源：http://gf.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wh.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://yv.szxytkj.cn

Path(__file__).resolve().parent
来源：http://qd.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://vr.shxzskj.cn

sys.stdout.isatty()
来源：http://qn.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://kb.521024.cn

print("err", file=sys.stderr)
来源：http://vx.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://yr.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mw.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://rm.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ar.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://yd.yuntaijiaju.cn

namespace App\Http;
来源：http://tp.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://ri.yuntaijiaju.cn

declare(strict_types=1);
来源：http://fh.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://qi.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.szxytkj.cn

[U46] PHP：可空类型
来源：http://lo.muxihuayi.cn

?string $name = null
来源：http://mn.chemitech.net.cn

[U47] PHP：联合类型
来源：http://tc.jianghongdianzi.cn

int|string $id
来源：http://oc.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://hs.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wa.hahajie.cn

[U49] PHP：只读属性
来源：http://no.szsharing.cn

public readonly string $name
来源：http://wk.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://io.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://lr.521024.cn

[U51] PHP：数组解构
来源：http://to.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://qo.gzmigu.cn

[U52] PHP：箭头函数
来源：http://wp.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://hj.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://xo.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://zt.gzmigu.cn

[U54] PHP：空安全调用
来源：http://rq.chemitech.net.cn

$obj?->method()
来源：http://lq.521024.cn

[U55] PHP：match 表达式
来源：http://qg.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gk.gzmigu.cn

[U56] PHP：命名参数
来源：http://je.lnxyls.cn

f(a: 1, b: 2)
来源：http://pc.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://be.haigaiapp.cn

"值: {$a}"
来源：http://yt.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://xi.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kh.szsharing.cn

[U59] PHP：自定义排序
来源：http://lt.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xk.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://rg.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ro.bjjhwx.cn

[U61] PHP：正则
来源：http://vg.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ma.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ta.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hm.521024.cn

[U63] PHP：文件读写
来源：http://ef.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://em.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://wn.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://dh.muxihuayi.cn


<!-- 参考信息 -->