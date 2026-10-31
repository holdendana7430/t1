代发 wailian999

[S37] C++：set
来源：http://zl.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.shtwfgs.cn

[S38] C++：排序
来源：http://os.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://xh.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://wq.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xe.nicolike.cn

[S40] C++：查找元素
来源：http://qf.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nt.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ov.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ho.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://we.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://gh.521024.cn

[S43] C++：智能指针
来源：http://xj.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://za.wgjwhj.cn

[S44] C++：引用传参
来源：http://qh.asd995.cn

void inc(int &x) { ++x; }
来源：http://az.szxytkj.cn

[S45] C++：lambda
来源：http://pt.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://us.shtwfgs.cn

[S46] C++：函数模板
来源：http://hk.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ga.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://vr.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pr.lnxyls.cn

[S48] C++：逐行读文件
来源：http://wo.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fq.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://wa.huanxung.cn

[S49] C++：写文件
来源：http://su.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vd.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://hd.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dk.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://uc.colortex.cn

static_cast<double>(a) / b
来源：http://co.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://wk.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://ol.colortex.cn

[S53] C++：移动语义
来源：http://sn.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://ka.lnxyls.cn

[S54] C++：异常处理
来源：http://rr.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eb.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://xv.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nb.bjjhwx.cn

[S56] C++：optional
来源：http://vl.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dp.shtwfgs.cn

[S57] C++：编译期常量
来源：http://iw.szxytkj.cn

constexpr int N = 10;
来源：http://cf.yuexingan06.cn

[S58] C++：命名空间
来源：http://er.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://ur.muxihuayi.cn

[S59] C++：静态断言
来源：http://uu.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iw.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://th.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ie.szsharing.cn

================================================================================
来源：http://hl.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zw.nszjky.cn

================================================================================
来源：http://mp.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://wo.huixiangedu.cn

println("Hello")
来源：http://ml.szxytkj.cn

[T02] Kotlin：变量
来源：http://ve.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ve.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://nv.wgjwhj.cn

"值: $b"
来源：http://pj.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://gt.newstarts.cn

val n: String? = null;  n?.length
来源：http://di.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://jq.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://im.nicolike.cn

[T06] Kotlin：集合映射
来源：http://jy.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ih.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://mf.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fn.gzmigu.cn

[T08] Kotlin：数据类
来源：http://hy.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://tw.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://ql.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://el.szsharing.cn

[T10] Kotlin：默认参数
来源：http://vr.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cr.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://ra.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ja.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://tr.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://cx.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://lo.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://hr.haigaiapp.cn

[T14] Kotlin：循环
来源：http://at.panjiajie.cn

for (i in 1..10) println(i)
来源：http://yv.wgjwhj.cn

[T15] Kotlin：接口
来源：http://ax.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://kf.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://rv.gzmigu.cn

print("Hello")
来源：http://uu.colortex.cn

[T17] Swift：变量与常量
来源：http://oh.bjjhwx.cn

var a = 1;  let b = 2
来源：http://zk.hnjuh.cn

[T18] Swift：字符串插值
来源：http://hc.nicolike.cn

"值: \(b)"
来源：http://js.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://lq.gzmigu.cn

if let n = opt { print(n) }
来源：http://ow.521024.cn

[T20] Swift：数组操作
来源：http://tq.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://es.haigaiapp.cn

[T21] Swift：遍历
来源：http://sc.hnjuh.cn

for x in a { print(x) }
来源：http://np.wgjwhj.cn

[T22] Swift：字典
来源：http://ml.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dt.asd995.cn

[T23] Swift：函数
来源：http://yr.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tx.newstarts.cn

[T24] Swift：闭包
来源：http://oo.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xy.newstarts.cn

[T25] Swift：结构体
来源：http://mh.yuexingan06.cn

struct P { var x: Int }
来源：http://dr.gzmigu.cn

[T26] Swift：类与重写
来源：http://wp.panjiajie.cn

class A: Base { override func f() {} }
来源：http://ns.shxzukj.cn

[T27] Swift：错误处理
来源：http://tv.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://zj.9csxet.cn

[T28] Swift：枚举
来源：http://my.chemitech.net.cn

enum Color { case red, green }
来源：http://oh.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://nj.hnjuh.cn

guard let x = opt else { return }
来源：http://ix.nicolike.cn

