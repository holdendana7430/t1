代发 wailian999

[S39] C++：自定义比较器排序
来源：http://pb.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jh.521024.cn

[S40] C++：查找元素
来源：http://xr.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lr.shxzukj.cn

[S41] C++：类与构造函数
来源：http://tw.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xs.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://cr.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://lk.gzmigu.cn

[S43] C++：智能指针
来源：http://cw.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://mv.gzmigu.cn

[S44] C++：引用传参
来源：http://ln.szsharing.cn

void inc(int &x) { ++x; }
来源：http://sq.chemitech.net.cn

[S45] C++：lambda
来源：http://gb.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wj.newstarts.cn

[S46] C++：函数模板
来源：http://pf.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pa.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://be.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rp.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://xy.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://is.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://nr.huixinmuqiang.cn

[S49] C++：写文件
来源：http://lm.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ku.521024.cn

[S50] C++：格式化数字
来源：http://xa.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gi.9csxet.cn

[S51] C++：显式类型转换
来源：http://if.muxihuayi.cn

static_cast<double>(a) / b
来源：http://bk.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://kk.szsharing.cn

int size() const noexcept { return n_; }
来源：http://kp.nicolike.cn

[S53] C++：移动语义
来源：http://uk.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://ht.yuexingan06.cn

[S54] C++：异常处理
来源：http://vi.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nm.shxzukj.cn

[S55] C++：结构化绑定
来源：http://hh.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xw.szsharing.cn

[S56] C++：optional
来源：http://sr.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pu.szxytkj.cn

[S57] C++：编译期常量
来源：http://es.bookmarksfly.cn

constexpr int N = 10;
来源：http://wr.bookmarksfly.cn

[S58] C++：命名空间
来源：http://ej.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://na.newstarts.cn

[S59] C++：静态断言
来源：http://hj.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ty.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://wt.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://en.shtwfgs.cn

================================================================================
来源：http://nc.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gg.shxzukj.cn

================================================================================
来源：http://da.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://ha.newstarts.cn

println("Hello")
来源：http://kw.colortex.cn

[T02] Kotlin：变量
来源：http://ke.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oh.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://zs.shxzskj.cn

"值: $b"
来源：http://qw.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://rh.asd995.cn

val n: String? = null;  n?.length
来源：http://gp.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://wb.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nj.521024.cn

[T06] Kotlin：集合映射
来源：http://po.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dj.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://cf.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ea.szsharing.cn

[T08] Kotlin：数据类
来源：http://hx.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://qr.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://qb.asd995.cn

fun String.exclaim() = this + "!"
来源：http://ru.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://mf.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ul.gzmigu.cn

[T11] Kotlin：协程
来源：http://ah.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ow.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://nc.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://jf.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://jy.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://bg.muxihuayi.cn

[T14] Kotlin：循环
来源：http://zf.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://yh.nszjky.cn

[T15] Kotlin：接口
来源：http://gf.huanxung.cn

interface Shape { fun area(): Double }
来源：http://ml.chemitech.net.cn

[T16] Swift：Hello World
来源：http://zu.shxzukj.cn

print("Hello")
来源：http://rp.shxzukj.cn

[T17] Swift：变量与常量
来源：http://zm.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://cy.shxzskj.cn

[T18] Swift：字符串插值
来源：http://yi.lnxyls.cn

"值: \(b)"
来源：http://kr.huanxung.cn

[T19] Swift：可选绑定
来源：http://jp.nszjky.cn

if let n = opt { print(n) }
来源：http://cv.hahajie.cn

[T20] Swift：数组操作
来源：http://sm.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ei.nicolike.cn

[T21] Swift：遍历
来源：http://qi.bjjhwx.cn

for x in a { print(x) }
来源：http://vm.muxihuayi.cn

[T22] Swift：字典
来源：http://tn.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bj.jianghongdianzi.cn

[T23] Swift：函数
来源：http://bp.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xw.yuexingan06.cn

[T24] Swift：闭包
来源：http://rg.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gi.hnjuh.cn

[T25] Swift：结构体
来源：http://no.hahajie.cn

struct P { var x: Int }
来源：http://ng.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://sg.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://qp.asd995.cn

[T27] Swift：错误处理
来源：http://lz.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://zc.hahajie.cn

