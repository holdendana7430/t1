代发 wailian999

[S37] C++：set
来源：http://ql.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qc.hnjuh.cn

[S38] C++：排序
来源：http://wl.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://uf.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://pe.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://df.yuexingan06.cn

[S40] C++：查找元素
来源：http://yw.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ti.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://ca.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rj.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://st.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://ax.nicolike.cn

[S43] C++：智能指针
来源：http://om.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ek.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://fe.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://kg.huixiangedu.cn

[S45] C++：lambda
来源：http://ii.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gg.yuexingan06.cn

[S46] C++：函数模板
来源：http://kb.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ch.521024.cn

[S47] C++：结构化绑定遍历
来源：http://vq.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fc.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://pg.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yz.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://sj.yuntaijiaju.cn

[S49] C++：写文件
来源：http://jr.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gc.haigaiapp.cn

[S50] C++：格式化数字
来源：http://pe.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ov.asd995.cn

[S51] C++：显式类型转换
来源：http://fi.huanxung.cn

static_cast<double>(a) / b
来源：http://fh.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://wn.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://ib.jctech888.com.cn

[S53] C++：移动语义
来源：http://yx.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://db.huanxung.cn

[S54] C++：异常处理
来源：http://rj.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qo.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://rq.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gs.colortex.cn

[S56] C++：optional
来源：http://dg.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ec.nszjky.cn

[S57] C++：编译期常量
来源：http://uw.huixiangedu.cn

constexpr int N = 10;
来源：http://yo.bjjhwx.cn

[S58] C++：命名空间
来源：http://fc.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://zn.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://zt.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tb.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://wy.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lo.nicolike.cn

================================================================================
来源：http://vd.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gp.colortex.cn

================================================================================
来源：http://fq.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://vn.szsharing.cn

println("Hello")
来源：http://sb.muxihuayi.cn

[T02] Kotlin：变量
来源：http://pf.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ep.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://hh.szxytkj.cn

"值: $b"
来源：http://pc.nicolike.cn

[T04] Kotlin：空安全
来源：http://lb.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://ir.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://ox.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://av.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://qx.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xu.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://kg.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cs.panjiajie.cn

[T08] Kotlin：数据类
来源：http://dh.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://tu.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ex.colortex.cn

fun String.exclaim() = this + "!"
来源：http://ix.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://wi.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aa.chemitech.net.cn

[T11] Kotlin：协程
来源：http://xz.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vv.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://mz.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://fy.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://zp.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://xq.shtwfgs.cn

[T14] Kotlin：循环
来源：http://qf.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ml.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://oi.nicolike.cn

interface Shape { fun area(): Double }
来源：http://av.chemitech.net.cn

[T16] Swift：Hello World
来源：http://us.gzmigu.cn

print("Hello")
来源：http://xs.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://my.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://ro.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://cl.asd995.cn

"值: \(b)"
来源：http://ml.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://jb.nicolike.cn

if let n = opt { print(n) }
来源：http://xu.szsharing.cn

[T20] Swift：数组操作
来源：http://bk.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wk.bjjhwx.cn

[T21] Swift：遍历
来源：http://ca.colortex.cn

for x in a { print(x) }
来源：http://op.nszjky.cn

[T22] Swift：字典
来源：http://fu.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bi.chemitech.net.cn

[T23] Swift：函数
来源：http://bd.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qm.9csxet.cn

[T24] Swift：闭包
来源：http://sa.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yc.yuexingan06.cn

[T25] Swift：结构体
来源：http://bt.gzmigu.cn

struct P { var x: Int }
来源：http://un.shtwfgs.cn

[T26] Swift：类与重写
来源：http://ow.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ms.haigaiapp.cn

[T27] Swift：错误处理
来源：http://lx.521024.cn

do { try f() } catch { print(error) }
来源：http://zt.huanxung.cn

[T28] Swift：枚举
来源：http://xb.hahajie.cn

enum Color { case red, green }
来源：http://er.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://iq.bjjhwx.cn

guard let x = opt else { return }
来源：http://kx.huixinmuqiang.cn

