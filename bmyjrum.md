代发 wailian999

[S41] C++：类与构造函数
来源：http://ff.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zv.newstarts.cn

[S42] C++：继承与虚函数
来源：http://db.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ce.bjjhwx.cn

[S43] C++：智能指针
来源：http://rl.521024.cn

auto p = std::make_unique<int>(5);
来源：http://pn.bjjhwx.cn

[S44] C++：引用传参
来源：http://ox.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://gn.nicolike.cn

[S45] C++：lambda
来源：http://vx.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zk.nicolike.cn

[S46] C++：函数模板
来源：http://lr.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iv.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ad.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qi.panjiajie.cn

[S48] C++：逐行读文件
来源：http://hy.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pb.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://yr.bjjhwx.cn

[S49] C++：写文件
来源：http://xm.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ko.shxzskj.cn

[S50] C++：格式化数字
来源：http://dv.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qd.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://az.lnxyls.cn

static_cast<double>(a) / b
来源：http://wt.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://vh.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://ma.colortex.cn

[S53] C++：移动语义
来源：http://uy.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://hw.hnjuh.cn

[S54] C++：异常处理
来源：http://yh.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jm.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://rd.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zp.haigaiapp.cn

[S56] C++：optional
来源：http://md.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kf.newstarts.cn

[S57] C++：编译期常量
来源：http://vl.szsharing.cn

constexpr int N = 10;
来源：http://vh.panjiajie.cn

[S58] C++：命名空间
来源：http://gz.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://iz.wgjwhj.cn

[S59] C++：静态断言
来源：http://jl.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kx.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://rn.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://at.jianghongdianzi.cn

================================================================================
来源：http://pn.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vo.gzmigu.cn

================================================================================
来源：http://qy.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://fo.huixiangedu.cn

println("Hello")
来源：http://qk.nicolike.cn

[T02] Kotlin：变量
来源：http://zr.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sv.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://ce.yuexingan06.cn

"值: $b"
来源：http://gb.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://sa.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://hm.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://xh.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jk.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://vm.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dx.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://iu.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qp.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://hp.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://gm.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://fm.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://zy.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://dc.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hu.chemitech.net.cn

[T11] Kotlin：协程
来源：http://hp.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uf.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://ki.521024.cn

val (a, b) = Pair(1, 2)
来源：http://ln.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://yn.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ii.newstarts.cn

[T14] Kotlin：循环
来源：http://so.asd995.cn

for (i in 1..10) println(i)
来源：http://nc.lnxyls.cn

[T15] Kotlin：接口
来源：http://yf.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://am.panjiajie.cn

[T16] Swift：Hello World
来源：http://eh.gzmigu.cn

print("Hello")
来源：http://xj.hnjuh.cn

[T17] Swift：变量与常量
来源：http://rb.asd995.cn

var a = 1;  let b = 2
来源：http://rr.szsharing.cn

[T18] Swift：字符串插值
来源：http://jj.huixinmuqiang.cn

"值: \(b)"
来源：http://cu.hahajie.cn

[T19] Swift：可选绑定
来源：http://gm.hahajie.cn

if let n = opt { print(n) }
来源：http://pi.huixiangedu.cn

[T20] Swift：数组操作
来源：http://mt.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jj.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://gy.521024.cn

for x in a { print(x) }
来源：http://bd.huanxung.cn

[T22] Swift：字典
来源：http://us.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wn.asd995.cn

[T23] Swift：函数
来源：http://co.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ko.muxihuayi.cn

[T24] Swift：闭包
来源：http://bp.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dk.asd995.cn

[T25] Swift：结构体
来源：http://ry.haigaiapp.cn

struct P { var x: Int }
来源：http://sa.hahajie.cn

[T26] Swift：类与重写
来源：http://kp.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://bt.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://dx.newstarts.cn

do { try f() } catch { print(error) }
来源：http://vz.panjiajie.cn

[T28] Swift：枚举
来源：http://ut.newstarts.cn

enum Color { case red, green }
来源：http://rc.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://nn.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://ut.shxzukj.cn

