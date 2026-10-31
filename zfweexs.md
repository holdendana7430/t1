代发 wailian999

[S35] C++：map
来源：http://wh.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aj.huixiangedu.cn

[S36] C++：unordered_map
来源：http://de.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wg.shtwfgs.cn

[S37] C++：set
来源：http://sw.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lt.huanxung.cn

[S38] C++：排序
来源：http://ae.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://sk.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://mf.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pq.gzmigu.cn

[S40] C++：查找元素
来源：http://gv.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kt.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://vz.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xz.9csxet.cn

[S42] C++：继承与虚函数
来源：http://eo.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://yy.gzmigu.cn

[S43] C++：智能指针
来源：http://bz.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://gv.lnxyls.cn

[S44] C++：引用传参
来源：http://ep.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://pm.nicolike.cn

[S45] C++：lambda
来源：http://ce.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sy.shxzukj.cn

[S46] C++：函数模板
来源：http://ly.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hd.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://ya.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gs.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://pk.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hm.9csxet.cn

while (std::getline(in, line)) { }
来源：http://zo.colortex.cn

[S49] C++：写文件
来源：http://yf.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xl.huixiangedu.cn

[S50] C++：格式化数字
来源：http://kb.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yu.newstarts.cn

[S51] C++：显式类型转换
来源：http://fw.shtwfgs.cn

static_cast<double>(a) / b
来源：http://qi.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://tg.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://yu.lnxyls.cn

[S53] C++：移动语义
来源：http://ux.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://eq.nicolike.cn

[S54] C++：异常处理
来源：http://mu.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://my.szsharing.cn

[S55] C++：结构化绑定
来源：http://ag.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yd.lnxyls.cn

[S56] C++：optional
来源：http://sd.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xp.shxzskj.cn

[S57] C++：编译期常量
来源：http://cz.panjiajie.cn

constexpr int N = 10;
来源：http://eh.huixiangedu.cn

[S58] C++：命名空间
来源：http://qx.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://sw.newstarts.cn

[S59] C++：静态断言
来源：http://se.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rk.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://yh.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yo.colortex.cn

================================================================================
来源：http://mk.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lq.yuexingan06.cn

================================================================================
来源：http://kw.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://cp.bjjhwx.cn

println("Hello")
来源：http://hz.yuexingan06.cn

[T02] Kotlin：变量
来源：http://rp.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uv.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://kc.lnxyls.cn

"值: $b"
来源：http://co.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://ma.colortex.cn

val n: String? = null;  n?.length
来源：http://qh.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://vm.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sc.nszjky.cn

[T06] Kotlin：集合映射
来源：http://xx.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tg.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://rt.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://na.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://zy.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://wo.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ln.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://xo.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://yu.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mn.521024.cn

[T11] Kotlin：协程
来源：http://ar.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://il.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://xe.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://mt.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://wk.newstarts.cn

val m = mapOf("a" to 1)
来源：http://ng.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://zl.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://jy.chemitech.net.cn

[T15] Kotlin：接口
来源：http://he.nszjky.cn

interface Shape { fun area(): Double }
来源：http://hh.wgjwhj.cn

[T16] Swift：Hello World
来源：http://nn.521024.cn

print("Hello")
来源：http://jq.nszjky.cn

[T17] Swift：变量与常量
来源：http://mt.9csxet.cn

var a = 1;  let b = 2
来源：http://zh.nszjky.cn

[T18] Swift：字符串插值
来源：http://hm.bjjhwx.cn

"值: \(b)"
来源：http://kv.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://pn.huanxung.cn

if let n = opt { print(n) }
来源：http://dj.colortex.cn

[T20] Swift：数组操作
来源：http://la.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xe.szsharing.cn

[T21] Swift：遍历
来源：http://di.colortex.cn

for x in a { print(x) }
来源：http://nf.colortex.cn

[T22] Swift：字典
来源：http://dr.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ak.huixiangedu.cn

[T23] Swift：函数
来源：http://qq.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gl.lnxyls.cn

[T24] Swift：闭包
来源：http://up.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aw.bookmarksfly.cn

[T25] Swift：结构体
来源：http://fd.shxzskj.cn

struct P { var x: Int }
来源：http://ca.shxzskj.cn

