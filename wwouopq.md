代发 wailian999

[S35] C++：map
来源：http://ty.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lh.yuexingan06.cn

[S36] C++：unordered_map
来源：http://mx.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jt.521024.cn

[S37] C++：set
来源：http://xt.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eq.jctech888.com.cn

[S38] C++：排序
来源：http://pn.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://pi.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://lp.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ye.wgjwhj.cn

[S40] C++：查找元素
来源：http://cc.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ka.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://jq.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wp.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://pr.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://rq.colortex.cn

[S43] C++：智能指针
来源：http://kw.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://gh.bookmarksfly.cn

[S44] C++：引用传参
来源：http://bf.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://yp.yuexingan06.cn

[S45] C++：lambda
来源：http://pf.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xw.nicolike.cn

[S46] C++：函数模板
来源：http://ld.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gg.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://nn.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aq.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://rw.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zc.nszjky.cn

while (std::getline(in, line)) { }
来源：http://cl.gzmigu.cn

[S49] C++：写文件
来源：http://ff.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gx.nicolike.cn

[S50] C++：格式化数字
来源：http://oe.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://or.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://mi.bjjhwx.cn

static_cast<double>(a) / b
来源：http://lu.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://di.szsharing.cn

int size() const noexcept { return n_; }
来源：http://xi.gzmigu.cn

[S53] C++：移动语义
来源：http://gj.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://td.bjjhwx.cn

[S54] C++：异常处理
来源：http://ed.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://js.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://wk.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rn.yuntaijiaju.cn

[S56] C++：optional
来源：http://yu.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://na.521024.cn

[S57] C++：编译期常量
来源：http://pg.huixinmuqiang.cn

constexpr int N = 10;
来源：http://os.shxzskj.cn

[S58] C++：命名空间
来源：http://tl.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://rw.shxzukj.cn

[S59] C++：静态断言
来源：http://mb.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vl.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://gx.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dz.521024.cn

================================================================================
来源：http://se.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tq.chemitech.net.cn

================================================================================
来源：http://wh.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://os.szsharing.cn

println("Hello")
来源：http://qy.huanxung.cn

[T02] Kotlin：变量
来源：http://kc.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pj.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://rg.9csxet.cn

"值: $b"
来源：http://ao.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://gh.lnxyls.cn

val n: String? = null;  n?.length
来源：http://yz.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://ox.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fc.szsharing.cn

[T06] Kotlin：集合映射
来源：http://es.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uv.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://ay.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rm.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://de.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://gh.521024.cn

[T09] Kotlin：扩展函数
来源：http://fw.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://tz.huanxung.cn

[T10] Kotlin：默认参数
来源：http://vb.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.jctech888.com.cn

[T11] Kotlin：协程
来源：http://jh.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://km.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://ju.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://qj.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://ky.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://gy.panjiajie.cn

[T14] Kotlin：循环
来源：http://di.9csxet.cn

for (i in 1..10) println(i)
来源：http://sp.jctech888.com.cn

[T15] Kotlin：接口
来源：http://kk.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://kf.newstarts.cn

[T16] Swift：Hello World
来源：http://wv.nszjky.cn

print("Hello")
来源：http://vz.asd995.cn

[T17] Swift：变量与常量
来源：http://nj.wgjwhj.cn

var a = 1;  let b = 2
来源：http://uq.hahajie.cn

[T18] Swift：字符串插值
来源：http://uy.wgjwhj.cn

"值: \(b)"
来源：http://ev.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://cg.chemitech.net.cn

if let n = opt { print(n) }
来源：http://cv.panjiajie.cn

[T20] Swift：数组操作
来源：http://mu.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ln.yuexingan06.cn

[T21] Swift：遍历
来源：http://ve.gzmigu.cn

for x in a { print(x) }
来源：http://xf.shtwfgs.cn

[T22] Swift：字典
来源：http://dh.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dl.jctech888.com.cn

[T23] Swift：函数
来源：http://mo.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hk.gzmigu.cn

[T24] Swift：闭包
来源：http://bj.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ep.asd995.cn

[T25] Swift：结构体
来源：http://rt.bjjhwx.cn

