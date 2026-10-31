代发 wailian999

[S43] C++：智能指针
来源：http://zh.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://ey.hahajie.cn

[S44] C++：引用传参
来源：http://pw.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://td.yuntaijiaju.cn

[S45] C++：lambda
来源：http://ri.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tj.jctech888.com.cn

[S46] C++：函数模板
来源：http://ko.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rs.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://uq.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ku.lnxyls.cn

[S48] C++：逐行读文件
来源：http://oo.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://np.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://wp.huixinmuqiang.cn

[S49] C++：写文件
来源：http://zg.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://te.shtwfgs.cn

[S50] C++：格式化数字
来源：http://sv.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ld.gzmigu.cn

[S51] C++：显式类型转换
来源：http://yc.newstarts.cn

static_cast<double>(a) / b
来源：http://sz.colortex.cn

[S52] C++：const 与 noexcept
来源：http://gc.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://so.szxytkj.cn

[S53] C++：移动语义
来源：http://qm.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://gs.bookmarksfly.cn

[S54] C++：异常处理
来源：http://no.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sk.521024.cn

[S55] C++：结构化绑定
来源：http://sl.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hc.shxzukj.cn

[S56] C++：optional
来源：http://cs.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tr.hnjuh.cn

[S57] C++：编译期常量
来源：http://yo.szsharing.cn

constexpr int N = 10;
来源：http://jq.gzmigu.cn

[S58] C++：命名空间
来源：http://ts.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ka.lnxyls.cn

[S59] C++：静态断言
来源：http://ey.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wh.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://fh.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ew.colortex.cn

================================================================================
来源：http://qh.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zp.521024.cn

================================================================================
来源：http://lx.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://af.lnxyls.cn

println("Hello")
来源：http://ou.newstarts.cn

[T02] Kotlin：变量
来源：http://ts.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nc.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://uz.huanxung.cn

"值: $b"
来源：http://gv.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://nv.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://qq.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://yc.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://se.9csxet.cn

[T06] Kotlin：集合映射
来源：http://jr.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://in.colortex.cn

[T07] Kotlin：集合过滤
来源：http://ev.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qw.shxzukj.cn

[T08] Kotlin：数据类
来源：http://fb.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://fs.521024.cn

[T09] Kotlin：扩展函数
来源：http://od.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://xh.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://ju.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://js.yuexingan06.cn

[T11] Kotlin：协程
来源：http://hi.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://th.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://la.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://tl.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://cf.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://en.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://br.nicolike.cn

for (i in 1..10) println(i)
来源：http://nu.huanxung.cn

[T15] Kotlin：接口
来源：http://ui.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://qq.yuexingan06.cn

[T16] Swift：Hello World
来源：http://ul.bjjhwx.cn

print("Hello")
来源：http://od.colortex.cn

[T17] Swift：变量与常量
来源：http://dl.gzmigu.cn

var a = 1;  let b = 2
来源：http://kl.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://ao.jianghongdianzi.cn

"值: \(b)"
来源：http://vy.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ew.nicolike.cn

if let n = opt { print(n) }
来源：http://gb.shxzukj.cn

[T20] Swift：数组操作
来源：http://st.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uy.huixiangedu.cn

[T21] Swift：遍历
来源：http://ic.lnxyls.cn

for x in a { print(x) }
来源：http://fh.bookmarksfly.cn

[T22] Swift：字典
来源：http://zh.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fk.9csxet.cn

[T23] Swift：函数
来源：http://lp.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uh.huanxung.cn

[T24] Swift：闭包
来源：http://zz.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mp.asd995.cn

[T25] Swift：结构体
来源：http://ts.huixiangedu.cn

struct P { var x: Int }
来源：http://zi.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://ei.huanxung.cn

class A: Base { override func f() {} }
来源：http://ex.wgjwhj.cn

[T27] Swift：错误处理
来源：http://tr.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://ul.colortex.cn

[T28] Swift：枚举
来源：http://of.chemitech.net.cn

enum Color { case red, green }
来源：http://rb.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://zx.asd995.cn

guard let x = opt else { return }
来源：http://pl.bjjhwx.cn

[T30] Swift：协议
来源：http://ef.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://eb.newstarts.cn

