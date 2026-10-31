代发 wailian999

[S41] C++：类与构造函数
来源：http://wn.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rf.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://bo.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://pd.asd995.cn

[S43] C++：智能指针
来源：http://gs.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://te.wgjwhj.cn

[S44] C++：引用传参
来源：http://im.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://sw.shxzukj.cn

[S45] C++：lambda
来源：http://uw.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fo.hnjuh.cn

[S46] C++：函数模板
来源：http://ac.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qj.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://na.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yq.hahajie.cn

[S48] C++：逐行读文件
来源：http://oi.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xp.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://yl.huixiangedu.cn

[S49] C++：写文件
来源：http://ab.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nr.huanxung.cn

[S50] C++：格式化数字
来源：http://ik.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tp.colortex.cn

[S51] C++：显式类型转换
来源：http://rr.panjiajie.cn

static_cast<double>(a) / b
来源：http://kg.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://jw.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://lm.shxzskj.cn

[S53] C++：移动语义
来源：http://ml.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ot.szxytkj.cn

[S54] C++：异常处理
来源：http://kv.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sy.521024.cn

[S55] C++：结构化绑定
来源：http://nd.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jt.jctech888.com.cn

[S56] C++：optional
来源：http://yt.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bv.muxihuayi.cn

[S57] C++：编译期常量
来源：http://mr.bookmarksfly.cn

constexpr int N = 10;
来源：http://ki.asd995.cn

[S58] C++：命名空间
来源：http://bo.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://gb.chemitech.net.cn

[S59] C++：静态断言
来源：http://ld.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gp.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://ca.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ub.szsharing.cn

================================================================================
来源：http://nc.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eg.huixinmuqiang.cn

================================================================================
来源：http://qp.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ag.gzmigu.cn

println("Hello")
来源：http://ll.jctech888.com.cn

[T02] Kotlin：变量
来源：http://th.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tp.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://jm.colortex.cn

"值: $b"
来源：http://oq.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ww.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://af.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://nh.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pq.szsharing.cn

[T06] Kotlin：集合映射
来源：http://zg.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://is.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ts.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gh.shxzukj.cn

[T08] Kotlin：数据类
来源：http://le.colortex.cn

data class User(val name: String, val age: Int)
来源：http://vq.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://iw.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://sq.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://ct.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wh.hnjuh.cn

[T11] Kotlin：协程
来源：http://ac.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jf.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://ce.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://uk.asd995.cn

[T13] Kotlin：只读 Map
来源：http://sq.asd995.cn

val m = mapOf("a" to 1)
来源：http://ro.gzmigu.cn

[T14] Kotlin：循环
来源：http://if.shxzskj.cn

for (i in 1..10) println(i)
来源：http://js.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://js.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://by.szsharing.cn

[T16] Swift：Hello World
来源：http://di.jctech888.com.cn

print("Hello")
来源：http://px.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://kv.gzmigu.cn

var a = 1;  let b = 2
来源：http://ym.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://yd.gzmigu.cn

"值: \(b)"
来源：http://ui.shxzskj.cn

[T19] Swift：可选绑定
来源：http://bu.shxzukj.cn

if let n = opt { print(n) }
来源：http://ku.shxzukj.cn

[T20] Swift：数组操作
来源：http://rc.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yd.9csxet.cn

[T21] Swift：遍历
来源：http://ei.gzmigu.cn

for x in a { print(x) }
来源：http://um.haigaiapp.cn

[T22] Swift：字典
来源：http://oi.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://en.yuexingan06.cn

[T23] Swift：函数
来源：http://sr.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vc.muxihuayi.cn

[T24] Swift：闭包
来源：http://lz.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oh.colortex.cn

[T25] Swift：结构体
来源：http://ji.haigaiapp.cn

struct P { var x: Int }
来源：http://on.jctech888.com.cn

[T26] Swift：类与重写
来源：http://zj.lnxyls.cn

class A: Base { override func f() {} }
来源：http://bo.colortex.cn

[T27] Swift：错误处理
来源：http://ey.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://sg.521024.cn

[T28] Swift：枚举
来源：http://aw.huixiangedu.cn

enum Color { case red, green }
来源：http://ou.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://ym.9csxet.cn

guard let x = opt else { return }
来源：http://tj.bookmarksfly.cn

