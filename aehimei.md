代发 wailian999

[S41] C++：类与构造函数
来源：http://og.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ei.9csxet.cn

[S42] C++：继承与虚函数
来源：http://rf.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://on.huixiangedu.cn

[S43] C++：智能指针
来源：http://sv.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://la.shtwfgs.cn

[S44] C++：引用传参
来源：http://aw.521024.cn

void inc(int &x) { ++x; }
来源：http://wd.szxytkj.cn

[S45] C++：lambda
来源：http://qw.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ht.lnxyls.cn

[S46] C++：函数模板
来源：http://yl.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wc.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://gu.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xh.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://os.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ll.9csxet.cn

while (std::getline(in, line)) { }
来源：http://uu.bjjhwx.cn

[S49] C++：写文件
来源：http://bc.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gz.gzmigu.cn

[S50] C++：格式化数字
来源：http://nn.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zl.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://zu.haigaiapp.cn

static_cast<double>(a) / b
来源：http://vw.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://cx.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://du.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://mh.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://qz.hnjuh.cn

[S54] C++：异常处理
来源：http://qi.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qi.newstarts.cn

[S55] C++：结构化绑定
来源：http://uu.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://je.yuntaijiaju.cn

[S56] C++：optional
来源：http://pm.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xf.nicolike.cn

[S57] C++：编译期常量
来源：http://sn.panjiajie.cn

constexpr int N = 10;
来源：http://bw.9csxet.cn

[S58] C++：命名空间
来源：http://vn.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://xo.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://gt.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sh.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://ub.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pc.haigaiapp.cn

================================================================================
来源：http://nh.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://at.521024.cn

================================================================================
来源：http://vj.nszjky.cn

[T01] Kotlin：Hello World
来源：http://jr.asd995.cn

println("Hello")
来源：http://jm.jctech888.com.cn

[T02] Kotlin：变量
来源：http://ic.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zg.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://oc.huanxung.cn

"值: $b"
来源：http://mm.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://nu.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://wz.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://hc.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yc.9csxet.cn

[T06] Kotlin：集合映射
来源：http://sv.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://os.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://io.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dy.asd995.cn

[T08] Kotlin：数据类
来源：http://oq.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://zx.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://ws.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://va.9csxet.cn

[T10] Kotlin：默认参数
来源：http://tt.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jp.yuexingan06.cn

[T11] Kotlin：协程
来源：http://hg.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lu.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://oo.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://gn.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://rz.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://yl.nszjky.cn

[T14] Kotlin：循环
来源：http://kd.panjiajie.cn

for (i in 1..10) println(i)
来源：http://td.huanxung.cn

[T15] Kotlin：接口
来源：http://ve.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://wp.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://ru.nszjky.cn

print("Hello")
来源：http://oa.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://di.lnxyls.cn

var a = 1;  let b = 2
来源：http://ge.9csxet.cn

[T18] Swift：字符串插值
来源：http://ow.haigaiapp.cn

"值: \(b)"
来源：http://tt.hahajie.cn

[T19] Swift：可选绑定
来源：http://eh.haigaiapp.cn

if let n = opt { print(n) }
来源：http://mj.jctech888.com.cn

[T20] Swift：数组操作
来源：http://nt.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zs.gzmigu.cn

[T21] Swift：遍历
来源：http://kd.hahajie.cn

for x in a { print(x) }
来源：http://xp.asd995.cn

[T22] Swift：字典
来源：http://fi.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sr.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ka.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bh.asd995.cn

[T24] Swift：闭包
来源：http://xk.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jq.muxihuayi.cn

[T25] Swift：结构体
来源：http://lc.panjiajie.cn

struct P { var x: Int }
来源：http://al.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://vs.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://xl.newstarts.cn

[T27] Swift：错误处理
来源：http://pr.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://wt.yuexingan06.cn

[T28] Swift：枚举
来源：http://xh.muxihuayi.cn

enum Color { case red, green }
来源：http://qg.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://qg.szxytkj.cn

guard let x = opt else { return }
来源：http://nm.szxytkj.cn

