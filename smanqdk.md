代发 wailian999

[S33] C++：vector 增删
来源：http://xr.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://po.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://nt.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://vo.newstarts.cn

[S35] C++：map
来源：http://va.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qr.shxzukj.cn

[S36] C++：unordered_map
来源：http://ei.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iz.huanxung.cn

[S37] C++：set
来源：http://dg.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cx.shxzukj.cn

[S38] C++：排序
来源：http://ea.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://gu.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://wg.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pf.hahajie.cn

[S40] C++：查找元素
来源：http://bs.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vy.gzmigu.cn

[S41] C++：类与构造函数
来源：http://dy.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gt.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://am.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://fk.shxzskj.cn

[S43] C++：智能指针
来源：http://xd.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://br.shxzukj.cn

[S44] C++：引用传参
来源：http://mp.newstarts.cn

void inc(int &x) { ++x; }
来源：http://sl.muxihuayi.cn

[S45] C++：lambda
来源：http://es.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uq.nszjky.cn

[S46] C++：函数模板
来源：http://tr.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uo.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://uc.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ju.panjiajie.cn

[S48] C++：逐行读文件
来源：http://vo.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tp.newstarts.cn

while (std::getline(in, line)) { }
来源：http://tl.9csxet.cn

[S49] C++：写文件
来源：http://kn.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wa.huanxung.cn

[S50] C++：格式化数字
来源：http://af.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wm.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ql.jctech888.com.cn

static_cast<double>(a) / b
来源：http://gz.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://cy.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://bl.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://cp.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ah.huanxung.cn

[S54] C++：异常处理
来源：http://tm.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ns.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://zj.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://en.muxihuayi.cn

[S56] C++：optional
来源：http://rn.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yy.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://zp.shxzukj.cn

constexpr int N = 10;
来源：http://fq.gzmigu.cn

[S58] C++：命名空间
来源：http://va.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://kr.panjiajie.cn

[S59] C++：静态断言
来源：http://zd.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://as.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://yr.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gn.nicolike.cn

================================================================================
来源：http://tt.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qb.muxihuayi.cn

================================================================================
来源：http://fh.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://ci.yuntaijiaju.cn

println("Hello")
来源：http://vl.hnjuh.cn

[T02] Kotlin：变量
来源：http://eb.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://or.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://dw.hahajie.cn

"值: $b"
来源：http://aj.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://ee.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ud.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://oe.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yb.9csxet.cn

[T06] Kotlin：集合映射
来源：http://si.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qx.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ct.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qd.asd995.cn

[T08] Kotlin：数据类
来源：http://zg.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://ec.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://zs.colortex.cn

fun String.exclaim() = this + "!"
来源：http://hn.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ix.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gi.jctech888.com.cn

[T11] Kotlin：协程
来源：http://gy.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mh.521024.cn

[T12] Kotlin：解构声明
来源：http://dc.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://qd.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://zm.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://jm.hnjuh.cn

[T14] Kotlin：循环
来源：http://ff.nszjky.cn

for (i in 1..10) println(i)
来源：http://wv.521024.cn

[T15] Kotlin：接口
来源：http://wj.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://as.gzmigu.cn

[T16] Swift：Hello World
来源：http://jg.huanxung.cn

print("Hello")
来源：http://nl.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://bv.szsharing.cn

var a = 1;  let b = 2
来源：http://wb.521024.cn

[T18] Swift：字符串插值
来源：http://qb.panjiajie.cn

"值: \(b)"
来源：http://nv.shxzukj.cn

[T19] Swift：可选绑定
来源：http://be.gzmigu.cn

if let n = opt { print(n) }
来源：http://yy.nicolike.cn

[T20] Swift：数组操作
来源：http://ta.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wq.hnjuh.cn

[T21] Swift：遍历
来源：http://xj.szxytkj.cn

for x in a { print(x) }
来源：http://ed.chemitech.net.cn

[T22] Swift：字典
来源：http://zb.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lh.bookmarksfly.cn

