代发 wailian999

[S35] C++：map
来源：http://ji.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ur.shtwfgs.cn

[S36] C++：unordered_map
来源：http://eb.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bw.nicolike.cn

[S37] C++：set
来源：http://ij.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://it.hnjuh.cn

[S38] C++：排序
来源：http://pz.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://wt.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ij.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cv.shtwfgs.cn

[S40] C++：查找元素
来源：http://mn.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ay.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://mv.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eb.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://yz.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://ds.bookmarksfly.cn

[S43] C++：智能指针
来源：http://hf.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://qk.chemitech.net.cn

[S44] C++：引用传参
来源：http://nl.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://cg.lnxyls.cn

[S45] C++：lambda
来源：http://zj.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rn.jctech888.com.cn

[S46] C++：函数模板
来源：http://ht.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ny.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://js.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zm.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://lg.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sv.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://lh.9csxet.cn

[S49] C++：写文件
来源：http://ec.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qg.9csxet.cn

[S50] C++：格式化数字
来源：http://yi.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vs.nicolike.cn

[S51] C++：显式类型转换
来源：http://ri.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://as.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://dc.nicolike.cn

int size() const noexcept { return n_; }
来源：http://dq.haigaiapp.cn

[S53] C++：移动语义
来源：http://xh.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://rb.jctech888.com.cn

[S54] C++：异常处理
来源：http://ic.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ph.hahajie.cn

[S55] C++：结构化绑定
来源：http://co.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ua.gzmigu.cn

[S56] C++：optional
来源：http://hs.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sn.szxytkj.cn

[S57] C++：编译期常量
来源：http://jf.jianghongdianzi.cn

constexpr int N = 10;
来源：http://xn.muxihuayi.cn

[S58] C++：命名空间
来源：http://rl.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://lv.shxzukj.cn

[S59] C++：静态断言
来源：http://ya.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qa.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://op.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kn.szxytkj.cn

================================================================================
来源：http://cz.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://si.bookmarksfly.cn

================================================================================
来源：http://lr.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://gw.nszjky.cn

println("Hello")
来源：http://fn.shxzskj.cn

[T02] Kotlin：变量
来源：http://vw.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qk.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://yc.nszjky.cn

"值: $b"
来源：http://hm.panjiajie.cn

[T04] Kotlin：空安全
来源：http://yt.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://im.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://cz.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fm.hahajie.cn

[T06] Kotlin：集合映射
来源：http://oo.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cq.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ux.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bf.asd995.cn

[T08] Kotlin：数据类
来源：http://xj.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://vf.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://ps.asd995.cn

fun String.exclaim() = this + "!"
来源：http://ay.nicolike.cn

[T10] Kotlin：默认参数
来源：http://lk.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ma.colortex.cn

[T11] Kotlin：协程
来源：http://lb.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ms.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://wo.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://jh.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://fc.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://sz.huanxung.cn

[T14] Kotlin：循环
来源：http://lg.nszjky.cn

for (i in 1..10) println(i)
来源：http://xx.colortex.cn

[T15] Kotlin：接口
来源：http://zr.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://mb.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://ez.huanxung.cn

print("Hello")
来源：http://cf.shxzskj.cn

[T17] Swift：变量与常量
来源：http://fb.szsharing.cn

var a = 1;  let b = 2
来源：http://uu.szsharing.cn

[T18] Swift：字符串插值
来源：http://ao.shtwfgs.cn

"值: \(b)"
来源：http://kh.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://ad.haigaiapp.cn

if let n = opt { print(n) }
来源：http://le.colortex.cn

[T20] Swift：数组操作
来源：http://qt.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xj.nicolike.cn

[T21] Swift：遍历
来源：http://jx.yuntaijiaju.cn

for x in a { print(x) }
来源：http://lk.shxzukj.cn

[T22] Swift：字典
来源：http://nv.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://id.huixiangedu.cn

[T23] Swift：函数
来源：http://pt.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://we.nszjky.cn

[T24] Swift：闭包
来源：http://qb.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://br.shxzskj.cn

[T25] Swift：结构体
来源：http://ai.haigaiapp.cn

struct P { var x: Int }
来源：http://gp.nszjky.cn

