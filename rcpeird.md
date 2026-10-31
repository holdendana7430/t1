代发 wailian999

[S41] C++：类与构造函数
来源：http://we.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xk.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://pc.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://qc.hahajie.cn

[S43] C++：智能指针
来源：http://fx.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://ya.panjiajie.cn

[S44] C++：引用传参
来源：http://qk.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://oh.newstarts.cn

[S45] C++：lambda
来源：http://wv.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xs.nicolike.cn

[S46] C++：函数模板
来源：http://xo.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://df.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ca.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lk.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ta.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zs.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ho.jianghongdianzi.cn

[S49] C++：写文件
来源：http://jj.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sn.szxytkj.cn

[S50] C++：格式化数字
来源：http://ao.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pa.colortex.cn

[S51] C++：显式类型转换
来源：http://hy.shtwfgs.cn

static_cast<double>(a) / b
来源：http://zr.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://kq.szsharing.cn

int size() const noexcept { return n_; }
来源：http://we.szxytkj.cn

[S53] C++：移动语义
来源：http://vx.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://fr.szxytkj.cn

[S54] C++：异常处理
来源：http://dj.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uu.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://mb.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ww.huixiangedu.cn

[S56] C++：optional
来源：http://gy.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mi.shxzukj.cn

[S57] C++：编译期常量
来源：http://ex.haigaiapp.cn

constexpr int N = 10;
来源：http://ce.szxytkj.cn

[S58] C++：命名空间
来源：http://sr.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://lo.nicolike.cn

[S59] C++：静态断言
来源：http://dj.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zb.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://hn.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dn.shxzukj.cn

================================================================================
来源：http://hf.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nd.asd995.cn

================================================================================
来源：http://pz.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://cn.yuntaijiaju.cn

println("Hello")
来源：http://nf.asd995.cn

[T02] Kotlin：变量
来源：http://vk.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kb.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://yn.bjjhwx.cn

"值: $b"
来源：http://xy.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://sd.panjiajie.cn

val n: String? = null;  n?.length
来源：http://jh.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://bf.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://az.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://cd.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jx.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://wh.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vx.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://dx.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://am.521024.cn

[T09] Kotlin：扩展函数
来源：http://li.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://jz.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://ij.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dd.haigaiapp.cn

[T11] Kotlin：协程
来源：http://jj.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hm.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://tz.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://ma.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://kn.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://oo.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ck.shxzskj.cn

for (i in 1..10) println(i)
来源：http://wv.asd995.cn

[T15] Kotlin：接口
来源：http://vk.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://hf.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://hh.9csxet.cn

print("Hello")
来源：http://qk.9csxet.cn

[T17] Swift：变量与常量
来源：http://np.hahajie.cn

var a = 1;  let b = 2
来源：http://hj.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://dg.hnjuh.cn

"值: \(b)"
来源：http://yw.nszjky.cn

[T19] Swift：可选绑定
来源：http://gt.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://qg.asd995.cn

[T20] Swift：数组操作
来源：http://rg.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mz.hnjuh.cn

[T21] Swift：遍历
来源：http://gj.nszjky.cn

for x in a { print(x) }
来源：http://kz.huixinmuqiang.cn

[T22] Swift：字典
来源：http://hg.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hq.colortex.cn

[T23] Swift：函数
来源：http://hz.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tp.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://zs.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://am.jctech888.com.cn

[T25] Swift：结构体
来源：http://xw.muxihuayi.cn

struct P { var x: Int }
来源：http://nt.huanxung.cn

[T26] Swift：类与重写
来源：http://sg.panjiajie.cn

class A: Base { override func f() {} }
来源：http://vi.szsharing.cn

[T27] Swift：错误处理
来源：http://ne.9csxet.cn

do { try f() } catch { print(error) }
来源：http://fk.shxzskj.cn

[T28] Swift：枚举
来源：http://ie.gzmigu.cn

enum Color { case red, green }
来源：http://yw.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://qn.lnxyls.cn

guard let x = opt else { return }
来源：http://wu.newstarts.cn

