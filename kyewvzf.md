代发 wailian999

[S39] C++：自定义比较器排序
来源：http://ou.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://al.gzmigu.cn

[S40] C++：查找元素
来源：http://nh.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ay.lnxyls.cn

[S41] C++：类与构造函数
来源：http://im.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cb.hahajie.cn

[S42] C++：继承与虚函数
来源：http://rr.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://fa.hahajie.cn

[S43] C++：智能指针
来源：http://bq.521024.cn

auto p = std::make_unique<int>(5);
来源：http://gn.colortex.cn

[S44] C++：引用传参
来源：http://of.521024.cn

void inc(int &x) { ++x; }
来源：http://sg.shxzskj.cn

[S45] C++：lambda
来源：http://zw.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ty.shxzskj.cn

[S46] C++：函数模板
来源：http://hw.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nq.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://cc.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jn.hahajie.cn

[S48] C++：逐行读文件
来源：http://ws.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ag.asd995.cn

while (std::getline(in, line)) { }
来源：http://dy.panjiajie.cn

[S49] C++：写文件
来源：http://bu.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://te.nszjky.cn

[S50] C++：格式化数字
来源：http://rk.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ak.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://lg.yuexingan06.cn

static_cast<double>(a) / b
来源：http://ak.colortex.cn

[S52] C++：const 与 noexcept
来源：http://sn.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://vc.muxihuayi.cn

[S53] C++：移动语义
来源：http://sj.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ny.muxihuayi.cn

[S54] C++：异常处理
来源：http://zl.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lm.521024.cn

[S55] C++：结构化绑定
来源：http://ie.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ru.nicolike.cn

[S56] C++：optional
来源：http://ff.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tj.muxihuayi.cn

[S57] C++：编译期常量
来源：http://op.newstarts.cn

constexpr int N = 10;
来源：http://ii.newstarts.cn

[S58] C++：命名空间
来源：http://oe.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://zr.nszjky.cn

[S59] C++：静态断言
来源：http://cp.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fm.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://mk.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jf.panjiajie.cn

================================================================================
来源：http://un.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lz.szsharing.cn

================================================================================
来源：http://zk.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://zg.jianghongdianzi.cn

println("Hello")
来源：http://mq.gzmigu.cn

[T02] Kotlin：变量
来源：http://ac.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pg.asd995.cn

[T03] Kotlin：字符串模板
来源：http://ue.nicolike.cn

"值: $b"
来源：http://bt.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://zt.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://os.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://lw.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qh.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://nc.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hy.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://kl.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nk.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://eo.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://qb.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://yz.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ug.nicolike.cn

[T10] Kotlin：默认参数
来源：http://uj.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rw.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://jy.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wi.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://mp.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://ac.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://cn.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://es.huanxung.cn

[T14] Kotlin：循环
来源：http://iw.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://tx.muxihuayi.cn

[T15] Kotlin：接口
来源：http://zq.asd995.cn

interface Shape { fun area(): Double }
来源：http://pu.shtwfgs.cn

[T16] Swift：Hello World
来源：http://dm.colortex.cn

print("Hello")
来源：http://cl.521024.cn

[T17] Swift：变量与常量
来源：http://il.huixiangedu.cn

var a = 1;  let b = 2
来源：http://lz.521024.cn

[T18] Swift：字符串插值
来源：http://xj.szxytkj.cn

"值: \(b)"
来源：http://xa.nszjky.cn

[T19] Swift：可选绑定
来源：http://hg.huixiangedu.cn

if let n = opt { print(n) }
来源：http://ga.521024.cn

[T20] Swift：数组操作
来源：http://qe.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ko.haigaiapp.cn

[T21] Swift：遍历
来源：http://cy.bjjhwx.cn

for x in a { print(x) }
来源：http://kq.huixiangedu.cn

[T22] Swift：字典
来源：http://wc.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qj.huixiangedu.cn

[T23] Swift：函数
来源：http://yl.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fz.panjiajie.cn

[T24] Swift：闭包
来源：http://ye.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lu.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://dv.szsharing.cn

