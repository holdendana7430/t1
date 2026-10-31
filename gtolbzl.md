代发 wailian999

[S45] C++：lambda
来源：http://cc.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qt.jctech888.com.cn

[S46] C++：函数模板
来源：http://bu.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://so.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://mw.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xa.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://xl.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fb.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://ip.chemitech.net.cn

[S49] C++：写文件
来源：http://oh.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ga.gzmigu.cn

[S50] C++：格式化数字
来源：http://xr.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ry.huanxung.cn

[S51] C++：显式类型转换
来源：http://qk.haigaiapp.cn

static_cast<double>(a) / b
来源：http://qx.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://hm.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://yg.nicolike.cn

[S53] C++：移动语义
来源：http://zw.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://aj.bookmarksfly.cn

[S54] C++：异常处理
来源：http://jv.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rr.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://vl.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wj.colortex.cn

[S56] C++：optional
来源：http://ij.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lm.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://do.huanxung.cn

constexpr int N = 10;
来源：http://yt.muxihuayi.cn

[S58] C++：命名空间
来源：http://jz.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://jk.521024.cn

[S59] C++：静态断言
来源：http://lh.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ad.colortex.cn

[S60] C++：遍历并删除元素
来源：http://le.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://il.szsharing.cn

================================================================================
来源：http://gg.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://md.gzmigu.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://hi.shxzukj.cn

println("Hello")
来源：http://em.9csxet.cn

[T02] Kotlin：变量
来源：http://qk.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ob.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://ef.hahajie.cn

"值: $b"
来源：http://cm.shxzukj.cn

[T04] Kotlin：空安全
来源：http://tq.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://fm.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://tx.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ym.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://yv.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vg.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://vj.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pa.gzmigu.cn

[T08] Kotlin：数据类
来源：http://vn.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://mi.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://zq.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://ip.521024.cn

[T10] Kotlin：默认参数
来源：http://gs.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pz.jctech888.com.cn

[T11] Kotlin：协程
来源：http://aa.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vw.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://ls.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://uf.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://dh.hahajie.cn

val m = mapOf("a" to 1)
来源：http://sq.colortex.cn

[T14] Kotlin：循环
来源：http://oy.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://wq.shtwfgs.cn

[T15] Kotlin：接口
来源：http://bn.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://uw.nszjky.cn

[T16] Swift：Hello World
来源：http://cl.hnjuh.cn

print("Hello")
来源：http://td.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://ig.nszjky.cn

var a = 1;  let b = 2
来源：http://ng.colortex.cn

[T18] Swift：字符串插值
来源：http://xa.szxytkj.cn

"值: \(b)"
来源：http://nj.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://li.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://ck.chemitech.net.cn

[T20] Swift：数组操作
来源：http://xn.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iw.nicolike.cn

[T21] Swift：遍历
来源：http://pj.shxzukj.cn

for x in a { print(x) }
来源：http://es.hnjuh.cn

[T22] Swift：字典
来源：http://le.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ad.panjiajie.cn

[T23] Swift：函数
来源：http://sb.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rd.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://uj.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dy.shxzskj.cn

[T25] Swift：结构体
来源：http://mf.huixinmuqiang.cn

struct P { var x: Int }
来源：http://ic.asd995.cn

[T26] Swift：类与重写
来源：http://fv.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://qo.colortex.cn

[T27] Swift：错误处理
来源：http://ic.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://xi.muxihuayi.cn

[T28] Swift：枚举
来源：http://ns.nicolike.cn

enum Color { case red, green }
来源：http://kc.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://ud.9csxet.cn

guard let x = opt else { return }
来源：http://hp.nicolike.cn

[T30] Swift：协议
来源：http://ju.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://wf.panjiajie.cn

[T31] Lua：Hello World
来源：http://ci.gzmigu.cn

print("Hello")
来源：http://wy.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://ap.huanxung.cn

local a = 1
来源：http://oc.shxzukj.cn

[T33] Lua：表（数组）
来源：http://qg.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zv.shtwfgs.cn

[T34] Lua：遍历表
来源：http://ln.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ix.muxihuayi.cn