[T30] Swift：协议
来源：http://vf.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ve.huanxung.cn

[T31] Lua：Hello World
来源：http://zg.jctech888.com.cn

print("Hello")
来源：http://td.521024.cn

[T32] Lua：局部变量
来源：http://fz.panjiajie.cn

local a = 1
来源：http://jl.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://hy.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nv.nicolike.cn

[T34] Lua：遍历表
来源：http://oy.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ab.shxzskj.cn

[T35] Lua：字典表
来源：http://eb.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://cu.hnjuh.cn

[T36] Lua：函数
来源：http://ba.nicolike.cn

function add(a, b) return a + b end
来源：http://sp.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://tz.szsharing.cn

"a" .. "b"
来源：http://jy.jianghongdianzi.cn

[T38] Lua：条件
来源：http://yt.nszjky.cn

if x > 0 then print("正") end
来源：http://wj.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://wk.haigaiapp.cn

string.find(s, "%d+")
来源：http://wm.shxzskj.cn

[T40] Lua：元表
来源：http://kx.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://yv.shxzukj.cn

[T41] Perl：Hello World
来源：http://di.szsharing.cn

print "Hello\n";
来源：http://bc.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://ok.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bo.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://gr.colortex.cn

"值: $a"
来源：http://zj.jctech888.com.cn

[T44] Perl：条件
来源：http://ws.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ln.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://nv.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://du.hahajie.cn

[T46] Perl：哈希操作
来源：http://yc.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://em.hahajie.cn

[T47] Perl：正则捕获
来源：http://fg.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eu.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://xx.521024.cn

$s =~ s/old/new/g;
来源：http://jl.hahajie.cn

[T49] Perl：函数
来源：http://mk.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ja.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://iv.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fd.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://ow.hahajie.cn

[T51] Scala：Hello World
来源：http://kg.shtwfgs.cn

println("Hello")
来源：http://oy.colortex.cn

[T52] Scala：变量
来源：http://vh.shtwfgs.cn

val a = 1;  var b = 2
来源：http://yz.nszjky.cn

[T53] Scala：字符串插值
来源：http://ka.haigaiapp.cn

s"值: $b"
来源：http://gf.shtwfgs.cn

[T54] Scala：集合映射
来源：http://yf.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://wx.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://nu.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iy.szsharing.cn

[T56] Scala：样例类
来源：http://uz.hahajie.cn

case class User(name: String, age: Int)
来源：http://pu.lnxyls.cn

[T57] Scala：模式匹配
来源：http://xc.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fd.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://dl.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zr.chemitech.net.cn

[T59] Scala：循环
来源：http://le.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://xu.muxihuayi.cn

[T60] Scala：折叠
来源：http://qu.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fx.haigaiapp.cn

================================================================================
来源：http://zm.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fj.bjjhwx.cn

================================================================================
来源：http://uz.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ax.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ff.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://iq.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iw.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://cu.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pq.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://lx.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ml.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://ea.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://pa.nszjky.cn

[U06] Py：合并两个字典
来源：http://dz.huanxung.cn

{**a, **b}
来源：http://as.shxzskj.cn

[U07] Py：反转字典键值
来源：http://do.9csxet.cn

{v: k for k, v in d.items()}
来源：http://br.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://td.521024.cn

[y for x in nested for y in x]
来源：http://uz.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://ia.9csxet.cn

max(d, key=d.get)
来源：http://kp.gzmigu.cn

[U10] Py：按值排序字典
来源：http://tw.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vh.panjiajie.cn

[U11] Py：生成器表达式
来源：http://ms.521024.cn

(x * 2 for x in arr)
来源：http://mc.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lk.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://kx.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://be.haigaiapp.cn

deque(maxlen=10)
来源：http://xd.colortex.cn

[U14] Py：分组收集到列表
来源：http://ek.colortex.cn

defaultdict(list)
来源：http://ek.asd995.cn

[U15] Py：高精度计时
来源：http://tb.yuexingan06.cn

