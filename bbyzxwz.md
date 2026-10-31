代发 wailian999

[S37] C++：set
来源：http://br.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tc.nicolike.cn

[S38] C++：排序
来源：http://rh.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://gq.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://lj.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rm.asd995.cn

[S40] C++：查找元素
来源：http://sw.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ma.colortex.cn

[S41] C++：类与构造函数
来源：http://tk.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ep.newstarts.cn

[S42] C++：继承与虚函数
来源：http://lh.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://rw.yuexingan06.cn

[S43] C++：智能指针
来源：http://yx.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://nh.nszjky.cn

[S44] C++：引用传参
来源：http://cz.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://jr.bookmarksfly.cn

[S45] C++：lambda
来源：http://ox.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hf.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://yl.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tw.521024.cn

[S47] C++：结构化绑定遍历
来源：http://aa.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ve.nicolike.cn

[S48] C++：逐行读文件
来源：http://uw.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mn.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://xg.panjiajie.cn

[S49] C++：写文件
来源：http://eg.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hw.newstarts.cn

[S50] C++：格式化数字
来源：http://du.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vn.nicolike.cn

[S51] C++：显式类型转换
来源：http://vn.hahajie.cn

static_cast<double>(a) / b
来源：http://jb.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://gg.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://yw.521024.cn

[S53] C++：移动语义
来源：http://vu.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://qz.szsharing.cn

[S54] C++：异常处理
来源：http://og.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ch.shxzskj.cn

[S55] C++：结构化绑定
来源：http://cu.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sf.gzmigu.cn

[S56] C++：optional
来源：http://aw.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rs.haigaiapp.cn

[S57] C++：编译期常量
来源：http://ss.szxytkj.cn

constexpr int N = 10;
来源：http://vp.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://jb.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://pb.nszjky.cn

[S59] C++：静态断言
来源：http://io.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zn.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://di.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yb.9csxet.cn

================================================================================
来源：http://xi.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gq.shxzskj.cn

================================================================================
来源：http://gd.521024.cn

[T01] Kotlin：Hello World
来源：http://rv.huanxung.cn

println("Hello")
来源：http://tx.huixiangedu.cn

[T02] Kotlin：变量
来源：http://yo.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ha.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://cq.szxytkj.cn

"值: $b"
来源：http://no.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://dd.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://tq.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://ro.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hf.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ft.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hi.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://yz.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nf.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://tf.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://xk.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://bs.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://cw.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://jr.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://so.nicolike.cn

[T11] Kotlin：协程
来源：http://gn.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ly.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://nq.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://jh.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://rw.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://hx.szxytkj.cn

[T14] Kotlin：循环
来源：http://ip.shxzskj.cn

for (i in 1..10) println(i)
来源：http://af.szxytkj.cn

[T15] Kotlin：接口
来源：http://dm.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ov.hahajie.cn

[T16] Swift：Hello World
来源：http://aj.haigaiapp.cn

print("Hello")
来源：http://xk.521024.cn

[T17] Swift：变量与常量
来源：http://be.yuexingan06.cn

var a = 1;  let b = 2
来源：http://qk.szsharing.cn

[T18] Swift：字符串插值
来源：http://ze.hahajie.cn

"值: \(b)"
来源：http://wh.521024.cn

[T19] Swift：可选绑定
来源：http://sp.haigaiapp.cn

if let n = opt { print(n) }
来源：http://ja.hnjuh.cn

[T20] Swift：数组操作
来源：http://ul.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tb.hahajie.cn

[T21] Swift：遍历
来源：http://wj.szxytkj.cn

for x in a { print(x) }
来源：http://wn.hnjuh.cn

[T22] Swift：字典
来源：http://kn.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://th.bookmarksfly.cn

[T23] Swift：函数
来源：http://bb.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uw.bjjhwx.cn

[T24] Swift：闭包
来源：http://cc.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sp.szxytkj.cn

[T25] Swift：结构体
来源：http://iu.huanxung.cn

struct P { var x: Int }
来源：http://tg.haigaiapp.cn

[T26] Swift：类与重写
来源：http://wh.9csxet.cn

