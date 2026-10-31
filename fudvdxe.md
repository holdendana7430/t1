代发 wailian999

[S37] C++：set
来源：http://zo.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cl.colortex.cn

[S38] C++：排序
来源：http://nx.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://wa.colortex.cn

[S39] C++：自定义比较器排序
来源：http://og.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bq.muxihuayi.cn

[S40] C++：查找元素
来源：http://uo.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tu.huanxung.cn

[S41] C++：类与构造函数
来源：http://oo.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jh.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://jt.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://rv.hahajie.cn

[S43] C++：智能指针
来源：http://dn.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://nu.gzmigu.cn

[S44] C++：引用传参
来源：http://px.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://bw.nicolike.cn

[S45] C++：lambda
来源：http://ed.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ff.521024.cn

[S46] C++：函数模板
来源：http://me.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wq.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://ua.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qf.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://bj.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pb.nszjky.cn

while (std::getline(in, line)) { }
来源：http://bk.9csxet.cn

[S49] C++：写文件
来源：http://xj.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sr.lnxyls.cn

[S50] C++：格式化数字
来源：http://xj.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uw.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://te.gzmigu.cn

static_cast<double>(a) / b
来源：http://jo.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://wz.huanxung.cn

int size() const noexcept { return n_; }
来源：http://nf.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://uq.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://yp.shtwfgs.cn

[S54] C++：异常处理
来源：http://ov.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ti.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ha.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lc.muxihuayi.cn

[S56] C++：optional
来源：http://wx.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tp.bjjhwx.cn

[S57] C++：编译期常量
来源：http://tf.gzmigu.cn

constexpr int N = 10;
来源：http://cj.muxihuayi.cn

[S58] C++：命名空间
来源：http://bq.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://vk.jctech888.com.cn

[S59] C++：静态断言
来源：http://rf.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://za.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://lc.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://po.muxihuayi.cn

================================================================================
来源：http://xu.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mr.wgjwhj.cn

================================================================================
来源：http://ko.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://ui.newstarts.cn

println("Hello")
来源：http://or.521024.cn

[T02] Kotlin：变量
来源：http://ew.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jc.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://sk.lnxyls.cn

"值: $b"
来源：http://ut.szsharing.cn

[T04] Kotlin：空安全
来源：http://yp.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://kj.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://tr.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ce.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://br.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tm.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://ai.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://du.huanxung.cn

[T08] Kotlin：数据类
来源：http://gb.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://sl.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://pv.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://dc.colortex.cn

[T10] Kotlin：默认参数
来源：http://gi.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lt.szsharing.cn

[T11] Kotlin：协程
来源：http://ov.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ed.newstarts.cn

[T12] Kotlin：解构声明
来源：http://kt.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://vq.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://uv.hahajie.cn

val m = mapOf("a" to 1)
来源：http://lf.hahajie.cn

[T14] Kotlin：循环
来源：http://az.lnxyls.cn

for (i in 1..10) println(i)
来源：http://ce.szsharing.cn

[T15] Kotlin：接口
来源：http://yj.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://fo.asd995.cn

[T16] Swift：Hello World
来源：http://sk.bjjhwx.cn

print("Hello")
来源：http://ea.gzmigu.cn

[T17] Swift：变量与常量
来源：http://kv.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://zf.asd995.cn

[T18] Swift：字符串插值
来源：http://pc.hahajie.cn

"值: \(b)"
来源：http://nx.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://ea.szsharing.cn

if let n = opt { print(n) }
来源：http://cy.gzmigu.cn

[T20] Swift：数组操作
来源：http://yw.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gp.shxzskj.cn

[T21] Swift：遍历
来源：http://dp.9csxet.cn

for x in a { print(x) }
来源：http://rj.colortex.cn

[T22] Swift：字典
来源：http://kv.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ui.nszjky.cn

[T23] Swift：函数
来源：http://qz.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wg.9csxet.cn

[T24] Swift：闭包
来源：http://ju.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ud.newstarts.cn

[T25] Swift：结构体
来源：http://lm.asd995.cn

struct P { var x: Int }
来源：http://bq.9csxet.cn

[T26] Swift：类与重写
来源：http://cj.lnxyls.cn

class A: Base { override func f() {} }
来源：http://jz.shxzskj.cn

