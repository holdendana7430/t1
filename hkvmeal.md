代发 wailian999

[S33] C++：vector 增删
来源：http://bd.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iw.szsharing.cn

[S34] C++：遍历 vector
来源：http://zr.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://xn.colortex.cn

[S35] C++：map
来源：http://ky.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://we.asd995.cn

[S36] C++：unordered_map
来源：http://at.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qy.shtwfgs.cn

[S37] C++：set
来源：http://op.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qd.bookmarksfly.cn

[S38] C++：排序
来源：http://tu.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://tz.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://te.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hq.shxzskj.cn

[S40] C++：查找元素
来源：http://al.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gr.panjiajie.cn

[S41] C++：类与构造函数
来源：http://mw.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bo.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://vk.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://cz.shtwfgs.cn

[S43] C++：智能指针
来源：http://sq.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://qs.szxytkj.cn

[S44] C++：引用传参
来源：http://ah.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ee.shtwfgs.cn

[S45] C++：lambda
来源：http://ol.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nr.panjiajie.cn

[S46] C++：函数模板
来源：http://mp.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ds.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://lr.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xh.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://mx.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mn.521024.cn

while (std::getline(in, line)) { }
来源：http://ti.huanxung.cn

[S49] C++：写文件
来源：http://uc.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://em.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://oh.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://du.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ge.muxihuayi.cn

static_cast<double>(a) / b
来源：http://py.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://sl.huanxung.cn

int size() const noexcept { return n_; }
来源：http://pd.muxihuayi.cn

[S53] C++：移动语义
来源：http://fa.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://nk.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://tm.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://st.hahajie.cn

[S55] C++：结构化绑定
来源：http://xh.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vv.yuexingan06.cn

[S56] C++：optional
来源：http://tx.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ia.huanxung.cn

[S57] C++：编译期常量
来源：http://ug.huixiangedu.cn

constexpr int N = 10;
来源：http://lw.wgjwhj.cn

[S58] C++：命名空间
来源：http://xy.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://fa.shxzskj.cn

[S59] C++：静态断言
来源：http://ik.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lq.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://rr.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cb.newstarts.cn

================================================================================
来源：http://dx.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ox.bookmarksfly.cn

================================================================================
来源：http://ua.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://cd.nszjky.cn

println("Hello")
来源：http://sq.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ao.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cu.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://yp.shtwfgs.cn

"值: $b"
来源：http://gj.lnxyls.cn

[T04] Kotlin：空安全
来源：http://zj.hnjuh.cn

val n: String? = null;  n?.length
来源：http://ds.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://wl.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ha.newstarts.cn

[T06] Kotlin：集合映射
来源：http://mf.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qf.colortex.cn

[T07] Kotlin：集合过滤
来源：http://st.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fy.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://jj.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://hn.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://lx.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://qi.huanxung.cn

[T10] Kotlin：默认参数
来源：http://fy.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yy.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ng.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vo.colortex.cn

[T12] Kotlin：解构声明
来源：http://jd.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://jk.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://ma.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://vm.muxihuayi.cn

[T14] Kotlin：循环
来源：http://kg.asd995.cn

for (i in 1..10) println(i)
来源：http://aa.lnxyls.cn

[T15] Kotlin：接口
来源：http://ml.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://nf.colortex.cn

[T16] Swift：Hello World
来源：http://hv.haigaiapp.cn

print("Hello")
来源：http://oh.521024.cn

[T17] Swift：变量与常量
来源：http://yx.chemitech.net.cn

var a = 1;  let b = 2
来源：http://tp.gzmigu.cn

[T18] Swift：字符串插值
来源：http://lo.panjiajie.cn

"值: \(b)"
来源：http://ef.shxzskj.cn

[T19] Swift：可选绑定
来源：http://lb.gzmigu.cn

if let n = opt { print(n) }
来源：http://rv.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://eo.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hv.yuexingan06.cn

[T21] Swift：遍历
来源：http://yb.shtwfgs.cn

for x in a { print(x) }
来源：http://vx.lnxyls.cn

[T22] Swift：字典
来源：http://gk.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vd.huixinmuqiang.cn

[T23] Swift：函数
来源：http://vx.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lv.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://sn.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fr.chemitech.net.cn

