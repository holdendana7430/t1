代发 wailian999

[S43] C++：智能指针
来源：http://ol.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://is.szsharing.cn

[S44] C++：引用传参
来源：http://iu.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://md.shxzskj.cn

[S45] C++：lambda
来源：http://lr.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nf.nicolike.cn

[S46] C++：函数模板
来源：http://ly.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://em.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://jy.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vw.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://sl.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bz.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://vv.szxytkj.cn

[S49] C++：写文件
来源：http://em.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wb.yuexingan06.cn

[S50] C++：格式化数字
来源：http://tv.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zc.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://mx.hahajie.cn

static_cast<double>(a) / b
来源：http://qd.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://gk.hahajie.cn

int size() const noexcept { return n_; }
来源：http://xt.asd995.cn

[S53] C++：移动语义
来源：http://qe.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://ty.wgjwhj.cn

[S54] C++：异常处理
来源：http://wx.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bs.hahajie.cn

[S55] C++：结构化绑定
来源：http://zi.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mq.shxzukj.cn

[S56] C++：optional
来源：http://ax.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://og.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://um.yuntaijiaju.cn

constexpr int N = 10;
来源：http://rs.shxzskj.cn

[S58] C++：命名空间
来源：http://ni.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://in.colortex.cn

[S59] C++：静态断言
来源：http://rr.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vm.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://hg.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vz.gzmigu.cn

================================================================================
来源：http://rr.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wx.hahajie.cn

================================================================================
来源：http://lu.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://rx.szxytkj.cn

println("Hello")
来源：http://ww.panjiajie.cn

[T02] Kotlin：变量
来源：http://yz.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tl.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ma.muxihuayi.cn

"值: $b"
来源：http://xu.shxzukj.cn

[T04] Kotlin：空安全
来源：http://ew.nszjky.cn

val n: String? = null;  n?.length
来源：http://ok.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://bx.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rf.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://uu.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wb.asd995.cn

[T07] Kotlin：集合过滤
来源：http://yd.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uk.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ul.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://sw.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://wi.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://lf.colortex.cn

[T10] Kotlin：默认参数
来源：http://sj.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gd.haigaiapp.cn

[T11] Kotlin：协程
来源：http://nm.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hj.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://rl.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://az.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://gn.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://hu.hnjuh.cn

[T14] Kotlin：循环
来源：http://vj.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://hk.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://iv.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://xy.asd995.cn

[T16] Swift：Hello World
来源：http://qe.newstarts.cn

print("Hello")
来源：http://aq.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://lw.muxihuayi.cn

var a = 1;  let b = 2
来源：http://ln.hnjuh.cn

[T18] Swift：字符串插值
来源：http://ea.wgjwhj.cn

"值: \(b)"
来源：http://mt.colortex.cn

[T19] Swift：可选绑定
来源：http://ej.asd995.cn

if let n = opt { print(n) }
来源：http://rc.shtwfgs.cn

[T20] Swift：数组操作
来源：http://wx.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jx.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://xv.huanxung.cn

for x in a { print(x) }
来源：http://sk.huixiangedu.cn

[T22] Swift：字典
来源：http://tf.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xg.shxzskj.cn

[T23] Swift：函数
来源：http://bh.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ca.haigaiapp.cn

[T24] Swift：闭包
来源：http://at.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qw.gzmigu.cn

[T25] Swift：结构体
来源：http://kb.wgjwhj.cn

struct P { var x: Int }
来源：http://nl.9csxet.cn

[T26] Swift：类与重写
来源：http://pe.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://sk.9csxet.cn

[T27] Swift：错误处理
来源：http://ru.9csxet.cn

do { try f() } catch { print(error) }
来源：http://jk.wgjwhj.cn

[T28] Swift：枚举
来源：http://ls.panjiajie.cn

enum Color { case red, green }
来源：http://ct.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://zq.9csxet.cn

guard let x = opt else { return }
来源：http://cz.huixinmuqiang.cn

[T30] Swift：协议
来源：http://jf.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://wk.wgjwhj.cn