[T23] Swift：函数
来源：http://uv.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ux.jctech888.com.cn

[T24] Swift：闭包
来源：http://xe.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hv.shtwfgs.cn

[T25] Swift：结构体
来源：http://eo.wgjwhj.cn

struct P { var x: Int }
来源：http://uu.jctech888.com.cn

[T26] Swift：类与重写
来源：http://qn.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://vu.szsharing.cn

[T27] Swift：错误处理
来源：http://gf.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ok.yuexingan06.cn

[T28] Swift：枚举
来源：http://to.huixinmuqiang.cn

enum Color { case red, green }
来源：http://ik.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://zv.shxzukj.cn

guard let x = opt else { return }
来源：http://ky.huixiangedu.cn

[T30] Swift：协议
来源：http://vl.asd995.cn

protocol Shape { func area() -> Double }
来源：http://pa.szsharing.cn

[T31] Lua：Hello World
来源：http://bk.nicolike.cn

print("Hello")
来源：http://hy.nszjky.cn

[T32] Lua：局部变量
来源：http://nc.521024.cn

local a = 1
来源：http://hr.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://wk.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ag.shxzukj.cn

[T34] Lua：遍历表
来源：http://nd.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yy.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://io.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://ff.9csxet.cn

[T36] Lua：函数
来源：http://jq.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ou.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://zq.szxytkj.cn

"a" .. "b"
来源：http://cx.colortex.cn

[T38] Lua：条件
来源：http://qh.huixiangedu.cn

if x > 0 then print("正") end
来源：http://dh.gzmigu.cn

[T39] Lua：模式匹配
来源：http://ck.chemitech.net.cn

string.find(s, "%d+")
来源：http://jc.colortex.cn

[T40] Lua：元表
来源：http://nq.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://qb.lnxyls.cn

[T41] Perl：Hello World
来源：http://hh.muxihuayi.cn

print "Hello\n";
来源：http://ze.521024.cn

[T42] Perl：变量类型
来源：http://qq.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qm.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://li.szsharing.cn

"值: $a"
来源：http://gk.bookmarksfly.cn

[T44] Perl：条件
来源：http://rm.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://ex.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://qf.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://qg.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://br.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qh.lnxyls.cn

[T47] Perl：正则捕获
来源：http://gs.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qg.szsharing.cn

[T48] Perl：正则替换
来源：http://vi.nicolike.cn

$s =~ s/old/new/g;
来源：http://ar.panjiajie.cn

[T49] Perl：函数
来源：http://lw.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ay.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://nd.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tn.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://fs.muxihuayi.cn

[T51] Scala：Hello World
来源：http://md.szsharing.cn

println("Hello")
来源：http://gp.szxytkj.cn

[T52] Scala：变量
来源：http://zn.wgjwhj.cn

val a = 1;  var b = 2
来源：http://dp.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://rz.newstarts.cn

s"值: $b"
来源：http://ec.huanxung.cn

[T54] Scala：集合映射
来源：http://xj.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://jd.asd995.cn

[T55] Scala：集合过滤
来源：http://ic.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oo.gzmigu.cn

[T56] Scala：样例类
来源：http://ms.hnjuh.cn

case class User(name: String, age: Int)
来源：http://ig.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://yt.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://do.yuexingan06.cn

[T58] Scala：函数定义
来源：http://oi.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://su.jctech888.com.cn

[T59] Scala：循环
来源：http://zu.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://yt.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://aw.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tw.muxihuayi.cn

================================================================================
来源：http://qz.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tk.muxihuayi.cn

================================================================================
来源：http://fw.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://bm.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jk.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://hq.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cb.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://ul.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://in.asd995.cn

[U04] Py：变量调试打印
来源：http://ec.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hf.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://bg.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://ho.nszjky.cn

[U06] Py：合并两个字典
来源：http://xf.gzmigu.cn

{**a, **b}
来源：http://qe.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://oo.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://rs.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://uq.szxytkj.cn