[T26] Swift：类与重写
来源：http://fk.huanxung.cn

class A: Base { override func f() {} }
来源：http://yi.hahajie.cn

[T27] Swift：错误处理
来源：http://pt.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://wl.chemitech.net.cn

[T28] Swift：枚举
来源：http://it.jctech888.com.cn

enum Color { case red, green }
来源：http://vm.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://tc.huanxung.cn

guard let x = opt else { return }
来源：http://zi.yuexingan06.cn

[T30] Swift：协议
来源：http://fb.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://lr.nicolike.cn

[T31] Lua：Hello World
来源：http://si.panjiajie.cn

print("Hello")
来源：http://xl.hnjuh.cn

[T32] Lua：局部变量
来源：http://yq.yuexingan06.cn

local a = 1
来源：http://cu.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ok.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yg.521024.cn

[T34] Lua：遍历表
来源：http://sp.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hp.asd995.cn

[T35] Lua：字典表
来源：http://om.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://xr.hahajie.cn

[T36] Lua：函数
来源：http://wx.yuexingan06.cn

function add(a, b) return a + b end
来源：http://pq.colortex.cn

[T37] Lua：字符串拼接
来源：http://sb.hnjuh.cn

"a" .. "b"
来源：http://jc.muxihuayi.cn

[T38] Lua：条件
来源：http://nj.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://pv.colortex.cn

[T39] Lua：模式匹配
来源：http://zt.bjjhwx.cn

string.find(s, "%d+")
来源：http://dl.yuexingan06.cn

[T40] Lua：元表
来源：http://dh.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://rq.hahajie.cn

[T41] Perl：Hello World
来源：http://ba.521024.cn

print "Hello\n";
来源：http://za.muxihuayi.cn

[T42] Perl：变量类型
来源：http://yz.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xg.panjiajie.cn

[T43] Perl：字符串插值
来源：http://be.panjiajie.cn

"值: $a"
来源：http://lk.yuexingan06.cn

[T44] Perl：条件
来源：http://xj.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://qu.nicolike.cn

[T45] Perl：数组遍历
来源：http://oi.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://jn.hnjuh.cn

[T46] Perl：哈希操作
来源：http://bs.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xo.asd995.cn

[T47] Perl：正则捕获
来源：http://de.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ou.hahajie.cn

[T48] Perl：正则替换
来源：http://oq.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://jq.huixiangedu.cn

[T49] Perl：函数
来源：http://pf.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gu.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://yz.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xu.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://wb.521024.cn

[T51] Scala：Hello World
来源：http://st.nicolike.cn

println("Hello")
来源：http://qt.shtwfgs.cn

[T52] Scala：变量
来源：http://ma.colortex.cn

val a = 1;  var b = 2
来源：http://zm.huanxung.cn

[T53] Scala：字符串插值
来源：http://lk.colortex.cn

s"值: $b"
来源：http://sl.wgjwhj.cn

[T54] Scala：集合映射
来源：http://xy.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://hd.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://sp.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ig.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://ii.hahajie.cn

case class User(name: String, age: Int)
来源：http://le.asd995.cn

[T57] Scala：模式匹配
来源：http://gg.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zc.9csxet.cn

[T58] Scala：函数定义
来源：http://yb.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ol.jianghongdianzi.cn

[T59] Scala：循环
来源：http://rg.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://fe.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://jl.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ec.jctech888.com.cn

================================================================================
来源：http://ao.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hu.bjjhwx.cn

================================================================================
来源：http://sw.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://cz.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oh.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://nv.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aw.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://cg.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sg.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://rc.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ld.nicolike.cn

[U05] Py：列表去重且保序
来源：http://oa.newstarts.cn

list(dict.fromkeys(arr))
来源：http://lu.shxzskj.cn

[U06] Py：合并两个字典
来源：http://rg.yuntaijiaju.cn

{**a, **b}
来源：http://tc.hahajie.cn

[U07] Py：反转字典键值
来源：http://xm.hahajie.cn

{v: k for k, v in d.items()}
来源：http://nw.newstarts.cn

[U08] Py：展平二维列表
来源：http://pl.hnjuh.cn

[y for x in nested for y in x]
来源：http://hh.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://qq.huixinmuqiang.cn

