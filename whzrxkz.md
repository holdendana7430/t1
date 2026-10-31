代发 wailian999

[S45] C++：lambda
来源：http://tw.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mm.9csxet.cn

[S46] C++：函数模板
来源：http://bm.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rv.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://aa.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zb.shxzukj.cn

[S48] C++：逐行读文件
来源：http://zc.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ll.huanxung.cn

while (std::getline(in, line)) { }
来源：http://qn.bjjhwx.cn

[S49] C++：写文件
来源：http://pq.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cl.huanxung.cn

[S50] C++：格式化数字
来源：http://na.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sv.asd995.cn

[S51] C++：显式类型转换
来源：http://ar.panjiajie.cn

static_cast<double>(a) / b
来源：http://tq.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://ji.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://gh.asd995.cn

[S53] C++：移动语义
来源：http://vh.colortex.cn

std::vector<int> w = std::move(v);
来源：http://og.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://xq.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oe.shxzukj.cn

[S55] C++：结构化绑定
来源：http://bw.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gt.szsharing.cn

[S56] C++：optional
来源：http://wr.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yn.colortex.cn

[S57] C++：编译期常量
来源：http://ie.jctech888.com.cn

constexpr int N = 10;
来源：http://qw.asd995.cn

[S58] C++：命名空间
来源：http://oi.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://sw.hnjuh.cn

[S59] C++：静态断言
来源：http://tu.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://po.521024.cn

[S60] C++：遍历并删除元素
来源：http://bj.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uf.jctech888.com.cn

================================================================================
来源：http://ti.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://he.szxytkj.cn

================================================================================
来源：http://wr.szsharing.cn

[T01] Kotlin：Hello World
来源：http://em.bookmarksfly.cn

println("Hello")
来源：http://yz.wgjwhj.cn

[T02] Kotlin：变量
来源：http://ud.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ls.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://kj.hahajie.cn

"值: $b"
来源：http://gz.panjiajie.cn

[T04] Kotlin：空安全
来源：http://nb.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://yl.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://pp.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yp.colortex.cn

[T06] Kotlin：集合映射
来源：http://ge.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jj.asd995.cn

[T07] Kotlin：集合过滤
来源：http://nb.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yx.shxzskj.cn

[T08] Kotlin：数据类
来源：http://ju.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://xd.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://so.521024.cn

fun String.exclaim() = this + "!"
来源：http://zs.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://to.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wf.colortex.cn

[T11] Kotlin：协程
来源：http://ab.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hh.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ub.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://nv.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://uf.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://bf.jctech888.com.cn

[T14] Kotlin：循环
来源：http://gp.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://pn.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://fj.huanxung.cn

interface Shape { fun area(): Double }
来源：http://wd.asd995.cn

[T16] Swift：Hello World
来源：http://oc.521024.cn

print("Hello")
来源：http://mx.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://pk.nszjky.cn

var a = 1;  let b = 2
来源：http://gu.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://hc.shxzskj.cn

"值: \(b)"
来源：http://ef.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://vh.haigaiapp.cn

if let n = opt { print(n) }
来源：http://lm.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://rk.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qi.huanxung.cn

[T21] Swift：遍历
来源：http://yg.colortex.cn

for x in a { print(x) }
来源：http://fz.huixinmuqiang.cn

[T22] Swift：字典
来源：http://nj.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sg.shxzukj.cn

[T23] Swift：函数
来源：http://xt.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://me.shtwfgs.cn

[T24] Swift：闭包
来源：http://rk.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ft.szxytkj.cn

[T25] Swift：结构体
来源：http://cx.haigaiapp.cn

struct P { var x: Int }
来源：http://lv.gzmigu.cn

[T26] Swift：类与重写
来源：http://la.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://gt.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://al.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://hf.gzmigu.cn

[T28] Swift：枚举
来源：http://gf.haigaiapp.cn

enum Color { case red, green }
来源：http://fa.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://nh.nicolike.cn

guard let x = opt else { return }
来源：http://yk.asd995.cn

[T30] Swift：协议
来源：http://ly.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://gz.asd995.cn

[T31] Lua：Hello World
来源：http://yv.yuexingan06.cn

