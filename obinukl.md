代发 wailian999

[S39] C++：自定义比较器排序
来源：http://uh.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aq.szsharing.cn

[S40] C++：查找元素
来源：http://dj.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ov.521024.cn

[S41] C++：类与构造函数
来源：http://nx.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bq.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://aa.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://hq.hnjuh.cn

[S43] C++：智能指针
来源：http://is.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://pg.hnjuh.cn

[S44] C++：引用传参
来源：http://xm.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://rz.shxzskj.cn

[S45] C++：lambda
来源：http://ha.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zv.bjjhwx.cn

[S46] C++：函数模板
来源：http://qw.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gd.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://hr.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ur.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://ic.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ii.colortex.cn

while (std::getline(in, line)) { }
来源：http://wx.9csxet.cn

[S49] C++：写文件
来源：http://ka.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bm.hnjuh.cn

[S50] C++：格式化数字
来源：http://zi.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ne.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://ce.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://av.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://wu.nszjky.cn

int size() const noexcept { return n_; }
来源：http://vb.muxihuayi.cn

[S53] C++：移动语义
来源：http://li.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://ij.huanxung.cn

[S54] C++：异常处理
来源：http://sn.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dp.panjiajie.cn

[S55] C++：结构化绑定
来源：http://oe.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zj.huixinmuqiang.cn

[S56] C++：optional
来源：http://af.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://id.newstarts.cn

[S57] C++：编译期常量
来源：http://pw.szxytkj.cn

constexpr int N = 10;
来源：http://vy.asd995.cn

[S58] C++：命名空间
来源：http://co.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://lc.shxzukj.cn

[S59] C++：静态断言
来源：http://tk.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ov.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://dc.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rc.jctech888.com.cn

================================================================================
来源：http://pv.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ga.asd995.cn

================================================================================
来源：http://vi.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://te.shxzukj.cn

println("Hello")
来源：http://lr.muxihuayi.cn

[T02] Kotlin：变量
来源：http://em.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ec.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://mi.wgjwhj.cn

"值: $b"
来源：http://pw.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://ui.hahajie.cn

val n: String? = null;  n?.length
来源：http://wb.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://er.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://od.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://qy.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mo.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://eb.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ex.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://la.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://np.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://wl.asd995.cn

fun String.exclaim() = this + "!"
来源：http://fx.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://qk.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jn.nszjky.cn

[T11] Kotlin：协程
来源：http://ek.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nv.szsharing.cn

[T12] Kotlin：解构声明
来源：http://mf.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://ko.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://yo.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ev.nszjky.cn

[T14] Kotlin：循环
来源：http://ey.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://gm.shtwfgs.cn

[T15] Kotlin：接口
来源：http://si.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://fx.shtwfgs.cn

[T16] Swift：Hello World
来源：http://vv.hahajie.cn

print("Hello")
来源：http://wv.shxzskj.cn

[T17] Swift：变量与常量
来源：http://nw.panjiajie.cn

var a = 1;  let b = 2
来源：http://md.shxzukj.cn

[T18] Swift：字符串插值
来源：http://sj.shxzukj.cn

"值: \(b)"
来源：http://xr.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://sf.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://nc.nszjky.cn

[T20] Swift：数组操作
来源：http://yu.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ej.hahajie.cn

[T21] Swift：遍历
来源：http://kf.szsharing.cn

for x in a { print(x) }
来源：http://ih.huanxung.cn

[T22] Swift：字典
来源：http://tq.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vy.bjjhwx.cn

[T23] Swift：函数
来源：http://zm.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gq.shxzskj.cn

[T24] Swift：闭包
来源：http://aa.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mr.shtwfgs.cn

[T25] Swift：结构体
来源：http://fr.yuntaijiaju.cn

struct P { var x: Int }
来源：http://fk.szsharing.cn

[T26] Swift：类与重写
来源：http://ps.lnxyls.cn

class A: Base { override func f() {} }
来源：http://zd.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ir.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://as.szxytkj.cn

[T28] Swift：枚举
来源：http://iy.colortex.cn