[T30] Swift：协议
来源：http://cz.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://wg.wgjwhj.cn

[T31] Lua：Hello World
来源：http://xf.521024.cn

print("Hello")
来源：http://hn.shxzskj.cn

[T32] Lua：局部变量
来源：http://vv.huixiangedu.cn

local a = 1
来源：http://rk.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://yd.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zp.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://iu.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rf.panjiajie.cn

[T35] Lua：字典表
来源：http://km.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://do.colortex.cn

[T36] Lua：函数
来源：http://cz.nicolike.cn

function add(a, b) return a + b end
来源：http://fj.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://oi.yuntaijiaju.cn

"a" .. "b"
来源：http://vk.yuntaijiaju.cn

[T38] Lua：条件
来源：http://oi.colortex.cn

if x > 0 then print("正") end
来源：http://kh.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://ch.521024.cn

string.find(s, "%d+")
来源：http://lj.yuntaijiaju.cn

[T40] Lua：元表
来源：http://pp.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://ch.nszjky.cn

[T41] Perl：Hello World
来源：http://xh.huanxung.cn

print "Hello\n";
来源：http://wp.muxihuayi.cn

[T42] Perl：变量类型
来源：http://ef.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://el.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://rt.jianghongdianzi.cn

"值: $a"
来源：http://fy.panjiajie.cn

[T44] Perl：条件
来源：http://ob.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://wa.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://li.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://rq.colortex.cn

[T46] Perl：哈希操作
来源：http://lg.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gl.szxytkj.cn

[T47] Perl：正则捕获
来源：http://ei.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ux.haigaiapp.cn

[T48] Perl：正则替换
来源：http://nn.colortex.cn

$s =~ s/old/new/g;
来源：http://zp.muxihuayi.cn

[T49] Perl：函数
来源：http://wf.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vk.szsharing.cn

[T50] Perl：逐行读文件
来源：http://qf.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jt.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://kv.jctech888.com.cn

[T51] Scala：Hello World
来源：http://es.jianghongdianzi.cn

println("Hello")
来源：http://ko.nicolike.cn

[T52] Scala：变量
来源：http://wd.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://wk.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://go.nszjky.cn

s"值: $b"
来源：http://vf.gzmigu.cn

[T54] Scala：集合映射
来源：http://dh.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ch.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://wi.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tn.szsharing.cn

[T56] Scala：样例类
来源：http://gi.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://sh.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://co.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wg.wgjwhj.cn

[T58] Scala：函数定义
来源：http://gc.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yd.nicolike.cn

[T59] Scala：循环
来源：http://ph.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://bs.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://kf.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lp.hahajie.cn

================================================================================
来源：http://dv.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pm.bookmarksfly.cn

================================================================================
来源：http://iz.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://as.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dr.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://cf.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://we.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://cj.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wd.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://fg.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bz.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://vs.nszjky.cn

list(dict.fromkeys(arr))
来源：http://uv.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://fs.gzmigu.cn

{**a, **b}
来源：http://db.asd995.cn

[U07] Py：反转字典键值
来源：http://cl.nicolike.cn

{v: k for k, v in d.items()}
来源：http://le.lnxyls.cn

[U08] Py：展平二维列表
来源：http://xd.panjiajie.cn

[y for x in nested for y in x]
来源：http://qf.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://sp.asd995.cn

max(d, key=d.get)
来源：http://fa.shxzskj.cn

[U10] Py：按值排序字典
来源：http://pd.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sm.panjiajie.cn

[U11] Py：生成器表达式
来源：http://zf.asd995.cn

(x * 2 for x in arr)
来源：http://jq.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ax.szsharing.cn

Counter(arr).most_common(3)
来源：http://aj.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://bj.gzmigu.cn

deque(maxlen=10)
来源：http://mg.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://xb.szsharing.cn

defaultdict(list)
来源：http://dy.panjiajie.cn

[U15] Py：高精度计时
来源：http://hw.colortex.cn

t = time.perf_counter()
来源：http://gb.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://jr.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wq.hahajie.cn

