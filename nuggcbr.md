代发 wailian999

[S45] C++：lambda
来源：http://gw.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qi.yuexingan06.cn

[S46] C++：函数模板
来源：http://wb.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://de.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://cp.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ks.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ci.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bl.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://rf.gzmigu.cn

[S49] C++：写文件
来源：http://wf.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cv.521024.cn

[S50] C++：格式化数字
来源：http://ye.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mr.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://yx.chemitech.net.cn

static_cast<double>(a) / b
来源：http://ms.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://bx.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://vy.gzmigu.cn

[S53] C++：移动语义
来源：http://pl.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://mu.shtwfgs.cn

[S54] C++：异常处理
来源：http://hm.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bn.nszjky.cn

[S55] C++：结构化绑定
来源：http://pp.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sm.panjiajie.cn

[S56] C++：optional
来源：http://or.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vd.shtwfgs.cn

[S57] C++：编译期常量
来源：http://po.nszjky.cn

constexpr int N = 10;
来源：http://gx.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://xk.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://no.hnjuh.cn

[S59] C++：静态断言
来源：http://fg.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dy.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://jx.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ed.nszjky.cn

================================================================================
来源：http://ly.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ds.nicolike.cn

================================================================================
来源：http://ee.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://pf.521024.cn

println("Hello")
来源：http://bm.chemitech.net.cn

[T02] Kotlin：变量
来源：http://bv.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iw.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://sl.shxzskj.cn

"值: $b"
来源：http://do.hahajie.cn

[T04] Kotlin：空安全
来源：http://fk.nicolike.cn

val n: String? = null;  n?.length
来源：http://bt.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://br.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lv.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://np.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tp.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://xk.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ca.lnxyls.cn

[T08] Kotlin：数据类
来源：http://oo.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://lf.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://dw.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://wu.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ri.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tv.colortex.cn

[T11] Kotlin：协程
来源：http://nl.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bp.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://va.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://zt.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://xj.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://kb.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://ua.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://kn.hahajie.cn

[T15] Kotlin：接口
来源：http://bk.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://bf.shtwfgs.cn

[T16] Swift：Hello World
来源：http://nv.szsharing.cn

print("Hello")
来源：http://ys.szsharing.cn

[T17] Swift：变量与常量
来源：http://lo.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://wz.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ab.hahajie.cn

"值: \(b)"
来源：http://cw.nszjky.cn

[T19] Swift：可选绑定
来源：http://bs.colortex.cn

if let n = opt { print(n) }
来源：http://bw.szsharing.cn

[T20] Swift：数组操作
来源：http://jy.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kw.panjiajie.cn

[T21] Swift：遍历
来源：http://sj.hnjuh.cn

for x in a { print(x) }
来源：http://rm.huixiangedu.cn

[T22] Swift：字典
来源：http://ny.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ut.jianghongdianzi.cn

[T23] Swift：函数
来源：http://mz.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fv.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://qg.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vb.yuexingan06.cn

[T25] Swift：结构体
来源：http://ri.hahajie.cn

struct P { var x: Int }
来源：http://ti.hnjuh.cn

[T26] Swift：类与重写
来源：http://lk.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ed.nszjky.cn

[T27] Swift：错误处理
来源：http://xh.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://ad.shtwfgs.cn

[T28] Swift：枚举
来源：http://rz.shtwfgs.cn

enum Color { case red, green }
来源：http://oi.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://iu.muxihuayi.cn

guard let x = opt else { return }
来源：http://ut.panjiajie.cn

[T30] Swift：协议
来源：http://yk.colortex.cn

protocol Shape { func area() -> Double }
来源：http://mh.wgjwhj.cn

[T31] Lua：Hello World
来源：http://xw.bookmarksfly.cn

print("Hello")
来源：http://hb.521024.cn

[T32] Lua：局部变量
来源：http://vc.hnjuh.cn

local a = 1
来源：http://hk.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://uy.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hk.bjjhwx.cn