[T28] Swift：枚举
来源：http://gf.bjjhwx.cn

enum Color { case red, green }
来源：http://bb.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://yo.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://uu.szsharing.cn

[T30] Swift：协议
来源：http://ia.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ri.nszjky.cn

[T31] Lua：Hello World
来源：http://fp.haigaiapp.cn

print("Hello")
来源：http://qi.521024.cn

[T32] Lua：局部变量
来源：http://kg.lnxyls.cn

local a = 1
来源：http://ok.hahajie.cn

[T33] Lua：表（数组）
来源：http://mn.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vx.wgjwhj.cn

[T34] Lua：遍历表
来源：http://wz.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ur.shtwfgs.cn

[T35] Lua：字典表
来源：http://fy.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://jo.hnjuh.cn

[T36] Lua：函数
来源：http://et.szsharing.cn

function add(a, b) return a + b end
来源：http://bs.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://gi.bjjhwx.cn

"a" .. "b"
来源：http://rk.shxzskj.cn

[T38] Lua：条件
来源：http://pe.newstarts.cn

if x > 0 then print("正") end
来源：http://og.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://ta.haigaiapp.cn

string.find(s, "%d+")
来源：http://si.jctech888.com.cn

[T40] Lua：元表
来源：http://bi.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://qj.hnjuh.cn

[T41] Perl：Hello World
来源：http://zr.bookmarksfly.cn

print "Hello\n";
来源：http://su.colortex.cn

[T42] Perl：变量类型
来源：http://mw.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wg.szxytkj.cn

[T43] Perl：字符串插值
来源：http://gv.nicolike.cn

"值: $a"
来源：http://bm.shtwfgs.cn

[T44] Perl：条件
来源：http://bz.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://rf.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://sz.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://vh.szxytkj.cn

[T46] Perl：哈希操作
来源：http://cq.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ia.newstarts.cn

[T47] Perl：正则捕获
来源：http://tt.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gn.521024.cn

[T48] Perl：正则替换
来源：http://bz.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://vl.szsharing.cn

[T49] Perl：函数
来源：http://im.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qs.nicolike.cn

[T50] Perl：逐行读文件
来源：http://bn.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pv.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://no.shxzskj.cn

[T51] Scala：Hello World
来源：http://mq.jctech888.com.cn

println("Hello")
来源：http://oo.newstarts.cn

[T52] Scala：变量
来源：http://fv.bjjhwx.cn

val a = 1;  var b = 2
来源：http://zf.shxzskj.cn

[T53] Scala：字符串插值
来源：http://zo.panjiajie.cn

s"值: $b"
来源：http://wv.9csxet.cn

[T54] Scala：集合映射
来源：http://mn.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://tr.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ne.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ld.huixiangedu.cn

[T56] Scala：样例类
来源：http://kl.asd995.cn

case class User(name: String, age: Int)
来源：http://bf.hnjuh.cn

[T57] Scala：模式匹配
来源：http://hi.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qr.hahajie.cn

[T58] Scala：函数定义
来源：http://rv.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://as.panjiajie.cn

[T59] Scala：循环
来源：http://yh.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://nh.shxzukj.cn

[T60] Scala：折叠
来源：http://hd.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eg.newstarts.cn

================================================================================
来源：http://qi.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tc.9csxet.cn

================================================================================
来源：http://dz.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://gf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dl.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://ty.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mq.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://qh.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pa.hahajie.cn

[U04] Py：变量调试打印
来源：http://xy.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dh.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://rs.colortex.cn

list(dict.fromkeys(arr))
来源：http://dk.szxytkj.cn

[U06] Py：合并两个字典
来源：http://ky.muxihuayi.cn

{**a, **b}
来源：http://yk.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://gm.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://nk.hnjuh.cn

[U08] Py：展平二维列表
来源：http://vf.asd995.cn

[y for x in nested for y in x]
来源：http://nn.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://ht.shxzskj.cn

max(d, key=d.get)
来源：http://jp.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://wh.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://no.colortex.cn

[U11] Py：生成器表达式
来源：http://ls.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://dd.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://du.asd995.cn

Counter(arr).most_common(3)
来源：http://zw.asd995.cn

[U13] Py：固定长度队列
来源：http://bz.shxzskj.cn

deque(maxlen=10)
来源：http://ef.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://lo.yuntaijiaju.cn

