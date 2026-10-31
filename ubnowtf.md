代发 wailian999

[S41] C++：类与构造函数
来源：http://vk.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xg.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://nx.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://em.shxzskj.cn

[S43] C++：智能指针
来源：http://xu.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://rj.hnjuh.cn

[S44] C++：引用传参
来源：http://aq.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://gf.hnjuh.cn

[S45] C++：lambda
来源：http://kk.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vb.szxytkj.cn

[S46] C++：函数模板
来源：http://il.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qq.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://el.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ta.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://fl.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dx.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://fi.szxytkj.cn

[S49] C++：写文件
来源：http://dd.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cz.yuexingan06.cn

[S50] C++：格式化数字
来源：http://av.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oe.lnxyls.cn

[S51] C++：显式类型转换
来源：http://ji.521024.cn

static_cast<double>(a) / b
来源：http://db.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://mv.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://xq.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://ow.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://wb.newstarts.cn

[S54] C++：异常处理
来源：http://fn.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ap.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://gs.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ky.wgjwhj.cn

[S56] C++：optional
来源：http://nb.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fh.9csxet.cn

[S57] C++：编译期常量
来源：http://wu.yuexingan06.cn

constexpr int N = 10;
来源：http://wr.bookmarksfly.cn

[S58] C++：命名空间
来源：http://iw.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://ua.nszjky.cn

[S59] C++：静态断言
来源：http://tl.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gw.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://yr.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://se.newstarts.cn

================================================================================
来源：http://ix.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sf.jctech888.com.cn

================================================================================
来源：http://wc.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://fu.yuntaijiaju.cn

println("Hello")
来源：http://en.haigaiapp.cn

[T02] Kotlin：变量
来源：http://lf.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fj.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://nt.jianghongdianzi.cn

"值: $b"
来源：http://he.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://op.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ue.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://gj.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rf.newstarts.cn

[T06] Kotlin：集合映射
来源：http://aj.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fq.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://uh.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bx.huanxung.cn

[T08] Kotlin：数据类
来源：http://de.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://nd.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://so.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://bz.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://vw.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xk.huanxung.cn

[T11] Kotlin：协程
来源：http://ab.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xg.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://dy.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://ty.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://ok.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://lg.bjjhwx.cn

[T14] Kotlin：循环
来源：http://cm.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://ni.hahajie.cn

[T15] Kotlin：接口
来源：http://ml.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://kl.jctech888.com.cn

[T16] Swift：Hello World
来源：http://qt.huixiangedu.cn

print("Hello")
来源：http://bk.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://ka.lnxyls.cn

var a = 1;  let b = 2
来源：http://dg.shxzskj.cn

[T18] Swift：字符串插值
来源：http://ng.wgjwhj.cn

"值: \(b)"
来源：http://dw.lnxyls.cn

[T19] Swift：可选绑定
来源：http://oz.newstarts.cn

if let n = opt { print(n) }
来源：http://ul.huanxung.cn

[T20] Swift：数组操作
来源：http://vc.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://od.asd995.cn

[T21] Swift：遍历
来源：http://gq.shxzskj.cn

for x in a { print(x) }
来源：http://hs.bjjhwx.cn

[T22] Swift：字典
来源：http://dp.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vk.hnjuh.cn

[T23] Swift：函数
来源：http://rr.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ev.nicolike.cn

[T24] Swift：闭包
来源：http://ey.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ex.bjjhwx.cn

[T25] Swift：结构体
来源：http://bn.szxytkj.cn

struct P { var x: Int }
来源：http://xs.wgjwhj.cn

[T26] Swift：类与重写
来源：http://qj.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://gi.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://la.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://xp.521024.cn

[T28] Swift：枚举
来源：http://aq.9csxet.cn

enum Color { case red, green }
来源：http://ft.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://my.lnxyls.cn

guard let x = opt else { return }
来源：http://uj.huanxung.cn

[T30] Swift：协议
来源：http://zn.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://qd.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ah.hnjuh.cn

print("Hello")
来源：http://kg.shxzukj.cn

[T32] Lua：局部变量
来源：http://ho.huixiangedu.cn