max(d, key=d.get)
来源：http://cq.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://gn.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://en.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://ve.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://tr.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lt.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://gp.hnjuh.cn

[U13] Py：固定长度队列
来源：http://qg.panjiajie.cn

deque(maxlen=10)
来源：http://xm.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://xe.huanxung.cn

defaultdict(list)
来源：http://oy.hnjuh.cn

[U15] Py：高精度计时
来源：http://et.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ck.nicolike.cn

[U16] Py：命令行参数解析
来源：http://qe.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jd.jctech888.com.cn

[U17] Py：初始化日志
来源：http://lm.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://ao.gzmigu.cn

[U18] Py：预编译正则
来源：http://nd.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://vp.9csxet.cn

[U19] Py：正则替换带回调
来源：http://sf.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dc.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://rp.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://ab.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://da.jctech888.com.cn

@contextlib.contextmanager
来源：http://wu.shxzskj.cn

[U22] Py：矩阵转置
来源：http://pe.newstarts.cn

list(zip(*m))
来源：http://qc.colortex.cn

[U23] Py：分块读取大文件
来源：http://js.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qr.shxzskj.cn

[U24] Py：路径操作
来源：http://cb.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ow.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://wo.wgjwhj.cn

csv.DictReader(f)
来源：http://vf.shxzukj.cn

[U26] Py：并发下载
来源：http://js.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kp.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://zo.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://go.9csxet.cn

[U28] Py：类型别名
来源：http://ht.huixinmuqiang.cn

UserId = int
来源：http://mz.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://mh.nicolike.cn

@property 与 @x.setter 配合
来源：http://aa.nszjky.cn

[U30] Py：数据类
来源：http://ho.newstarts.cn

@dataclass(slots=True)
来源：http://qa.huixinmuqiang.cn

[U31] Py：单测
来源：http://io.asd995.cn

python -m pytest -q
来源：http://fj.shxzskj.cn

[U32] Py：代码格式化
来源：http://te.newstarts.cn

ruff format . && ruff check --fix .
来源：http://ck.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://tz.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://gy.hnjuh.cn

[U34] Py：判断编码
来源：http://bp.muxihuayi.cn

chardet.detect(raw)
来源：http://rh.9csxet.cn

[U35] Py：发送邮件
来源：http://qa.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ug.9csxet.cn

[U36] Py：定时任务
来源：http://sc.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://aj.newstarts.cn

[U37] Py：读写 Excel
来源：http://yn.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ek.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://mq.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://fp.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://xq.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://wt.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://eo.521024.cn

print("err", file=sys.stderr)
来源：http://ow.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://sk.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bp.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://ty.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rx.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://ep.shtwfgs.cn

namespace App\Http;
来源：http://ts.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://fi.521024.cn

declare(strict_types=1);
来源：http://wx.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://fx.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dm.colortex.cn

[U46] PHP：可空类型
来源：http://ao.yuntaijiaju.cn

?string $name = null
来源：http://hf.shxzskj.cn

[U47] PHP：联合类型
来源：http://rj.jianghongdianzi.cn

int|string $id
来源：http://op.newstarts.cn

[U48] PHP：纯枚举
来源：http://xb.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oo.chemitech.net.cn

[U49] PHP：只读属性
来源：http://ay.lnxyls.cn

public readonly string $name
来源：http://dg.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://mh.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://jv.panjiajie.cn

[U51] PHP：数组解构
来源：http://jf.shxzskj.cn

[$a, $b] = $arr;
来源：http://ci.9csxet.cn

[U52] PHP：箭头函数
来源：http://zj.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://jp.nicolike.cn

[U53] PHP：空合并运算符
来源：http://ul.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://sn.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://gb.nszjky.cn

$obj?->method()
来源：http://jx.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ap.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://is.9csxet.cn

[U56] PHP：命名参数
来源：http://za.shtwfgs.cn

f(a: 1, b: 2)
来源：http://gt.hahajie.cn

[U57] PHP：字符串插值
来源：http://rh.chemitech.net.cn

"值: {$a}"
来源：http://je.shxzskj.cn

[U58] PHP：数组三件套
来源：http://is.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nl.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://gr.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hq.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://xj.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ga.521024.cn


<!-- 参考信息 -->