[T34] Lua：遍历表
来源：http://zv.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jg.yuexingan06.cn

[T35] Lua：字典表
来源：http://bh.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://aj.huanxung.cn

[T36] Lua：函数
来源：http://bi.nicolike.cn

function add(a, b) return a + b end
来源：http://ak.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://rc.yuexingan06.cn

"a" .. "b"
来源：http://sc.panjiajie.cn

[T38] Lua：条件
来源：http://oh.huixiangedu.cn

if x > 0 then print("正") end
来源：http://dd.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://eg.yuexingan06.cn

string.find(s, "%d+")
来源：http://jd.huixinmuqiang.cn

[T40] Lua：元表
来源：http://jo.colortex.cn

setmetatable({}, { __index = base })
来源：http://fs.hnjuh.cn

[T41] Perl：Hello World
来源：http://dv.huixiangedu.cn

print "Hello\n";
来源：http://gb.shtwfgs.cn

[T42] Perl：变量类型
来源：http://qr.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mf.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://ir.hahajie.cn

"值: $a"
来源：http://dg.asd995.cn

[T44] Perl：条件
来源：http://yb.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://jd.gzmigu.cn

[T45] Perl：数组遍历
来源：http://lg.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://ff.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ha.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://up.521024.cn

[T47] Perl：正则捕获
来源：http://kt.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://he.chemitech.net.cn

[T48] Perl：正则替换
来源：http://hy.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://vh.huixiangedu.cn

[T49] Perl：函数
来源：http://ic.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lu.colortex.cn

[T50] Perl：逐行读文件
来源：http://fe.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ko.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://fx.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://ba.colortex.cn

println("Hello")
来源：http://pv.newstarts.cn

[T52] Scala：变量
来源：http://nn.521024.cn

val a = 1;  var b = 2
来源：http://xq.521024.cn

[T53] Scala：字符串插值
来源：http://tt.huixiangedu.cn

s"值: $b"
来源：http://io.muxihuayi.cn

[T54] Scala：集合映射
来源：http://wh.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://bs.gzmigu.cn

[T55] Scala：集合过滤
来源：http://tg.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zs.szsharing.cn

[T56] Scala：样例类
来源：http://qh.hnjuh.cn

case class User(name: String, age: Int)
来源：http://fo.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://ux.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gw.colortex.cn

[T58] Scala：函数定义
来源：http://ig.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vn.lnxyls.cn

[T59] Scala：循环
来源：http://yh.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://cq.521024.cn

[T60] Scala：折叠
来源：http://qq.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ox.huixiangedu.cn

================================================================================
来源：http://dt.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cb.huanxung.cn

================================================================================
来源：http://um.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://du.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dh.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://oc.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rb.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://br.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bs.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://wb.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pf.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://yz.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://vk.nszjky.cn

[U06] Py：合并两个字典
来源：http://ng.shxzukj.cn

{**a, **b}
来源：http://nf.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://mj.asd995.cn

{v: k for k, v in d.items()}
来源：http://yq.panjiajie.cn

[U08] Py：展平二维列表
来源：http://fg.muxihuayi.cn

[y for x in nested for y in x]
来源：http://hc.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://gf.hnjuh.cn

max(d, key=d.get)
来源：http://fv.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://ls.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iz.shxzskj.cn

[U11] Py：生成器表达式
来源：http://xb.szsharing.cn

(x * 2 for x in arr)
来源：http://xg.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yl.nszjky.cn

Counter(arr).most_common(3)
来源：http://ec.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://qf.lnxyls.cn

deque(maxlen=10)
来源：http://gp.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://fe.huixiangedu.cn

defaultdict(list)
来源：http://oh.lnxyls.cn

[U15] Py：高精度计时
来源：http://fr.bookmarksfly.cn

t = time.perf_counter()
来源：http://th.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://wu.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ug.nicolike.cn

[U17] Py：初始化日志
来源：http://vh.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://mm.haigaiapp.cn