[T35] Lua：字典表
来源：http://je.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://bi.shxzukj.cn

[T36] Lua：函数
来源：http://gf.9csxet.cn

function add(a, b) return a + b end
来源：http://al.nicolike.cn

[T37] Lua：字符串拼接
来源：http://uk.colortex.cn

"a" .. "b"
来源：http://cx.muxihuayi.cn

[T38] Lua：条件
来源：http://us.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ku.521024.cn

[T39] Lua：模式匹配
来源：http://nn.nicolike.cn

string.find(s, "%d+")
来源：http://kp.shxzukj.cn

[T40] Lua：元表
来源：http://kn.asd995.cn

setmetatable({}, { __index = base })
来源：http://cd.hnjuh.cn

[T41] Perl：Hello World
来源：http://ao.shxzskj.cn

print "Hello\n";
来源：http://eh.lnxyls.cn

[T42] Perl：变量类型
来源：http://ab.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eh.shxzukj.cn

[T43] Perl：字符串插值
来源：http://hy.nicolike.cn

"值: $a"
来源：http://tn.jianghongdianzi.cn

[T44] Perl：条件
来源：http://ts.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://hf.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://qa.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ib.hahajie.cn

[T46] Perl：哈希操作
来源：http://qf.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://se.newstarts.cn

[T47] Perl：正则捕获
来源：http://nm.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dp.521024.cn

[T48] Perl：正则替换
来源：http://mt.shxzskj.cn

$s =~ s/old/new/g;
来源：http://yg.jianghongdianzi.cn

[T49] Perl：函数
来源：http://au.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ti.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://jb.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uv.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://bo.hahajie.cn

[T51] Scala：Hello World
来源：http://ju.jianghongdianzi.cn

println("Hello")
来源：http://cr.jctech888.com.cn

[T52] Scala：变量
来源：http://if.yuexingan06.cn

val a = 1;  var b = 2
来源：http://bs.nszjky.cn

[T53] Scala：字符串插值
来源：http://td.jianghongdianzi.cn

s"值: $b"
来源：http://uh.gzmigu.cn

[T54] Scala：集合映射
来源：http://ce.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://qr.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://sp.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qg.gzmigu.cn

[T56] Scala：样例类
来源：http://te.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://wd.asd995.cn

[T57] Scala：模式匹配
来源：http://so.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vx.shtwfgs.cn

[T58] Scala：函数定义
来源：http://uf.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rx.jctech888.com.cn

[T59] Scala：循环
来源：http://rh.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://pe.shtwfgs.cn

[T60] Scala：折叠
来源：http://li.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fz.shtwfgs.cn

================================================================================
来源：http://cm.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aa.gzmigu.cn

================================================================================
来源：http://rc.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://fs.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yy.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://dz.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://in.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://bg.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ro.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://se.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qd.newstarts.cn

[U05] Py：列表去重且保序
来源：http://dk.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ip.521024.cn

[U06] Py：合并两个字典
来源：http://oi.gzmigu.cn

{**a, **b}
来源：http://nr.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://db.hahajie.cn

{v: k for k, v in d.items()}
来源：http://ll.nicolike.cn

[U08] Py：展平二维列表
来源：http://xo.lnxyls.cn

[y for x in nested for y in x]
来源：http://rj.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://xt.huanxung.cn

max(d, key=d.get)
来源：http://vp.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://ne.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jl.hahajie.cn

[U11] Py：生成器表达式
来源：http://dl.521024.cn

(x * 2 for x in arr)
来源：http://lg.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bw.hahajie.cn

Counter(arr).most_common(3)
来源：http://ru.nicolike.cn

[U13] Py：固定长度队列
来源：http://li.gzmigu.cn

deque(maxlen=10)
来源：http://ro.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://bw.chemitech.net.cn

defaultdict(list)
来源：http://ot.chemitech.net.cn

[U15] Py：高精度计时
来源：http://ko.hnjuh.cn

t = time.perf_counter()
来源：http://aj.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://vg.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bd.yuexingan06.cn

[U17] Py：初始化日志
来源：http://fs.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://ry.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://zy.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://ts.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://wt.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qw.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ma.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://pc.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://qw.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://pa.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://ap.wgjwhj.cn

