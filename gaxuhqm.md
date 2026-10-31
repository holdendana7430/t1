代发 wailian999

[S43] C++：智能指针
来源：http://wc.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://fd.nszjky.cn

[S44] C++：引用传参
来源：http://hh.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://wu.shtwfgs.cn

[S45] C++：lambda
来源：http://wy.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xg.nicolike.cn

[S46] C++：函数模板
来源：http://ii.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xk.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ym.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xg.shxzskj.cn

[S48] C++：逐行读文件
来源：http://do.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ln.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://an.shtwfgs.cn

[S49] C++：写文件
来源：http://rm.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cn.shxzukj.cn

[S50] C++：格式化数字
来源：http://os.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qc.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://im.wgjwhj.cn

static_cast<double>(a) / b
来源：http://vs.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://lb.huanxung.cn

int size() const noexcept { return n_; }
来源：http://pp.9csxet.cn

[S53] C++：移动语义
来源：http://qg.colortex.cn

std::vector<int> w = std::move(v);
来源：http://gh.521024.cn

[S54] C++：异常处理
来源：http://ad.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lt.lnxyls.cn

[S55] C++：结构化绑定
来源：http://bt.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dc.nszjky.cn

[S56] C++：optional
来源：http://vy.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ub.colortex.cn

[S57] C++：编译期常量
来源：http://uk.gzmigu.cn

constexpr int N = 10;
来源：http://ay.panjiajie.cn

[S58] C++：命名空间
来源：http://yi.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://yi.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://mn.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xj.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://of.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sn.muxihuayi.cn

================================================================================
来源：http://qm.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zh.jianghongdianzi.cn

================================================================================
来源：http://pm.521024.cn

[T01] Kotlin：Hello World
来源：http://wk.chemitech.net.cn

println("Hello")
来源：http://yf.newstarts.cn

[T02] Kotlin：变量
来源：http://ye.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sx.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://gz.hnjuh.cn

"值: $b"
来源：http://nu.nszjky.cn

[T04] Kotlin：空安全
来源：http://ox.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://ai.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://eu.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ap.szsharing.cn

[T06] Kotlin：集合映射
来源：http://js.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bi.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://tc.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oe.szxytkj.cn

[T08] Kotlin：数据类
来源：http://to.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://vt.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://gl.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://lj.szsharing.cn

[T10] Kotlin：默认参数
来源：http://fw.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jk.nszjky.cn

[T11] Kotlin：协程
来源：http://am.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ej.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://mm.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://co.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://kj.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://ed.bjjhwx.cn

[T14] Kotlin：循环
来源：http://gc.szsharing.cn

for (i in 1..10) println(i)
来源：http://go.521024.cn

[T15] Kotlin：接口
来源：http://hd.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://qo.yuexingan06.cn

[T16] Swift：Hello World
来源：http://wq.asd995.cn

print("Hello")
来源：http://zh.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://mw.lnxyls.cn

var a = 1;  let b = 2
来源：http://go.szsharing.cn

[T18] Swift：字符串插值
来源：http://yg.yuexingan06.cn

"值: \(b)"
来源：http://ym.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://cq.jctech888.com.cn

if let n = opt { print(n) }
来源：http://vz.asd995.cn

[T20] Swift：数组操作
来源：http://he.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mr.9csxet.cn

[T21] Swift：遍历
来源：http://ds.huanxung.cn

for x in a { print(x) }
来源：http://hg.nicolike.cn

[T22] Swift：字典
来源：http://yn.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bs.shtwfgs.cn

[T23] Swift：函数
来源：http://nu.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vb.hahajie.cn

[T24] Swift：闭包
来源：http://hz.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eb.huanxung.cn

[T25] Swift：结构体
来源：http://sg.szsharing.cn

struct P { var x: Int }
来源：http://vq.hahajie.cn

[T26] Swift：类与重写
来源：http://mq.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://la.bjjhwx.cn

[T27] Swift：错误处理
来源：http://id.szsharing.cn

do { try f() } catch { print(error) }
来源：http://rt.newstarts.cn

[T28] Swift：枚举
来源：http://bs.yuexingan06.cn

enum Color { case red, green }
来源：http://yc.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://so.haigaiapp.cn

guard let x = opt else { return }
来源：http://yo.hahajie.cn

