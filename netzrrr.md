代发 wailian999

[S37] C++：set
来源：http://rw.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lv.yuntaijiaju.cn

[S38] C++：排序
来源：http://bd.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://ax.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://nc.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wv.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://ib.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jt.hnjuh.cn

[S41] C++：类与构造函数
来源：http://ta.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ui.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://wm.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://bb.521024.cn

[S43] C++：智能指针
来源：http://sv.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://ww.asd995.cn

[S44] C++：引用传参
来源：http://em.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://is.szxytkj.cn

[S45] C++：lambda
来源：http://mr.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ra.shxzskj.cn

[S46] C++：函数模板
来源：http://px.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vt.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://nq.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yw.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://oe.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gr.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://nn.9csxet.cn

[S49] C++：写文件
来源：http://ay.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cy.9csxet.cn

[S50] C++：格式化数字
来源：http://eb.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ju.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://oh.hnjuh.cn

static_cast<double>(a) / b
来源：http://za.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://xi.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://oe.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://wj.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://gd.shxzukj.cn

[S54] C++：异常处理
来源：http://ad.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tt.panjiajie.cn

[S55] C++：结构化绑定
来源：http://uu.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tm.huanxung.cn

[S56] C++：optional
来源：http://ut.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gs.jctech888.com.cn

[S57] C++：编译期常量
来源：http://vp.colortex.cn

constexpr int N = 10;
来源：http://le.chemitech.net.cn

[S58] C++：命名空间
来源：http://ro.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://tv.asd995.cn

[S59] C++：静态断言
来源：http://or.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://un.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://rv.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rl.gzmigu.cn

================================================================================
来源：http://fo.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://we.bookmarksfly.cn

================================================================================
来源：http://fb.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://jy.chemitech.net.cn

println("Hello")
来源：http://va.shxzskj.cn

[T02] Kotlin：变量
来源：http://lg.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ja.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://be.jctech888.com.cn

"值: $b"
来源：http://es.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ye.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://vr.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://mo.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jd.521024.cn

[T06] Kotlin：集合映射
来源：http://ab.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jg.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://uz.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://be.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://ks.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://nv.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://ld.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://mp.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://sm.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pj.nszjky.cn

[T11] Kotlin：协程
来源：http://tq.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ci.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://av.521024.cn

val (a, b) = Pair(1, 2)
来源：http://wh.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://dh.9csxet.cn

val m = mapOf("a" to 1)
来源：http://pw.szxytkj.cn

[T14] Kotlin：循环
来源：http://lv.colortex.cn

for (i in 1..10) println(i)
来源：http://uv.lnxyls.cn

[T15] Kotlin：接口
来源：http://cg.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://lk.nicolike.cn

[T16] Swift：Hello World
来源：http://us.shtwfgs.cn

print("Hello")
来源：http://tj.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://as.huixiangedu.cn

var a = 1;  let b = 2
来源：http://eb.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://uj.bjjhwx.cn

"值: \(b)"
来源：http://gm.9csxet.cn

[T19] Swift：可选绑定
来源：http://wt.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://ys.muxihuayi.cn

[T20] Swift：数组操作
来源：http://kw.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aq.shxzukj.cn

[T21] Swift：遍历
来源：http://ty.jctech888.com.cn

for x in a { print(x) }
来源：http://gb.szxytkj.cn

[T22] Swift：字典
来源：http://yt.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wv.hnjuh.cn

[T23] Swift：函数
来源：http://vb.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://na.muxihuayi.cn

[T24] Swift：闭包
来源：http://vs.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vu.gzmigu.cn

[T25] Swift：结构体
来源：http://xz.chemitech.net.cn

struct P { var x: Int }
来源：http://yw.bjjhwx.cn

[T26] Swift：类与重写
来源：http://fm.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://wz.jctech888.com.cn

[T27] Swift：错误处理
来源：http://pg.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://kf.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://dq.521024.cn

enum Color { case red, green }
来源：http://um.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://rp.shxzskj.cn

guard let x = opt else { return }
来源：http://py.asd995.cn

[T30] Swift：协议
来源：http://wt.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://bo.haigaiapp.cn

