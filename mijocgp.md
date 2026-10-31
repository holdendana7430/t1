代发 wailian999

[S35] C++：map
来源：http://hz.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://df.wgjwhj.cn

[S36] C++：unordered_map
来源：http://gx.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ar.yuntaijiaju.cn

[S37] C++：set
来源：http://xm.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ev.yuexingan06.cn

[S38] C++：排序
来源：http://kb.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://sv.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://ck.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://co.nszjky.cn

[S40] C++：查找元素
来源：http://mg.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gf.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://kv.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://be.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://dw.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://zo.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://pc.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://rr.nszjky.cn

[S44] C++：引用传参
来源：http://bh.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://zv.szxytkj.cn

[S45] C++：lambda
来源：http://hv.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uf.hnjuh.cn

[S46] C++：函数模板
来源：http://to.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jl.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://wg.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zn.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://rl.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dn.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://tt.jctech888.com.cn

[S49] C++：写文件
来源：http://bo.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uv.szsharing.cn

[S50] C++：格式化数字
来源：http://fx.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xf.521024.cn

[S51] C++：显式类型转换
来源：http://fd.bjjhwx.cn

static_cast<double>(a) / b
来源：http://cw.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://lt.hahajie.cn

int size() const noexcept { return n_; }
来源：http://il.shxzskj.cn

[S53] C++：移动语义
来源：http://nm.521024.cn

std::vector<int> w = std::move(v);
来源：http://he.bjjhwx.cn

[S54] C++：异常处理
来源：http://sa.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gz.szsharing.cn

[S55] C++：结构化绑定
来源：http://as.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mx.lnxyls.cn

[S56] C++：optional
来源：http://le.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bm.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://qb.jianghongdianzi.cn

constexpr int N = 10;
来源：http://df.nszjky.cn

[S58] C++：命名空间
来源：http://ct.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://su.shtwfgs.cn

[S59] C++：静态断言
来源：http://nj.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eo.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://ck.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oy.chemitech.net.cn

================================================================================
来源：http://hd.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://cp.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://nc.muxihuayi.cn

println("Hello")
来源：http://sj.colortex.cn

[T02] Kotlin：变量
来源：http://ta.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ak.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://fl.asd995.cn

"值: $b"
来源：http://yo.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://qb.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://um.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://sv.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jk.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://ie.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nz.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://ap.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pt.asd995.cn

[T08] Kotlin：数据类
来源：http://hf.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://in.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://vd.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://bt.colortex.cn

[T10] Kotlin：默认参数
来源：http://qr.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mh.huanxung.cn

[T11] Kotlin：协程
来源：http://fi.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://at.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://zn.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://lo.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://pu.asd995.cn

val m = mapOf("a" to 1)
来源：http://ep.hahajie.cn

[T14] Kotlin：循环
来源：http://vv.521024.cn

for (i in 1..10) println(i)
来源：http://sm.huixiangedu.cn

[T15] Kotlin：接口
来源：http://xa.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://mu.haigaiapp.cn

[T16] Swift：Hello World
来源：http://zi.521024.cn

print("Hello")
来源：http://za.newstarts.cn

[T17] Swift：变量与常量
来源：http://wm.nszjky.cn

var a = 1;  let b = 2
来源：http://nw.huanxung.cn

[T18] Swift：字符串插值
来源：http://sn.shxzskj.cn

"值: \(b)"
来源：http://qf.9csxet.cn

[T19] Swift：可选绑定
来源：http://xo.szsharing.cn

if let n = opt { print(n) }
来源：http://xm.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://kp.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uz.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://zp.lnxyls.cn

for x in a { print(x) }
来源：http://pl.yuexingan06.cn

[T22] Swift：字典
来源：http://ez.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ls.haigaiapp.cn

[T23] Swift：函数
来源：http://dm.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dt.521024.cn

[T24] Swift：闭包
来源：http://gs.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gl.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://oy.panjiajie.cn

struct P { var x: Int }
来源：http://qa.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://vk.hahajie.cn