[T30] Swift：协议
来源：http://oa.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://do.shtwfgs.cn

[T31] Lua：Hello World
来源：http://av.colortex.cn

print("Hello")
来源：http://is.wgjwhj.cn

[T32] Lua：局部变量
来源：http://fp.shxzskj.cn

local a = 1
来源：http://um.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://gs.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gg.hnjuh.cn

[T34] Lua：遍历表
来源：http://bb.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vi.shtwfgs.cn

[T35] Lua：字典表
来源：http://cy.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://dn.nicolike.cn

[T36] Lua：函数
来源：http://at.asd995.cn

function add(a, b) return a + b end
来源：http://dg.hahajie.cn

[T37] Lua：字符串拼接
来源：http://oe.bookmarksfly.cn

"a" .. "b"
来源：http://qd.chemitech.net.cn

[T38] Lua：条件
来源：http://cu.newstarts.cn

if x > 0 then print("正") end
来源：http://oq.newstarts.cn

[T39] Lua：模式匹配
来源：http://in.shxzskj.cn

string.find(s, "%d+")
来源：http://ts.shtwfgs.cn

[T40] Lua：元表
来源：http://ab.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://oa.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://ya.asd995.cn

print "Hello\n";
来源：http://ei.yuexingan06.cn

[T42] Perl：变量类型
来源：http://ed.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bu.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ei.hnjuh.cn

"值: $a"
来源：http://hn.shxzukj.cn

[T44] Perl：条件
来源：http://al.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://pd.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://xr.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://ir.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ju.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://er.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://vo.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xj.huanxung.cn

[T48] Perl：正则替换
来源：http://cn.521024.cn

$s =~ s/old/new/g;
来源：http://zv.9csxet.cn

[T49] Perl：函数
来源：http://yl.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://um.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://ij.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fq.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://np.gzmigu.cn

[T51] Scala：Hello World
来源：http://rc.haigaiapp.cn

println("Hello")
来源：http://mi.jctech888.com.cn

[T52] Scala：变量
来源：http://oq.shtwfgs.cn

val a = 1;  var b = 2
来源：http://hw.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://ki.shxzukj.cn

s"值: $b"
来源：http://bj.9csxet.cn

[T54] Scala：集合映射
来源：http://hh.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://jk.colortex.cn

[T55] Scala：集合过滤
来源：http://fh.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ry.hahajie.cn

[T56] Scala：样例类
来源：http://at.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://bn.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://jz.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ox.panjiajie.cn

[T58] Scala：函数定义
来源：http://sj.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jo.jianghongdianzi.cn

[T59] Scala：循环
来源：http://ip.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://zk.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://nv.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cs.wgjwhj.cn

================================================================================
来源：http://jz.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pj.bookmarksfly.cn

================================================================================
来源：http://ci.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://zs.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tz.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://in.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ik.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://li.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jl.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://cz.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ge.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://ne.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://zl.shxzukj.cn

[U06] Py：合并两个字典
来源：http://lx.asd995.cn

{**a, **b}
来源：http://ou.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://qo.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://fm.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://ia.chemitech.net.cn

[y for x in nested for y in x]
来源：http://tl.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://mr.muxihuayi.cn

max(d, key=d.get)
来源：http://if.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ax.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yp.shxzskj.cn

[U11] Py：生成器表达式
来源：http://ma.hnjuh.cn

(x * 2 for x in arr)
来源：http://hg.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cm.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://lx.nszjky.cn

[U13] Py：固定长度队列
来源：http://nv.nicolike.cn

deque(maxlen=10)
来源：http://wa.szsharing.cn

[U14] Py：分组收集到列表
来源：http://cs.jctech888.com.cn

defaultdict(list)
来源：http://zk.shxzukj.cn

[U15] Py：高精度计时
来源：http://mk.huixinmuqiang.cn

t = time.perf_counter()
来源：http://dp.asd995.cn

[U16] Py：命令行参数解析
来源：http://ie.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wm.9csxet.cn

[U17] Py：初始化日志
来源：http://au.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://sq.szxytkj.cn