[T30] Swift：协议
来源：http://xi.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://bt.hnjuh.cn

[T31] Lua：Hello World
来源：http://nh.newstarts.cn

print("Hello")
来源：http://ph.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://mu.yuntaijiaju.cn

local a = 1
来源：http://pf.shxzukj.cn

[T33] Lua：表（数组）
来源：http://aw.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ws.wgjwhj.cn

[T34] Lua：遍历表
来源：http://wi.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xs.shxzskj.cn

[T35] Lua：字典表
来源：http://pe.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://ee.huixiangedu.cn

[T36] Lua：函数
来源：http://bi.yuexingan06.cn

function add(a, b) return a + b end
来源：http://zw.hahajie.cn

[T37] Lua：字符串拼接
来源：http://vu.521024.cn

"a" .. "b"
来源：http://fv.shxzskj.cn

[T38] Lua：条件
来源：http://xt.chemitech.net.cn

if x > 0 then print("正") end
来源：http://px.hahajie.cn

[T39] Lua：模式匹配
来源：http://bd.huanxung.cn

string.find(s, "%d+")
来源：http://vn.newstarts.cn

[T40] Lua：元表
来源：http://jh.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://gs.nszjky.cn

[T41] Perl：Hello World
来源：http://qr.nicolike.cn

print "Hello\n";
来源：http://bf.nszjky.cn

[T42] Perl：变量类型
来源：http://wx.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://af.9csxet.cn

[T43] Perl：字符串插值
来源：http://wk.shxzukj.cn

"值: $a"
来源：http://kq.haigaiapp.cn

[T44] Perl：条件
来源：http://be.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://xa.asd995.cn

[T45] Perl：数组遍历
来源：http://vv.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://eh.shxzskj.cn

[T46] Perl：哈希操作
来源：http://ia.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://os.huanxung.cn

[T47] Perl：正则捕获
来源：http://ha.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mi.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://td.gzmigu.cn

$s =~ s/old/new/g;
来源：http://oj.panjiajie.cn

[T49] Perl：函数
来源：http://jy.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pl.nicolike.cn

[T50] Perl：逐行读文件
来源：http://xl.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uh.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://xx.shxzukj.cn

[T51] Scala：Hello World
来源：http://er.bjjhwx.cn

println("Hello")
来源：http://hw.nszjky.cn

[T52] Scala：变量
来源：http://zt.9csxet.cn

val a = 1;  var b = 2
来源：http://bj.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://dk.huixiangedu.cn

s"值: $b"
来源：http://aj.chemitech.net.cn

[T54] Scala：集合映射
来源：http://xr.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://hi.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://bg.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gg.asd995.cn

[T56] Scala：样例类
来源：http://ww.521024.cn

case class User(name: String, age: Int)
来源：http://ap.9csxet.cn

[T57] Scala：模式匹配
来源：http://hp.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xk.huanxung.cn

[T58] Scala：函数定义
来源：http://yp.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ws.huixiangedu.cn

[T59] Scala：循环
来源：http://me.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://om.colortex.cn

[T60] Scala：折叠
来源：http://yy.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rp.colortex.cn

================================================================================
来源：http://gk.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pq.hahajie.cn

================================================================================
来源：http://ya.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ab.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qv.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://yx.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://um.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://wb.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sr.nicolike.cn

[U04] Py：变量调试打印
来源：http://tq.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pp.nicolike.cn

[U05] Py：列表去重且保序
来源：http://tn.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://de.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://wr.shxzskj.cn

{**a, **b}
来源：http://an.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://wj.9csxet.cn

{v: k for k, v in d.items()}
来源：http://rh.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://yh.9csxet.cn

[y for x in nested for y in x]
来源：http://zf.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://re.hnjuh.cn

max(d, key=d.get)
来源：http://bf.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://sx.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tg.nszjky.cn

[U11] Py：生成器表达式
来源：http://yd.shxzukj.cn

(x * 2 for x in arr)
来源：http://ad.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ez.szsharing.cn

Counter(arr).most_common(3)
来源：http://ts.newstarts.cn

[U13] Py：固定长度队列
来源：http://lt.521024.cn

deque(maxlen=10)
来源：http://rn.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://mw.szsharing.cn

defaultdict(list)
来源：http://lp.huixiangedu.cn

