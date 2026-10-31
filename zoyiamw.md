代发 wailian999

[S41] C++：类与构造函数
来源：http://ah.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rj.newstarts.cn

[S42] C++：继承与虚函数
来源：http://pw.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://sl.muxihuayi.cn

[S43] C++：智能指针
来源：http://ch.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://hz.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://mr.huanxung.cn

void inc(int &x) { ++x; }
来源：http://bk.hahajie.cn

[S45] C++：lambda
来源：http://eg.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iz.nicolike.cn

[S46] C++：函数模板
来源：http://xu.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zv.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://wr.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ou.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://cz.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dy.9csxet.cn

while (std::getline(in, line)) { }
来源：http://pf.huanxung.cn

[S49] C++：写文件
来源：http://wu.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://he.shtwfgs.cn

[S50] C++：格式化数字
来源：http://jx.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://it.shxzukj.cn

[S51] C++：显式类型转换
来源：http://xa.muxihuayi.cn

static_cast<double>(a) / b
来源：http://wy.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ly.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://ub.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://iu.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://xz.asd995.cn

[S54] C++：异常处理
来源：http://hg.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zs.asd995.cn

[S55] C++：结构化绑定
来源：http://dt.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ew.newstarts.cn

[S56] C++：optional
来源：http://di.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vh.panjiajie.cn

[S57] C++：编译期常量
来源：http://eb.gzmigu.cn

constexpr int N = 10;
来源：http://ei.haigaiapp.cn

[S58] C++：命名空间
来源：http://ij.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://kp.nicolike.cn

[S59] C++：静态断言
来源：http://xd.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mj.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://tu.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lh.bjjhwx.cn

================================================================================
来源：http://cz.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://co.haigaiapp.cn

================================================================================
来源：http://ga.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ga.huixiangedu.cn

println("Hello")
来源：http://pg.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ya.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ia.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://ie.huixinmuqiang.cn

"值: $b"
来源：http://ik.shxzukj.cn

[T04] Kotlin：空安全
来源：http://gv.shxzskj.cn

val n: String? = null;  n?.length
来源：http://sb.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://uo.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lz.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://sx.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oa.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ac.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nx.asd995.cn

[T08] Kotlin：数据类
来源：http://dc.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://dd.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://eb.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://sg.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://kg.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hr.shxzskj.cn

[T11] Kotlin：协程
来源：http://xp.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ov.newstarts.cn

[T12] Kotlin：解构声明
来源：http://gc.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://nc.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://uj.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://vo.gzmigu.cn

[T14] Kotlin：循环
来源：http://az.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://rt.shxzukj.cn

[T15] Kotlin：接口
来源：http://tq.colortex.cn

interface Shape { fun area(): Double }
来源：http://rs.nszjky.cn

[T16] Swift：Hello World
来源：http://qh.colortex.cn

print("Hello")
来源：http://uy.shxzukj.cn

[T17] Swift：变量与常量
来源：http://gc.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://da.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://fw.jctech888.com.cn

"值: \(b)"
来源：http://oa.nicolike.cn

[T19] Swift：可选绑定
来源：http://sy.panjiajie.cn

if let n = opt { print(n) }
来源：http://kh.jctech888.com.cn

[T20] Swift：数组操作
来源：http://bq.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jg.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://kc.hnjuh.cn

for x in a { print(x) }
来源：http://rb.bookmarksfly.cn

[T22] Swift：字典
来源：http://ir.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oo.newstarts.cn

[T23] Swift：函数
来源：http://jp.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kw.shxzskj.cn

[T24] Swift：闭包
来源：http://eb.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jd.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://se.bjjhwx.cn

struct P { var x: Int }
来源：http://jt.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://zh.nszjky.cn

class A: Base { override func f() {} }
来源：http://ep.bjjhwx.cn

[T27] Swift：错误处理
来源：http://sf.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://iy.hahajie.cn

[T28] Swift：枚举
来源：http://ha.szsharing.cn

enum Color { case red, green }
来源：http://eh.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://sx.haigaiapp.cn

guard let x = opt else { return }
来源：http://in.szsharing.cn

[T30] Swift：协议
来源：http://rb.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://vc.muxihuayi.cn