[T31] Lua：Hello World
来源：http://iv.yuexingan06.cn

print("Hello")
来源：http://qu.shtwfgs.cn

[T32] Lua：局部变量
来源：http://gk.lnxyls.cn

local a = 1
来源：http://qy.lnxyls.cn

[T33] Lua：表（数组）
来源：http://hy.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mg.hahajie.cn

[T34] Lua：遍历表
来源：http://ws.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ra.wgjwhj.cn

[T35] Lua：字典表
来源：http://nx.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://co.yuexingan06.cn

[T36] Lua：函数
来源：http://hi.bjjhwx.cn

function add(a, b) return a + b end
来源：http://yk.asd995.cn

[T37] Lua：字符串拼接
来源：http://gx.jianghongdianzi.cn

"a" .. "b"
来源：http://xw.lnxyls.cn

[T38] Lua：条件
来源：http://re.chemitech.net.cn

if x > 0 then print("正") end
来源：http://fg.gzmigu.cn

[T39] Lua：模式匹配
来源：http://sy.chemitech.net.cn

string.find(s, "%d+")
来源：http://fd.lnxyls.cn

[T40] Lua：元表
来源：http://wv.szsharing.cn

setmetatable({}, { __index = base })
来源：http://av.hnjuh.cn

[T41] Perl：Hello World
来源：http://mn.shxzskj.cn

print "Hello\n";
来源：http://mr.colortex.cn

[T42] Perl：变量类型
来源：http://do.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://et.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://yv.muxihuayi.cn

"值: $a"
来源：http://pu.nicolike.cn

[T44] Perl：条件
来源：http://mh.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ec.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://qr.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://cl.521024.cn

[T46] Perl：哈希操作
来源：http://oy.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kh.hnjuh.cn

[T47] Perl：正则捕获
来源：http://dt.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zt.huixiangedu.cn

[T48] Perl：正则替换
来源：http://cd.gzmigu.cn

$s =~ s/old/new/g;
来源：http://yi.szsharing.cn

[T49] Perl：函数
来源：http://hi.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fg.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://xl.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://in.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://zo.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://gz.hahajie.cn

println("Hello")
来源：http://tf.hahajie.cn

[T52] Scala：变量
来源：http://xe.colortex.cn

val a = 1;  var b = 2
来源：http://ak.gzmigu.cn

[T53] Scala：字符串插值
来源：http://da.yuntaijiaju.cn

s"值: $b"
来源：http://hc.huanxung.cn

[T54] Scala：集合映射
来源：http://ai.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://hg.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://hm.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qc.szsharing.cn

[T56] Scala：样例类
来源：http://ac.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://lm.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://jj.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iv.hahajie.cn

[T58] Scala：函数定义
来源：http://ab.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xz.huanxung.cn

[T59] Scala：循环
来源：http://ur.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://ze.colortex.cn

[T60] Scala：折叠
来源：http://sh.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yj.lnxyls.cn

================================================================================
来源：http://gk.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ad.newstarts.cn

================================================================================
来源：http://lj.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://vw.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://se.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://ui.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wq.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://zr.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ae.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://cg.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uq.hahajie.cn

[U05] Py：列表去重且保序
来源：http://tk.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://fg.newstarts.cn

[U06] Py：合并两个字典
来源：http://pa.szsharing.cn

{**a, **b}
来源：http://tx.gzmigu.cn

[U07] Py：反转字典键值
来源：http://pp.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://fy.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://ca.gzmigu.cn

[y for x in nested for y in x]
来源：http://xn.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://ez.chemitech.net.cn

max(d, key=d.get)
来源：http://kd.panjiajie.cn

[U10] Py：按值排序字典
来源：http://pc.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://di.szsharing.cn

[U11] Py：生成器表达式
来源：http://as.nszjky.cn

(x * 2 for x in arr)
来源：http://hz.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zs.szxytkj.cn

Counter(arr).most_common(3)
来源：http://eh.9csxet.cn

[U13] Py：固定长度队列
来源：http://tu.haigaiapp.cn

