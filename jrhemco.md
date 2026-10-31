代发 wailian999

[S39] C++：自定义比较器排序
来源：http://br.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kj.shxzskj.cn

[S40] C++：查找元素
来源：http://ca.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nl.9csxet.cn

[S41] C++：类与构造函数
来源：http://sv.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ca.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://jj.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ta.lnxyls.cn

[S43] C++：智能指针
来源：http://gr.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://cv.huanxung.cn

[S44] C++：引用传参
来源：http://jk.nicolike.cn

void inc(int &x) { ++x; }
来源：http://dx.huixinmuqiang.cn

[S45] C++：lambda
来源：http://nd.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nc.newstarts.cn

[S46] C++：函数模板
来源：http://oq.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rx.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://zo.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oc.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://dm.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://th.szsharing.cn

while (std::getline(in, line)) { }
来源：http://di.bookmarksfly.cn

[S49] C++：写文件
来源：http://tw.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ep.haigaiapp.cn

[S50] C++：格式化数字
来源：http://fc.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uw.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://jz.wgjwhj.cn

static_cast<double>(a) / b
来源：http://rc.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ph.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://db.nszjky.cn

[S53] C++：移动语义
来源：http://wh.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://zm.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://ny.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ko.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://in.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vy.huixiangedu.cn

[S56] C++：optional
来源：http://yg.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ch.newstarts.cn

[S57] C++：编译期常量
来源：http://zb.newstarts.cn

constexpr int N = 10;
来源：http://fi.yuexingan06.cn

[S58] C++：命名空间
来源：http://nv.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://dj.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://yz.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tc.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ol.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uk.nicolike.cn

================================================================================
来源：http://ec.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ku.panjiajie.cn

================================================================================
来源：http://da.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ng.huixinmuqiang.cn

println("Hello")
来源：http://km.asd995.cn

[T02] Kotlin：变量
来源：http://fa.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eb.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://qy.bookmarksfly.cn

"值: $b"
来源：http://pa.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://od.521024.cn

val n: String? = null;  n?.length
来源：http://gt.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://ki.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://im.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://hy.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ao.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://wm.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pn.shxzukj.cn

[T08] Kotlin：数据类
来源：http://jv.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://sc.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://jq.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ry.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ak.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oj.9csxet.cn

[T11] Kotlin：协程
来源：http://xg.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mo.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://mi.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://rr.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://dg.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://on.asd995.cn

[T14] Kotlin：循环
来源：http://nj.shxzukj.cn

for (i in 1..10) println(i)
来源：http://mb.wgjwhj.cn

[T15] Kotlin：接口
来源：http://yg.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://sg.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://wp.jctech888.com.cn

print("Hello")
来源：http://gb.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://kw.colortex.cn

var a = 1;  let b = 2
来源：http://fp.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://tg.panjiajie.cn

"值: \(b)"
来源：http://wk.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://tm.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://tv.colortex.cn

[T20] Swift：数组操作
来源：http://vt.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qk.szsharing.cn

[T21] Swift：遍历
来源：http://lg.huixiangedu.cn

for x in a { print(x) }
来源：http://bk.yuexingan06.cn

[T22] Swift：字典
来源：http://tc.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://td.shxzskj.cn

[T23] Swift：函数
来源：http://qe.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ui.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://ic.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ds.wgjwhj.cn

[T25] Swift：结构体
来源：http://kl.asd995.cn

struct P { var x: Int }
来源：http://uo.521024.cn

[T26] Swift：类与重写
来源：http://za.gzmigu.cn

class A: Base { override func f() {} }
来源：http://sm.shxzskj.cn

[T27] Swift：错误处理
来源：http://io.nicolike.cn

do { try f() } catch { print(error) }
来源：http://gz.haigaiapp.cn

[T28] Swift：枚举
来源：http://bw.bjjhwx.cn

enum Color { case red, green }
来源：http://bx.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://rs.colortex.cn

guard let x = opt else { return }
来源：http://gh.nszjky.cn

[T30] Swift：协议
来源：http://rr.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://wa.panjiajie.cn

[T31] Lua：Hello World
来源：http://fr.bjjhwx.cn