struct P { var x: Int }
来源：http://qr.panjiajie.cn

[T26] Swift：类与重写
来源：http://fj.panjiajie.cn

class A: Base { override func f() {} }
来源：http://xi.wgjwhj.cn

[T27] Swift：错误处理
来源：http://by.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ob.gzmigu.cn

[T28] Swift：枚举
来源：http://mp.shtwfgs.cn

enum Color { case red, green }
来源：http://wt.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://af.bjjhwx.cn

guard let x = opt else { return }
来源：http://bd.jctech888.com.cn

[T30] Swift：协议
来源：http://bv.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://hx.9csxet.cn

[T31] Lua：Hello World
来源：http://pi.jctech888.com.cn

print("Hello")
来源：http://qs.muxihuayi.cn

[T32] Lua：局部变量
来源：http://zh.szsharing.cn

local a = 1
来源：http://wb.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://gw.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rx.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://zu.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bh.shtwfgs.cn

[T35] Lua：字典表
来源：http://re.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://te.9csxet.cn

[T36] Lua：函数
来源：http://lk.chemitech.net.cn

function add(a, b) return a + b end
来源：http://rz.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://ap.asd995.cn

"a" .. "b"
来源：http://bc.yuexingan06.cn

[T38] Lua：条件
来源：http://ye.chemitech.net.cn

if x > 0 then print("正") end
来源：http://xd.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ox.shtwfgs.cn

string.find(s, "%d+")
来源：http://ht.colortex.cn

[T40] Lua：元表
来源：http://vr.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://xa.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://xm.shxzskj.cn

print "Hello\n";
来源：http://wd.nszjky.cn

[T42] Perl：变量类型
来源：http://cc.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sb.9csxet.cn

[T43] Perl：字符串插值
来源：http://nd.szsharing.cn

"值: $a"
来源：http://pd.bjjhwx.cn

[T44] Perl：条件
来源：http://kl.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://sj.huanxung.cn

[T45] Perl：数组遍历
来源：http://lr.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://th.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://zv.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mg.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://nz.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sc.9csxet.cn

[T48] Perl：正则替换
来源：http://ss.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://gn.colortex.cn

[T49] Perl：函数
来源：http://sv.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wp.asd995.cn

[T50] Perl：逐行读文件
来源：http://vy.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eu.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://qp.colortex.cn

[T51] Scala：Hello World
来源：http://kr.521024.cn

println("Hello")
来源：http://tq.gzmigu.cn

[T52] Scala：变量
来源：http://eh.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://ak.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://ox.newstarts.cn

s"值: $b"
来源：http://jx.panjiajie.cn

[T54] Scala：集合映射
来源：http://tu.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://lc.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ph.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ro.yuexingan06.cn

[T56] Scala：样例类
来源：http://ze.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://vt.shxzukj.cn

[T57] Scala：模式匹配
来源：http://sx.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dy.shxzskj.cn

[T58] Scala：函数定义
来源：http://pz.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zz.huixiangedu.cn

[T59] Scala：循环
来源：http://zu.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://qb.colortex.cn

[T60] Scala：折叠
来源：http://ti.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://an.huixinmuqiang.cn

================================================================================
来源：http://id.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uu.yuexingan06.cn

================================================================================
来源：http://xo.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ou.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wt.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://dw.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ox.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://we.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ut.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://bo.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ab.newstarts.cn

[U05] Py：列表去重且保序
来源：http://ts.hahajie.cn

list(dict.fromkeys(arr))
来源：http://fg.shxzskj.cn

[U06] Py：合并两个字典
来源：http://sk.panjiajie.cn

{**a, **b}
来源：http://nm.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://ik.asd995.cn

{v: k for k, v in d.items()}
来源：http://gm.huanxung.cn

[U08] Py：展平二维列表
来源：http://qu.lnxyls.cn

[y for x in nested for y in x]
来源：http://wb.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://jb.bookmarksfly.cn

max(d, key=d.get)
来源：http://qw.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://pd.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zs.521024.cn

[U11] Py：生成器表达式
来源：http://ai.lnxyls.cn

(x * 2 for x in arr)
来源：http://yp.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gj.521024.cn