[T30] Swift：协议
来源：http://ve.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ry.9csxet.cn

[T31] Lua：Hello World
来源：http://qp.shtwfgs.cn

print("Hello")
来源：http://gj.szxytkj.cn

[T32] Lua：局部变量
来源：http://dj.nszjky.cn

local a = 1
来源：http://vp.shxzskj.cn

[T33] Lua：表（数组）
来源：http://qi.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tr.gzmigu.cn

[T34] Lua：遍历表
来源：http://uc.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pc.colortex.cn

[T35] Lua：字典表
来源：http://mj.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://xw.newstarts.cn

[T36] Lua：函数
来源：http://cs.szsharing.cn

function add(a, b) return a + b end
来源：http://gc.521024.cn

[T37] Lua：字符串拼接
来源：http://gh.szxytkj.cn

"a" .. "b"
来源：http://bv.9csxet.cn

[T38] Lua：条件
来源：http://tu.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://vv.shxzskj.cn

[T39] Lua：模式匹配
来源：http://nc.szsharing.cn

string.find(s, "%d+")
来源：http://kj.shtwfgs.cn

[T40] Lua：元表
来源：http://aa.9csxet.cn

setmetatable({}, { __index = base })
来源：http://ot.521024.cn

[T41] Perl：Hello World
来源：http://pc.shtwfgs.cn

print "Hello\n";
来源：http://rn.shxzukj.cn

[T42] Perl：变量类型
来源：http://dd.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://js.521024.cn

[T43] Perl：字符串插值
来源：http://wu.bookmarksfly.cn

"值: $a"
来源：http://bi.jctech888.com.cn

[T44] Perl：条件
来源：http://st.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://po.nicolike.cn

[T45] Perl：数组遍历
来源：http://ha.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://jt.szsharing.cn

[T46] Perl：哈希操作
来源：http://zp.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ks.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://ou.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pp.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://ra.9csxet.cn

$s =~ s/old/new/g;
来源：http://hz.huixinmuqiang.cn

[T49] Perl：函数
来源：http://oc.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vh.newstarts.cn

[T50] Perl：逐行读文件
来源：http://wz.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mi.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://bn.chemitech.net.cn

[T51] Scala：Hello World
来源：http://sd.huixiangedu.cn

println("Hello")
来源：http://rp.shxzukj.cn

[T52] Scala：变量
来源：http://iw.newstarts.cn

val a = 1;  var b = 2
来源：http://ca.shxzukj.cn

[T53] Scala：字符串插值
来源：http://tx.hahajie.cn

s"值: $b"
来源：http://zg.yuexingan06.cn

[T54] Scala：集合映射
来源：http://dg.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://iz.9csxet.cn

[T55] Scala：集合过滤
来源：http://pk.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gy.nicolike.cn

[T56] Scala：样例类
来源：http://fk.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://el.szxytkj.cn

[T57] Scala：模式匹配
来源：http://lt.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lm.shtwfgs.cn

[T58] Scala：函数定义
来源：http://ah.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ks.lnxyls.cn

[T59] Scala：循环
来源：http://rg.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://do.521024.cn

[T60] Scala：折叠
来源：http://dt.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cu.muxihuayi.cn

================================================================================
来源：http://am.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xm.shxzskj.cn

================================================================================
来源：http://wz.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://xb.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zy.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://gt.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vx.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://vv.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dr.szxytkj.cn

[U04] Py：变量调试打印
来源：http://of.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hh.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://dc.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://gt.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://ij.haigaiapp.cn

{**a, **b}
来源：http://yg.colortex.cn

[U07] Py：反转字典键值
来源：http://hg.hahajie.cn

{v: k for k, v in d.items()}
来源：http://hz.huanxung.cn

[U08] Py：展平二维列表
来源：http://lq.yuexingan06.cn

[y for x in nested for y in x]
来源：http://md.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://mf.hnjuh.cn

max(d, key=d.get)
来源：http://id.asd995.cn

[U10] Py：按值排序字典
来源：http://sk.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tu.colortex.cn

[U11] Py：生成器表达式
来源：http://sk.panjiajie.cn

(x * 2 for x in arr)
来源：http://up.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lz.nszjky.cn

Counter(arr).most_common(3)
来源：http://ow.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://yj.gzmigu.cn