deque(maxlen=10)
来源：http://pd.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://fd.nszjky.cn

defaultdict(list)
来源：http://oj.nicolike.cn

[U15] Py：高精度计时
来源：http://kt.haigaiapp.cn

t = time.perf_counter()
来源：http://oi.hahajie.cn

[U16] Py：命令行参数解析
来源：http://sl.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oe.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://st.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://pv.wgjwhj.cn

[U18] Py：预编译正则
来源：http://ns.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://fd.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://ui.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kw.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://pi.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://vx.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://ib.9csxet.cn

@contextlib.contextmanager
来源：http://el.panjiajie.cn

[U22] Py：矩阵转置
来源：http://sd.jianghongdianzi.cn

list(zip(*m))
来源：http://cc.hahajie.cn

[U23] Py：分块读取大文件
来源：http://cv.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vz.huanxung.cn

[U24] Py：路径操作
来源：http://cn.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yj.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://kn.shxzukj.cn

csv.DictReader(f)
来源：http://tb.nszjky.cn

[U26] Py：并发下载
来源：http://vn.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ca.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://yx.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://ti.muxihuayi.cn

[U28] Py：类型别名
来源：http://zu.huixiangedu.cn

UserId = int
来源：http://ep.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://cj.newstarts.cn

@property 与 @x.setter 配合
来源：http://an.hnjuh.cn

[U30] Py：数据类
来源：http://pf.gzmigu.cn

@dataclass(slots=True)
来源：http://bx.lnxyls.cn

[U31] Py：单测
来源：http://gl.huanxung.cn

python -m pytest -q
来源：http://wn.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://jo.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://mz.521024.cn

[U33] Py：打包发布
来源：http://as.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://kd.nszjky.cn

[U34] Py：判断编码
来源：http://hr.panjiajie.cn

chardet.detect(raw)
来源：http://gj.huanxung.cn

[U35] Py：发送邮件
来源：http://pc.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zu.chemitech.net.cn

[U36] Py：定时任务
来源：http://xa.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://hs.asd995.cn

[U37] Py：读写 Excel
来源：http://iw.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://it.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://oi.newstarts.cn

Path(__file__).resolve().parent
来源：http://qo.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://ue.nszjky.cn

sys.stdout.isatty()
来源：http://pw.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://sm.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://rt.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://if.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gi.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ta.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sb.nicolike.cn

[U43] PHP：声明命名空间
来源：http://dn.szsharing.cn

namespace App\Http;
来源：http://zp.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://lj.521024.cn

declare(strict_types=1);
来源：http://hg.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://rw.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://av.shxzskj.cn

[U46] PHP：可空类型
来源：http://pt.szsharing.cn

?string $name = null
来源：http://gq.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ei.szsharing.cn

int|string $id
来源：http://nu.shxzukj.cn

[U48] PHP：纯枚举
来源：http://cn.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xu.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://me.hahajie.cn

public readonly string $name
来源：http://ha.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://vl.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://xz.asd995.cn

[U51] PHP：数组解构
来源：http://hy.nszjky.cn

[$a, $b] = $arr;
来源：http://ws.asd995.cn

[U52] PHP：箭头函数
来源：http://ee.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://dd.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ur.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://ga.asd995.cn

[U54] PHP：空安全调用
来源：http://lw.jianghongdianzi.cn

$obj?->method()
来源：http://lk.521024.cn

[U55] PHP：match 表达式
来源：http://tf.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pu.colortex.cn

[U56] PHP：命名参数
来源：http://vu.jctech888.com.cn

f(a: 1, b: 2)
来源：http://qb.szsharing.cn

[U57] PHP：字符串插值
来源：http://bn.shxzukj.cn

"值: {$a}"
来源：http://tb.huanxung.cn

[U58] PHP：数组三件套
来源：http://qm.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cr.nszjky.cn

[U59] PHP：自定义排序
来源：http://vy.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://wx.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mj.yuexingan06.cn

[U61] PHP：正则
来源：http://dx.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ul.gzmigu.cn

[U62] PHP：日期对象
来源：http://eg.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kt.bookmarksfly.cn


<!-- 参考信息 -->