[T30] Swift：协议
来源：http://dc.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://py.szxytkj.cn

[T31] Lua：Hello World
来源：http://zg.panjiajie.cn

print("Hello")
来源：http://dv.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://nh.nszjky.cn

local a = 1
来源：http://wv.szsharing.cn

[T33] Lua：表（数组）
来源：http://dd.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ez.lnxyls.cn

[T34] Lua：遍历表
来源：http://tl.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://za.hahajie.cn

[T35] Lua：字典表
来源：http://ag.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://bh.lnxyls.cn

[T36] Lua：函数
来源：http://mc.lnxyls.cn

function add(a, b) return a + b end
来源：http://wu.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://zy.521024.cn

"a" .. "b"
来源：http://yd.shxzskj.cn

[T38] Lua：条件
来源：http://tq.nicolike.cn

if x > 0 then print("正") end
来源：http://ti.9csxet.cn

[T39] Lua：模式匹配
来源：http://vv.hahajie.cn

string.find(s, "%d+")
来源：http://kn.521024.cn

[T40] Lua：元表
来源：http://ni.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://ly.asd995.cn

[T41] Perl：Hello World
来源：http://zs.newstarts.cn

print "Hello\n";
来源：http://uc.9csxet.cn

[T42] Perl：变量类型
来源：http://lk.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sg.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://nz.hahajie.cn

"值: $a"
来源：http://gv.nszjky.cn

[T44] Perl：条件
来源：http://jy.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://yv.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://pz.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://ju.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://tz.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ie.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://zd.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fi.nszjky.cn

[T48] Perl：正则替换
来源：http://sc.colortex.cn

$s =~ s/old/new/g;
来源：http://uf.521024.cn

[T49] Perl：函数
来源：http://vs.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xg.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://od.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sr.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ro.shxzskj.cn

[T51] Scala：Hello World
来源：http://ri.521024.cn

println("Hello")
来源：http://iy.szxytkj.cn

[T52] Scala：变量
来源：http://uf.szxytkj.cn

val a = 1;  var b = 2
来源：http://nq.lnxyls.cn

[T53] Scala：字符串插值
来源：http://nh.haigaiapp.cn

s"值: $b"
来源：http://oi.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://ex.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://wk.newstarts.cn

[T55] Scala：集合过滤
来源：http://ix.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mc.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://lx.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://xn.521024.cn

[T57] Scala：模式匹配
来源：http://oj.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ru.hnjuh.cn

[T58] Scala：函数定义
来源：http://dg.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://td.newstarts.cn

[T59] Scala：循环
来源：http://nf.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://gk.lnxyls.cn

[T60] Scala：折叠
来源：http://iy.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lk.9csxet.cn

================================================================================
来源：http://fg.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sa.szxytkj.cn

================================================================================
来源：http://tt.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://pk.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://az.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ao.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fn.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://sf.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fx.hnjuh.cn

[U04] Py：变量调试打印
来源：http://lv.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zl.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://ll.521024.cn

list(dict.fromkeys(arr))
来源：http://dy.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://qw.nicolike.cn

{**a, **b}
来源：http://ms.shxzskj.cn

[U07] Py：反转字典键值
来源：http://kl.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://pm.hahajie.cn

[U08] Py：展平二维列表
来源：http://vh.521024.cn

[y for x in nested for y in x]
来源：http://xf.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://yz.jianghongdianzi.cn

max(d, key=d.get)
来源：http://uf.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://iu.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hp.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://cs.wgjwhj.cn

(x * 2 for x in arr)
来源：http://gq.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://je.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://ht.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://tc.wgjwhj.cn

deque(maxlen=10)
来源：http://mc.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://yg.yuntaijiaju.cn

defaultdict(list)
来源：http://hv.hnjuh.cn

[U15] Py：高精度计时
来源：http://te.gzmigu.cn

t = time.perf_counter()
来源：http://vi.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://od.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eh.szsharing.cn

[U17] Py：初始化日志
来源：http://fb.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ji.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ob.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://ea.9csxet.cn