[U18] Py：预编译正则
来源：http://as.newstarts.cn

pat = re.compile(r"\d+")
来源：http://pa.nszjky.cn

[U19] Py：正则替换带回调
来源：http://fu.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ea.huanxung.cn

[U20] Py：缓存函数结果
来源：http://ee.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://yn.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://dz.shxzskj.cn

@contextlib.contextmanager
来源：http://bv.panjiajie.cn

[U22] Py：矩阵转置
来源：http://oa.lnxyls.cn

list(zip(*m))
来源：http://oq.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://gm.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xh.huixiangedu.cn

[U24] Py：路径操作
来源：http://ci.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lm.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://gm.hnjuh.cn

csv.DictReader(f)
来源：http://wp.szsharing.cn

[U26] Py：并发下载
来源：http://dr.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rt.521024.cn

[U27] Py：异步 HTTP
来源：http://yr.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://rz.521024.cn

[U28] Py：类型别名
来源：http://ec.colortex.cn

UserId = int
来源：http://kt.9csxet.cn

[U29] Py：属性校验
来源：http://zo.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://fj.muxihuayi.cn

[U30] Py：数据类
来源：http://ez.yuexingan06.cn

@dataclass(slots=True)
来源：http://te.yuexingan06.cn

[U31] Py：单测
来源：http://qz.newstarts.cn

python -m pytest -q
来源：http://uu.shxzukj.cn

[U32] Py：代码格式化
来源：http://eo.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://he.hnjuh.cn

[U33] Py：打包发布
来源：http://np.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://ry.bjjhwx.cn

[U34] Py：判断编码
来源：http://so.haigaiapp.cn

chardet.detect(raw)
来源：http://yk.haigaiapp.cn

[U35] Py：发送邮件
来源：http://nw.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qs.haigaiapp.cn

[U36] Py：定时任务
来源：http://xf.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://cj.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://qu.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qj.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://iw.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://qf.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://jf.wgjwhj.cn

sys.stdout.isatty()
来源：http://vh.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://sp.szsharing.cn

print("err", file=sys.stderr)
来源：http://bc.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://ig.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gy.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://me.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gc.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://fh.nicolike.cn

namespace App\Http;
来源：http://is.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://hy.colortex.cn

declare(strict_types=1);
来源：http://ge.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://co.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tt.chemitech.net.cn

[U46] PHP：可空类型
来源：http://mm.panjiajie.cn

?string $name = null
来源：http://vq.chemitech.net.cn

[U47] PHP：联合类型
来源：http://rn.huixinmuqiang.cn

int|string $id
来源：http://wz.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://wm.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rd.bjjhwx.cn

[U49] PHP：只读属性
来源：http://zu.jianghongdianzi.cn

public readonly string $name
来源：http://lv.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://dk.521024.cn

public function __construct(private int $id) {}
来源：http://kv.nicolike.cn

[U51] PHP：数组解构
来源：http://fi.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://cm.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://tp.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://gn.newstarts.cn

[U53] PHP：空合并运算符
来源：http://eb.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://pa.asd995.cn

[U54] PHP：空安全调用
来源：http://fu.haigaiapp.cn

$obj?->method()
来源：http://ee.hahajie.cn

[U55] PHP：match 表达式
来源：http://tr.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xi.yuexingan06.cn

[U56] PHP：命名参数
来源：http://wo.shxzukj.cn

f(a: 1, b: 2)
来源：http://ue.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://zt.9csxet.cn

"值: {$a}"
来源：http://bw.colortex.cn

[U58] PHP：数组三件套
来源：http://rg.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nz.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://ry.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pg.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://jb.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vt.newstarts.cn

[U61] PHP：正则
来源：http://ty.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://di.haigaiapp.cn

[U62] PHP：日期对象
来源：http://cd.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uo.huanxung.cn

[U63] PHP：文件读写
来源：http://jn.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://if.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://gt.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://px.szsharing.cn

[U65] PHP：会话
来源：http://oj.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dp.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://gr.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gu.hnjuh.cn


<!-- 参考信息 -->