class A: Base { override func f() {} }
来源：http://xb.wgjwhj.cn

[T27] Swift：错误处理
来源：http://ke.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://lh.lnxyls.cn

[T28] Swift：枚举
来源：http://xr.9csxet.cn

enum Color { case red, green }
来源：http://zo.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://mk.shxzskj.cn

guard let x = opt else { return }
来源：http://ju.jianghongdianzi.cn

[T30] Swift：协议
来源：http://go.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://yg.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://qt.haigaiapp.cn

print("Hello")
来源：http://cy.shtwfgs.cn

[T32] Lua：局部变量
来源：http://tt.nszjky.cn

local a = 1
来源：http://ne.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://sa.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lu.jctech888.com.cn

[T34] Lua：遍历表
来源：http://zc.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ra.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://nx.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://nv.huanxung.cn

[T36] Lua：函数
来源：http://xu.shxzskj.cn

function add(a, b) return a + b end
来源：http://ee.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://wj.huixinmuqiang.cn

"a" .. "b"
来源：http://iy.jianghongdianzi.cn

[T38] Lua：条件
来源：http://od.shtwfgs.cn

if x > 0 then print("正") end
来源：http://cj.shxzskj.cn

[T39] Lua：模式匹配
来源：http://fl.chemitech.net.cn

string.find(s, "%d+")
来源：http://fa.jctech888.com.cn

[T40] Lua：元表
来源：http://ex.521024.cn

setmetatable({}, { __index = base })
来源：http://gv.shxzskj.cn

[T41] Perl：Hello World
来源：http://cj.muxihuayi.cn

print "Hello\n";
来源：http://jy.nszjky.cn

[T42] Perl：变量类型
来源：http://tw.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lz.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://kb.huixiangedu.cn

"值: $a"
来源：http://mm.hnjuh.cn

[T44] Perl：条件
来源：http://vx.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://hx.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://qz.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://lj.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://tn.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bc.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://mg.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wm.hahajie.cn

[T48] Perl：正则替换
来源：http://we.panjiajie.cn

$s =~ s/old/new/g;
来源：http://lq.jctech888.com.cn

[T49] Perl：函数
来源：http://yc.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://db.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://gq.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://di.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://om.huanxung.cn

[T51] Scala：Hello World
来源：http://ws.521024.cn

println("Hello")
来源：http://ku.lnxyls.cn

[T52] Scala：变量
来源：http://ot.nszjky.cn

val a = 1;  var b = 2
来源：http://zj.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ue.nszjky.cn

s"值: $b"
来源：http://dr.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://rc.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://rb.lnxyls.cn

[T55] Scala：集合过滤
来源：http://ps.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jr.panjiajie.cn

[T56] Scala：样例类
来源：http://tf.shxzukj.cn

case class User(name: String, age: Int)
来源：http://xy.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://ns.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bw.muxihuayi.cn

[T58] Scala：函数定义
来源：http://pl.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nm.newstarts.cn

[T59] Scala：循环
来源：http://ub.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://rz.yuexingan06.cn

[T60] Scala：折叠
来源：http://az.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ej.szxytkj.cn

================================================================================
来源：http://ul.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lz.szxytkj.cn

================================================================================
来源：http://lb.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://cv.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ua.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://hx.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eo.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://ob.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ov.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://tt.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://au.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://yk.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://un.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://mi.hnjuh.cn

{**a, **b}
来源：http://ic.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://hl.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://tt.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://yn.nicolike.cn

[y for x in nested for y in x]
来源：http://au.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://qa.hnjuh.cn

max(d, key=d.get)
来源：http://yz.hahajie.cn

[U10] Py：按值排序字典
来源：http://wj.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ni.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://xd.yuexingan06.cn

(x * 2 for x in arr)
来源：http://aq.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://if.colortex.cn

Counter(arr).most_common(3)
来源：http://zk.shxzskj.cn

[U13] Py：固定长度队列
来源：http://qx.huixiangedu.cn

deque(maxlen=10)
来源：http://be.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://ls.huanxung.cn

defaultdict(list)
来源：http://tc.nicolike.cn

[U15] Py：高精度计时
来源：http://bi.shxzukj.cn