[T26] Swift：类与重写
来源：http://ph.newstarts.cn

class A: Base { override func f() {} }
来源：http://cd.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://ah.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://cn.szxytkj.cn

[T28] Swift：枚举
来源：http://ol.yuexingan06.cn

enum Color { case red, green }
来源：http://ox.colortex.cn

[T29] Swift：guard 提前返回
来源：http://px.huixiangedu.cn

guard let x = opt else { return }
来源：http://sr.asd995.cn

[T30] Swift：协议
来源：http://gn.521024.cn

protocol Shape { func area() -> Double }
来源：http://df.hahajie.cn

[T31] Lua：Hello World
来源：http://xl.9csxet.cn

print("Hello")
来源：http://yl.jctech888.com.cn

[T32] Lua：局部变量
来源：http://kq.haigaiapp.cn

local a = 1
来源：http://zy.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://ht.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sq.lnxyls.cn

[T34] Lua：遍历表
来源：http://ac.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kb.huixiangedu.cn

[T35] Lua：字典表
来源：http://js.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://qc.shtwfgs.cn

[T36] Lua：函数
来源：http://hb.lnxyls.cn

function add(a, b) return a + b end
来源：http://ah.newstarts.cn

[T37] Lua：字符串拼接
来源：http://ol.nszjky.cn

"a" .. "b"
来源：http://tm.shxzukj.cn

[T38] Lua：条件
来源：http://ou.panjiajie.cn

if x > 0 then print("正") end
来源：http://fa.9csxet.cn

[T39] Lua：模式匹配
来源：http://og.jctech888.com.cn

string.find(s, "%d+")
来源：http://id.huanxung.cn

[T40] Lua：元表
来源：http://yx.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://sh.newstarts.cn

[T41] Perl：Hello World
来源：http://er.gzmigu.cn

print "Hello\n";
来源：http://pv.jctech888.com.cn

[T42] Perl：变量类型
来源：http://vr.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tl.nicolike.cn

[T43] Perl：字符串插值
来源：http://qx.521024.cn

"值: $a"
来源：http://ze.lnxyls.cn

[T44] Perl：条件
来源：http://ym.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://mf.colortex.cn

[T45] Perl：数组遍历
来源：http://zb.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://gd.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://kn.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pq.hahajie.cn

[T47] Perl：正则捕获
来源：http://ec.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cz.lnxyls.cn

[T48] Perl：正则替换
来源：http://bv.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://xh.9csxet.cn

[T49] Perl：函数
来源：http://yy.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yv.asd995.cn

[T50] Perl：逐行读文件
来源：http://vw.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://su.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ik.gzmigu.cn

[T51] Scala：Hello World
来源：http://lb.asd995.cn

println("Hello")
来源：http://zg.huanxung.cn

[T52] Scala：变量
来源：http://tn.nicolike.cn

val a = 1;  var b = 2
来源：http://ss.hahajie.cn

[T53] Scala：字符串插值
来源：http://ts.szsharing.cn

s"值: $b"
来源：http://ve.colortex.cn

[T54] Scala：集合映射
来源：http://jj.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://gm.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://kq.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hi.panjiajie.cn

[T56] Scala：样例类
来源：http://dw.gzmigu.cn

case class User(name: String, age: Int)
来源：http://pr.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://hi.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://db.shxzukj.cn

[T58] Scala：函数定义
来源：http://jz.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kp.huixiangedu.cn

[T59] Scala：循环
来源：http://cx.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://fj.panjiajie.cn

[T60] Scala：折叠
来源：http://wx.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jr.asd995.cn

================================================================================
来源：http://jr.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nd.jianghongdianzi.cn

================================================================================
来源：http://od.asd995.cn

[U01] Py：创建虚拟环境
来源：http://ir.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wu.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://ma.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ky.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://ei.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://va.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://eu.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qh.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://ul.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://qy.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://zd.szxytkj.cn

{**a, **b}
来源：http://sk.shxzskj.cn

[U07] Py：反转字典键值
来源：http://vg.szsharing.cn

{v: k for k, v in d.items()}
来源：http://vv.szxytkj.cn

[U08] Py：展平二维列表
来源：http://io.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://zm.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://rn.newstarts.cn