[T30] Swift：协议
来源：http://oq.521024.cn

protocol Shape { func area() -> Double }
来源：http://fv.asd995.cn

[T31] Lua：Hello World
来源：http://cd.haigaiapp.cn

print("Hello")
来源：http://hc.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ir.haigaiapp.cn

local a = 1
来源：http://wx.lnxyls.cn

[T33] Lua：表（数组）
来源：http://qy.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ap.shtwfgs.cn

[T34] Lua：遍历表
来源：http://sv.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tl.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://jd.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://ku.panjiajie.cn

[T36] Lua：函数
来源：http://hf.panjiajie.cn

function add(a, b) return a + b end
来源：http://tg.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://yg.gzmigu.cn

"a" .. "b"
来源：http://ks.huixiangedu.cn

[T38] Lua：条件
来源：http://ib.jctech888.com.cn

if x > 0 then print("正") end
来源：http://xd.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://pr.szsharing.cn

string.find(s, "%d+")
来源：http://cz.szxytkj.cn

[T40] Lua：元表
来源：http://wz.nicolike.cn

setmetatable({}, { __index = base })
来源：http://eo.huanxung.cn

[T41] Perl：Hello World
来源：http://ct.yuntaijiaju.cn

print "Hello\n";
来源：http://re.asd995.cn

[T42] Perl：变量类型
来源：http://wc.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gf.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://ni.szxytkj.cn

"值: $a"
来源：http://vq.panjiajie.cn

[T44] Perl：条件
来源：http://zr.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ao.panjiajie.cn

[T45] Perl：数组遍历
来源：http://pv.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://pl.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://dx.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vs.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://gy.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mi.panjiajie.cn

[T48] Perl：正则替换
来源：http://sa.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://pf.yuntaijiaju.cn

[T49] Perl：函数
来源：http://ly.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yi.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://rd.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://od.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://fv.9csxet.cn

[T51] Scala：Hello World
来源：http://mo.szsharing.cn

println("Hello")
来源：http://ij.jctech888.com.cn

[T52] Scala：变量
来源：http://ng.asd995.cn

val a = 1;  var b = 2
来源：http://jv.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://ih.huixiangedu.cn

s"值: $b"
来源：http://pc.shxzukj.cn

[T54] Scala：集合映射
来源：http://ld.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://px.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://ed.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jz.haigaiapp.cn

[T56] Scala：样例类
来源：http://zm.lnxyls.cn

case class User(name: String, age: Int)
来源：http://hs.szsharing.cn

[T57] Scala：模式匹配
来源：http://av.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mn.521024.cn

[T58] Scala：函数定义
来源：http://qw.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://us.yuntaijiaju.cn

[T59] Scala：循环
来源：http://bw.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://iy.521024.cn

[T60] Scala：折叠
来源：http://rp.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bd.szxytkj.cn

================================================================================
来源：http://rq.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hx.shtwfgs.cn

================================================================================
来源：http://xz.521024.cn

[U01] Py：创建虚拟环境
来源：http://ec.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rn.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://or.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sl.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://dy.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tm.szxytkj.cn

[U04] Py：变量调试打印
来源：http://id.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ut.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://jn.huanxung.cn

list(dict.fromkeys(arr))
来源：http://ls.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://yb.huixinmuqiang.cn

{**a, **b}
来源：http://ny.newstarts.cn

[U07] Py：反转字典键值
来源：http://nk.nicolike.cn

{v: k for k, v in d.items()}
来源：http://in.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://ow.jctech888.com.cn

[y for x in nested for y in x]
来源：http://lx.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://tj.bjjhwx.cn

max(d, key=d.get)
来源：http://lw.panjiajie.cn

[U10] Py：按值排序字典
来源：http://al.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://db.9csxet.cn

[U11] Py：生成器表达式
来源：http://ee.yuexingan06.cn

(x * 2 for x in arr)
来源：http://pl.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fc.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://kp.newstarts.cn

[U13] Py：固定长度队列
来源：http://ih.chemitech.net.cn

deque(maxlen=10)
来源：http://jg.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://jr.521024.cn

defaultdict(list)
来源：http://xn.haigaiapp.cn

[U15] Py：高精度计时
来源：http://mn.bjjhwx.cn

t = time.perf_counter()
来源：http://lk.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://vx.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cw.chemitech.net.cn