[U18] Py：预编译正则
来源：http://pc.newstarts.cn

pat = re.compile(r"\d+")
来源：http://vg.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://io.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yg.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://ds.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://nw.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://qy.panjiajie.cn

@contextlib.contextmanager
来源：http://fj.huanxung.cn

[U22] Py：矩阵转置
来源：http://qm.lnxyls.cn

list(zip(*m))
来源：http://li.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ni.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sz.9csxet.cn

[U24] Py：路径操作
来源：http://iq.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gq.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://vx.huixinmuqiang.cn

csv.DictReader(f)
来源：http://oh.shxzskj.cn

[U26] Py：并发下载
来源：http://nj.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pt.521024.cn

[U27] Py：异步 HTTP
来源：http://do.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://hx.huanxung.cn

[U28] Py：类型别名
来源：http://aq.shxzskj.cn

UserId = int
来源：http://yh.bookmarksfly.cn

[U29] Py：属性校验
来源：http://sb.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://za.nicolike.cn

[U30] Py：数据类
来源：http://wx.asd995.cn

@dataclass(slots=True)
来源：http://zy.bookmarksfly.cn

[U31] Py：单测
来源：http://pm.asd995.cn

python -m pytest -q
来源：http://tj.huanxung.cn

[U32] Py：代码格式化
来源：http://ig.colortex.cn

ruff format . && ruff check --fix .
来源：http://qc.521024.cn

[U33] Py：打包发布
来源：http://sw.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://fd.huanxung.cn

[U34] Py：判断编码
来源：http://xw.asd995.cn

chardet.detect(raw)
来源：http://gv.huixiangedu.cn

[U35] Py：发送邮件
来源：http://jo.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yv.chemitech.net.cn

[U36] Py：定时任务
来源：http://ib.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://ak.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://qz.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ua.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://ki.shxzskj.cn

Path(__file__).resolve().parent
来源：http://jh.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://kd.huanxung.cn

sys.stdout.isatty()
来源：http://qg.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://tv.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://bp.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xq.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://es.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://oj.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ty.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://gk.asd995.cn

namespace App\Http;
来源：http://vn.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://yb.9csxet.cn

declare(strict_types=1);
来源：http://jm.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://qd.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://if.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://jl.lnxyls.cn

?string $name = null
来源：http://du.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://vs.jianghongdianzi.cn

int|string $id
来源：http://wz.nszjky.cn

[U48] PHP：纯枚举
来源：http://hh.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mk.haigaiapp.cn

[U49] PHP：只读属性
来源：http://rr.hahajie.cn

public readonly string $name
来源：http://mw.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://pr.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ss.jctech888.com.cn

[U51] PHP：数组解构
来源：http://qu.shtwfgs.cn

[$a, $b] = $arr;
来源：http://ek.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://xd.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://ly.huanxung.cn

[U53] PHP：空合并运算符
来源：http://ja.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://he.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://wb.shxzukj.cn

$obj?->method()
来源：http://wv.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://cf.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://py.yuexingan06.cn

[U56] PHP：命名参数
来源：http://kh.shtwfgs.cn

f(a: 1, b: 2)
来源：http://bd.huanxung.cn

[U57] PHP：字符串插值
来源：http://hx.szsharing.cn

"值: {$a}"
来源：http://st.panjiajie.cn

[U58] PHP：数组三件套
来源：http://jf.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xi.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://rx.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zz.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://eo.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tx.asd995.cn

[U61] PHP：正则
来源：http://tx.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ed.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ih.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qk.shtwfgs.cn

[U63] PHP：文件读写
来源：http://ir.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://td.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://vq.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://we.hnjuh.cn

[U65] PHP：会话
来源：http://hb.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dr.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://wv.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hb.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://ci.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jl.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://uz.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iq.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://fg.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hp.asd995.cn

[U70] PHP：PDO 事务
来源：http://ta.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dq.yuexingan06.cn


<!-- 参考信息 -->