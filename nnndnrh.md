代发 wailian999

[S33] C++：vector 增删
来源：http://sm.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gk.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://jh.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ba.hnjuh.cn

[S35] C++：map
来源：http://vq.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zi.nicolike.cn

[S36] C++：unordered_map
来源：http://cu.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.muxihuayi.cn

[S37] C++：set
来源：http://um.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ob.newstarts.cn

[S38] C++：排序
来源：http://ve.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://qu.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://uh.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xl.asd995.cn

[S40] C++：查找元素
来源：http://qv.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rx.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://bt.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mp.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://ji.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://he.haigaiapp.cn

[S43] C++：智能指针
来源：http://bw.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://nk.haigaiapp.cn

[S44] C++：引用传参
来源：http://wl.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://xi.hahajie.cn

[S45] C++：lambda
来源：http://bi.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://th.hnjuh.cn

[S46] C++：函数模板
来源：http://gv.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://um.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://kp.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pv.szsharing.cn

[S48] C++：逐行读文件
来源：http://un.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://al.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://zb.shtwfgs.cn

[S49] C++：写文件
来源：http://ix.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cv.hahajie.cn

[S50] C++：格式化数字
来源：http://hj.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ro.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://ha.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://mp.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://yx.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://uz.huanxung.cn

[S53] C++：移动语义
来源：http://vq.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://qx.yuexingan06.cn

[S54] C++：异常处理
来源：http://sb.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tq.nszjky.cn

[S55] C++：结构化绑定
来源：http://bl.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yi.shxzskj.cn

[S56] C++：optional
来源：http://ms.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mq.szxytkj.cn

[S57] C++：编译期常量
来源：http://te.szxytkj.cn

constexpr int N = 10;
来源：http://uq.shxzskj.cn

[S58] C++：命名空间
来源：http://iz.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://as.huixiangedu.cn

[S59] C++：静态断言
来源：http://dr.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ix.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://th.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kv.szsharing.cn

================================================================================
来源：http://rj.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aa.chemitech.net.cn

================================================================================
来源：http://xc.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://jo.521024.cn

println("Hello")
来源：http://hp.newstarts.cn

[T02] Kotlin：变量
来源：http://wl.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eq.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://gt.9csxet.cn

"值: $b"
来源：http://zi.colortex.cn

[T04] Kotlin：空安全
来源：http://ss.szxytkj.cn

val n: String? = null;  n?.length
来源：http://cl.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://cs.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ij.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://qw.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://be.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ze.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bw.szxytkj.cn

[T08] Kotlin：数据类
来源：http://gs.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://oa.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://va.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://ys.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://cg.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sn.hnjuh.cn

[T11] Kotlin：协程
来源：http://mu.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oz.nszjky.cn

[T12] Kotlin：解构声明
来源：http://mp.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://ch.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://gx.huanxung.cn

val m = mapOf("a" to 1)
来源：http://eg.newstarts.cn

[T14] Kotlin：循环
来源：http://sk.szxytkj.cn

for (i in 1..10) println(i)
来源：http://ed.huixiangedu.cn

[T15] Kotlin：接口
来源：http://ji.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://to.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://wg.shtwfgs.cn

print("Hello")
来源：http://kx.huanxung.cn

[T17] Swift：变量与常量
来源：http://hb.521024.cn

var a = 1;  let b = 2
来源：http://vr.shxzskj.cn

[T18] Swift：字符串插值
来源：http://fi.lnxyls.cn

"值: \(b)"
来源：http://oi.9csxet.cn

[T19] Swift：可选绑定
来源：http://mn.shtwfgs.cn

if let n = opt { print(n) }
来源：http://gb.shxzukj.cn

[T20] Swift：数组操作
来源：http://fw.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zx.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://dz.jianghongdianzi.cn

for x in a { print(x) }
来源：http://pr.huanxung.cn

[T22] Swift：字典
来源：http://kb.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qd.jctech888.com.cn

[T23] Swift：函数
来源：http://bq.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jn.chemitech.net.cn