[T25] Swift：结构体
来源：http://gn.colortex.cn

struct P { var x: Int }
来源：http://rt.shxzukj.cn

[T26] Swift：类与重写
来源：http://jm.newstarts.cn

class A: Base { override func f() {} }
来源：http://ws.jctech888.com.cn

[T27] Swift：错误处理
来源：http://bu.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://ht.yuexingan06.cn

[T28] Swift：枚举
来源：http://oq.chemitech.net.cn

enum Color { case red, green }
来源：http://eo.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://uq.asd995.cn

guard let x = opt else { return }
来源：http://fv.nszjky.cn

[T30] Swift：协议
来源：http://pq.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://nh.shxzskj.cn

[T31] Lua：Hello World
来源：http://dk.521024.cn

print("Hello")
来源：http://qi.nszjky.cn

[T32] Lua：局部变量
来源：http://of.hnjuh.cn

local a = 1
来源：http://cv.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ip.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://md.gzmigu.cn

[T34] Lua：遍历表
来源：http://fb.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://md.chemitech.net.cn

[T35] Lua：字典表
来源：http://na.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://yn.lnxyls.cn

[T36] Lua：函数
来源：http://pt.szxytkj.cn

function add(a, b) return a + b end
来源：http://ip.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://dp.panjiajie.cn

"a" .. "b"
来源：http://kl.colortex.cn

[T38] Lua：条件
来源：http://vi.gzmigu.cn

if x > 0 then print("正") end
来源：http://fx.gzmigu.cn

[T39] Lua：模式匹配
来源：http://hw.szsharing.cn

string.find(s, "%d+")
来源：http://vb.chemitech.net.cn

[T40] Lua：元表
来源：http://uu.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://yu.yuexingan06.cn

[T41] Perl：Hello World
来源：http://bv.bookmarksfly.cn

print "Hello\n";
来源：http://gu.nszjky.cn

[T42] Perl：变量类型
来源：http://ai.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jo.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://oc.newstarts.cn

"值: $a"
来源：http://jy.szsharing.cn

[T44] Perl：条件
来源：http://gu.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://sp.asd995.cn

[T45] Perl：数组遍历
来源：http://df.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://tt.9csxet.cn

[T46] Perl：哈希操作
来源：http://fs.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nd.szsharing.cn

[T47] Perl：正则捕获
来源：http://vi.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tq.huanxung.cn

[T48] Perl：正则替换
来源：http://tm.szsharing.cn

$s =~ s/old/new/g;
来源：http://ht.huixiangedu.cn

[T49] Perl：函数
来源：http://xw.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ir.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://aa.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kw.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://kb.wgjwhj.cn

[T51] Scala：Hello World
来源：http://vs.shtwfgs.cn

println("Hello")
来源：http://ew.shxzskj.cn

[T52] Scala：变量
来源：http://kj.chemitech.net.cn

val a = 1;  var b = 2
来源：http://bv.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://fh.szsharing.cn

s"值: $b"
来源：http://bj.521024.cn

[T54] Scala：集合映射
来源：http://ig.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://kh.nicolike.cn

[T55] Scala：集合过滤
来源：http://gh.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zi.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://sn.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://qr.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://tc.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://on.panjiajie.cn

[T58] Scala：函数定义
来源：http://fi.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xf.szsharing.cn

[T59] Scala：循环
来源：http://nr.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://jb.asd995.cn

[T60] Scala：折叠
来源：http://bd.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xv.huixiangedu.cn

================================================================================
来源：http://el.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rm.yuntaijiaju.cn

================================================================================
来源：http://ae.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://mk.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zv.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://fx.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mr.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://yp.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kc.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://lc.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fz.nicolike.cn

[U05] Py：列表去重且保序
来源：http://gs.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://vi.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://cc.shtwfgs.cn

{**a, **b}
来源：http://fb.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://fa.9csxet.cn

{v: k for k, v in d.items()}
来源：http://fp.lnxyls.cn

[U08] Py：展平二维列表
来源：http://eu.jctech888.com.cn

[y for x in nested for y in x]
来源：http://nl.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://fr.bjjhwx.cn

max(d, key=d.get)
来源：http://hl.szxytkj.cn

[U10] Py：按值排序字典
来源：http://bj.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qa.panjiajie.cn