[T31] Lua：Hello World
来源：http://dt.szxytkj.cn

print("Hello")
来源：http://hv.lnxyls.cn

[T32] Lua：局部变量
来源：http://gd.huanxung.cn

local a = 1
来源：http://je.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ti.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oo.szsharing.cn

[T34] Lua：遍历表
来源：http://oe.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dh.nszjky.cn

[T35] Lua：字典表
来源：http://fi.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://bb.wgjwhj.cn

[T36] Lua：函数
来源：http://ev.szsharing.cn

function add(a, b) return a + b end
来源：http://xz.newstarts.cn

[T37] Lua：字符串拼接
来源：http://by.hnjuh.cn

"a" .. "b"
来源：http://hj.9csxet.cn

[T38] Lua：条件
来源：http://sj.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://hl.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://xl.huixiangedu.cn

string.find(s, "%d+")
来源：http://sb.shxzukj.cn

[T40] Lua：元表
来源：http://ap.newstarts.cn

setmetatable({}, { __index = base })
来源：http://eu.asd995.cn

[T41] Perl：Hello World
来源：http://lp.huixiangedu.cn

print "Hello\n";
来源：http://ib.hnjuh.cn

[T42] Perl：变量类型
来源：http://yq.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kq.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://zo.newstarts.cn

"值: $a"
来源：http://qb.hnjuh.cn

[T44] Perl：条件
来源：http://lg.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://is.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://mr.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://zf.szsharing.cn

[T46] Perl：哈希操作
来源：http://bi.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tg.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://gf.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xl.nicolike.cn

[T48] Perl：正则替换
来源：http://mp.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ln.shxzskj.cn

[T49] Perl：函数
来源：http://qb.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nx.hahajie.cn

[T50] Perl：逐行读文件
来源：http://qr.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bl.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://zv.colortex.cn

[T51] Scala：Hello World
来源：http://ln.lnxyls.cn

println("Hello")
来源：http://em.colortex.cn

[T52] Scala：变量
来源：http://uj.shxzukj.cn

val a = 1;  var b = 2
来源：http://tl.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://ev.jianghongdianzi.cn

s"值: $b"
来源：http://vl.9csxet.cn

[T54] Scala：集合映射
来源：http://uk.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://pz.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://pr.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sg.huixiangedu.cn

[T56] Scala：样例类
来源：http://ck.asd995.cn

case class User(name: String, age: Int)
来源：http://xl.shxzukj.cn

[T57] Scala：模式匹配
来源：http://sa.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aq.newstarts.cn

[T58] Scala：函数定义
来源：http://pm.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bn.hnjuh.cn

[T59] Scala：循环
来源：http://nj.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://xe.shxzukj.cn

[T60] Scala：折叠
来源：http://io.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gn.521024.cn

================================================================================
来源：http://zz.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ih.colortex.cn

================================================================================
来源：http://pt.asd995.cn

[U01] Py：创建虚拟环境
来源：http://wo.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nj.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://sc.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zy.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://th.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oi.szxytkj.cn

[U04] Py：变量调试打印
来源：http://um.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ya.newstarts.cn

[U05] Py：列表去重且保序
来源：http://ey.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://ke.hahajie.cn

[U06] Py：合并两个字典
来源：http://nh.hahajie.cn

{**a, **b}
来源：http://rp.hnjuh.cn

[U07] Py：反转字典键值
来源：http://tl.newstarts.cn

{v: k for k, v in d.items()}
来源：http://yk.gzmigu.cn

[U08] Py：展平二维列表
来源：http://fb.521024.cn

[y for x in nested for y in x]
来源：http://xp.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://hm.hahajie.cn

max(d, key=d.get)
来源：http://jf.521024.cn

[U10] Py：按值排序字典
来源：http://bu.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mw.colortex.cn

[U11] Py：生成器表达式
来源：http://ng.asd995.cn

(x * 2 for x in arr)
来源：http://lu.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qw.shxzskj.cn

Counter(arr).most_common(3)
来源：http://jx.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://ss.9csxet.cn

deque(maxlen=10)
来源：http://bc.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://if.panjiajie.cn

defaultdict(list)
来源：http://sv.jctech888.com.cn