[T31] Lua：Hello World
来源：http://jn.newstarts.cn

print("Hello")
来源：http://oj.lnxyls.cn

[T32] Lua：局部变量
来源：http://ob.chemitech.net.cn

local a = 1
来源：http://cy.521024.cn

[T33] Lua：表（数组）
来源：http://vb.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dw.asd995.cn

[T34] Lua：遍历表
来源：http://ni.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dm.bjjhwx.cn

[T35] Lua：字典表
来源：http://jc.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://vj.bjjhwx.cn

[T36] Lua：函数
来源：http://ug.szxytkj.cn

function add(a, b) return a + b end
来源：http://dn.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://wy.jctech888.com.cn

"a" .. "b"
来源：http://yy.jctech888.com.cn

[T38] Lua：条件
来源：http://ko.hahajie.cn

if x > 0 then print("正") end
来源：http://nv.colortex.cn

[T39] Lua：模式匹配
来源：http://by.huixiangedu.cn

string.find(s, "%d+")
来源：http://nv.nicolike.cn

[T40] Lua：元表
来源：http://kp.colortex.cn

setmetatable({}, { __index = base })
来源：http://ur.hahajie.cn

[T41] Perl：Hello World
来源：http://ba.wgjwhj.cn

print "Hello\n";
来源：http://fw.panjiajie.cn

[T42] Perl：变量类型
来源：http://ya.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vu.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://qp.huixinmuqiang.cn

"值: $a"
来源：http://uy.9csxet.cn

[T44] Perl：条件
来源：http://eb.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://fb.nszjky.cn

[T45] Perl：数组遍历
来源：http://tr.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ea.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://ty.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hf.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://aj.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rx.lnxyls.cn

[T48] Perl：正则替换
来源：http://gh.9csxet.cn

$s =~ s/old/new/g;
来源：http://lc.hahajie.cn

[T49] Perl：函数
来源：http://yh.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rl.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://do.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://os.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://ym.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://pw.huixinmuqiang.cn

println("Hello")
来源：http://jv.huixinmuqiang.cn

[T52] Scala：变量
来源：http://yl.shxzskj.cn

val a = 1;  var b = 2
来源：http://zf.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://kz.wgjwhj.cn

s"值: $b"
来源：http://ps.newstarts.cn

[T54] Scala：集合映射
来源：http://vr.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://mf.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://kz.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ap.hnjuh.cn

[T56] Scala：样例类
来源：http://nq.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://xq.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ug.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fo.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://me.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ga.gzmigu.cn

[T59] Scala：循环
来源：http://pd.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://hb.hnjuh.cn

[T60] Scala：折叠
来源：http://zv.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vf.bjjhwx.cn

================================================================================
来源：http://nb.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://in.521024.cn

================================================================================
来源：http://nl.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://mp.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://li.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ut.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ln.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://qq.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qa.panjiajie.cn

[U04] Py：变量调试打印
来源：http://sa.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zs.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://xh.asd995.cn

list(dict.fromkeys(arr))
来源：http://fr.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://je.yuntaijiaju.cn

{**a, **b}
来源：http://hf.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://pk.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://sr.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://oi.bjjhwx.cn

[y for x in nested for y in x]
来源：http://ll.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://tp.huixiangedu.cn

max(d, key=d.get)
来源：http://cx.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://jv.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fh.huanxung.cn

[U11] Py：生成器表达式
来源：http://ro.muxihuayi.cn

(x * 2 for x in arr)
来源：http://xh.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gx.nicolike.cn

Counter(arr).most_common(3)
来源：http://hb.szxytkj.cn

[U13] Py：固定长度队列
来源：http://za.lnxyls.cn

deque(maxlen=10)
来源：http://nm.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://gg.wgjwhj.cn

defaultdict(list)
来源：http://zj.jctech888.com.cn

[U15] Py：高精度计时
来源：http://of.haigaiapp.cn

t = time.perf_counter()
来源：http://sz.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://zu.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xx.panjiajie.cn