deque(maxlen=10)
来源：http://jw.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://cv.shtwfgs.cn

defaultdict(list)
来源：http://ox.asd995.cn

[U15] Py：高精度计时
来源：http://ok.hahajie.cn

t = time.perf_counter()
来源：http://gd.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://vh.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rt.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://tn.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://hd.huanxung.cn

[U18] Py：预编译正则
来源：http://tu.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://wa.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://bz.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jd.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://nt.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://pz.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://hn.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://te.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://xz.panjiajie.cn

list(zip(*m))
来源：http://ja.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://en.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ie.jctech888.com.cn

[U24] Py：路径操作
来源：http://db.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ny.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://dz.muxihuayi.cn

csv.DictReader(f)
来源：http://ll.bjjhwx.cn

[U26] Py：并发下载
来源：http://ce.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ej.colortex.cn

[U27] Py：异步 HTTP
来源：http://fh.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://za.chemitech.net.cn

[U28] Py：类型别名
来源：http://uk.huanxung.cn

UserId = int
来源：http://iv.jctech888.com.cn

[U29] Py：属性校验
来源：http://yg.nszjky.cn

@property 与 @x.setter 配合
来源：http://we.gzmigu.cn

[U30] Py：数据类
来源：http://uj.hahajie.cn

@dataclass(slots=True)
来源：http://in.hahajie.cn

[U31] Py：单测
来源：http://gm.jctech888.com.cn

python -m pytest -q
来源：http://wf.nszjky.cn

[U32] Py：代码格式化
来源：http://rv.asd995.cn

ruff format . && ruff check --fix .
来源：http://fa.newstarts.cn

[U33] Py：打包发布
来源：http://fl.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://nd.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://tb.szxytkj.cn

chardet.detect(raw)
来源：http://wq.colortex.cn

[U35] Py：发送邮件
来源：http://fb.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uv.newstarts.cn

[U36] Py：定时任务
来源：http://bo.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://gp.newstarts.cn

[U37] Py：读写 Excel
来源：http://ky.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mt.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://jl.nszjky.cn

Path(__file__).resolve().parent
来源：http://lm.521024.cn

[U39] Py：判断是否在交互环境
来源：http://ca.haigaiapp.cn

sys.stdout.isatty()
来源：http://kn.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://ap.gzmigu.cn

print("err", file=sys.stderr)
来源：http://nk.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://nu.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oq.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://zd.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lx.9csxet.cn

[U43] PHP：声明命名空间
来源：http://xe.gzmigu.cn

namespace App\Http;
来源：http://wt.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://hk.chemitech.net.cn

declare(strict_types=1);
来源：http://dw.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://wh.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ih.newstarts.cn

[U46] PHP：可空类型
来源：http://xi.yuexingan06.cn

?string $name = null
来源：http://aw.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://ac.yuexingan06.cn

int|string $id
来源：http://cf.shxzukj.cn

[U48] PHP：纯枚举
来源：http://kk.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dt.shtwfgs.cn

[U49] PHP：只读属性
来源：http://dj.yuntaijiaju.cn

public readonly string $name
来源：http://hx.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://rm.shxzskj.cn

public function __construct(private int $id) {}
来源：http://cj.muxihuayi.cn

[U51] PHP：数组解构
来源：http://gs.muxihuayi.cn

[$a, $b] = $arr;
来源：http://ua.lnxyls.cn

[U52] PHP：箭头函数
来源：http://ui.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://lv.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://dy.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://od.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://fp.9csxet.cn

$obj?->method()
来源：http://oh.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://kk.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nf.gzmigu.cn

[U56] PHP：命名参数
来源：http://zg.huixiangedu.cn

f(a: 1, b: 2)
来源：http://di.gzmigu.cn

[U57] PHP：字符串插值
来源：http://yv.asd995.cn

"值: {$a}"
来源：http://zf.asd995.cn

[U58] PHP：数组三件套
来源：http://ad.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xq.newstarts.cn

[U59] PHP：自定义排序
来源：http://sx.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vp.colortex.cn

[U60] PHP：JSON 编解码
来源：http://oc.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qb.jianghongdianzi.cn

[U61] PHP：正则
来源：http://fp.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zw.szxytkj.cn

[U62] PHP：日期对象
来源：http://lp.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://je.jctech888.com.cn


<!-- 参考信息 -->