print("Hello")
来源：http://kz.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ab.nicolike.cn

local a = 1
来源：http://gk.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://pn.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://is.hahajie.cn

[T34] Lua：遍历表
来源：http://oj.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ep.shxzukj.cn

[T35] Lua：字典表
来源：http://sl.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://xj.szsharing.cn

[T36] Lua：函数
来源：http://hs.asd995.cn

function add(a, b) return a + b end
来源：http://wk.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://uu.shxzukj.cn

"a" .. "b"
来源：http://vv.jctech888.com.cn

[T38] Lua：条件
来源：http://dq.lnxyls.cn

if x > 0 then print("正") end
来源：http://cs.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://co.nicolike.cn

string.find(s, "%d+")
来源：http://sm.521024.cn

[T40] Lua：元表
来源：http://hc.huanxung.cn

setmetatable({}, { __index = base })
来源：http://ef.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ot.bjjhwx.cn

print "Hello\n";
来源：http://nn.shxzukj.cn

[T42] Perl：变量类型
来源：http://fw.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gp.shxzukj.cn

[T43] Perl：字符串插值
来源：http://kr.szsharing.cn

"值: $a"
来源：http://ti.jianghongdianzi.cn

[T44] Perl：条件
来源：http://dw.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ov.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://qb.colortex.cn

for my $x (@arr) { print $x; }
来源：http://ns.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://rb.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://be.hahajie.cn

[T47] Perl：正则捕获
来源：http://qx.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kh.bjjhwx.cn

[T48] Perl：正则替换
来源：http://fv.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://qq.shxzukj.cn

[T49] Perl：函数
来源：http://gb.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ia.asd995.cn

[T50] Perl：逐行读文件
来源：http://of.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qy.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://ql.gzmigu.cn

[T51] Scala：Hello World
来源：http://ic.bjjhwx.cn

println("Hello")
来源：http://bm.nszjky.cn

[T52] Scala：变量
来源：http://cm.colortex.cn

val a = 1;  var b = 2
来源：http://kn.shxzskj.cn

[T53] Scala：字符串插值
来源：http://my.huixinmuqiang.cn

s"值: $b"
来源：http://ff.9csxet.cn

[T54] Scala：集合映射
来源：http://eh.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://tg.gzmigu.cn

[T55] Scala：集合过滤
来源：http://yx.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ra.nicolike.cn

[T56] Scala：样例类
来源：http://ns.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://fy.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://eb.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sn.nicolike.cn

[T58] Scala：函数定义
来源：http://cc.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://na.nszjky.cn

[T59] Scala：循环
来源：http://is.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://lz.jctech888.com.cn

[T60] Scala：折叠
来源：http://hb.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ss.shtwfgs.cn

================================================================================
来源：http://cu.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zr.bookmarksfly.cn

================================================================================
来源：http://tt.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://qs.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fi.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://oi.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xl.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://kc.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iw.huanxung.cn

[U04] Py：变量调试打印
来源：http://ws.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zw.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ly.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://an.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://pg.bjjhwx.cn

{**a, **b}
来源：http://lj.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://nv.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://tw.9csxet.cn

[U08] Py：展平二维列表
来源：http://rp.newstarts.cn

[y for x in nested for y in x]
来源：http://ou.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ix.jianghongdianzi.cn

max(d, key=d.get)
来源：http://hr.szxytkj.cn

[U10] Py：按值排序字典
来源：http://xg.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tp.nicolike.cn

[U11] Py：生成器表达式
来源：http://ll.9csxet.cn

(x * 2 for x in arr)
来源：http://ds.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://is.panjiajie.cn

Counter(arr).most_common(3)
来源：http://nc.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ci.haigaiapp.cn

deque(maxlen=10)
来源：http://km.nszjky.cn

[U14] Py：分组收集到列表
来源：http://ud.jctech888.com.cn

defaultdict(list)
来源：http://ie.shxzskj.cn

[U15] Py：高精度计时
来源：http://nv.huixinmuqiang.cn

t = time.perf_counter()
来源：http://sl.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ar.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ju.newstarts.cn