t = time.perf_counter()
来源：http://zx.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://wp.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hu.bjjhwx.cn

[U17] Py：初始化日志
来源：http://xx.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://vu.chemitech.net.cn

[U18] Py：预编译正则
来源：http://us.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://qn.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://oy.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ed.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://vo.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://nk.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://rl.panjiajie.cn

@contextlib.contextmanager
来源：http://od.asd995.cn

[U22] Py：矩阵转置
来源：http://ck.wgjwhj.cn

list(zip(*m))
来源：http://qx.nicolike.cn

[U23] Py：分块读取大文件
来源：http://kn.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tl.lnxyls.cn

[U24] Py：路径操作
来源：http://ak.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xb.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ay.shxzskj.cn

csv.DictReader(f)
来源：http://fc.shxzskj.cn

[U26] Py：并发下载
来源：http://fa.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jc.nicolike.cn

[U27] Py：异步 HTTP
来源：http://pr.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://ys.lnxyls.cn

[U28] Py：类型别名
来源：http://ys.nicolike.cn

UserId = int
来源：http://xh.newstarts.cn

[U29] Py：属性校验
来源：http://dj.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://kw.521024.cn

[U30] Py：数据类
来源：http://xp.shtwfgs.cn

@dataclass(slots=True)
来源：http://bd.huixiangedu.cn

[U31] Py：单测
来源：http://fn.bjjhwx.cn

python -m pytest -q
来源：http://pi.jctech888.com.cn

[U32] Py：代码格式化
来源：http://cr.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://jl.lnxyls.cn

[U33] Py：打包发布
来源：http://bv.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://vl.chemitech.net.cn

[U34] Py：判断编码
来源：http://ub.szsharing.cn

chardet.detect(raw)
来源：http://ht.wgjwhj.cn

[U35] Py：发送邮件
来源：http://tp.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eg.szsharing.cn

[U36] Py：定时任务
来源：http://tk.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://dr.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://jn.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nk.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://ex.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://yo.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://ac.shxzukj.cn

sys.stdout.isatty()
来源：http://pa.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://jh.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://sg.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://tz.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gv.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://ge.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rt.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://sr.muxihuayi.cn

namespace App\Http;
来源：http://fs.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://kt.huanxung.cn

declare(strict_types=1);
来源：http://ki.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://ot.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qj.lnxyls.cn

[U46] PHP：可空类型
来源：http://ex.wgjwhj.cn

?string $name = null
来源：http://dz.wgjwhj.cn

[U47] PHP：联合类型
来源：http://vb.muxihuayi.cn

int|string $id
来源：http://uk.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://cv.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hr.colortex.cn

[U49] PHP：只读属性
来源：http://fb.asd995.cn

public readonly string $name
来源：http://cx.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://ix.hnjuh.cn

public function __construct(private int $id) {}
来源：http://in.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://aj.shtwfgs.cn

[$a, $b] = $arr;
来源：http://ju.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://kq.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://sg.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://pe.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://wu.shxzukj.cn

[U54] PHP：空安全调用
来源：http://zr.nszjky.cn

$obj?->method()
来源：http://rf.szxytkj.cn

[U55] PHP：match 表达式
来源：http://hy.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vi.shxzskj.cn

[U56] PHP：命名参数
来源：http://hu.newstarts.cn

f(a: 1, b: 2)
来源：http://bv.9csxet.cn

[U57] PHP：字符串插值
来源：http://yy.shxzukj.cn

"值: {$a}"
来源：http://vc.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://xf.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nz.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://bz.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vo.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://tc.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yx.haigaiapp.cn

[U61] PHP：正则
来源：http://dz.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cq.panjiajie.cn

[U62] PHP：日期对象
来源：http://rt.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mj.haigaiapp.cn

[U63] PHP：文件读写
来源：http://re.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wj.newstarts.cn

[U64] PHP：目录遍历
来源：http://cs.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://gl.shxzukj.cn

[U65] PHP：会话
来源：http://rc.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cl.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://mc.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bq.muxihuayi.cn


<!-- 参考信息 -->