[U17] Py：初始化日志
来源：http://rl.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ir.colortex.cn

[U18] Py：预编译正则
来源：http://ul.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://at.asd995.cn

[U19] Py：正则替换带回调
来源：http://qk.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ls.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://jp.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://nq.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://bl.hnjuh.cn

@contextlib.contextmanager
来源：http://zk.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://ee.nszjky.cn

list(zip(*m))
来源：http://vz.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://hc.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fb.chemitech.net.cn

[U24] Py：路径操作
来源：http://xx.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ak.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://zg.hahajie.cn

csv.DictReader(f)
来源：http://lj.hahajie.cn

[U26] Py：并发下载
来源：http://ib.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ol.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://le.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://ew.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://kc.szsharing.cn

UserId = int
来源：http://js.huanxung.cn

[U29] Py：属性校验
来源：http://dl.nszjky.cn

@property 与 @x.setter 配合
来源：http://iz.wgjwhj.cn

[U30] Py：数据类
来源：http://bl.wgjwhj.cn

@dataclass(slots=True)
来源：http://wr.newstarts.cn

[U31] Py：单测
来源：http://ru.nicolike.cn

python -m pytest -q
来源：http://zp.bjjhwx.cn

[U32] Py：代码格式化
来源：http://rf.colortex.cn

ruff format . && ruff check --fix .
来源：http://tv.jctech888.com.cn

[U33] Py：打包发布
来源：http://wk.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://xw.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://oe.shtwfgs.cn

chardet.detect(raw)
来源：http://zu.hahajie.cn

[U35] Py：发送邮件
来源：http://hx.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://np.9csxet.cn

[U36] Py：定时任务
来源：http://dy.521024.cn

schedule.every(10).minutes.do(job)
来源：http://el.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://jk.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pc.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://rj.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://mt.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://yy.haigaiapp.cn

sys.stdout.isatty()
来源：http://sk.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://yk.shxzskj.cn

print("err", file=sys.stderr)
来源：http://sa.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ga.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gq.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://cy.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cx.nszjky.cn

[U43] PHP：声明命名空间
来源：http://bl.huixinmuqiang.cn

namespace App\Http;
来源：http://fu.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://nv.newstarts.cn

declare(strict_types=1);
来源：http://di.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://su.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fk.nicolike.cn

[U46] PHP：可空类型
来源：http://gx.asd995.cn

?string $name = null
来源：http://yc.bjjhwx.cn

[U47] PHP：联合类型
来源：http://wz.huixinmuqiang.cn

int|string $id
来源：http://ca.hahajie.cn

[U48] PHP：纯枚举
来源：http://ln.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zd.9csxet.cn

[U49] PHP：只读属性
来源：http://hr.colortex.cn

public readonly string $name
来源：http://pq.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://hl.hnjuh.cn

public function __construct(private int $id) {}
来源：http://pq.szxytkj.cn

[U51] PHP：数组解构
来源：http://pk.shxzskj.cn

[$a, $b] = $arr;
来源：http://xe.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://rd.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://ya.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://uy.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://wf.colortex.cn

[U54] PHP：空安全调用
来源：http://po.chemitech.net.cn

$obj?->method()
来源：http://js.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://vd.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gd.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://xf.shxzukj.cn

f(a: 1, b: 2)
来源：http://pb.szsharing.cn

[U57] PHP：字符串插值
来源：http://fq.huixiangedu.cn

"值: {$a}"
来源：http://xt.shxzskj.cn

[U58] PHP：数组三件套
来源：http://qn.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vn.asd995.cn

[U59] PHP：自定义排序
来源：http://wq.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yj.asd995.cn

[U60] PHP：JSON 编解码
来源：http://vn.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gg.nszjky.cn

[U61] PHP：正则
来源：http://qz.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uh.jctech888.com.cn

[U62] PHP：日期对象
来源：http://cc.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sf.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://cq.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zx.9csxet.cn

[U64] PHP：目录遍历
来源：http://ju.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://ge.hnjuh.cn

[U65] PHP：会话
来源：http://ok.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zd.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://wb.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://if.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://oc.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oz.9csxet.cn

[U68] PHP：PDO 连接
来源：http://ve.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ns.newstarts.cn


<!-- 参考信息 -->