defaultdict(list)
来源：http://kv.nicolike.cn

[U15] Py：高精度计时
来源：http://lo.huixiangedu.cn

t = time.perf_counter()
来源：http://fh.newstarts.cn

[U16] Py：命令行参数解析
来源：http://zd.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pg.shxzukj.cn

[U17] Py：初始化日志
来源：http://vp.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://sh.yuexingan06.cn

[U18] Py：预编译正则
来源：http://oh.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://lq.9csxet.cn

[U19] Py：正则替换带回调
来源：http://ra.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hl.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://ix.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://kr.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://pu.shxzukj.cn

@contextlib.contextmanager
来源：http://wt.szsharing.cn

[U22] Py：矩阵转置
来源：http://wy.nszjky.cn

list(zip(*m))
来源：http://aq.asd995.cn

[U23] Py：分块读取大文件
来源：http://ig.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ud.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://at.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hk.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://yl.chemitech.net.cn

csv.DictReader(f)
来源：http://vi.colortex.cn

[U26] Py：并发下载
来源：http://yc.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ic.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://kp.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://pm.szxytkj.cn

[U28] Py：类型别名
来源：http://um.jianghongdianzi.cn

UserId = int
来源：http://yf.huanxung.cn

[U29] Py：属性校验
来源：http://jm.newstarts.cn

@property 与 @x.setter 配合
来源：http://ko.bookmarksfly.cn

[U30] Py：数据类
来源：http://dy.shtwfgs.cn

@dataclass(slots=True)
来源：http://zl.szsharing.cn

[U31] Py：单测
来源：http://ir.nicolike.cn

python -m pytest -q
来源：http://uc.9csxet.cn

[U32] Py：代码格式化
来源：http://cf.asd995.cn

ruff format . && ruff check --fix .
来源：http://pf.9csxet.cn

[U33] Py：打包发布
来源：http://ge.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://bs.shxzukj.cn

[U34] Py：判断编码
来源：http://ht.jctech888.com.cn

chardet.detect(raw)
来源：http://yz.gzmigu.cn

[U35] Py：发送邮件
来源：http://ex.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pg.lnxyls.cn

[U36] Py：定时任务
来源：http://wr.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://bv.nicolike.cn

[U37] Py：读写 Excel
来源：http://nr.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jp.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://yg.9csxet.cn

Path(__file__).resolve().parent
来源：http://us.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://pb.lnxyls.cn

sys.stdout.isatty()
来源：http://zw.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ob.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://ha.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://go.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ea.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://hm.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ux.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://gh.shtwfgs.cn

namespace App\Http;
来源：http://su.szsharing.cn

[U44] PHP：开启严格类型
来源：http://qh.szxytkj.cn

declare(strict_types=1);
来源：http://hc.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://kl.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ww.jctech888.com.cn

[U46] PHP：可空类型
来源：http://lk.hahajie.cn

?string $name = null
来源：http://yx.shxzukj.cn

[U47] PHP：联合类型
来源：http://gf.nszjky.cn

int|string $id
来源：http://xa.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://ov.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ux.haigaiapp.cn

[U49] PHP：只读属性
来源：http://lc.jianghongdianzi.cn

public readonly string $name
来源：http://km.colortex.cn

[U50] PHP：构造器属性提升
来源：http://dy.shxzskj.cn

public function __construct(private int $id) {}
来源：http://dr.wgjwhj.cn

[U51] PHP：数组解构
来源：http://uy.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://jp.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://pd.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://gq.szsharing.cn

[U53] PHP：空合并运算符
来源：http://kn.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://ur.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://hw.szsharing.cn

$obj?->method()
来源：http://oe.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://kk.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ty.huixiangedu.cn

[U56] PHP：命名参数
来源：http://yi.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://da.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://sl.lnxyls.cn

"值: {$a}"
来源：http://vd.newstarts.cn

[U58] PHP：数组三件套
来源：http://wg.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lr.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ld.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://bc.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ao.bjjhwx.cn

[U61] PHP：正则
来源：http://um.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dw.bjjhwx.cn

[U62] PHP：日期对象
来源：http://nd.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cc.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://gs.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kr.shxzskj.cn

[U64] PHP：目录遍历
来源：http://ka.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://cj.shtwfgs.cn


<!-- 参考信息 -->