[y for x in nested for y in x]
来源：http://ie.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://zr.521024.cn

max(d, key=d.get)
来源：http://xn.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://jv.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vm.colortex.cn

[U11] Py：生成器表达式
来源：http://mo.jctech888.com.cn

(x * 2 for x in arr)
来源：http://ib.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nx.newstarts.cn

Counter(arr).most_common(3)
来源：http://jh.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://kk.jctech888.com.cn

deque(maxlen=10)
来源：http://cg.hahajie.cn

[U14] Py：分组收集到列表
来源：http://vn.bookmarksfly.cn

defaultdict(list)
来源：http://jd.jctech888.com.cn

[U15] Py：高精度计时
来源：http://bv.huanxung.cn

t = time.perf_counter()
来源：http://du.hahajie.cn

[U16] Py：命令行参数解析
来源：http://sz.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qm.hahajie.cn

[U17] Py：初始化日志
来源：http://rz.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://bj.hnjuh.cn

[U18] Py：预编译正则
来源：http://ud.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://rh.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://gm.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vx.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://jm.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ir.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://se.panjiajie.cn

@contextlib.contextmanager
来源：http://fa.hnjuh.cn

[U22] Py：矩阵转置
来源：http://xc.szsharing.cn

list(zip(*m))
来源：http://lw.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://pc.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fk.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://rx.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://js.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://ay.gzmigu.cn

csv.DictReader(f)
来源：http://mc.huanxung.cn

[U26] Py：并发下载
来源：http://iq.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jp.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://fp.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://qh.panjiajie.cn

[U28] Py：类型别名
来源：http://an.huanxung.cn

UserId = int
来源：http://ph.shtwfgs.cn

[U29] Py：属性校验
来源：http://sq.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://xa.521024.cn

[U30] Py：数据类
来源：http://ap.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://hd.shxzskj.cn

[U31] Py：单测
来源：http://vg.yuexingan06.cn

python -m pytest -q
来源：http://ax.nszjky.cn

[U32] Py：代码格式化
来源：http://jr.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://zc.haigaiapp.cn

[U33] Py：打包发布
来源：http://sh.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://gz.9csxet.cn

[U34] Py：判断编码
来源：http://kt.lnxyls.cn

chardet.detect(raw)
来源：http://bn.shxzskj.cn

[U35] Py：发送邮件
来源：http://pl.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ap.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ne.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://qz.colortex.cn

[U37] Py：读写 Excel
来源：http://ok.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ho.521024.cn

[U38] Py：获取脚本所在目录
来源：http://tf.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://je.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://fc.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://xt.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ty.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://vs.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://nn.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://af.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://ps.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qi.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://kc.huixiangedu.cn

namespace App\Http;
来源：http://eb.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://dt.hahajie.cn

declare(strict_types=1);
来源：http://le.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://kb.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://yx.nicolike.cn

?string $name = null
来源：http://rs.nszjky.cn

[U47] PHP：联合类型
来源：http://ig.yuexingan06.cn

int|string $id
来源：http://cc.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://kl.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zm.shtwfgs.cn

[U49] PHP：只读属性
来源：http://me.yuexingan06.cn

public readonly string $name
来源：http://rn.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://il.panjiajie.cn

public function __construct(private int $id) {}
来源：http://ao.panjiajie.cn

[U51] PHP：数组解构
来源：http://qy.szxytkj.cn

[$a, $b] = $arr;
来源：http://dy.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://zm.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://zl.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://ma.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://gd.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://gm.haigaiapp.cn

$obj?->method()
来源：http://xf.szsharing.cn

[U55] PHP：match 表达式
来源：http://sq.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oa.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://tk.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://xa.shxzukj.cn

[U57] PHP：字符串插值
来源：http://fl.asd995.cn

"值: {$a}"
来源：http://gv.nszjky.cn

[U58] PHP：数组三件套
来源：http://wq.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vq.szsharing.cn


<!-- 参考信息 -->