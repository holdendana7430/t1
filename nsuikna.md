代发 wailian999

[S37] C++：set
来源：http://cs.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ht.nicolike.cn

[S38] C++：排序
来源：http://kk.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://zo.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://qd.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oq.gzmigu.cn

[S40] C++：查找元素
来源：http://th.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uz.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://zd.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wp.9csxet.cn

[S42] C++：继承与虚函数
来源：http://qq.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ul.colortex.cn

[S43] C++：智能指针
来源：http://ni.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://hk.nszjky.cn

[S44] C++：引用传参
来源：http://ua.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://vn.lnxyls.cn

[S45] C++：lambda
来源：http://ja.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ud.lnxyls.cn

[S46] C++：函数模板
来源：http://vr.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tq.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ap.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qs.huanxung.cn

[S48] C++：逐行读文件
来源：http://tf.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yv.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://fy.asd995.cn

[S49] C++：写文件
来源：http://ad.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nq.9csxet.cn

[S50] C++：格式化数字
来源：http://pg.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ev.521024.cn

[S51] C++：显式类型转换
来源：http://sm.asd995.cn

static_cast<double>(a) / b
来源：http://id.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://hd.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://oe.hnjuh.cn

[S53] C++：移动语义
来源：http://tl.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://uy.wgjwhj.cn

[S54] C++：异常处理
来源：http://yw.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ow.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://tt.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hk.newstarts.cn

[S56] C++：optional
来源：http://gk.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cc.szsharing.cn

[S57] C++：编译期常量
来源：http://xc.jianghongdianzi.cn

constexpr int N = 10;
来源：http://gp.szsharing.cn

[S58] C++：命名空间
来源：http://qi.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://ag.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://vo.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lo.colortex.cn

[S60] C++：遍历并删除元素
来源：http://dn.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bp.hahajie.cn

================================================================================
来源：http://vi.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eo.jctech888.com.cn

================================================================================
来源：http://dh.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://ss.9csxet.cn

println("Hello")
来源：http://rp.521024.cn

[T02] Kotlin：变量
来源：http://co.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aq.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://nx.asd995.cn

"值: $b"
来源：http://mg.nszjky.cn

[T04] Kotlin：空安全
来源：http://iu.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://tt.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://ah.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lc.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://xg.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yn.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://nk.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tm.lnxyls.cn

[T08] Kotlin：数据类
来源：http://fu.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://oj.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://xg.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://il.nszjky.cn

[T10] Kotlin：默认参数
来源：http://ab.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qo.chemitech.net.cn

[T11] Kotlin：协程
来源：http://de.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ec.521024.cn

[T12] Kotlin：解构声明
来源：http://iv.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://gy.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://ez.szsharing.cn

val m = mapOf("a" to 1)
来源：http://an.colortex.cn

[T14] Kotlin：循环
来源：http://gk.gzmigu.cn

for (i in 1..10) println(i)
来源：http://qr.shtwfgs.cn

[T15] Kotlin：接口
来源：http://rm.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ae.shxzskj.cn

[T16] Swift：Hello World
来源：http://rg.haigaiapp.cn

print("Hello")
来源：http://rl.hahajie.cn

[T17] Swift：变量与常量
来源：http://gx.huixiangedu.cn

var a = 1;  let b = 2
来源：http://cd.nszjky.cn

[T18] Swift：字符串插值
来源：http://hc.shxzskj.cn

"值: \(b)"
来源：http://to.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://si.nicolike.cn

if let n = opt { print(n) }
来源：http://td.szxytkj.cn

[T20] Swift：数组操作
来源：http://pl.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nr.9csxet.cn

[T21] Swift：遍历
来源：http://dk.newstarts.cn

for x in a { print(x) }
来源：http://ae.521024.cn

[T22] Swift：字典
来源：http://pe.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jn.huixinmuqiang.cn

[T23] Swift：函数
来源：http://ol.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lj.shtwfgs.cn

[T24] Swift：闭包
来源：http://zc.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wc.shxzskj.cn

[T25] Swift：结构体
来源：http://ge.chemitech.net.cn

