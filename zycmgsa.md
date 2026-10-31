代发 wailian999

[S35] C++：map
来源：http://or.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ky.huixiangedu.cn

[S36] C++：unordered_map
来源：http://tc.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dn.colortex.cn

[S37] C++：set
来源：http://on.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pn.muxihuayi.cn

[S38] C++：排序
来源：http://tx.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://as.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://tx.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zg.bookmarksfly.cn

[S40] C++：查找元素
来源：http://mp.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sg.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://mi.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ph.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://ba.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://wh.szsharing.cn

[S43] C++：智能指针
来源：http://ja.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://oh.nszjky.cn

[S44] C++：引用传参
来源：http://al.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://rm.lnxyls.cn

[S45] C++：lambda
来源：http://vr.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mp.9csxet.cn

[S46] C++：函数模板
来源：http://qo.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mn.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://so.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://az.521024.cn

[S48] C++：逐行读文件
来源：http://bm.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sq.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://pp.huixiangedu.cn

[S49] C++：写文件
来源：http://mg.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ze.haigaiapp.cn

[S50] C++：格式化数字
来源：http://fv.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gt.shxzskj.cn

[S51] C++：显式类型转换
来源：http://pt.chemitech.net.cn

static_cast<double>(a) / b
来源：http://ox.colortex.cn

[S52] C++：const 与 noexcept
来源：http://rv.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://re.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://nh.colortex.cn

std::vector<int> w = std::move(v);
来源：http://xt.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://mo.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gu.szxytkj.cn

[S55] C++：结构化绑定
来源：http://fk.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gy.panjiajie.cn

[S56] C++：optional
来源：http://np.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hg.huanxung.cn

[S57] C++：编译期常量
来源：http://ol.newstarts.cn

constexpr int N = 10;
来源：http://ar.asd995.cn

[S58] C++：命名空间
来源：http://pr.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://kf.huanxung.cn

[S59] C++：静态断言
来源：http://it.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://id.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://yj.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hv.yuexingan06.cn

================================================================================
来源：http://ht.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ka.shxzskj.cn

================================================================================
来源：http://yc.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://kg.521024.cn

println("Hello")
来源：http://td.wgjwhj.cn

[T02] Kotlin：变量
来源：http://jb.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jy.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ze.yuntaijiaju.cn

"值: $b"
来源：http://vd.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://nd.lnxyls.cn

val n: String? = null;  n?.length
来源：http://dr.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://pd.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uy.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://rs.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ee.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ut.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mt.asd995.cn

[T08] Kotlin：数据类
来源：http://tf.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://he.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://do.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://wl.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://dc.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pt.yuexingan06.cn

[T11] Kotlin：协程
来源：http://gc.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bi.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://ij.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://hw.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://ua.szsharing.cn

val m = mapOf("a" to 1)
来源：http://yw.huixiangedu.cn

[T14] Kotlin：循环
来源：http://pv.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://gh.chemitech.net.cn

[T15] Kotlin：接口
来源：http://lj.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://qq.nicolike.cn

[T16] Swift：Hello World
来源：http://mk.yuexingan06.cn

print("Hello")
来源：http://vq.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://jo.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://vk.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://cu.hnjuh.cn

"值: \(b)"
来源：http://yg.asd995.cn

[T19] Swift：可选绑定
来源：http://ss.colortex.cn

if let n = opt { print(n) }
来源：http://bg.lnxyls.cn

[T20] Swift：数组操作
来源：http://cs.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xb.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://qk.bjjhwx.cn

for x in a { print(x) }
来源：http://nd.huanxung.cn

[T22] Swift：字典
来源：http://zf.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ei.shtwfgs.cn

[T23] Swift：函数
来源：http://hj.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vj.lnxyls.cn

[T24] Swift：闭包
来源：http://lw.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oy.nicolike.cn

[T25] Swift：结构体
来源：http://lt.panjiajie.cn

struct P { var x: Int }
来源：http://zg.gzmigu.cn