[U19] Py：正则替换带回调
来源：http://ro.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sm.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://qx.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ec.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://am.newstarts.cn

@contextlib.contextmanager
来源：http://bw.hnjuh.cn

[U22] Py：矩阵转置
来源：http://wd.nicolike.cn

list(zip(*m))
来源：http://pt.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://vm.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://um.nicolike.cn

[U24] Py：路径操作
来源：http://zf.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rh.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://rg.muxihuayi.cn

csv.DictReader(f)
来源：http://ho.huanxung.cn

[U26] Py：并发下载
来源：http://ji.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gw.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://sp.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://jd.haigaiapp.cn

[U28] Py：类型别名
来源：http://fu.521024.cn

UserId = int
来源：http://cx.jctech888.com.cn

[U29] Py：属性校验
来源：http://px.521024.cn

@property 与 @x.setter 配合
来源：http://wd.lnxyls.cn

[U30] Py：数据类
来源：http://eh.huixiangedu.cn

@dataclass(slots=True)
来源：http://oa.szxytkj.cn

[U31] Py：单测
来源：http://pf.yuntaijiaju.cn

python -m pytest -q
来源：http://ja.hnjuh.cn

[U32] Py：代码格式化
来源：http://tg.nszjky.cn

ruff format . && ruff check --fix .
来源：http://tf.521024.cn

[U33] Py：打包发布
来源：http://ci.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://st.haigaiapp.cn

[U34] Py：判断编码
来源：http://on.lnxyls.cn

chardet.detect(raw)
来源：http://jp.panjiajie.cn

[U35] Py：发送邮件
来源：http://ee.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nu.bjjhwx.cn

[U36] Py：定时任务
来源：http://uo.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://gb.lnxyls.cn

[U37] Py：读写 Excel
来源：http://cj.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ih.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://vi.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://mz.colortex.cn

sys.stdout.isatty()
来源：http://xo.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://sz.panjiajie.cn

print("err", file=sys.stderr)
来源：http://ad.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://va.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ih.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://wp.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fq.huanxung.cn

[U43] PHP：声明命名空间
来源：http://ep.521024.cn

namespace App\Http;
来源：http://eq.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://nj.huixiangedu.cn

declare(strict_types=1);
来源：http://xj.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://bp.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ix.newstarts.cn

[U46] PHP：可空类型
来源：http://ir.521024.cn

?string $name = null
来源：http://qw.muxihuayi.cn

[U47] PHP：联合类型
来源：http://ht.9csxet.cn

int|string $id
来源：http://uf.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://jw.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ps.shxzukj.cn

[U49] PHP：只读属性
来源：http://mw.bookmarksfly.cn

public readonly string $name
来源：http://zk.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://tc.lnxyls.cn

public function __construct(private int $id) {}
来源：http://mi.colortex.cn

[U51] PHP：数组解构
来源：http://hp.lnxyls.cn

[$a, $b] = $arr;
来源：http://rm.gzmigu.cn

[U52] PHP：箭头函数
来源：http://hz.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://qt.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://wy.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://fg.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://nj.huixiangedu.cn

$obj?->method()
来源：http://tq.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ut.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ne.asd995.cn

[U56] PHP：命名参数
来源：http://mr.nicolike.cn

f(a: 1, b: 2)
来源：http://xi.colortex.cn

[U57] PHP：字符串插值
来源：http://jl.wgjwhj.cn

"值: {$a}"
来源：http://et.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://xu.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ho.nszjky.cn

[U59] PHP：自定义排序
来源：http://ag.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vx.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://mg.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qe.huixiangedu.cn

[U61] PHP：正则
来源：http://li.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://du.panjiajie.cn

[U62] PHP：日期对象
来源：http://wi.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://he.521024.cn

[U63] PHP：文件读写
来源：http://iy.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ym.shxzukj.cn

[U64] PHP：目录遍历
来源：http://vu.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://ib.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ca.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lj.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://jh.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xk.haigaiapp.cn


<!-- 参考信息 -->