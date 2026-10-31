代发 wailian999

[S41] C++：类与构造函数
来源：http://gz.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xe.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://zb.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://vg.colortex.cn

[S43] C++：智能指针
来源：http://fo.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://jm.szxytkj.cn

[S44] C++：引用传参
来源：http://nt.hahajie.cn

void inc(int &x) { ++x; }
来源：http://wc.521024.cn

[S45] C++：lambda
来源：http://oa.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ca.hnjuh.cn

[S46] C++：函数模板
来源：http://ga.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jx.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://wp.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jy.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://he.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bf.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://rc.jctech888.com.cn

[S49] C++：写文件
来源：http://jl.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zp.jctech888.com.cn

[S50] C++：格式化数字
来源：http://vy.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hg.shxzukj.cn

[S51] C++：显式类型转换
来源：http://uj.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://fu.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://fk.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://lc.wgjwhj.cn

[S53] C++：移动语义
来源：http://sn.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://lc.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://vc.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bz.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://tz.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eb.yuexingan06.cn

[S56] C++：optional
来源：http://ty.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vr.colortex.cn

[S57] C++：编译期常量
来源：http://bp.nicolike.cn

constexpr int N = 10;
来源：http://or.hahajie.cn

[S58] C++：命名空间
来源：http://tl.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://so.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://cr.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://al.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://iz.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gt.521024.cn

================================================================================
来源：http://hq.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fu.szsharing.cn

================================================================================
来源：http://xg.nicolike.cn

[T01] Kotlin：Hello World
来源：http://ey.huixiangedu.cn

println("Hello")
来源：http://jl.bjjhwx.cn

[T02] Kotlin：变量
来源：http://jm.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dx.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://dt.huanxung.cn

"值: $b"
来源：http://jb.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://nn.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://ew.asd995.cn

[T05] Kotlin：when 表达式
来源：http://hm.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ut.huanxung.cn

[T06] Kotlin：集合映射
来源：http://xp.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://af.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://lp.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ro.lnxyls.cn

[T08] Kotlin：数据类
来源：http://gh.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://pz.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://uu.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://qz.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://rk.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ju.shxzukj.cn

[T11] Kotlin：协程
来源：http://zt.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nz.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://ct.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://pp.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://us.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://cf.hahajie.cn

[T14] Kotlin：循环
来源：http://oq.hahajie.cn

for (i in 1..10) println(i)
来源：http://wv.yuexingan06.cn

[T15] Kotlin：接口
来源：http://dg.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://pw.shxzskj.cn

[T16] Swift：Hello World
来源：http://zt.521024.cn

print("Hello")
来源：http://zu.521024.cn

[T17] Swift：变量与常量
来源：http://va.hnjuh.cn

var a = 1;  let b = 2
来源：http://jy.colortex.cn

[T18] Swift：字符串插值
来源：http://ou.huixinmuqiang.cn

"值: \(b)"
来源：http://vm.colortex.cn

[T19] Swift：可选绑定
来源：http://ck.huixiangedu.cn

if let n = opt { print(n) }
来源：http://kd.hnjuh.cn

[T20] Swift：数组操作
来源：http://gh.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vu.wgjwhj.cn

[T21] Swift：遍历
来源：http://hg.shxzskj.cn

for x in a { print(x) }
来源：http://hl.shxzskj.cn

[T22] Swift：字典
来源：http://ox.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cq.yuexingan06.cn

[T23] Swift：函数
来源：http://uo.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lf.shxzukj.cn

[T24] Swift：闭包
来源：http://wj.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fh.nicolike.cn

[T25] Swift：结构体
来源：http://tl.shtwfgs.cn

struct P { var x: Int }
来源：http://sc.szsharing.cn

[T26] Swift：类与重写
来源：http://hf.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://wh.yuexingan06.cn

[T27] Swift：错误处理
来源：http://sf.521024.cn

do { try f() } catch { print(error) }
来源：http://lk.wgjwhj.cn

[T28] Swift：枚举
来源：http://nw.hnjuh.cn

enum Color { case red, green }
来源：http://ea.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://ak.wgjwhj.cn

guard let x = opt else { return }
来源：http://um.gzmigu.cn