print("Hello")
来源：http://wx.521024.cn

[T32] Lua：局部变量
来源：http://tg.shtwfgs.cn

local a = 1
来源：http://gf.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://pg.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bs.gzmigu.cn

[T34] Lua：遍历表
来源：http://fm.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jf.asd995.cn

[T35] Lua：字典表
来源：http://df.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://cb.colortex.cn

[T36] Lua：函数
来源：http://kl.hnjuh.cn

function add(a, b) return a + b end
来源：http://am.huanxung.cn

[T37] Lua：字符串拼接
来源：http://bd.asd995.cn

"a" .. "b"
来源：http://bf.szsharing.cn

[T38] Lua：条件
来源：http://yx.newstarts.cn

if x > 0 then print("正") end
来源：http://dz.hahajie.cn

[T39] Lua：模式匹配
来源：http://vs.bookmarksfly.cn

string.find(s, "%d+")
来源：http://sd.newstarts.cn

[T40] Lua：元表
来源：http://ht.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://oq.asd995.cn

[T41] Perl：Hello World
来源：http://bo.lnxyls.cn

print "Hello\n";
来源：http://xe.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://yb.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://im.huanxung.cn

[T43] Perl：字符串插值
来源：http://qi.gzmigu.cn

"值: $a"
来源：http://jq.yuexingan06.cn

[T44] Perl：条件
来源：http://om.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://yw.szsharing.cn

[T45] Perl：数组遍历
来源：http://qw.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://zo.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://lq.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dm.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://pq.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cw.gzmigu.cn

[T48] Perl：正则替换
来源：http://xf.hnjuh.cn

$s =~ s/old/new/g;
来源：http://rn.szsharing.cn

[T49] Perl：函数
来源：http://pm.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cg.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ve.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://af.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://pa.521024.cn

[T51] Scala：Hello World
来源：http://wk.wgjwhj.cn

println("Hello")
来源：http://dn.bjjhwx.cn

[T52] Scala：变量
来源：http://wt.haigaiapp.cn

val a = 1;  var b = 2
来源：http://zv.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://ou.yuexingan06.cn

s"值: $b"
来源：http://jf.szsharing.cn

[T54] Scala：集合映射
来源：http://zn.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://bs.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://gz.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://de.panjiajie.cn

[T56] Scala：样例类
来源：http://mr.shxzukj.cn

case class User(name: String, age: Int)
来源：http://um.nszjky.cn

[T57] Scala：模式匹配
来源：http://by.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gg.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://fo.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mp.shxzskj.cn

[T59] Scala：循环
来源：http://ei.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://mf.huixiangedu.cn

[T60] Scala：折叠
来源：http://qz.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qd.yuntaijiaju.cn

================================================================================
来源：http://de.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yo.muxihuayi.cn

================================================================================
来源：http://bp.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://hj.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fq.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://ac.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ov.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://dr.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ym.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://yt.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jb.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://yy.huanxung.cn

list(dict.fromkeys(arr))
来源：http://sg.hnjuh.cn

[U06] Py：合并两个字典
来源：http://po.yuntaijiaju.cn

{**a, **b}
来源：http://nw.newstarts.cn

[U07] Py：反转字典键值
来源：http://gx.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://qe.lnxyls.cn

[U08] Py：展平二维列表
来源：http://jx.yuexingan06.cn

[y for x in nested for y in x]
来源：http://yl.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://sb.chemitech.net.cn

max(d, key=d.get)
来源：http://pr.asd995.cn

[U10] Py：按值排序字典
来源：http://eg.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tr.gzmigu.cn

[U11] Py：生成器表达式
来源：http://hl.asd995.cn

(x * 2 for x in arr)
来源：http://on.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hs.9csxet.cn

Counter(arr).most_common(3)
来源：http://ey.521024.cn

[U13] Py：固定长度队列
来源：http://pa.gzmigu.cn

deque(maxlen=10)
来源：http://tg.colortex.cn

[U14] Py：分组收集到列表
来源：http://py.huanxung.cn

defaultdict(list)
来源：http://hw.huanxung.cn

[U15] Py：高精度计时
来源：http://zn.9csxet.cn