Counter(arr).most_common(3)
来源：http://ci.newstarts.cn

[U13] Py：固定长度队列
来源：http://ph.szsharing.cn

deque(maxlen=10)
来源：http://kk.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://lp.nicolike.cn

defaultdict(list)
来源：http://nw.nicolike.cn

[U15] Py：高精度计时
来源：http://rf.9csxet.cn

t = time.perf_counter()
来源：http://xt.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://pp.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hv.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ck.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://hh.nszjky.cn

[U18] Py：预编译正则
来源：http://ic.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ek.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://co.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qv.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://lm.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://ap.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://lz.gzmigu.cn

@contextlib.contextmanager
来源：http://gh.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://ca.bookmarksfly.cn

list(zip(*m))
来源：http://wf.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://zn.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wu.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://tn.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kt.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://ur.bookmarksfly.cn

csv.DictReader(f)
来源：http://ls.bookmarksfly.cn

[U26] Py：并发下载
来源：http://qd.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jr.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://lj.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ei.szsharing.cn

[U28] Py：类型别名
来源：http://rc.szsharing.cn

UserId = int
来源：http://jl.haigaiapp.cn

[U29] Py：属性校验
来源：http://wl.colortex.cn

@property 与 @x.setter 配合
来源：http://up.colortex.cn

[U30] Py：数据类
来源：http://io.newstarts.cn

@dataclass(slots=True)
来源：http://qx.yuexingan06.cn

[U31] Py：单测
来源：http://dc.nicolike.cn

python -m pytest -q
来源：http://hv.9csxet.cn

[U32] Py：代码格式化
来源：http://rc.szsharing.cn

ruff format . && ruff check --fix .
来源：http://bj.chemitech.net.cn

[U33] Py：打包发布
来源：http://ue.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://zd.chemitech.net.cn

[U34] Py：判断编码
来源：http://wo.nszjky.cn

chardet.detect(raw)
来源：http://yc.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://rb.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oj.chemitech.net.cn

[U36] Py：定时任务
来源：http://ij.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://kv.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://ii.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jx.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://fc.521024.cn

Path(__file__).resolve().parent
来源：http://rl.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://fg.gzmigu.cn

sys.stdout.isatty()
来源：http://ga.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://cy.panjiajie.cn

print("err", file=sys.stderr)
来源：http://qs.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://ag.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xd.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://dq.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ok.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://xx.bjjhwx.cn

namespace App\Http;
来源：http://tm.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://he.jctech888.com.cn

declare(strict_types=1);
来源：http://uq.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://bc.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://re.nicolike.cn

[U46] PHP：可空类型
来源：http://hi.haigaiapp.cn

?string $name = null
来源：http://iq.huanxung.cn

[U47] PHP：联合类型
来源：http://fn.huixinmuqiang.cn

int|string $id
来源：http://lh.szsharing.cn

[U48] PHP：纯枚举
来源：http://mv.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ux.asd995.cn

[U49] PHP：只读属性
来源：http://zg.bjjhwx.cn

public readonly string $name
来源：http://jz.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://ad.newstarts.cn

public function __construct(private int $id) {}
来源：http://ty.muxihuayi.cn

[U51] PHP：数组解构
来源：http://tl.panjiajie.cn

[$a, $b] = $arr;
来源：http://ob.szxytkj.cn

[U52] PHP：箭头函数
来源：http://uo.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://fv.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://eh.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://zk.gzmigu.cn

[U54] PHP：空安全调用
来源：http://dh.shxzskj.cn

$obj?->method()
来源：http://lg.521024.cn

[U55] PHP：match 表达式
来源：http://pk.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fp.wgjwhj.cn

[U56] PHP：命名参数
来源：http://vu.panjiajie.cn

f(a: 1, b: 2)
来源：http://qm.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://ee.shxzukj.cn

"值: {$a}"
来源：http://tc.9csxet.cn

[U58] PHP：数组三件套
来源：http://cl.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bd.521024.cn

[U59] PHP：自定义排序
来源：http://tw.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uu.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://uy.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rv.yuntaijiaju.cn


<!-- 参考信息 -->