[T30] Swift：协议
来源：http://fw.521024.cn

protocol Shape { func area() -> Double }
来源：http://pr.521024.cn

[T31] Lua：Hello World
来源：http://zx.521024.cn

print("Hello")
来源：http://is.huixiangedu.cn

[T32] Lua：局部变量
来源：http://nf.shtwfgs.cn

local a = 1
来源：http://bl.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://af.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://er.hnjuh.cn

[T34] Lua：遍历表
来源：http://rz.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cm.521024.cn

[T35] Lua：字典表
来源：http://nj.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://aw.hahajie.cn

[T36] Lua：函数
来源：http://ad.hahajie.cn

function add(a, b) return a + b end
来源：http://nq.huanxung.cn

[T37] Lua：字符串拼接
来源：http://xi.szsharing.cn

"a" .. "b"
来源：http://ib.yuntaijiaju.cn

[T38] Lua：条件
来源：http://zu.yuexingan06.cn

if x > 0 then print("正") end
来源：http://yp.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://jb.hahajie.cn

string.find(s, "%d+")
来源：http://br.haigaiapp.cn

[T40] Lua：元表
来源：http://tm.szsharing.cn

setmetatable({}, { __index = base })
来源：http://yx.muxihuayi.cn

[T41] Perl：Hello World
来源：http://lb.huixinmuqiang.cn

print "Hello\n";
来源：http://pp.shxzukj.cn

[T42] Perl：变量类型
来源：http://rc.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bv.9csxet.cn

[T43] Perl：字符串插值
来源：http://xs.newstarts.cn

"值: $a"
来源：http://wg.szsharing.cn

[T44] Perl：条件
来源：http://jq.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://nc.huanxung.cn

[T45] Perl：数组遍历
来源：http://me.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://md.lnxyls.cn

[T46] Perl：哈希操作
来源：http://vy.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ta.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://fx.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mj.huanxung.cn

[T48] Perl：正则替换
来源：http://ws.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://lv.wgjwhj.cn

[T49] Perl：函数
来源：http://dm.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tn.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://md.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ps.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://yo.haigaiapp.cn

[T51] Scala：Hello World
来源：http://rl.bjjhwx.cn

println("Hello")
来源：http://ma.huanxung.cn

[T52] Scala：变量
来源：http://ua.shxzukj.cn

val a = 1;  var b = 2
来源：http://tv.colortex.cn

[T53] Scala：字符串插值
来源：http://ia.bookmarksfly.cn

s"值: $b"
来源：http://sh.yuexingan06.cn

[T54] Scala：集合映射
来源：http://rp.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://ie.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://cw.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ds.huanxung.cn

[T56] Scala：样例类
来源：http://sd.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://kf.szxytkj.cn

[T57] Scala：模式匹配
来源：http://yq.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eg.yuexingan06.cn

[T58] Scala：函数定义
来源：http://fi.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tk.asd995.cn

[T59] Scala：循环
来源：http://sx.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://av.yuexingan06.cn

[T60] Scala：折叠
来源：http://zk.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gp.haigaiapp.cn

================================================================================
来源：http://yw.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sb.9csxet.cn

================================================================================
来源：http://pe.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://dr.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bm.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://pk.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pv.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://bj.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ff.shxzukj.cn

[U04] Py：变量调试打印
来源：http://jl.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://za.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://rz.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://co.asd995.cn

[U06] Py：合并两个字典
来源：http://td.shxzskj.cn

{**a, **b}
来源：http://im.gzmigu.cn

[U07] Py：反转字典键值
来源：http://hz.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://lv.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://cp.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://sg.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://dj.wgjwhj.cn

max(d, key=d.get)
来源：http://ll.shxzukj.cn

[U10] Py：按值排序字典
来源：http://vg.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dq.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://yg.nicolike.cn

(x * 2 for x in arr)
来源：http://oo.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tw.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://fk.gzmigu.cn

[U13] Py：固定长度队列
来源：http://gv.huixinmuqiang.cn

deque(maxlen=10)
来源：http://bs.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://tg.wgjwhj.cn

defaultdict(list)
来源：http://cs.nicolike.cn