[U11] Py：生成器表达式
来源：http://mq.nicolike.cn

(x * 2 for x in arr)
来源：http://bb.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qd.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://jm.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://ri.szsharing.cn

deque(maxlen=10)
来源：http://yp.huanxung.cn

[U14] Py：分组收集到列表
来源：http://ad.521024.cn

defaultdict(list)
来源：http://te.bjjhwx.cn

[U15] Py：高精度计时
来源：http://zk.panjiajie.cn

t = time.perf_counter()
来源：http://od.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://wy.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cb.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://di.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://lt.521024.cn

[U18] Py：预编译正则
来源：http://nc.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://dd.asd995.cn

[U19] Py：正则替换带回调
来源：http://hz.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zp.asd995.cn

[U20] Py：缓存函数结果
来源：http://pb.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://gv.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://xq.wgjwhj.cn

@contextlib.contextmanager
来源：http://of.newstarts.cn

[U22] Py：矩阵转置
来源：http://lu.521024.cn

list(zip(*m))
来源：http://ax.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://oz.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qe.panjiajie.cn

[U24] Py：路径操作
来源：http://qh.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ou.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://gu.colortex.cn

csv.DictReader(f)
来源：http://dj.hnjuh.cn

[U26] Py：并发下载
来源：http://ck.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tx.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://oy.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://de.huixiangedu.cn

[U28] Py：类型别名
来源：http://zy.panjiajie.cn

UserId = int
来源：http://ih.chemitech.net.cn

[U29] Py：属性校验
来源：http://jm.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://ua.colortex.cn

[U30] Py：数据类
来源：http://jm.shxzskj.cn

@dataclass(slots=True)
来源：http://wq.shtwfgs.cn

[U31] Py：单测
来源：http://mf.panjiajie.cn

python -m pytest -q
来源：http://hd.521024.cn

[U32] Py：代码格式化
来源：http://zg.szsharing.cn

ruff format . && ruff check --fix .
来源：http://tt.9csxet.cn

[U33] Py：打包发布
来源：http://tx.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://xm.shxzukj.cn

[U34] Py：判断编码
来源：http://ga.9csxet.cn

chardet.detect(raw)
来源：http://su.szsharing.cn

[U35] Py：发送邮件
来源：http://au.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zs.newstarts.cn

[U36] Py：定时任务
来源：http://qu.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://ao.shxzskj.cn

[U37] Py：读写 Excel
来源：http://pm.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://le.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://di.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://hf.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://pr.colortex.cn

sys.stdout.isatty()
来源：http://no.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://wd.huanxung.cn

print("err", file=sys.stderr)
来源：http://hj.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ki.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ix.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://nv.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mw.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://be.hahajie.cn

namespace App\Http;
来源：http://lf.huanxung.cn

[U44] PHP：开启严格类型
来源：http://zs.jianghongdianzi.cn

declare(strict_types=1);
来源：http://yu.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://zw.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rk.panjiajie.cn

[U46] PHP：可空类型
来源：http://de.shxzskj.cn

?string $name = null
来源：http://rg.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://jw.lnxyls.cn

int|string $id
来源：http://ny.colortex.cn

[U48] PHP：纯枚举
来源：http://gg.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ui.wgjwhj.cn

[U49] PHP：只读属性
来源：http://od.yuexingan06.cn

public readonly string $name
来源：http://om.521024.cn

[U50] PHP：构造器属性提升
来源：http://fr.szxytkj.cn

public function __construct(private int $id) {}
来源：http://um.asd995.cn

[U51] PHP：数组解构
来源：http://cu.chemitech.net.cn

[$a, $b] = $arr;
来源：http://jq.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://eg.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://hl.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://op.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://md.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://pd.gzmigu.cn

$obj?->method()
来源：http://wg.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://xi.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ga.yuexingan06.cn

[U56] PHP：命名参数
来源：http://rq.521024.cn

f(a: 1, b: 2)
来源：http://hd.shxzukj.cn

[U57] PHP：字符串插值
来源：http://bs.asd995.cn

"值: {$a}"
来源：http://gp.asd995.cn

[U58] PHP：数组三件套
来源：http://zt.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jo.jctech888.com.cn


<!-- 参考信息 -->