list(zip(*m))
来源：http://ze.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ix.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yf.asd995.cn

[U24] Py：路径操作
来源：http://ew.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bc.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://rd.huixiangedu.cn

csv.DictReader(f)
来源：http://ed.521024.cn

[U26] Py：并发下载
来源：http://rb.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://do.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://yk.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://db.chemitech.net.cn

[U28] Py：类型别名
来源：http://gs.bookmarksfly.cn

UserId = int
来源：http://ar.9csxet.cn

[U29] Py：属性校验
来源：http://gz.szxytkj.cn

@property 与 @x.setter 配合
来源：http://kl.chemitech.net.cn

[U30] Py：数据类
来源：http://sd.huanxung.cn

@dataclass(slots=True)
来源：http://wt.hnjuh.cn

[U31] Py：单测
来源：http://hp.yuexingan06.cn

python -m pytest -q
来源：http://ga.asd995.cn

[U32] Py：代码格式化
来源：http://hn.nszjky.cn

ruff format . && ruff check --fix .
来源：http://gd.nicolike.cn

[U33] Py：打包发布
来源：http://tm.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://pf.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://dz.bjjhwx.cn

chardet.detect(raw)
来源：http://cw.hahajie.cn

[U35] Py：发送邮件
来源：http://rd.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ne.colortex.cn

[U36] Py：定时任务
来源：http://nm.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://bn.521024.cn

[U37] Py：读写 Excel
来源：http://aw.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ft.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://ww.hahajie.cn

Path(__file__).resolve().parent
来源：http://st.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://lh.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://rq.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://dt.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://bs.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://fm.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dl.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://bl.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xq.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://cs.yuntaijiaju.cn

namespace App\Http;
来源：http://er.nszjky.cn

[U44] PHP：开启严格类型
来源：http://cl.hnjuh.cn

declare(strict_types=1);
来源：http://qu.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://lo.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mh.wgjwhj.cn

[U46] PHP：可空类型
来源：http://pq.bookmarksfly.cn

?string $name = null
来源：http://xy.wgjwhj.cn

[U47] PHP：联合类型
来源：http://fr.asd995.cn

int|string $id
来源：http://tt.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://my.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pw.panjiajie.cn

[U49] PHP：只读属性
来源：http://ri.nszjky.cn

public readonly string $name
来源：http://fj.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://wh.shxzskj.cn

public function __construct(private int $id) {}
来源：http://id.yuexingan06.cn

[U51] PHP：数组解构
来源：http://va.chemitech.net.cn

[$a, $b] = $arr;
来源：http://co.newstarts.cn

[U52] PHP：箭头函数
来源：http://je.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://bg.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ur.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://pk.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://hj.shxzskj.cn

$obj?->method()
来源：http://ob.hnjuh.cn

[U55] PHP：match 表达式
来源：http://wt.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://je.lnxyls.cn

[U56] PHP：命名参数
来源：http://by.shxzukj.cn

f(a: 1, b: 2)
来源：http://oz.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://ig.521024.cn

"值: {$a}"
来源：http://ue.nszjky.cn

[U58] PHP：数组三件套
来源：http://cm.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wb.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://gq.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hc.521024.cn

[U60] PHP：JSON 编解码
来源：http://qu.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://on.521024.cn

[U61] PHP：正则
来源：http://zr.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lq.shxzukj.cn

[U62] PHP：日期对象
来源：http://kc.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hm.muxihuayi.cn

[U63] PHP：文件读写
来源：http://sc.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://om.hahajie.cn

[U64] PHP：目录遍历
来源：http://bm.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://wb.gzmigu.cn

[U65] PHP：会话
来源：http://gv.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ew.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://fu.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ac.szsharing.cn

[U67] PHP：处理文件上传
来源：http://ub.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://it.szsharing.cn

[U68] PHP：PDO 连接
来源：http://ip.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mb.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://dj.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ch.colortex.cn

[U70] PHP：PDO 事务
来源：http://ec.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rg.521024.cn


<!-- 参考信息 -->