[U17] Py：初始化日志
来源：http://yo.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ni.colortex.cn

[U18] Py：预编译正则
来源：http://tx.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ye.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://tz.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wp.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://gd.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://kr.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ce.colortex.cn

@contextlib.contextmanager
来源：http://ci.gzmigu.cn

[U22] Py：矩阵转置
来源：http://id.bjjhwx.cn

list(zip(*m))
来源：http://ot.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://xj.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aq.lnxyls.cn

[U24] Py：路径操作
来源：http://lg.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bq.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://zx.shxzskj.cn

csv.DictReader(f)
来源：http://il.yuexingan06.cn

[U26] Py：并发下载
来源：http://mx.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bw.nicolike.cn

[U27] Py：异步 HTTP
来源：http://lo.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://xt.nszjky.cn

[U28] Py：类型别名
来源：http://vu.bookmarksfly.cn

UserId = int
来源：http://ok.newstarts.cn

[U29] Py：属性校验
来源：http://of.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://pu.bookmarksfly.cn

[U30] Py：数据类
来源：http://ft.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://tx.wgjwhj.cn

[U31] Py：单测
来源：http://nh.colortex.cn

python -m pytest -q
来源：http://uw.szsharing.cn

[U32] Py：代码格式化
来源：http://du.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://dw.shxzukj.cn

[U33] Py：打包发布
来源：http://js.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ac.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://jt.jianghongdianzi.cn

chardet.detect(raw)
来源：http://bj.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://yx.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ba.9csxet.cn

[U36] Py：定时任务
来源：http://tm.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://lm.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://wh.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pf.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://jx.521024.cn

Path(__file__).resolve().parent
来源：http://qv.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://bx.gzmigu.cn

sys.stdout.isatty()
来源：http://cu.521024.cn

[U40] Py：打印到标准错误
来源：http://wc.9csxet.cn

print("err", file=sys.stderr)
来源：http://dh.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://tb.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eb.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://dr.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://or.colortex.cn

[U43] PHP：声明命名空间
来源：http://ez.521024.cn

namespace App\Http;
来源：http://dk.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://tj.shxzskj.cn

declare(strict_types=1);
来源：http://zf.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://zt.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://if.panjiajie.cn

[U46] PHP：可空类型
来源：http://ll.wgjwhj.cn

?string $name = null
来源：http://dw.wgjwhj.cn

[U47] PHP：联合类型
来源：http://cy.wgjwhj.cn

int|string $id
来源：http://pu.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://fl.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kf.bjjhwx.cn

[U49] PHP：只读属性
来源：http://wj.bookmarksfly.cn

public readonly string $name
来源：http://bo.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ud.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://ne.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ap.szxytkj.cn

[$a, $b] = $arr;
来源：http://ny.asd995.cn

[U52] PHP：箭头函数
来源：http://vt.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://yf.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://cn.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://vl.colortex.cn

[U54] PHP：空安全调用
来源：http://an.huixinmuqiang.cn

$obj?->method()
来源：http://yt.nszjky.cn

[U55] PHP：match 表达式
来源：http://ut.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ay.jctech888.com.cn

[U56] PHP：命名参数
来源：http://qa.szxytkj.cn

f(a: 1, b: 2)
来源：http://vj.9csxet.cn

[U57] PHP：字符串插值
来源：http://tp.szsharing.cn

"值: {$a}"
来源：http://ex.nszjky.cn

[U58] PHP：数组三件套
来源：http://mn.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ge.9csxet.cn

[U59] PHP：自定义排序
来源：http://jb.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ce.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://kd.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://he.szsharing.cn

[U61] PHP：正则
来源：http://pg.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wd.colortex.cn

[U62] PHP：日期对象
来源：http://jp.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bg.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://jq.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yh.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://ys.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://us.szsharing.cn

[U65] PHP：会话
来源：http://mg.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ed.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://cu.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ig.nicolike.cn

[U67] PHP：处理文件上传
来源：http://bf.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gs.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://jv.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ob.wgjwhj.cn


<!-- 参考信息 -->