[U17] Py：初始化日志
来源：http://ld.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://dl.huixiangedu.cn

[U18] Py：预编译正则
来源：http://xu.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://dr.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://tb.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ri.hahajie.cn

[U20] Py：缓存函数结果
来源：http://ba.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://hv.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://cj.szxytkj.cn

@contextlib.contextmanager
来源：http://vy.9csxet.cn

[U22] Py：矩阵转置
来源：http://be.yuexingan06.cn

list(zip(*m))
来源：http://zz.nicolike.cn

[U23] Py：分块读取大文件
来源：http://ai.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eu.hnjuh.cn

[U24] Py：路径操作
来源：http://sv.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ef.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://fz.wgjwhj.cn

csv.DictReader(f)
来源：http://ih.hahajie.cn

[U26] Py：并发下载
来源：http://pd.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kk.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://wx.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://th.wgjwhj.cn

[U28] Py：类型别名
来源：http://sa.yuexingan06.cn

UserId = int
来源：http://as.muxihuayi.cn

[U29] Py：属性校验
来源：http://xq.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://yj.haigaiapp.cn

[U30] Py：数据类
来源：http://gh.shxzskj.cn

@dataclass(slots=True)
来源：http://rv.lnxyls.cn

[U31] Py：单测
来源：http://wc.lnxyls.cn

python -m pytest -q
来源：http://ly.wgjwhj.cn

[U32] Py：代码格式化
来源：http://dm.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ym.huanxung.cn

[U33] Py：打包发布
来源：http://ck.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://bz.bookmarksfly.cn

[U34] Py：判断编码
来源：http://fx.nszjky.cn

chardet.detect(raw)
来源：http://zf.shxzukj.cn

[U35] Py：发送邮件
来源：http://kq.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uo.shxzskj.cn

[U36] Py：定时任务
来源：http://cn.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://fd.shxzskj.cn

[U37] Py：读写 Excel
来源：http://de.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ae.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://gl.hahajie.cn

Path(__file__).resolve().parent
来源：http://sg.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://hn.szxytkj.cn

sys.stdout.isatty()
来源：http://wn.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ad.szsharing.cn

print("err", file=sys.stderr)
来源：http://km.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://lc.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hc.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://rr.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://et.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://py.hnjuh.cn

namespace App\Http;
来源：http://xi.colortex.cn

[U44] PHP：开启严格类型
来源：http://pe.szxytkj.cn

declare(strict_types=1);
来源：http://rd.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://zx.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lv.asd995.cn

[U46] PHP：可空类型
来源：http://ha.shtwfgs.cn

?string $name = null
来源：http://cs.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://qw.chemitech.net.cn

int|string $id
来源：http://kv.newstarts.cn

[U48] PHP：纯枚举
来源：http://vz.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tz.huanxung.cn

[U49] PHP：只读属性
来源：http://la.muxihuayi.cn

public readonly string $name
来源：http://zn.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://uw.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://mj.gzmigu.cn

[U51] PHP：数组解构
来源：http://la.colortex.cn

[$a, $b] = $arr;
来源：http://of.newstarts.cn

[U52] PHP：箭头函数
来源：http://zl.asd995.cn

$double = fn($x) => $x * 2;
来源：http://xd.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://ni.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://ma.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://rr.hnjuh.cn

$obj?->method()
来源：http://qf.colortex.cn

[U55] PHP：match 表达式
来源：http://wb.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ue.gzmigu.cn

[U56] PHP：命名参数
来源：http://vx.newstarts.cn

f(a: 1, b: 2)
来源：http://hb.shxzukj.cn

[U57] PHP：字符串插值
来源：http://et.szxytkj.cn

"值: {$a}"
来源：http://tg.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://tb.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cu.szsharing.cn

[U59] PHP：自定义排序
来源：http://nc.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pm.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://dc.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zf.newstarts.cn

[U61] PHP：正则
来源：http://uh.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ar.szxytkj.cn

[U62] PHP：日期对象
来源：http://ll.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vh.nicolike.cn


<!-- 参考信息 -->