struct P { var x: Int }
来源：http://kr.hnjuh.cn

[T26] Swift：类与重写
来源：http://qg.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://tt.521024.cn

[T27] Swift：错误处理
来源：http://me.9csxet.cn

do { try f() } catch { print(error) }
来源：http://ti.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://bl.szsharing.cn

enum Color { case red, green }
来源：http://qg.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://qg.wgjwhj.cn

guard let x = opt else { return }
来源：http://pg.bjjhwx.cn

[T30] Swift：协议
来源：http://gq.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://au.bjjhwx.cn

[T31] Lua：Hello World
来源：http://bi.bjjhwx.cn

print("Hello")
来源：http://sz.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://zm.9csxet.cn

local a = 1
来源：http://vm.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://vz.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fr.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://ni.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hk.shxzukj.cn

[T35] Lua：字典表
来源：http://ua.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://jb.jctech888.com.cn

[T36] Lua：函数
来源：http://bc.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://xb.9csxet.cn

[T37] Lua：字符串拼接
来源：http://nv.hnjuh.cn

"a" .. "b"
来源：http://ny.hahajie.cn

[T38] Lua：条件
来源：http://gh.hahajie.cn

if x > 0 then print("正") end
来源：http://ss.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://pz.huixiangedu.cn

string.find(s, "%d+")
来源：http://hq.newstarts.cn

[T40] Lua：元表
来源：http://xc.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://uc.huixiangedu.cn

[T41] Perl：Hello World
来源：http://yw.521024.cn

print "Hello\n";
来源：http://db.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://nr.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ym.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ef.hahajie.cn

"值: $a"
来源：http://mn.wgjwhj.cn

[T44] Perl：条件
来源：http://nr.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://ds.szxytkj.cn

[T45] Perl：数组遍历
来源：http://uh.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://jn.newstarts.cn

[T46] Perl：哈希操作
来源：http://zb.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://to.hnjuh.cn

[T47] Perl：正则捕获
来源：http://sd.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dt.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://wb.lnxyls.cn

$s =~ s/old/new/g;
来源：http://cl.szsharing.cn

[T49] Perl：函数
来源：http://vb.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vo.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://iz.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://px.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://go.shxzskj.cn

[T51] Scala：Hello World
来源：http://qd.hahajie.cn

println("Hello")
来源：http://vj.lnxyls.cn

[T52] Scala：变量
来源：http://by.chemitech.net.cn

val a = 1;  var b = 2
来源：http://by.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://bm.huixiangedu.cn

s"值: $b"
来源：http://oj.szxytkj.cn

[T54] Scala：集合映射
来源：http://yz.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ou.huanxung.cn

[T55] Scala：集合过滤
来源：http://cp.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ga.huanxung.cn

[T56] Scala：样例类
来源：http://lq.szxytkj.cn

case class User(name: String, age: Int)
来源：http://se.panjiajie.cn

[T57] Scala：模式匹配
来源：http://dm.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sp.shxzskj.cn

[T58] Scala：函数定义
来源：http://xi.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nc.wgjwhj.cn

[T59] Scala：循环
来源：http://lc.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://zp.szsharing.cn

[T60] Scala：折叠
来源：http://xg.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ag.521024.cn

================================================================================
来源：http://kv.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tr.szxytkj.cn

================================================================================
来源：http://wh.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://sh.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gm.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://pl.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oa.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://cz.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lr.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://ra.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ua.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://cj.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://vv.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://th.hahajie.cn

{**a, **b}
来源：http://vd.gzmigu.cn

[U07] Py：反转字典键值
来源：http://ed.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://zc.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://sf.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ui.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://ds.asd995.cn

max(d, key=d.get)
来源：http://sf.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://ni.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mw.521024.cn

[U11] Py：生成器表达式
来源：http://sg.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://ml.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mk.asd995.cn

Counter(arr).most_common(3)
来源：http://tn.hnjuh.cn

[U13] Py：固定长度队列
来源：http://un.haigaiapp.cn

deque(maxlen=10)
来源：http://il.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://cx.panjiajie.cn