[T24] Swift：闭包
来源：http://qf.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cz.shxzukj.cn

[T25] Swift：结构体
来源：http://hg.huixinmuqiang.cn

struct P { var x: Int }
来源：http://yn.nszjky.cn

[T26] Swift：类与重写
来源：http://yq.nszjky.cn

class A: Base { override func f() {} }
来源：http://jc.colortex.cn

[T27] Swift：错误处理
来源：http://ul.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://eb.chemitech.net.cn

[T28] Swift：枚举
来源：http://ne.wgjwhj.cn

enum Color { case red, green }
来源：http://yy.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://se.gzmigu.cn

guard let x = opt else { return }
来源：http://th.lnxyls.cn

[T30] Swift：协议
来源：http://zu.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://er.szsharing.cn

[T31] Lua：Hello World
来源：http://xk.lnxyls.cn

print("Hello")
来源：http://jh.hnjuh.cn

[T32] Lua：局部变量
来源：http://oj.szxytkj.cn

local a = 1
来源：http://ko.521024.cn

[T33] Lua：表（数组）
来源：http://wi.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mn.panjiajie.cn

[T34] Lua：遍历表
来源：http://tk.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tk.huanxung.cn

[T35] Lua：字典表
来源：http://br.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://jw.nicolike.cn

[T36] Lua：函数
来源：http://uc.nicolike.cn

function add(a, b) return a + b end
来源：http://br.huanxung.cn

[T37] Lua：字符串拼接
来源：http://hw.huanxung.cn

"a" .. "b"
来源：http://xp.shxzukj.cn

[T38] Lua：条件
来源：http://gy.nicolike.cn

if x > 0 then print("正") end
来源：http://wj.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://lw.chemitech.net.cn

string.find(s, "%d+")
来源：http://uq.szsharing.cn

[T40] Lua：元表
来源：http://uu.szsharing.cn

setmetatable({}, { __index = base })
来源：http://xa.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://ux.asd995.cn

print "Hello\n";
来源：http://xj.9csxet.cn

[T42] Perl：变量类型
来源：http://zu.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xv.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://jo.asd995.cn

"值: $a"
来源：http://oq.jianghongdianzi.cn

[T44] Perl：条件
来源：http://iw.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://mk.shxzukj.cn

[T45] Perl：数组遍历
来源：http://jm.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://qo.szxytkj.cn

[T46] Perl：哈希操作
来源：http://qn.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lp.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://hj.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aq.gzmigu.cn

[T48] Perl：正则替换
来源：http://kj.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://qu.asd995.cn

[T49] Perl：函数
来源：http://ua.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iz.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://mc.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ng.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://de.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://xk.shtwfgs.cn

println("Hello")
来源：http://ck.szsharing.cn

[T52] Scala：变量
来源：http://bc.panjiajie.cn

val a = 1;  var b = 2
来源：http://nt.newstarts.cn

[T53] Scala：字符串插值
来源：http://ho.jctech888.com.cn

s"值: $b"
来源：http://ht.nicolike.cn

[T54] Scala：集合映射
来源：http://mo.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://gk.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://pk.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gc.bookmarksfly.cn

[T56] Scala：样例类
来源：http://xi.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://po.colortex.cn

[T57] Scala：模式匹配
来源：http://ae.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dk.hnjuh.cn

[T58] Scala：函数定义
来源：http://py.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zs.asd995.cn

[T59] Scala：循环
来源：http://zv.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://hz.hahajie.cn

[T60] Scala：折叠
来源：http://fx.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lw.lnxyls.cn

================================================================================
来源：http://cw.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sq.jctech888.com.cn

================================================================================
来源：http://co.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://lp.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zs.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://vm.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bu.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://zu.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sj.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://mb.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yw.colortex.cn

[U05] Py：列表去重且保序
来源：http://yk.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://ba.gzmigu.cn

[U06] Py：合并两个字典
来源：http://mu.lnxyls.cn

{**a, **b}
来源：http://sk.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://pf.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://mp.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://uf.hnjuh.cn