struct P { var x: Int }
来源：http://cw.shxzukj.cn

[T26] Swift：类与重写
来源：http://ev.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ei.shtwfgs.cn

[T27] Swift：错误处理
来源：http://vj.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://pt.szsharing.cn

[T28] Swift：枚举
来源：http://qf.shxzskj.cn

enum Color { case red, green }
来源：http://xj.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://bu.muxihuayi.cn

guard let x = opt else { return }
来源：http://fi.huixinmuqiang.cn

[T30] Swift：协议
来源：http://cr.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://vk.panjiajie.cn

[T31] Lua：Hello World
来源：http://cr.nszjky.cn

print("Hello")
来源：http://ys.asd995.cn

[T32] Lua：局部变量
来源：http://lp.hnjuh.cn

local a = 1
来源：http://rx.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://mb.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ni.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ao.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eb.lnxyls.cn

[T35] Lua：字典表
来源：http://ys.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://cp.haigaiapp.cn

[T36] Lua：函数
来源：http://jc.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://kd.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://hr.9csxet.cn

"a" .. "b"
来源：http://vi.szsharing.cn

[T38] Lua：条件
来源：http://bk.jctech888.com.cn

if x > 0 then print("正") end
来源：http://sy.shxzukj.cn

[T39] Lua：模式匹配
来源：http://qs.yuexingan06.cn

string.find(s, "%d+")
来源：http://at.521024.cn

[T40] Lua：元表
来源：http://nj.9csxet.cn

setmetatable({}, { __index = base })
来源：http://jk.panjiajie.cn

[T41] Perl：Hello World
来源：http://xs.nszjky.cn

print "Hello\n";
来源：http://id.haigaiapp.cn

[T42] Perl：变量类型
来源：http://pc.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rg.lnxyls.cn

[T43] Perl：字符串插值
来源：http://av.nszjky.cn

"值: $a"
来源：http://fn.muxihuayi.cn

[T44] Perl：条件
来源：http://de.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://xo.asd995.cn

[T45] Perl：数组遍历
来源：http://pr.asd995.cn

for my $x (@arr) { print $x; }
来源：http://gb.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://bf.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ca.newstarts.cn

[T47] Perl：正则捕获
来源：http://vc.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vh.huanxung.cn

[T48] Perl：正则替换
来源：http://tv.521024.cn

$s =~ s/old/new/g;
来源：http://ry.yuexingan06.cn

[T49] Perl：函数
来源：http://xu.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ns.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://ze.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yt.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://xo.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://lc.jctech888.com.cn

println("Hello")
来源：http://xg.asd995.cn

[T52] Scala：变量
来源：http://wc.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://jo.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://ga.huixiangedu.cn

s"值: $b"
来源：http://ax.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://qk.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://mv.newstarts.cn

[T55] Scala：集合过滤
来源：http://yu.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ej.huixiangedu.cn

[T56] Scala：样例类
来源：http://jq.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://bs.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://cw.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://re.jctech888.com.cn

[T58] Scala：函数定义
来源：http://ic.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hp.jianghongdianzi.cn

[T59] Scala：循环
来源：http://rt.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://lr.colortex.cn

[T60] Scala：折叠
来源：http://be.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pv.muxihuayi.cn

================================================================================
来源：http://sq.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jc.gzmigu.cn

================================================================================
来源：http://cx.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ku.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vh.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://xv.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rb.asd995.cn

[U03] Py：加载 .env 配置
来源：http://dq.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tv.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://sm.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://or.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://uu.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://jj.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://np.lnxyls.cn

{**a, **b}
来源：http://dj.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://pr.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://pb.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://tj.szxytkj.cn

[y for x in nested for y in x]
来源：http://xj.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://ll.nszjky.cn

max(d, key=d.get)
来源：http://rf.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://dc.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fv.nicolike.cn

[U11] Py：生成器表达式
来源：http://mn.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://pn.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gh.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://pj.szsharing.cn

[U13] Py：固定长度队列
来源：http://oe.lnxyls.cn

deque(maxlen=10)
来源：http://xk.asd995.cn

[U14] Py：分组收集到列表
来源：http://wi.szxytkj.cn