[U15] Py：高精度计时
来源：http://zw.521024.cn

t = time.perf_counter()
来源：http://yw.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://xg.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vd.colortex.cn

[U17] Py：初始化日志
来源：http://rp.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ks.jctech888.com.cn

[U18] Py：预编译正则
来源：http://ho.521024.cn

pat = re.compile(r"\d+")
来源：http://zl.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://mr.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cb.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://mh.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ek.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://mv.9csxet.cn

@contextlib.contextmanager
来源：http://lp.szsharing.cn

[U22] Py：矩阵转置
来源：http://ix.huixiangedu.cn

list(zip(*m))
来源：http://uk.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://gl.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hf.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://lt.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://am.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://aq.9csxet.cn

csv.DictReader(f)
来源：http://hm.hnjuh.cn

[U26] Py：并发下载
来源：http://wz.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xr.newstarts.cn

[U27] Py：异步 HTTP
来源：http://hp.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ec.panjiajie.cn

[U28] Py：类型别名
来源：http://xk.nicolike.cn

UserId = int
来源：http://vv.szxytkj.cn

[U29] Py：属性校验
来源：http://wp.szxytkj.cn

@property 与 @x.setter 配合
来源：http://yt.gzmigu.cn

[U30] Py：数据类
来源：http://hv.szxytkj.cn

@dataclass(slots=True)
来源：http://ce.szxytkj.cn

[U31] Py：单测
来源：http://mm.colortex.cn

python -m pytest -q
来源：http://ss.yuexingan06.cn

[U32] Py：代码格式化
来源：http://kb.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://ov.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://zb.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://lh.jctech888.com.cn

[U34] Py：判断编码
来源：http://wz.szsharing.cn

chardet.detect(raw)
来源：http://xp.huixiangedu.cn

[U35] Py：发送邮件
来源：http://qj.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cj.gzmigu.cn

[U36] Py：定时任务
来源：http://kf.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://qs.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://ts.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ch.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://rc.asd995.cn

Path(__file__).resolve().parent
来源：http://lh.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://px.bjjhwx.cn

sys.stdout.isatty()
来源：http://fp.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ep.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://vg.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://jh.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uu.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://fm.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dw.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://dp.9csxet.cn

namespace App\Http;
来源：http://qp.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://xf.chemitech.net.cn

declare(strict_types=1);
来源：http://zz.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ko.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wu.huixiangedu.cn

[U46] PHP：可空类型
来源：http://yu.chemitech.net.cn

?string $name = null
来源：http://fz.panjiajie.cn

[U47] PHP：联合类型
来源：http://eh.gzmigu.cn

int|string $id
来源：http://wu.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://ld.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fa.haigaiapp.cn

[U49] PHP：只读属性
来源：http://qs.chemitech.net.cn

public readonly string $name
来源：http://ib.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://qo.9csxet.cn

public function __construct(private int $id) {}
来源：http://hw.huixiangedu.cn

[U51] PHP：数组解构
来源：http://ul.nicolike.cn

[$a, $b] = $arr;
来源：http://xv.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://rx.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://pp.huanxung.cn

[U53] PHP：空合并运算符
来源：http://td.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://uz.521024.cn

[U54] PHP：空安全调用
来源：http://kf.szxytkj.cn

$obj?->method()
来源：http://ka.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://qy.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fm.colortex.cn

[U56] PHP：命名参数
来源：http://wu.muxihuayi.cn

f(a: 1, b: 2)
来源：http://ph.hnjuh.cn

[U57] PHP：字符串插值
来源：http://yf.panjiajie.cn

"值: {$a}"
来源：http://wm.hnjuh.cn

[U58] PHP：数组三件套
来源：http://vu.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nk.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://yn.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ep.asd995.cn

[U60] PHP：JSON 编解码
来源：http://pi.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dy.huixinmuqiang.cn

[U61] PHP：正则
来源：http://ri.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fs.huixiangedu.cn

[U62] PHP：日期对象
来源：http://fo.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xe.newstarts.cn

[U63] PHP：文件读写
来源：http://nw.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mn.hahajie.cn

[U64] PHP：目录遍历
来源：http://wm.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://tw.nszjky.cn

[U65] PHP：会话
来源：http://bl.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cj.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://ad.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gw.muxihuayi.cn


<!-- 参考信息 -->