local a = 1
来源：http://hj.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://he.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lp.colortex.cn

[T34] Lua：遍历表
来源：http://ph.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://an.haigaiapp.cn

[T35] Lua：字典表
来源：http://tk.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://qg.yuexingan06.cn

[T36] Lua：函数
来源：http://ke.521024.cn

function add(a, b) return a + b end
来源：http://kz.521024.cn

[T37] Lua：字符串拼接
来源：http://xs.newstarts.cn

"a" .. "b"
来源：http://fs.newstarts.cn

[T38] Lua：条件
来源：http://mk.hnjuh.cn

if x > 0 then print("正") end
来源：http://gd.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://gf.9csxet.cn

string.find(s, "%d+")
来源：http://sv.jianghongdianzi.cn

[T40] Lua：元表
来源：http://nu.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://pw.huanxung.cn

[T41] Perl：Hello World
来源：http://dj.shxzskj.cn

print "Hello\n";
来源：http://au.shxzukj.cn

[T42] Perl：变量类型
来源：http://wp.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oz.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://lp.yuexingan06.cn

"值: $a"
来源：http://ao.gzmigu.cn

[T44] Perl：条件
来源：http://kb.521024.cn

if ($a > 0) { print "正"; }
来源：http://jp.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://ia.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://us.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://je.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ac.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ey.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vt.hahajie.cn

[T48] Perl：正则替换
来源：http://qr.szxytkj.cn

$s =~ s/old/new/g;
来源：http://wo.huixiangedu.cn

[T49] Perl：函数
来源：http://yi.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hx.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://bj.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gf.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://nt.nszjky.cn

[T51] Scala：Hello World
来源：http://kc.chemitech.net.cn

println("Hello")
来源：http://mj.yuexingan06.cn

[T52] Scala：变量
来源：http://ob.huixiangedu.cn

val a = 1;  var b = 2
来源：http://lf.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://oi.nicolike.cn

s"值: $b"
来源：http://xa.huixiangedu.cn

[T54] Scala：集合映射
来源：http://fr.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://sp.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://nq.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vr.nicolike.cn

[T56] Scala：样例类
来源：http://xh.shxzukj.cn

case class User(name: String, age: Int)
来源：http://gb.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://wh.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gk.hnjuh.cn

[T58] Scala：函数定义
来源：http://zd.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ti.shtwfgs.cn

[T59] Scala：循环
来源：http://pg.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://mk.huixiangedu.cn

[T60] Scala：折叠
来源：http://gh.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ha.huixinmuqiang.cn

================================================================================
来源：http://iw.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bs.huixinmuqiang.cn

================================================================================
来源：http://ji.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ht.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nl.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://fn.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zv.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://kv.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tq.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://qr.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fb.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://gd.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://zu.gzmigu.cn

[U06] Py：合并两个字典
来源：http://yz.hahajie.cn

{**a, **b}
来源：http://zf.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://rm.szsharing.cn

{v: k for k, v in d.items()}
来源：http://la.szxytkj.cn

[U08] Py：展平二维列表
来源：http://dy.nicolike.cn

[y for x in nested for y in x]
来源：http://wg.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://pv.shxzskj.cn

max(d, key=d.get)
来源：http://ir.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://jq.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wy.nszjky.cn

[U11] Py：生成器表达式
来源：http://so.lnxyls.cn

(x * 2 for x in arr)
来源：http://dy.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mr.gzmigu.cn

Counter(arr).most_common(3)
来源：http://qf.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://ff.521024.cn

deque(maxlen=10)
来源：http://pp.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://cy.szxytkj.cn

defaultdict(list)
来源：http://xk.haigaiapp.cn

[U15] Py：高精度计时
来源：http://wf.hnjuh.cn

t = time.perf_counter()
来源：http://hg.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://gm.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gh.bjjhwx.cn

[U17] Py：初始化日志
来源：http://go.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://gc.szsharing.cn

[U18] Py：预编译正则
来源：http://zo.huanxung.cn

pat = re.compile(r"\d+")
来源：http://mk.newstarts.cn

[U19] Py：正则替换带回调
来源：http://dy.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cx.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://ef.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://xk.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ux.szxytkj.cn