[T27] Swift：错误处理
来源：http://il.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://yv.newstarts.cn

[T28] Swift：枚举
来源：http://pw.colortex.cn

enum Color { case red, green }
来源：http://yy.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://vu.lnxyls.cn

guard let x = opt else { return }
来源：http://zx.szxytkj.cn

[T30] Swift：协议
来源：http://ow.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://yb.gzmigu.cn

[T31] Lua：Hello World
来源：http://sz.nszjky.cn

print("Hello")
来源：http://qo.hahajie.cn

[T32] Lua：局部变量
来源：http://gy.9csxet.cn

local a = 1
来源：http://jt.newstarts.cn

[T33] Lua：表（数组）
来源：http://zq.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kj.shxzskj.cn

[T34] Lua：遍历表
来源：http://kc.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://og.colortex.cn

[T35] Lua：字典表
来源：http://qa.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://ky.hahajie.cn

[T36] Lua：函数
来源：http://on.colortex.cn

function add(a, b) return a + b end
来源：http://yu.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://bg.hahajie.cn

"a" .. "b"
来源：http://sy.shxzskj.cn

[T38] Lua：条件
来源：http://it.panjiajie.cn

if x > 0 then print("正") end
来源：http://zu.huanxung.cn

[T39] Lua：模式匹配
来源：http://aa.hahajie.cn

string.find(s, "%d+")
来源：http://dv.bjjhwx.cn

[T40] Lua：元表
来源：http://me.9csxet.cn

setmetatable({}, { __index = base })
来源：http://px.gzmigu.cn

[T41] Perl：Hello World
来源：http://bx.9csxet.cn

print "Hello\n";
来源：http://eu.huanxung.cn

[T42] Perl：变量类型
来源：http://yh.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kw.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://vw.jctech888.com.cn

"值: $a"
来源：http://hx.yuexingan06.cn

[T44] Perl：条件
来源：http://xd.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://bl.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://ml.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://xk.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://ue.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ip.hahajie.cn

[T47] Perl：正则捕获
来源：http://fx.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qu.szsharing.cn

[T48] Perl：正则替换
来源：http://ka.521024.cn

$s =~ s/old/new/g;
来源：http://ys.wgjwhj.cn

[T49] Perl：函数
来源：http://mg.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ps.colortex.cn

[T50] Perl：逐行读文件
来源：http://fy.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tm.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://hm.521024.cn

[T51] Scala：Hello World
来源：http://xe.jctech888.com.cn

println("Hello")
来源：http://ug.gzmigu.cn

[T52] Scala：变量
来源：http://wa.chemitech.net.cn

val a = 1;  var b = 2
来源：http://zy.lnxyls.cn

[T53] Scala：字符串插值
来源：http://pu.haigaiapp.cn

s"值: $b"
来源：http://wp.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://ai.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://it.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ti.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wu.huixiangedu.cn

[T56] Scala：样例类
来源：http://bb.521024.cn

case class User(name: String, age: Int)
来源：http://dm.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://hr.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ug.wgjwhj.cn

[T58] Scala：函数定义
来源：http://xz.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dy.colortex.cn

[T59] Scala：循环
来源：http://zd.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://km.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://jd.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gd.colortex.cn

================================================================================
来源：http://oq.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://um.jianghongdianzi.cn

================================================================================
来源：http://pg.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://tn.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jc.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://ll.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wg.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://lx.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rf.colortex.cn

[U04] Py：变量调试打印
来源：http://uv.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pp.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://iv.asd995.cn

list(dict.fromkeys(arr))
来源：http://jn.hnjuh.cn

[U06] Py：合并两个字典
来源：http://ey.szsharing.cn

{**a, **b}
来源：http://xn.9csxet.cn

[U07] Py：反转字典键值
来源：http://yp.521024.cn

{v: k for k, v in d.items()}
来源：http://dl.lnxyls.cn

[U08] Py：展平二维列表
来源：http://ym.panjiajie.cn

[y for x in nested for y in x]
来源：http://dv.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://lw.chemitech.net.cn

max(d, key=d.get)
来源：http://wl.nszjky.cn

[U10] Py：按值排序字典
来源：http://zn.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qp.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://iu.gzmigu.cn

(x * 2 for x in arr)
来源：http://om.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nu.colortex.cn