class A: Base { override func f() {} }
来源：http://ca.hnjuh.cn

[T27] Swift：错误处理
来源：http://lx.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://vy.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://xq.bjjhwx.cn

enum Color { case red, green }
来源：http://wp.521024.cn

[T29] Swift：guard 提前返回
来源：http://xx.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://ki.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ln.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://mf.wgjwhj.cn

[T31] Lua：Hello World
来源：http://wp.hnjuh.cn

print("Hello")
来源：http://ro.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://yx.chemitech.net.cn

local a = 1
来源：http://yu.huanxung.cn

[T33] Lua：表（数组）
来源：http://tz.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rk.nicolike.cn

[T34] Lua：遍历表
来源：http://rl.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qu.521024.cn

[T35] Lua：字典表
来源：http://qm.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://uq.yuntaijiaju.cn

[T36] Lua：函数
来源：http://jl.chemitech.net.cn

function add(a, b) return a + b end
来源：http://nh.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://xp.wgjwhj.cn

"a" .. "b"
来源：http://pq.szsharing.cn

[T38] Lua：条件
来源：http://pk.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://sl.521024.cn

[T39] Lua：模式匹配
来源：http://aj.szxytkj.cn

string.find(s, "%d+")
来源：http://wl.yuexingan06.cn

[T40] Lua：元表
来源：http://jh.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://wl.nicolike.cn

[T41] Perl：Hello World
来源：http://kv.nszjky.cn

print "Hello\n";
来源：http://xm.gzmigu.cn

[T42] Perl：变量类型
来源：http://vd.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jn.huanxung.cn

[T43] Perl：字符串插值
来源：http://zy.hnjuh.cn

"值: $a"
来源：http://ci.newstarts.cn

[T44] Perl：条件
来源：http://uo.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://nt.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://xj.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://in.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://gb.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ld.newstarts.cn

[T47] Perl：正则捕获
来源：http://sg.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pf.nszjky.cn

[T48] Perl：正则替换
来源：http://ba.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://hq.szxytkj.cn

[T49] Perl：函数
来源：http://rx.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mh.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://kl.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yk.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://et.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://gl.panjiajie.cn

println("Hello")
来源：http://uo.szsharing.cn

[T52] Scala：变量
来源：http://vk.muxihuayi.cn

val a = 1;  var b = 2
来源：http://ci.colortex.cn

[T53] Scala：字符串插值
来源：http://ql.newstarts.cn

s"值: $b"
来源：http://iv.521024.cn

[T54] Scala：集合映射
来源：http://xb.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://ku.szsharing.cn

[T55] Scala：集合过滤
来源：http://sr.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mt.shxzukj.cn

[T56] Scala：样例类
来源：http://cw.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://pu.panjiajie.cn

[T57] Scala：模式匹配
来源：http://pt.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dc.521024.cn

[T58] Scala：函数定义
来源：http://ew.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tf.lnxyls.cn

[T59] Scala：循环
来源：http://gt.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://te.chemitech.net.cn

[T60] Scala：折叠
来源：http://ia.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gw.9csxet.cn

================================================================================
来源：http://tr.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fj.nszjky.cn

================================================================================
来源：http://ed.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://bf.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ji.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://gs.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dz.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://nb.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ss.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://sw.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://et.521024.cn

[U05] Py：列表去重且保序
来源：http://nm.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://tu.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://xn.lnxyls.cn

{**a, **b}
来源：http://at.hnjuh.cn

[U07] Py：反转字典键值
来源：http://gd.nicolike.cn

{v: k for k, v in d.items()}
来源：http://dd.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://fu.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://os.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://la.panjiajie.cn

max(d, key=d.get)
来源：http://cs.lnxyls.cn

[U10] Py：按值排序字典
来源：http://xa.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ok.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://pe.nicolike.cn

(x * 2 for x in arr)
来源：http://qm.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gn.lnxyls.cn

Counter(arr).most_common(3)
来源：http://df.szxytkj.cn