defaultdict(list)
来源：http://ya.huixiangedu.cn

[U15] Py：高精度计时
来源：http://wg.yuexingan06.cn

t = time.perf_counter()
来源：http://ve.asd995.cn

[U16] Py：命令行参数解析
来源：http://ss.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ec.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://hq.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ss.hnjuh.cn

[U18] Py：预编译正则
来源：http://bq.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://ji.nszjky.cn

[U19] Py：正则替换带回调
来源：http://zd.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://al.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://tt.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://ka.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://jx.hnjuh.cn

@contextlib.contextmanager
来源：http://xp.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://ha.yuntaijiaju.cn

list(zip(*m))
来源：http://mj.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://nz.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ym.bookmarksfly.cn

[U24] Py：路径操作
来源：http://kz.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jt.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://xw.asd995.cn

csv.DictReader(f)
来源：http://hr.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://kf.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nl.huanxung.cn

[U27] Py：异步 HTTP
来源：http://su.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://fx.wgjwhj.cn

[U28] Py：类型别名
来源：http://qp.jctech888.com.cn

UserId = int
来源：http://aq.colortex.cn

[U29] Py：属性校验
来源：http://sx.panjiajie.cn

@property 与 @x.setter 配合
来源：http://um.yuexingan06.cn

[U30] Py：数据类
来源：http://xd.panjiajie.cn

@dataclass(slots=True)
来源：http://mi.newstarts.cn

[U31] Py：单测
来源：http://wb.colortex.cn

python -m pytest -q
来源：http://ch.lnxyls.cn

[U32] Py：代码格式化
来源：http://hk.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ly.shtwfgs.cn

[U33] Py：打包发布
来源：http://wb.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://vx.hahajie.cn

[U34] Py：判断编码
来源：http://fs.bookmarksfly.cn

chardet.detect(raw)
来源：http://mq.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://rc.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fq.shxzukj.cn

[U36] Py：定时任务
来源：http://zl.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://rq.colortex.cn

[U37] Py：读写 Excel
来源：http://cs.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ll.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://bh.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ld.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://mv.lnxyls.cn

sys.stdout.isatty()
来源：http://bl.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://hy.szxytkj.cn

print("err", file=sys.stderr)
来源：http://dt.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://iq.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ug.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ld.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uz.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://tz.shtwfgs.cn

namespace App\Http;
来源：http://sp.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://lg.bjjhwx.cn

declare(strict_types=1);
来源：http://hc.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://qh.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nq.shxzukj.cn

[U46] PHP：可空类型
来源：http://ud.huanxung.cn

?string $name = null
来源：http://fk.panjiajie.cn

[U47] PHP：联合类型
来源：http://ev.jianghongdianzi.cn

int|string $id
来源：http://zz.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://ww.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ml.lnxyls.cn

[U49] PHP：只读属性
来源：http://ze.haigaiapp.cn

public readonly string $name
来源：http://xm.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://av.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://rb.shxzukj.cn

[U51] PHP：数组解构
来源：http://ro.nszjky.cn

[$a, $b] = $arr;
来源：http://wz.gzmigu.cn

[U52] PHP：箭头函数
来源：http://op.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://rh.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://ef.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://gm.shxzskj.cn

[U54] PHP：空安全调用
来源：http://cl.hahajie.cn

$obj?->method()
来源：http://rd.asd995.cn

[U55] PHP：match 表达式
来源：http://gx.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hb.nicolike.cn

[U56] PHP：命名参数
来源：http://mx.asd995.cn

f(a: 1, b: 2)
来源：http://tr.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://ct.nicolike.cn

"值: {$a}"
来源：http://jn.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ji.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xa.9csxet.cn

[U59] PHP：自定义排序
来源：http://cv.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tp.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://tu.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zt.huixinmuqiang.cn

[U61] PHP：正则
来源：http://cx.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sq.colortex.cn

[U62] PHP：日期对象
来源：http://jp.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://og.asd995.cn

[U63] PHP：文件读写
来源：http://od.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cu.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://kf.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://ly.gzmigu.cn


<!-- 参考信息 -->