[T26] Swift：类与重写
来源：http://kz.shxzukj.cn

class A: Base { override func f() {} }
来源：http://se.521024.cn

[T27] Swift：错误处理
来源：http://cn.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://le.gzmigu.cn

[T28] Swift：枚举
来源：http://xp.521024.cn

enum Color { case red, green }
来源：http://we.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://ut.yuexingan06.cn

guard let x = opt else { return }
来源：http://nw.9csxet.cn

[T30] Swift：协议
来源：http://ck.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://tf.huixiangedu.cn

[T31] Lua：Hello World
来源：http://hy.asd995.cn

print("Hello")
来源：http://wq.chemitech.net.cn

[T32] Lua：局部变量
来源：http://gr.panjiajie.cn

local a = 1
来源：http://rv.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://wz.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rx.521024.cn

[T34] Lua：遍历表
来源：http://av.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ir.newstarts.cn

[T35] Lua：字典表
来源：http://br.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://yr.hahajie.cn

[T36] Lua：函数
来源：http://gf.panjiajie.cn

function add(a, b) return a + b end
来源：http://ho.szsharing.cn

[T37] Lua：字符串拼接
来源：http://ij.panjiajie.cn

"a" .. "b"
来源：http://pn.yuexingan06.cn

[T38] Lua：条件
来源：http://ih.521024.cn

if x > 0 then print("正") end
来源：http://fn.hnjuh.cn

[T39] Lua：模式匹配
来源：http://gi.521024.cn

string.find(s, "%d+")
来源：http://fe.asd995.cn

[T40] Lua：元表
来源：http://fs.newstarts.cn

setmetatable({}, { __index = base })
来源：http://jr.asd995.cn

[T41] Perl：Hello World
来源：http://wh.bjjhwx.cn

print "Hello\n";
来源：http://sa.yuexingan06.cn

[T42] Perl：变量类型
来源：http://ls.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ya.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://ox.nszjky.cn

"值: $a"
来源：http://ao.huanxung.cn

[T44] Perl：条件
来源：http://pr.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://iu.nicolike.cn

[T45] Perl：数组遍历
来源：http://fg.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://sr.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://pr.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fs.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://fg.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ox.muxihuayi.cn

[T48] Perl：正则替换
来源：http://vo.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://xm.asd995.cn

[T49] Perl：函数
来源：http://pz.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zo.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://iw.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ey.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://vi.panjiajie.cn

[T51] Scala：Hello World
来源：http://od.hahajie.cn

println("Hello")
来源：http://ws.szsharing.cn

[T52] Scala：变量
来源：http://xk.newstarts.cn

val a = 1;  var b = 2
来源：http://lj.nicolike.cn

[T53] Scala：字符串插值
来源：http://vq.shtwfgs.cn

s"值: $b"
来源：http://uw.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://jl.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://qw.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://jy.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oj.panjiajie.cn

[T56] Scala：样例类
来源：http://mq.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://lk.nszjky.cn

[T57] Scala：模式匹配
来源：http://ji.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gd.huanxung.cn

[T58] Scala：函数定义
来源：http://hp.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uz.hahajie.cn

[T59] Scala：循环
来源：http://pg.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ex.colortex.cn

[T60] Scala：折叠
来源：http://xb.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tw.9csxet.cn

================================================================================
来源：http://jp.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pr.jianghongdianzi.cn

================================================================================
来源：http://kj.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://xa.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://op.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://aq.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jl.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://uc.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jf.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://qe.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qx.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://sr.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://iy.gzmigu.cn

[U06] Py：合并两个字典
来源：http://cb.newstarts.cn

{**a, **b}
来源：http://fj.gzmigu.cn

[U07] Py：反转字典键值
来源：http://uv.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://nk.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://da.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://bz.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://cb.hahajie.cn

max(d, key=d.get)
来源：http://ft.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://lh.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rk.szsharing.cn

[U11] Py：生成器表达式
来源：http://gm.hnjuh.cn

(x * 2 for x in arr)
来源：http://if.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mv.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://rc.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://yz.asd995.cn