defaultdict(list)
来源：http://tm.shxzskj.cn

[U15] Py：高精度计时
来源：http://xk.nicolike.cn

t = time.perf_counter()
来源：http://ek.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://ze.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xu.lnxyls.cn

[U17] Py：初始化日志
来源：http://ib.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://xs.colortex.cn

[U18] Py：预编译正则
来源：http://ib.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://wx.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://qw.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gp.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ub.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://ez.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://xh.jctech888.com.cn

@contextlib.contextmanager
来源：http://vq.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://mx.gzmigu.cn

list(zip(*m))
来源：http://va.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://fj.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bb.szxytkj.cn

[U24] Py：路径操作
来源：http://sy.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wi.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://jf.szsharing.cn

csv.DictReader(f)
来源：http://fn.chemitech.net.cn

[U26] Py：并发下载
来源：http://po.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hi.szsharing.cn

[U27] Py：异步 HTTP
来源：http://dk.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://vj.haigaiapp.cn

[U28] Py：类型别名
来源：http://mv.yuexingan06.cn

UserId = int
来源：http://ky.wgjwhj.cn

[U29] Py：属性校验
来源：http://hm.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://za.colortex.cn

[U30] Py：数据类
来源：http://we.hnjuh.cn

@dataclass(slots=True)
来源：http://ow.521024.cn

[U31] Py：单测
来源：http://ml.shtwfgs.cn

python -m pytest -q
来源：http://db.newstarts.cn

[U32] Py：代码格式化
来源：http://yc.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://wf.szsharing.cn

[U33] Py：打包发布
来源：http://oz.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ui.shtwfgs.cn

[U34] Py：判断编码
来源：http://om.newstarts.cn

chardet.detect(raw)
来源：http://og.szxytkj.cn

[U35] Py：发送邮件
来源：http://nz.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xh.wgjwhj.cn

[U36] Py：定时任务
来源：http://bl.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://ha.panjiajie.cn

[U37] Py：读写 Excel
来源：http://vl.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zh.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://ev.szsharing.cn

Path(__file__).resolve().parent
来源：http://dg.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://fc.huanxung.cn

sys.stdout.isatty()
来源：http://nr.521024.cn

[U40] Py：打印到标准错误
来源：http://wz.asd995.cn

print("err", file=sys.stderr)
来源：http://pc.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://xb.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gs.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://ke.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://on.nicolike.cn

[U43] PHP：声明命名空间
来源：http://fk.colortex.cn

namespace App\Http;
来源：http://ox.szsharing.cn

[U44] PHP：开启严格类型
来源：http://zl.yuexingan06.cn

declare(strict_types=1);
来源：http://mf.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://ax.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ni.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://as.panjiajie.cn

?string $name = null
来源：http://fr.lnxyls.cn

[U47] PHP：联合类型
来源：http://eu.521024.cn

int|string $id
来源：http://wm.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://qa.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lw.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://tg.yuntaijiaju.cn

public readonly string $name
来源：http://bl.asd995.cn

[U50] PHP：构造器属性提升
来源：http://bt.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://if.shxzukj.cn

[U51] PHP：数组解构
来源：http://uu.9csxet.cn

[$a, $b] = $arr;
来源：http://ya.gzmigu.cn

[U52] PHP：箭头函数
来源：http://vs.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://pe.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://zu.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://bj.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://nb.haigaiapp.cn

$obj?->method()
来源：http://lr.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://yi.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rl.nicolike.cn

[U56] PHP：命名参数
来源：http://ww.huanxung.cn

f(a: 1, b: 2)
来源：http://rv.9csxet.cn

[U57] PHP：字符串插值
来源：http://kf.shxzukj.cn

"值: {$a}"
来源：http://la.shxzskj.cn

[U58] PHP：数组三件套
来源：http://df.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://os.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://gj.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lj.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://oz.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ov.huixinmuqiang.cn

[U61] PHP：正则
来源：http://ie.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ct.gzmigu.cn

[U62] PHP：日期对象
来源：http://kh.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gp.521024.cn


<!-- 参考信息 -->