Counter(arr).most_common(3)
来源：http://wi.shxzukj.cn

[U13] Py：固定长度队列
来源：http://dr.gzmigu.cn

deque(maxlen=10)
来源：http://od.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://rl.bjjhwx.cn

defaultdict(list)
来源：http://rq.szsharing.cn

[U15] Py：高精度计时
来源：http://kc.muxihuayi.cn

t = time.perf_counter()
来源：http://pe.9csxet.cn

[U16] Py：命令行参数解析
来源：http://nv.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ki.muxihuayi.cn

[U17] Py：初始化日志
来源：http://cm.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://xc.huanxung.cn

[U18] Py：预编译正则
来源：http://tz.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://dc.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://qv.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ng.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://ul.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://yb.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ef.521024.cn

@contextlib.contextmanager
来源：http://bn.szxytkj.cn

[U22] Py：矩阵转置
来源：http://zp.muxihuayi.cn

list(zip(*m))
来源：http://ab.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ev.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gw.colortex.cn

[U24] Py：路径操作
来源：http://cj.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ke.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://nj.szsharing.cn

csv.DictReader(f)
来源：http://cu.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://me.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jx.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://ok.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://tu.shxzskj.cn

[U28] Py：类型别名
来源：http://bo.jctech888.com.cn

UserId = int
来源：http://lr.chemitech.net.cn

[U29] Py：属性校验
来源：http://mi.szsharing.cn

@property 与 @x.setter 配合
来源：http://sw.huanxung.cn

[U30] Py：数据类
来源：http://jb.huixiangedu.cn

@dataclass(slots=True)
来源：http://tu.muxihuayi.cn

[U31] Py：单测
来源：http://pn.colortex.cn

python -m pytest -q
来源：http://ss.huixiangedu.cn

[U32] Py：代码格式化
来源：http://mb.hahajie.cn

ruff format . && ruff check --fix .
来源：http://bq.panjiajie.cn

[U33] Py：打包发布
来源：http://he.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ia.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://kg.huixinmuqiang.cn

chardet.detect(raw)
来源：http://sf.9csxet.cn

[U35] Py：发送邮件
来源：http://qa.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xj.huixiangedu.cn

[U36] Py：定时任务
来源：http://ix.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://vj.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://wq.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hr.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://cy.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://kv.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://fb.shtwfgs.cn

sys.stdout.isatty()
来源：http://um.szsharing.cn

[U40] Py：打印到标准错误
来源：http://ei.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://kl.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://xw.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kn.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://gb.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ra.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://rv.colortex.cn

namespace App\Http;
来源：http://ia.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://ff.wgjwhj.cn

declare(strict_types=1);
来源：http://lb.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://jy.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.newstarts.cn

[U46] PHP：可空类型
来源：http://ns.szsharing.cn

?string $name = null
来源：http://qf.bjjhwx.cn

[U47] PHP：联合类型
来源：http://uo.newstarts.cn

int|string $id
来源：http://tl.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://am.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xe.muxihuayi.cn

[U49] PHP：只读属性
来源：http://pn.haigaiapp.cn

public readonly string $name
来源：http://bx.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://bv.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://yp.muxihuayi.cn

[U51] PHP：数组解构
来源：http://td.shtwfgs.cn

[$a, $b] = $arr;
来源：http://zq.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ae.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://kp.huanxung.cn

[U53] PHP：空合并运算符
来源：http://gc.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://gk.hnjuh.cn

[U54] PHP：空安全调用
来源：http://em.shxzukj.cn

$obj?->method()
来源：http://xx.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://qq.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xm.huixiangedu.cn

[U56] PHP：命名参数
来源：http://dl.newstarts.cn

f(a: 1, b: 2)
来源：http://yu.panjiajie.cn

[U57] PHP：字符串插值
来源：http://jq.521024.cn

"值: {$a}"
来源：http://lp.nicolike.cn

[U58] PHP：数组三件套
来源：http://ha.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ca.hnjuh.cn

[U59] PHP：自定义排序
来源：http://ph.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ym.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://yg.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ea.colortex.cn

[U61] PHP：正则
来源：http://jk.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iv.colortex.cn

[U62] PHP：日期对象
来源：http://lt.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pu.wgjwhj.cn


<!-- 参考信息 -->