[U13] Py：固定长度队列
来源：http://ie.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ds.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://gi.muxihuayi.cn

defaultdict(list)
来源：http://el.shxzukj.cn

[U15] Py：高精度计时
来源：http://si.panjiajie.cn

t = time.perf_counter()
来源：http://kb.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://nz.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qp.muxihuayi.cn

[U17] Py：初始化日志
来源：http://lp.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://ri.huixiangedu.cn

[U18] Py：预编译正则
来源：http://gz.colortex.cn

pat = re.compile(r"\d+")
来源：http://dn.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ca.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fd.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://yo.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://dh.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://pw.shtwfgs.cn

@contextlib.contextmanager
来源：http://zv.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://zu.bjjhwx.cn

list(zip(*m))
来源：http://cy.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://hv.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sp.chemitech.net.cn

[U24] Py：路径操作
来源：http://ks.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vc.521024.cn

[U25] Py：CSV 按字典读
来源：http://jf.nicolike.cn

csv.DictReader(f)
来源：http://lt.hnjuh.cn

[U26] Py：并发下载
来源：http://zv.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oi.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://ja.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://cb.nicolike.cn

[U28] Py：类型别名
来源：http://es.yuexingan06.cn

UserId = int
来源：http://aj.shxzukj.cn

[U29] Py：属性校验
来源：http://hu.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://pf.shxzskj.cn

[U30] Py：数据类
来源：http://na.lnxyls.cn

@dataclass(slots=True)
来源：http://lx.newstarts.cn

[U31] Py：单测
来源：http://ce.yuexingan06.cn

python -m pytest -q
来源：http://cw.521024.cn

[U32] Py：代码格式化
来源：http://og.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ak.colortex.cn

[U33] Py：打包发布
来源：http://xp.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://al.muxihuayi.cn

[U34] Py：判断编码
来源：http://np.521024.cn

chardet.detect(raw)
来源：http://bu.newstarts.cn

[U35] Py：发送邮件
来源：http://pc.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hp.shxzukj.cn

[U36] Py：定时任务
来源：http://zz.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://vk.panjiajie.cn

[U37] Py：读写 Excel
来源：http://dw.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vs.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://xk.9csxet.cn

Path(__file__).resolve().parent
来源：http://hl.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://el.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://ax.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://as.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://tb.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://kj.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vy.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://cf.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qj.nszjky.cn

[U43] PHP：声明命名空间
来源：http://uq.newstarts.cn

namespace App\Http;
来源：http://ri.huanxung.cn

[U44] PHP：开启严格类型
来源：http://fg.shtwfgs.cn

declare(strict_types=1);
来源：http://nc.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://jn.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://um.gzmigu.cn

[U46] PHP：可空类型
来源：http://gy.haigaiapp.cn

?string $name = null
来源：http://we.nicolike.cn

[U47] PHP：联合类型
来源：http://tt.yuntaijiaju.cn

int|string $id
来源：http://ca.lnxyls.cn

[U48] PHP：纯枚举
来源：http://zn.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ug.yuexingan06.cn

[U49] PHP：只读属性
来源：http://ox.521024.cn

public readonly string $name
来源：http://nj.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://cs.nszjky.cn

public function __construct(private int $id) {}
来源：http://zm.9csxet.cn

[U51] PHP：数组解构
来源：http://ih.muxihuayi.cn

[$a, $b] = $arr;
来源：http://mm.lnxyls.cn

[U52] PHP：箭头函数
来源：http://pq.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://qk.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://di.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://an.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://qs.szsharing.cn

$obj?->method()
来源：http://wl.lnxyls.cn

[U55] PHP：match 表达式
来源：http://vq.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wp.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://uo.panjiajie.cn

f(a: 1, b: 2)
来源：http://yd.nicolike.cn

[U57] PHP：字符串插值
来源：http://ax.9csxet.cn

"值: {$a}"
来源：http://ll.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://xv.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://al.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://ny.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nj.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://op.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qj.szxytkj.cn


<!-- 参考信息 -->