[U15] Py：高精度计时
来源：http://ms.asd995.cn

t = time.perf_counter()
来源：http://fy.521024.cn

[U16] Py：命令行参数解析
来源：http://sf.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gp.jctech888.com.cn

[U17] Py：初始化日志
来源：http://ed.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ce.newstarts.cn

[U18] Py：预编译正则
来源：http://zn.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://ji.szsharing.cn

[U19] Py：正则替换带回调
来源：http://ch.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cb.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://iz.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://hw.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ui.nszjky.cn

@contextlib.contextmanager
来源：http://ad.521024.cn

[U22] Py：矩阵转置
来源：http://vc.yuntaijiaju.cn

list(zip(*m))
来源：http://uk.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://pq.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://it.chemitech.net.cn

[U24] Py：路径操作
来源：http://ke.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fk.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ul.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ib.shxzukj.cn

[U26] Py：并发下载
来源：http://rn.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kz.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://wk.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://ny.shxzukj.cn

[U28] Py：类型别名
来源：http://yb.chemitech.net.cn

UserId = int
来源：http://iw.colortex.cn

[U29] Py：属性校验
来源：http://xa.shxzskj.cn

@property 与 @x.setter 配合
来源：http://te.521024.cn

[U30] Py：数据类
来源：http://so.muxihuayi.cn

@dataclass(slots=True)
来源：http://yj.gzmigu.cn

[U31] Py：单测
来源：http://at.nicolike.cn

python -m pytest -q
来源：http://ef.gzmigu.cn

[U32] Py：代码格式化
来源：http://ej.szsharing.cn

ruff format . && ruff check --fix .
来源：http://bg.huixiangedu.cn

[U33] Py：打包发布
来源：http://ev.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://lu.shtwfgs.cn

[U34] Py：判断编码
来源：http://va.yuexingan06.cn

chardet.detect(raw)
来源：http://rr.chemitech.net.cn

[U35] Py：发送邮件
来源：http://sq.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yq.newstarts.cn

[U36] Py：定时任务
来源：http://fk.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://kb.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://fn.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vu.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://gq.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://ru.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://rn.9csxet.cn

sys.stdout.isatty()
来源：http://cl.huanxung.cn

[U40] Py：打印到标准错误
来源：http://yo.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://zw.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://cb.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xh.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://bo.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uu.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://el.521024.cn

namespace App\Http;
来源：http://jr.huanxung.cn

[U44] PHP：开启严格类型
来源：http://so.hahajie.cn

declare(strict_types=1);
来源：http://gg.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://rt.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tp.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://cl.szsharing.cn

?string $name = null
来源：http://fm.asd995.cn

[U47] PHP：联合类型
来源：http://hk.shxzukj.cn

int|string $id
来源：http://jv.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://an.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tl.hnjuh.cn

[U49] PHP：只读属性
来源：http://km.9csxet.cn

public readonly string $name
来源：http://ey.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://bf.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://vk.jctech888.com.cn

[U51] PHP：数组解构
来源：http://qx.nicolike.cn

[$a, $b] = $arr;
来源：http://wg.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://fj.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://pv.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://wg.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://mi.newstarts.cn

[U54] PHP：空安全调用
来源：http://lb.huanxung.cn

$obj?->method()
来源：http://rc.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://lo.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dm.gzmigu.cn

[U56] PHP：命名参数
来源：http://ur.9csxet.cn

f(a: 1, b: 2)
来源：http://le.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://li.shtwfgs.cn

"值: {$a}"
来源：http://xi.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ge.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rn.szxytkj.cn

[U59] PHP：自定义排序
来源：http://uq.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wf.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://ob.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oh.panjiajie.cn

[U61] PHP：正则
来源：http://yq.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tx.chemitech.net.cn

[U62] PHP：日期对象
来源：http://ka.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ar.lnxyls.cn

[U63] PHP：文件读写
来源：http://xo.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gd.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://co.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://qp.9csxet.cn

[U65] PHP：会话
来源：http://db.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oj.colortex.cn

[U66] PHP：设置 Cookie
来源：http://lt.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bh.yuexingan06.cn


<!-- 参考信息 -->