[y for x in nested for y in x]
来源：http://zv.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://co.shxzskj.cn

max(d, key=d.get)
来源：http://wi.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://sx.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kf.lnxyls.cn

[U11] Py：生成器表达式
来源：http://qt.shxzukj.cn

(x * 2 for x in arr)
来源：http://ep.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mr.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://cb.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://et.huixiangedu.cn

deque(maxlen=10)
来源：http://te.szsharing.cn

[U14] Py：分组收集到列表
来源：http://av.haigaiapp.cn

defaultdict(list)
来源：http://ou.chemitech.net.cn

[U15] Py：高精度计时
来源：http://yf.shxzukj.cn

t = time.perf_counter()
来源：http://wc.9csxet.cn

[U16] Py：命令行参数解析
来源：http://zu.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sb.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://sk.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://gt.jctech888.com.cn

[U18] Py：预编译正则
来源：http://ab.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://oy.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://yb.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ns.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ap.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://nf.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://vh.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://uf.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://ul.gzmigu.cn

list(zip(*m))
来源：http://oa.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://wr.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hn.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://zz.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lf.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://or.shxzukj.cn

csv.DictReader(f)
来源：http://rd.newstarts.cn

[U26] Py：并发下载
来源：http://co.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lv.nszjky.cn

[U27] Py：异步 HTTP
来源：http://ej.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://cz.nicolike.cn

[U28] Py：类型别名
来源：http://vv.hahajie.cn

UserId = int
来源：http://jf.jctech888.com.cn

[U29] Py：属性校验
来源：http://xe.nszjky.cn

@property 与 @x.setter 配合
来源：http://hp.szsharing.cn

[U30] Py：数据类
来源：http://jn.szxytkj.cn

@dataclass(slots=True)
来源：http://fz.wgjwhj.cn

[U31] Py：单测
来源：http://os.newstarts.cn

python -m pytest -q
来源：http://rb.gzmigu.cn

[U32] Py：代码格式化
来源：http://qs.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://cl.szxytkj.cn

[U33] Py：打包发布
来源：http://nz.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://eg.nicolike.cn

[U34] Py：判断编码
来源：http://jp.yuexingan06.cn

chardet.detect(raw)
来源：http://nh.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ga.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iq.9csxet.cn

[U36] Py：定时任务
来源：http://uc.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://fe.colortex.cn

[U37] Py：读写 Excel
来源：http://ys.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zy.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://tw.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://iu.521024.cn

[U39] Py：判断是否在交互环境
来源：http://ct.newstarts.cn

sys.stdout.isatty()
来源：http://cf.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://qa.shxzskj.cn

print("err", file=sys.stderr)
来源：http://yj.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://xg.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ad.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://qa.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sa.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://fw.bookmarksfly.cn

namespace App\Http;
来源：http://sl.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://pb.colortex.cn

declare(strict_types=1);
来源：http://ss.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://if.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vp.yuexingan06.cn

[U46] PHP：可空类型
来源：http://za.yuexingan06.cn

?string $name = null
来源：http://hd.shxzskj.cn

[U47] PHP：联合类型
来源：http://bl.hnjuh.cn

int|string $id
来源：http://aa.9csxet.cn

[U48] PHP：纯枚举
来源：http://be.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ye.szxytkj.cn

[U49] PHP：只读属性
来源：http://yo.hnjuh.cn

public readonly string $name
来源：http://tr.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://ny.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ui.huanxung.cn

[U51] PHP：数组解构
来源：http://hd.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://qg.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://nx.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://ou.asd995.cn

[U53] PHP：空合并运算符
来源：http://ln.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://du.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://zz.wgjwhj.cn

$obj?->method()
来源：http://cn.shxzskj.cn

[U55] PHP：match 表达式
来源：http://ar.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yj.hnjuh.cn

[U56] PHP：命名参数
来源：http://hb.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://kn.szxytkj.cn

[U57] PHP：字符串插值
来源：http://ei.szsharing.cn

"值: {$a}"
来源：http://pf.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://vw.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ml.lnxyls.cn


<!-- 参考信息 -->