deque(maxlen=10)
来源：http://ce.newstarts.cn

[U14] Py：分组收集到列表
来源：http://io.hnjuh.cn

defaultdict(list)
来源：http://mr.hnjuh.cn

[U15] Py：高精度计时
来源：http://vi.jctech888.com.cn

t = time.perf_counter()
来源：http://dl.521024.cn

[U16] Py：命令行参数解析
来源：http://ks.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bi.hahajie.cn

[U17] Py：初始化日志
来源：http://aw.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://id.colortex.cn

[U18] Py：预编译正则
来源：http://ve.nicolike.cn

pat = re.compile(r"\d+")
来源：http://zr.nicolike.cn

[U19] Py：正则替换带回调
来源：http://sx.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sr.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://gi.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://dd.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://jd.9csxet.cn

@contextlib.contextmanager
来源：http://tc.szsharing.cn

[U22] Py：矩阵转置
来源：http://ij.lnxyls.cn

list(zip(*m))
来源：http://xi.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://qb.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tc.asd995.cn

[U24] Py：路径操作
来源：http://zb.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pz.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://tr.bookmarksfly.cn

csv.DictReader(f)
来源：http://ub.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://li.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kx.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://lg.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://fb.hahajie.cn

[U28] Py：类型别名
来源：http://is.gzmigu.cn

UserId = int
来源：http://gu.bjjhwx.cn

[U29] Py：属性校验
来源：http://mr.shxzskj.cn

@property 与 @x.setter 配合
来源：http://lb.haigaiapp.cn

[U30] Py：数据类
来源：http://oe.nszjky.cn

@dataclass(slots=True)
来源：http://ka.huixinmuqiang.cn

[U31] Py：单测
来源：http://by.nicolike.cn

python -m pytest -q
来源：http://ro.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://ju.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://ey.panjiajie.cn

[U33] Py：打包发布
来源：http://ob.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://wr.nicolike.cn

[U34] Py：判断编码
来源：http://ws.szsharing.cn

chardet.detect(raw)
来源：http://za.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://gg.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sz.panjiajie.cn

[U36] Py：定时任务
来源：http://zr.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://jr.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://jt.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iw.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://ij.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://fb.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://kg.lnxyls.cn

sys.stdout.isatty()
来源：http://nf.asd995.cn

[U40] Py：打印到标准错误
来源：http://fl.huanxung.cn

print("err", file=sys.stderr)
来源：http://fh.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://dd.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ns.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://fn.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tf.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://gz.shxzskj.cn

namespace App\Http;
来源：http://vn.521024.cn

[U44] PHP：开启严格类型
来源：http://ty.haigaiapp.cn

declare(strict_types=1);
来源：http://gw.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://xn.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aj.hnjuh.cn

[U46] PHP：可空类型
来源：http://hl.hahajie.cn

?string $name = null
来源：http://bv.9csxet.cn

[U47] PHP：联合类型
来源：http://gr.colortex.cn

int|string $id
来源：http://mk.nszjky.cn

[U48] PHP：纯枚举
来源：http://ur.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xa.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://us.bookmarksfly.cn

public readonly string $name
来源：http://yb.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://uq.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://qf.jctech888.com.cn

[U51] PHP：数组解构
来源：http://wu.szxytkj.cn

[$a, $b] = $arr;
来源：http://ap.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://qi.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://er.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://wj.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ko.newstarts.cn

[U54] PHP：空安全调用
来源：http://ff.jianghongdianzi.cn

$obj?->method()
来源：http://ou.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ip.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hq.szsharing.cn

[U56] PHP：命名参数
来源：http://gc.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://sb.hahajie.cn

[U57] PHP：字符串插值
来源：http://wz.shxzskj.cn

"值: {$a}"
来源：http://jc.colortex.cn

[U58] PHP：数组三件套
来源：http://ks.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tk.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://ao.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dg.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://kp.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bd.nicolike.cn


<!-- 参考信息 -->