enum Color { case red, green }
来源：http://ut.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://yi.gzmigu.cn

guard let x = opt else { return }
来源：http://yp.shxzskj.cn

[T30] Swift：协议
来源：http://wo.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://np.szsharing.cn

[T31] Lua：Hello World
来源：http://ta.szxytkj.cn

print("Hello")
来源：http://is.szsharing.cn

[T32] Lua：局部变量
来源：http://lm.shtwfgs.cn

local a = 1
来源：http://wi.shxzukj.cn

[T33] Lua：表（数组）
来源：http://mm.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gc.panjiajie.cn

[T34] Lua：遍历表
来源：http://oc.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nl.gzmigu.cn

[T35] Lua：字典表
来源：http://bg.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://gg.hahajie.cn

[T36] Lua：函数
来源：http://af.lnxyls.cn

function add(a, b) return a + b end
来源：http://aj.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://gv.panjiajie.cn

"a" .. "b"
来源：http://je.szsharing.cn

[T38] Lua：条件
来源：http://zl.newstarts.cn

if x > 0 then print("正") end
来源：http://qr.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://rr.nszjky.cn

string.find(s, "%d+")
来源：http://lx.huixiangedu.cn

[T40] Lua：元表
来源：http://ta.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://pd.asd995.cn

[T41] Perl：Hello World
来源：http://sa.yuexingan06.cn

print "Hello\n";
来源：http://fm.newstarts.cn

[T42] Perl：变量类型
来源：http://qo.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xv.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://qz.yuntaijiaju.cn

"值: $a"
来源：http://aj.hnjuh.cn

[T44] Perl：条件
来源：http://ei.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://hg.nicolike.cn

[T45] Perl：数组遍历
来源：http://lv.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ph.521024.cn

[T46] Perl：哈希操作
来源：http://vb.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ws.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://db.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://us.hnjuh.cn

[T48] Perl：正则替换
来源：http://wz.szxytkj.cn

$s =~ s/old/new/g;
来源：http://za.bookmarksfly.cn

[T49] Perl：函数
来源：http://vb.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nu.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://jm.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zk.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://lq.nicolike.cn

[T51] Scala：Hello World
来源：http://cz.9csxet.cn

println("Hello")
来源：http://yf.panjiajie.cn

[T52] Scala：变量
来源：http://hg.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://vo.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://wd.nszjky.cn

s"值: $b"
来源：http://gi.jctech888.com.cn

[T54] Scala：集合映射
来源：http://hq.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://hu.nicolike.cn

[T55] Scala：集合过滤
来源：http://yr.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xt.hahajie.cn

[T56] Scala：样例类
来源：http://pt.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://mx.hnjuh.cn

[T57] Scala：模式匹配
来源：http://pz.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dz.gzmigu.cn

[T58] Scala：函数定义
来源：http://hs.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bq.szxytkj.cn

[T59] Scala：循环
来源：http://bv.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://kv.huanxung.cn

[T60] Scala：折叠
来源：http://uj.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fm.bjjhwx.cn

================================================================================
来源：http://kd.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://of.hahajie.cn

================================================================================
来源：http://ls.asd995.cn

[U01] Py：创建虚拟环境
来源：http://dh.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wl.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://aj.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gr.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://ej.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fi.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://qe.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wd.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://xg.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://ez.521024.cn

[U06] Py：合并两个字典
来源：http://xl.nszjky.cn

{**a, **b}
来源：http://np.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://kr.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://nb.gzmigu.cn

[U08] Py：展平二维列表
来源：http://oq.szxytkj.cn

[y for x in nested for y in x]
来源：http://sb.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://zu.jctech888.com.cn

max(d, key=d.get)
来源：http://jk.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://bz.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ce.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://bl.9csxet.cn

(x * 2 for x in arr)
来源：http://gg.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://th.newstarts.cn

Counter(arr).most_common(3)
来源：http://fw.nszjky.cn

[U13] Py：固定长度队列
来源：http://lx.yuntaijiaju.cn

deque(maxlen=10)
来源：http://wg.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://mh.newstarts.cn