[T31] Lua：Hello World
来源：http://jz.nszjky.cn

print("Hello")
来源：http://us.hnjuh.cn

[T32] Lua：局部变量
来源：http://aj.lnxyls.cn

local a = 1
来源：http://bv.521024.cn

[T33] Lua：表（数组）
来源：http://ut.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hv.9csxet.cn

[T34] Lua：遍历表
来源：http://gm.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bk.szxytkj.cn

[T35] Lua：字典表
来源：http://ek.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://qz.huanxung.cn

[T36] Lua：函数
来源：http://mq.hnjuh.cn

function add(a, b) return a + b end
来源：http://pj.9csxet.cn

[T37] Lua：字符串拼接
来源：http://ux.szxytkj.cn

"a" .. "b"
来源：http://qo.hnjuh.cn

[T38] Lua：条件
来源：http://gj.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://lj.panjiajie.cn

[T39] Lua：模式匹配
来源：http://gv.muxihuayi.cn

string.find(s, "%d+")
来源：http://df.shtwfgs.cn

[T40] Lua：元表
来源：http://my.nicolike.cn

setmetatable({}, { __index = base })
来源：http://dc.panjiajie.cn

[T41] Perl：Hello World
来源：http://ri.muxihuayi.cn

print "Hello\n";
来源：http://ro.shtwfgs.cn

[T42] Perl：变量类型
来源：http://wg.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yv.huanxung.cn

[T43] Perl：字符串插值
来源：http://ap.lnxyls.cn

"值: $a"
来源：http://xe.hahajie.cn

[T44] Perl：条件
来源：http://uh.colortex.cn

if ($a > 0) { print "正"; }
来源：http://pv.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://wh.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ex.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://hq.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sk.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ac.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://og.muxihuayi.cn

[T48] Perl：正则替换
来源：http://sf.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://nh.521024.cn

[T49] Perl：函数
来源：http://qx.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hm.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://gv.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fl.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://bz.huanxung.cn

[T51] Scala：Hello World
来源：http://vr.huixinmuqiang.cn

println("Hello")
来源：http://jt.lnxyls.cn

[T52] Scala：变量
来源：http://qm.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://aa.lnxyls.cn

[T53] Scala：字符串插值
来源：http://bi.shxzskj.cn

s"值: $b"
来源：http://tj.bjjhwx.cn

[T54] Scala：集合映射
来源：http://qs.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://zc.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://qv.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yy.wgjwhj.cn

[T56] Scala：样例类
来源：http://sq.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://ac.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://kz.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pf.panjiajie.cn

[T58] Scala：函数定义
来源：http://vl.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nc.muxihuayi.cn

[T59] Scala：循环
来源：http://iu.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://bz.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://oc.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zh.newstarts.cn

================================================================================
来源：http://ck.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kk.shxzukj.cn

================================================================================
来源：http://sf.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://xa.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wp.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://bd.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ka.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://gf.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://be.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://du.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bi.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://ii.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://nb.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ey.nszjky.cn

{**a, **b}
来源：http://zd.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://qp.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://sg.szxytkj.cn

[U08] Py：展平二维列表
来源：http://jy.haigaiapp.cn

[y for x in nested for y in x]
来源：http://te.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://fr.521024.cn

max(d, key=d.get)
来源：http://su.hahajie.cn

[U10] Py：按值排序字典
来源：http://vv.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://au.lnxyls.cn

[U11] Py：生成器表达式
来源：http://hz.huixiangedu.cn

(x * 2 for x in arr)
来源：http://vf.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vs.shxzskj.cn

Counter(arr).most_common(3)
来源：http://de.521024.cn

[U13] Py：固定长度队列
来源：http://wk.bookmarksfly.cn

deque(maxlen=10)
来源：http://cn.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://tl.huanxung.cn

defaultdict(list)
来源：http://xe.huanxung.cn

[U15] Py：高精度计时
来源：http://he.colortex.cn

t = time.perf_counter()
来源：http://js.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://vz.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jx.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://ym.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ih.yuexingan06.cn

[U18] Py：预编译正则
来源：http://yv.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://ke.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://hm.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dp.huanxung.cn