@contextlib.contextmanager
来源：http://rv.521024.cn

[U22] Py：矩阵转置
来源：http://gd.9csxet.cn

list(zip(*m))
来源：http://lt.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://bp.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ni.shxzukj.cn

[U24] Py：路径操作
来源：http://gu.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zn.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://uu.jianghongdianzi.cn

csv.DictReader(f)
来源：http://bc.wgjwhj.cn

[U26] Py：并发下载
来源：http://ru.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dg.newstarts.cn

[U27] Py：异步 HTTP
来源：http://wr.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://oa.bookmarksfly.cn

[U28] Py：类型别名
来源：http://cr.9csxet.cn

UserId = int
来源：http://xp.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://ya.nszjky.cn

@property 与 @x.setter 配合
来源：http://wm.wgjwhj.cn

[U30] Py：数据类
来源：http://sl.lnxyls.cn

@dataclass(slots=True)
来源：http://mx.hahajie.cn

[U31] Py：单测
来源：http://bl.haigaiapp.cn

python -m pytest -q
来源：http://ok.chemitech.net.cn

[U32] Py：代码格式化
来源：http://qy.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://ho.lnxyls.cn

[U33] Py：打包发布
来源：http://mp.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://oz.nicolike.cn

[U34] Py：判断编码
来源：http://vx.nszjky.cn

chardet.detect(raw)
来源：http://pq.shxzskj.cn

[U35] Py：发送邮件
来源：http://wr.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qc.szxytkj.cn

[U36] Py：定时任务
来源：http://yo.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://tv.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://tv.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ml.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://kf.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://ca.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://gd.szxytkj.cn

sys.stdout.isatty()
来源：http://ju.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ke.szxytkj.cn

print("err", file=sys.stderr)
来源：http://fh.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://bd.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sk.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://nd.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tg.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://vk.hnjuh.cn

namespace App\Http;
来源：http://ae.521024.cn

[U44] PHP：开启严格类型
来源：http://yt.newstarts.cn

declare(strict_types=1);
来源：http://ay.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://cv.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fb.panjiajie.cn

[U46] PHP：可空类型
来源：http://ny.colortex.cn

?string $name = null
来源：http://yl.shtwfgs.cn

[U47] PHP：联合类型
来源：http://si.huixiangedu.cn

int|string $id
来源：http://sk.shxzskj.cn

[U48] PHP：纯枚举
来源：http://dj.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hb.chemitech.net.cn

[U49] PHP：只读属性
来源：http://ma.shxzukj.cn

public readonly string $name
来源：http://ng.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://yy.hnjuh.cn

public function __construct(private int $id) {}
来源：http://gt.asd995.cn

[U51] PHP：数组解构
来源：http://fi.szxytkj.cn

[$a, $b] = $arr;
来源：http://hd.gzmigu.cn

[U52] PHP：箭头函数
来源：http://kq.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://pu.colortex.cn

[U53] PHP：空合并运算符
来源：http://wm.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://ms.colortex.cn

[U54] PHP：空安全调用
来源：http://cz.haigaiapp.cn

$obj?->method()
来源：http://jb.hahajie.cn

[U55] PHP：match 表达式
来源：http://tz.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gn.521024.cn

[U56] PHP：命名参数
来源：http://wc.yuexingan06.cn

f(a: 1, b: 2)
来源：http://zy.panjiajie.cn

[U57] PHP：字符串插值
来源：http://vl.bookmarksfly.cn

"值: {$a}"
来源：http://hk.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://vb.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vy.nicolike.cn

[U59] PHP：自定义排序
来源：http://az.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://km.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://qg.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ef.asd995.cn

[U61] PHP：正则
来源：http://xp.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lp.colortex.cn

[U62] PHP：日期对象
来源：http://nc.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rq.szxytkj.cn

[U63] PHP：文件读写
来源：http://rv.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cy.szxytkj.cn

[U64] PHP：目录遍历
来源：http://ck.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://sm.huanxung.cn

[U65] PHP：会话
来源：http://uw.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ql.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://rv.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xx.muxihuayi.cn


<!-- 参考信息 -->