defaultdict(list)
来源：http://pu.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://ma.gzmigu.cn

t = time.perf_counter()
来源：http://ey.nszjky.cn

[U16] Py：命令行参数解析
来源：http://lh.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://np.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://hi.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://oq.haigaiapp.cn

[U18] Py：预编译正则
来源：http://rs.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://yr.newstarts.cn

[U19] Py：正则替换带回调
来源：http://mu.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kp.colortex.cn

[U20] Py：缓存函数结果
来源：http://qz.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://gi.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://um.colortex.cn

@contextlib.contextmanager
来源：http://ql.lnxyls.cn

[U22] Py：矩阵转置
来源：http://xs.newstarts.cn

list(zip(*m))
来源：http://az.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://ck.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wm.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ul.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yy.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://yt.shxzukj.cn

csv.DictReader(f)
来源：http://gc.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://ce.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xh.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://kb.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://rz.haigaiapp.cn

[U28] Py：类型别名
来源：http://pu.panjiajie.cn

UserId = int
来源：http://eb.huanxung.cn

[U29] Py：属性校验
来源：http://ds.nicolike.cn

@property 与 @x.setter 配合
来源：http://pf.muxihuayi.cn

[U30] Py：数据类
来源：http://bn.yuexingan06.cn

@dataclass(slots=True)
来源：http://lr.nszjky.cn

[U31] Py：单测
来源：http://vo.nszjky.cn

python -m pytest -q
来源：http://ek.bjjhwx.cn

[U32] Py：代码格式化
来源：http://fb.521024.cn

ruff format . && ruff check --fix .
来源：http://ep.huixiangedu.cn

[U33] Py：打包发布
来源：http://ov.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ir.bookmarksfly.cn

[U34] Py：判断编码
来源：http://gr.nszjky.cn

chardet.detect(raw)
来源：http://yt.lnxyls.cn

[U35] Py：发送邮件
来源：http://rf.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vv.panjiajie.cn

[U36] Py：定时任务
来源：http://eo.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://ie.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://wt.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gn.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://wh.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ji.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://qt.hahajie.cn

sys.stdout.isatty()
来源：http://xm.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://ty.521024.cn

print("err", file=sys.stderr)
来源：http://tu.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://gz.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ot.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://dt.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gx.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://yf.9csxet.cn

namespace App\Http;
来源：http://cc.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://nv.521024.cn

declare(strict_types=1);
来源：http://je.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://pr.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hr.colortex.cn

[U46] PHP：可空类型
来源：http://jq.jianghongdianzi.cn

?string $name = null
来源：http://by.bjjhwx.cn

[U47] PHP：联合类型
来源：http://bg.haigaiapp.cn

int|string $id
来源：http://ii.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://nb.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rd.chemitech.net.cn

[U49] PHP：只读属性
来源：http://qm.nicolike.cn

public readonly string $name
来源：http://zh.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://rn.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://yc.wgjwhj.cn

[U51] PHP：数组解构
来源：http://rg.521024.cn

[$a, $b] = $arr;
来源：http://rs.asd995.cn

[U52] PHP：箭头函数
来源：http://gp.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://vi.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://ow.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://mx.9csxet.cn

[U54] PHP：空安全调用
来源：http://bp.chemitech.net.cn

$obj?->method()
来源：http://ex.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ff.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ec.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://tt.bjjhwx.cn

f(a: 1, b: 2)
来源：http://jf.szxytkj.cn

[U57] PHP：字符串插值
来源：http://fw.shtwfgs.cn

"值: {$a}"
来源：http://rx.gzmigu.cn

[U58] PHP：数组三件套
来源：http://lc.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wb.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://gn.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ic.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://vh.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xa.colortex.cn

[U61] PHP：正则
来源：http://si.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://es.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://sj.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ix.bjjhwx.cn

[U63] PHP：文件读写
来源：http://hq.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pc.nszjky.cn

[U64] PHP：目录遍历
来源：http://uc.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://gd.nszjky.cn


<!-- 参考信息 -->