max(d, key=d.get)
来源：http://hj.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://cv.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uy.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://kq.wgjwhj.cn

(x * 2 for x in arr)
来源：http://ih.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hb.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://bx.huanxung.cn

[U13] Py：固定长度队列
来源：http://do.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ma.asd995.cn

[U14] Py：分组收集到列表
来源：http://fy.colortex.cn

defaultdict(list)
来源：http://ws.huixiangedu.cn

[U15] Py：高精度计时
来源：http://he.hahajie.cn

t = time.perf_counter()
来源：http://ak.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://xk.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hv.yuexingan06.cn

[U17] Py：初始化日志
来源：http://mm.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://wg.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://wq.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://wj.asd995.cn

[U19] Py：正则替换带回调
来源：http://fj.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ts.huanxung.cn

[U20] Py：缓存函数结果
来源：http://yr.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://mc.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://sn.huanxung.cn

@contextlib.contextmanager
来源：http://bc.521024.cn

[U22] Py：矩阵转置
来源：http://gj.yuntaijiaju.cn

list(zip(*m))
来源：http://fv.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ru.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sb.muxihuayi.cn

[U24] Py：路径操作
来源：http://qi.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bj.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://aw.szsharing.cn

csv.DictReader(f)
来源：http://if.shxzskj.cn

[U26] Py：并发下载
来源：http://zi.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mc.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://yb.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://cb.newstarts.cn

[U28] Py：类型别名
来源：http://yy.jctech888.com.cn

UserId = int
来源：http://ja.shxzukj.cn

[U29] Py：属性校验
来源：http://gj.521024.cn

@property 与 @x.setter 配合
来源：http://nq.521024.cn

[U30] Py：数据类
来源：http://xl.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ez.9csxet.cn

[U31] Py：单测
来源：http://vs.asd995.cn

python -m pytest -q
来源：http://rt.chemitech.net.cn

[U32] Py：代码格式化
来源：http://nw.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://wa.newstarts.cn

[U33] Py：打包发布
来源：http://jr.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://vp.szxytkj.cn

[U34] Py：判断编码
来源：http://jn.bookmarksfly.cn

chardet.detect(raw)
来源：http://fv.muxihuayi.cn

[U35] Py：发送邮件
来源：http://om.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kz.newstarts.cn

[U36] Py：定时任务
来源：http://jf.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://gc.9csxet.cn

[U37] Py：读写 Excel
来源：http://eq.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rl.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://gk.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://xd.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://sd.shxzskj.cn

sys.stdout.isatty()
来源：http://xo.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://da.nicolike.cn

print("err", file=sys.stderr)
来源：http://bp.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://dv.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mw.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://bb.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ob.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://jg.yuntaijiaju.cn

namespace App\Http;
来源：http://uh.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://hb.shxzukj.cn

declare(strict_types=1);
来源：http://ki.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://sn.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nb.hahajie.cn

[U46] PHP：可空类型
来源：http://hm.gzmigu.cn

?string $name = null
来源：http://wx.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://lv.muxihuayi.cn

int|string $id
来源：http://yy.9csxet.cn

[U48] PHP：纯枚举
来源：http://zc.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://me.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://vn.jianghongdianzi.cn

public readonly string $name
来源：http://zd.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://al.shxzukj.cn

public function __construct(private int $id) {}
来源：http://rb.yuexingan06.cn

[U51] PHP：数组解构
来源：http://dd.huanxung.cn

[$a, $b] = $arr;
来源：http://vu.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://xf.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://ue.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://it.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://xx.shxzskj.cn

[U54] PHP：空安全调用
来源：http://fp.jianghongdianzi.cn

$obj?->method()
来源：http://bu.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://xo.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ey.asd995.cn

[U56] PHP：命名参数
来源：http://dn.huixiangedu.cn

f(a: 1, b: 2)
来源：http://lj.hahajie.cn

[U57] PHP：字符串插值
来源：http://rb.shxzukj.cn

"值: {$a}"
来源：http://na.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ik.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sd.nszjky.cn

[U59] PHP：自定义排序
来源：http://lw.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://na.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://yj.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kh.shxzukj.cn


<!-- 参考信息 -->