[U15] Py：高精度计时
来源：http://yy.bjjhwx.cn

t = time.perf_counter()
来源：http://iw.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://tm.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hy.muxihuayi.cn

[U17] Py：初始化日志
来源：http://wc.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://vn.gzmigu.cn

[U18] Py：预编译正则
来源：http://tt.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://iz.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://gs.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qv.colortex.cn

[U20] Py：缓存函数结果
来源：http://es.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://av.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://im.hnjuh.cn

@contextlib.contextmanager
来源：http://uc.shxzukj.cn

[U22] Py：矩阵转置
来源：http://aj.szsharing.cn

list(zip(*m))
来源：http://mp.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://xr.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://th.shxzukj.cn

[U24] Py：路径操作
来源：http://hv.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zo.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://jw.panjiajie.cn

csv.DictReader(f)
来源：http://eq.szxytkj.cn

[U26] Py：并发下载
来源：http://br.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://he.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://dv.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://sg.szsharing.cn

[U28] Py：类型别名
来源：http://ub.huanxung.cn

UserId = int
来源：http://ai.bookmarksfly.cn

[U29] Py：属性校验
来源：http://yy.huanxung.cn

@property 与 @x.setter 配合
来源：http://yw.shxzskj.cn

[U30] Py：数据类
来源：http://iu.jctech888.com.cn

@dataclass(slots=True)
来源：http://ut.szxytkj.cn

[U31] Py：单测
来源：http://qg.szsharing.cn

python -m pytest -q
来源：http://yq.9csxet.cn

[U32] Py：代码格式化
来源：http://qf.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://pu.jctech888.com.cn

[U33] Py：打包发布
来源：http://gt.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://fi.shxzskj.cn

[U34] Py：判断编码
来源：http://dl.huixiangedu.cn

chardet.detect(raw)
来源：http://ul.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://mn.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mj.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://wg.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://jx.521024.cn

[U37] Py：读写 Excel
来源：http://ap.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uw.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://uc.521024.cn

Path(__file__).resolve().parent
来源：http://cp.521024.cn

[U39] Py：判断是否在交互环境
来源：http://ez.haigaiapp.cn

sys.stdout.isatty()
来源：http://tc.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://gr.521024.cn

print("err", file=sys.stderr)
来源：http://ew.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ld.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zi.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://fe.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jv.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://gn.hahajie.cn

namespace App\Http;
来源：http://ty.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://fv.bookmarksfly.cn

declare(strict_types=1);
来源：http://tl.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://pc.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sj.jctech888.com.cn

[U46] PHP：可空类型
来源：http://ot.shtwfgs.cn

?string $name = null
来源：http://ph.hnjuh.cn

[U47] PHP：联合类型
来源：http://wl.hnjuh.cn

int|string $id
来源：http://bv.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://ly.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lu.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://bj.panjiajie.cn

public readonly string $name
来源：http://bn.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://eo.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://vq.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://el.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://jh.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://ig.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://jq.asd995.cn

[U53] PHP：空合并运算符
来源：http://cw.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://vn.hnjuh.cn

[U54] PHP：空安全调用
来源：http://oa.jctech888.com.cn

$obj?->method()
来源：http://rx.huanxung.cn

[U55] PHP：match 表达式
来源：http://gc.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fa.bjjhwx.cn

[U56] PHP：命名参数
来源：http://qu.muxihuayi.cn

f(a: 1, b: 2)
来源：http://af.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://pz.bookmarksfly.cn

"值: {$a}"
来源：http://lx.521024.cn

[U58] PHP：数组三件套
来源：http://kj.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zo.lnxyls.cn

[U59] PHP：自定义排序
来源：http://fj.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eg.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://qg.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lj.jctech888.com.cn

[U61] PHP：正则
来源：http://fs.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vl.wgjwhj.cn

[U62] PHP：日期对象
来源：http://dm.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tx.hnjuh.cn

[U63] PHP：文件读写
来源：http://qp.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wy.szxytkj.cn

[U64] PHP：目录遍历
来源：http://cr.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ey.yuntaijiaju.cn

[U65] PHP：会话
来源：http://qy.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tk.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://qe.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hk.nicolike.cn


<!-- 参考信息 -->