[U17] Py：初始化日志
来源：http://ji.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://nj.chemitech.net.cn

[U18] Py：预编译正则
来源：http://sm.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://yi.nicolike.cn

[U19] Py：正则替换带回调
来源：http://st.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vw.9csxet.cn

[U20] Py：缓存函数结果
来源：http://tl.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ql.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://qr.huanxung.cn

@contextlib.contextmanager
来源：http://yr.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://jr.huanxung.cn

list(zip(*m))
来源：http://ck.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://ow.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://di.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://jj.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uv.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://iu.newstarts.cn

csv.DictReader(f)
来源：http://vw.chemitech.net.cn

[U26] Py：并发下载
来源：http://kq.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uw.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://gh.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://dz.9csxet.cn

[U28] Py：类型别名
来源：http://eo.nszjky.cn

UserId = int
来源：http://gz.panjiajie.cn

[U29] Py：属性校验
来源：http://wt.huanxung.cn

@property 与 @x.setter 配合
来源：http://zx.huixiangedu.cn

[U30] Py：数据类
来源：http://fw.shxzskj.cn

@dataclass(slots=True)
来源：http://ya.shxzskj.cn

[U31] Py：单测
来源：http://kr.yuexingan06.cn

python -m pytest -q
来源：http://fg.haigaiapp.cn

[U32] Py：代码格式化
来源：http://fw.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://cv.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://pp.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://ve.asd995.cn

[U34] Py：判断编码
来源：http://qk.nicolike.cn

chardet.detect(raw)
来源：http://re.lnxyls.cn

[U35] Py：发送邮件
来源：http://fb.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://my.bookmarksfly.cn

[U36] Py：定时任务
来源：http://xi.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://dp.521024.cn

[U37] Py：读写 Excel
来源：http://ha.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kd.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://hv.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://eo.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://eg.521024.cn

sys.stdout.isatty()
来源：http://un.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://vf.szxytkj.cn

print("err", file=sys.stderr)
来源：http://re.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://rp.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nw.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://gr.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cg.newstarts.cn

[U43] PHP：声明命名空间
来源：http://be.colortex.cn

namespace App\Http;
来源：http://va.asd995.cn

[U44] PHP：开启严格类型
来源：http://uv.wgjwhj.cn

declare(strict_types=1);
来源：http://kb.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://ba.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.szsharing.cn

[U46] PHP：可空类型
来源：http://nt.huixinmuqiang.cn

?string $name = null
来源：http://ha.yuexingan06.cn

[U47] PHP：联合类型
来源：http://wm.jianghongdianzi.cn

int|string $id
来源：http://ax.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://ep.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ly.muxihuayi.cn

[U49] PHP：只读属性
来源：http://we.lnxyls.cn

public readonly string $name
来源：http://li.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://ym.nicolike.cn

public function __construct(private int $id) {}
来源：http://fk.shxzskj.cn

[U51] PHP：数组解构
来源：http://wh.colortex.cn

[$a, $b] = $arr;
来源：http://co.nicolike.cn

[U52] PHP：箭头函数
来源：http://cc.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://yw.szsharing.cn

[U53] PHP：空合并运算符
来源：http://yh.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://xd.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://bk.lnxyls.cn

$obj?->method()
来源：http://pu.huanxung.cn

[U55] PHP：match 表达式
来源：http://dn.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xh.nszjky.cn

[U56] PHP：命名参数
来源：http://cr.huanxung.cn

f(a: 1, b: 2)
来源：http://bo.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://bf.szxytkj.cn

"值: {$a}"
来源：http://id.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://us.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jk.gzmigu.cn

[U59] PHP：自定义排序
来源：http://xm.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://va.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://yw.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wu.szxytkj.cn

[U61] PHP：正则
来源：http://ad.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qf.newstarts.cn

[U62] PHP：日期对象
来源：http://qg.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bj.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://ti.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ma.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://cr.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://fv.colortex.cn

[U65] PHP：会话
来源：http://tw.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yi.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://mg.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sk.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://qh.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xz.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://em.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yp.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://qy.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bk.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://sa.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yz.newstarts.cn


<!-- 参考信息 -->