t = time.perf_counter()
来源：http://of.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://pj.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pb.yuexingan06.cn

[U17] Py：初始化日志
来源：http://yf.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://vv.huanxung.cn

[U18] Py：预编译正则
来源：http://wv.szsharing.cn

pat = re.compile(r"\d+")
来源：http://xa.szsharing.cn

[U19] Py：正则替换带回调
来源：http://ov.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://at.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://fm.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://tw.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://wj.chemitech.net.cn

@contextlib.contextmanager
来源：http://jg.shxzskj.cn

[U22] Py：矩阵转置
来源：http://ju.shxzukj.cn

list(zip(*m))
来源：http://os.nszjky.cn

[U23] Py：分块读取大文件
来源：http://gi.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hw.9csxet.cn

[U24] Py：路径操作
来源：http://np.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zy.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://gw.szsharing.cn

csv.DictReader(f)
来源：http://mz.jctech888.com.cn

[U26] Py：并发下载
来源：http://zh.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wc.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://nq.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://fd.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://wp.szxytkj.cn

UserId = int
来源：http://yy.huixiangedu.cn

[U29] Py：属性校验
来源：http://ro.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://zu.huixinmuqiang.cn

[U30] Py：数据类
来源：http://dn.521024.cn

@dataclass(slots=True)
来源：http://ia.huixiangedu.cn

[U31] Py：单测
来源：http://nt.shxzskj.cn

python -m pytest -q
来源：http://hi.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://ez.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://zt.szxytkj.cn

[U33] Py：打包发布
来源：http://ax.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://hs.shtwfgs.cn

[U34] Py：判断编码
来源：http://ml.chemitech.net.cn

chardet.detect(raw)
来源：http://jm.huanxung.cn

[U35] Py：发送邮件
来源：http://nv.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rd.nicolike.cn

[U36] Py：定时任务
来源：http://tq.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://vk.9csxet.cn

[U37] Py：读写 Excel
来源：http://qy.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://om.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://rj.521024.cn

Path(__file__).resolve().parent
来源：http://js.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://nx.shxzukj.cn

sys.stdout.isatty()
来源：http://cj.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://pi.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://ax.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://nm.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gt.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://yu.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ox.nszjky.cn

[U43] PHP：声明命名空间
来源：http://kd.shtwfgs.cn

namespace App\Http;
来源：http://pp.9csxet.cn

[U44] PHP：开启严格类型
来源：http://wq.shxzukj.cn

declare(strict_types=1);
来源：http://qf.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://jp.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ok.chemitech.net.cn

[U46] PHP：可空类型
来源：http://lv.muxihuayi.cn

?string $name = null
来源：http://ye.muxihuayi.cn

[U47] PHP：联合类型
来源：http://pn.shxzskj.cn

int|string $id
来源：http://la.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://jn.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vt.lnxyls.cn

[U49] PHP：只读属性
来源：http://fv.shxzukj.cn

public readonly string $name
来源：http://lt.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://vk.szsharing.cn

public function __construct(private int $id) {}
来源：http://mk.shtwfgs.cn

[U51] PHP：数组解构
来源：http://hw.huixiangedu.cn

[$a, $b] = $arr;
来源：http://re.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://pj.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://ob.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ke.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://uz.newstarts.cn

[U54] PHP：空安全调用
来源：http://dg.muxihuayi.cn

$obj?->method()
来源：http://wl.nszjky.cn

[U55] PHP：match 表达式
来源：http://ql.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qs.shxzskj.cn

[U56] PHP：命名参数
来源：http://nr.szsharing.cn

f(a: 1, b: 2)
来源：http://sp.shxzukj.cn

[U57] PHP：字符串插值
来源：http://he.newstarts.cn

"值: {$a}"
来源：http://wu.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://kg.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nk.szsharing.cn

[U59] PHP：自定义排序
来源：http://am.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wg.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://xn.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://so.szsharing.cn

[U61] PHP：正则
来源：http://uw.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nb.shxzskj.cn

[U62] PHP：日期对象
来源：http://mx.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dj.nicolike.cn

[U63] PHP：文件读写
来源：http://ma.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wd.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://to.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://dj.shtwfgs.cn


<!-- 参考信息 -->