t = time.perf_counter()
来源：http://ty.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://ow.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yj.huanxung.cn

[U17] Py：初始化日志
来源：http://at.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://cb.szsharing.cn

[U18] Py：预编译正则
来源：http://cx.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://du.huanxung.cn

[U19] Py：正则替换带回调
来源：http://hk.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pr.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://bx.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://xr.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://id.bjjhwx.cn

@contextlib.contextmanager
来源：http://im.panjiajie.cn

[U22] Py：矩阵转置
来源：http://yy.nszjky.cn

list(zip(*m))
来源：http://sq.9csxet.cn

[U23] Py：分块读取大文件
来源：http://wb.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vo.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://oj.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://db.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://pk.shxzukj.cn

csv.DictReader(f)
来源：http://wo.hnjuh.cn

[U26] Py：并发下载
来源：http://qb.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uy.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://zp.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://as.asd995.cn

[U28] Py：类型别名
来源：http://cg.yuexingan06.cn

UserId = int
来源：http://jj.nszjky.cn

[U29] Py：属性校验
来源：http://ad.shxzukj.cn

@property 与 @x.setter 配合
来源：http://cs.huixinmuqiang.cn

[U30] Py：数据类
来源：http://mx.bjjhwx.cn

@dataclass(slots=True)
来源：http://sb.huixiangedu.cn

[U31] Py：单测
来源：http://gm.jianghongdianzi.cn

python -m pytest -q
来源：http://aa.shtwfgs.cn

[U32] Py：代码格式化
来源：http://kj.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://bw.yuexingan06.cn

[U33] Py：打包发布
来源：http://yk.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://md.szsharing.cn

[U34] Py：判断编码
来源：http://yy.huanxung.cn

chardet.detect(raw)
来源：http://cr.nicolike.cn

[U35] Py：发送邮件
来源：http://jd.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cp.bjjhwx.cn

[U36] Py：定时任务
来源：http://rr.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://pk.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://bh.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ye.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://rw.szsharing.cn

Path(__file__).resolve().parent
来源：http://yr.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://wc.huixiangedu.cn

sys.stdout.isatty()
来源：http://bz.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://lc.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://hj.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ho.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://um.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ni.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rl.huanxung.cn

[U43] PHP：声明命名空间
来源：http://lw.huixinmuqiang.cn

namespace App\Http;
来源：http://qs.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://wf.nszjky.cn

declare(strict_types=1);
来源：http://sd.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://zw.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.szxytkj.cn

[U46] PHP：可空类型
来源：http://fk.gzmigu.cn

?string $name = null
来源：http://eq.jctech888.com.cn

[U47] PHP：联合类型
来源：http://vp.chemitech.net.cn

int|string $id
来源：http://ux.szxytkj.cn

[U48] PHP：纯枚举
来源：http://tc.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dy.bjjhwx.cn

[U49] PHP：只读属性
来源：http://ik.yuntaijiaju.cn

public readonly string $name
来源：http://rz.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://bp.521024.cn

public function __construct(private int $id) {}
来源：http://xm.szxytkj.cn

[U51] PHP：数组解构
来源：http://st.shxzskj.cn

[$a, $b] = $arr;
来源：http://tt.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://gt.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://ib.521024.cn

[U53] PHP：空合并运算符
来源：http://ed.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://hi.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://xh.yuexingan06.cn

$obj?->method()
来源：http://ie.521024.cn

[U55] PHP：match 表达式
来源：http://ld.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xp.jctech888.com.cn

[U56] PHP：命名参数
来源：http://ny.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://wq.panjiajie.cn

[U57] PHP：字符串插值
来源：http://va.jctech888.com.cn

"值: {$a}"
来源：http://to.hnjuh.cn

[U58] PHP：数组三件套
来源：http://aw.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mf.hahajie.cn

[U59] PHP：自定义排序
来源：http://xb.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ln.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://fw.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://va.shxzskj.cn

[U61] PHP：正则
来源：http://ld.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gs.colortex.cn

[U62] PHP：日期对象
来源：http://yz.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wp.nszjky.cn


<!-- 参考信息 -->