[U20] Py：缓存函数结果
来源：http://pw.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ma.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://gs.nszjky.cn

@contextlib.contextmanager
来源：http://ch.gzmigu.cn

[U22] Py：矩阵转置
来源：http://gb.yuexingan06.cn

list(zip(*m))
来源：http://hp.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://gk.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qi.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://lo.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lv.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://mo.nicolike.cn

csv.DictReader(f)
来源：http://gm.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://vy.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sy.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://om.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://fd.wgjwhj.cn

[U28] Py：类型别名
来源：http://cq.colortex.cn

UserId = int
来源：http://zn.gzmigu.cn

[U29] Py：属性校验
来源：http://hd.lnxyls.cn

@property 与 @x.setter 配合
来源：http://cm.panjiajie.cn

[U30] Py：数据类
来源：http://kk.yuexingan06.cn

@dataclass(slots=True)
来源：http://uj.bjjhwx.cn

[U31] Py：单测
来源：http://ne.chemitech.net.cn

python -m pytest -q
来源：http://li.lnxyls.cn

[U32] Py：代码格式化
来源：http://ab.9csxet.cn

ruff format . && ruff check --fix .
来源：http://us.muxihuayi.cn

[U33] Py：打包发布
来源：http://ot.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://jg.newstarts.cn

[U34] Py：判断编码
来源：http://ow.nszjky.cn

chardet.detect(raw)
来源：http://xn.lnxyls.cn

[U35] Py：发送邮件
来源：http://ie.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ci.jctech888.com.cn

[U36] Py：定时任务
来源：http://gx.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://uh.9csxet.cn

[U37] Py：读写 Excel
来源：http://ln.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ap.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://nq.hahajie.cn

Path(__file__).resolve().parent
来源：http://xz.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://zu.shtwfgs.cn

sys.stdout.isatty()
来源：http://gg.huanxung.cn

[U40] Py：打印到标准错误
来源：http://az.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://go.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://cu.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hd.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://ip.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yz.9csxet.cn

[U43] PHP：声明命名空间
来源：http://tt.shxzukj.cn

namespace App\Http;
来源：http://dk.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://jq.chemitech.net.cn

declare(strict_types=1);
来源：http://so.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://ht.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vk.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://pg.jctech888.com.cn

?string $name = null
来源：http://iu.panjiajie.cn

[U47] PHP：联合类型
来源：http://ix.chemitech.net.cn

int|string $id
来源：http://ib.9csxet.cn

[U48] PHP：纯枚举
来源：http://kl.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hh.nicolike.cn

[U49] PHP：只读属性
来源：http://ss.jctech888.com.cn

public readonly string $name
来源：http://fz.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://xk.szsharing.cn

public function __construct(private int $id) {}
来源：http://dp.bjjhwx.cn

[U51] PHP：数组解构
来源：http://cr.panjiajie.cn

[$a, $b] = $arr;
来源：http://mm.asd995.cn

[U52] PHP：箭头函数
来源：http://ag.521024.cn

$double = fn($x) => $x * 2;
来源：http://da.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://on.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://br.newstarts.cn

[U54] PHP：空安全调用
来源：http://kf.shxzskj.cn

$obj?->method()
来源：http://el.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://im.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cl.nicolike.cn

[U56] PHP：命名参数
来源：http://qv.lnxyls.cn

f(a: 1, b: 2)
来源：http://aq.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://ip.521024.cn

"值: {$a}"
来源：http://hr.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://xg.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hi.hnjuh.cn

[U59] PHP：自定义排序
来源：http://bj.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qy.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://ww.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yw.lnxyls.cn

[U61] PHP：正则
来源：http://ch.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xv.nicolike.cn

[U62] PHP：日期对象
来源：http://bb.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ma.colortex.cn

[U63] PHP：文件读写
来源：http://uy.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wj.hahajie.cn

[U64] PHP：目录遍历
来源：http://wy.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://uj.huanxung.cn

[U65] PHP：会话
来源：http://zw.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ub.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://dy.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qv.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://to.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yd.nszjky.cn

[U68] PHP：PDO 连接
来源：http://mp.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lp.gzmigu.cn


<!-- 参考信息 -->