代发 wailian999

[S43] C++：智能指针
来源：http://rq.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://vd.nszjky.cn

[S44] C++：引用传参
来源：http://vy.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://in.newstarts.cn

[S45] C++：lambda
来源：http://sl.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mu.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://gm.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sp.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://sl.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ok.gzmigu.cn

[S48] C++：逐行读文件
来源：http://zm.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kr.colortex.cn

while (std::getline(in, line)) { }
来源：http://wg.chemitech.net.cn

[S49] C++：写文件
来源：http://ai.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cp.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://rw.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ve.hahajie.cn

[S51] C++：显式类型转换
来源：http://ho.hnjuh.cn

static_cast<double>(a) / b
来源：http://ul.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://ee.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://ib.haigaiapp.cn

[S53] C++：移动语义
来源：http://tp.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://rd.muxihuayi.cn

[S54] C++：异常处理
来源：http://ni.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lm.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ly.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vr.nszjky.cn

[S56] C++：optional
来源：http://zd.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oo.9csxet.cn

[S57] C++：编译期常量
来源：http://gj.521024.cn

constexpr int N = 10;
来源：http://uz.shxzskj.cn

[S58] C++：命名空间
来源：http://au.521024.cn

namespace ns { int f() { return 1; } }
来源：http://iw.colortex.cn

[S59] C++：静态断言
来源：http://hz.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dr.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://gg.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qs.shxzukj.cn

================================================================================
来源：http://ya.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tv.chemitech.net.cn

================================================================================
来源：http://sd.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://bd.newstarts.cn

println("Hello")
来源：http://gq.bjjhwx.cn

[T02] Kotlin：变量
来源：http://my.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gl.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://gv.wgjwhj.cn

"值: $b"
来源：http://fm.szxytkj.cn

[T04] Kotlin：空安全
来源：http://yo.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ku.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://tf.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fp.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://iq.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://og.asd995.cn

[T07] Kotlin：集合过滤
来源：http://pe.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qy.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://vh.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://fv.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ef.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://up.hahajie.cn

[T10] Kotlin：默认参数
来源：http://lr.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jt.huixiangedu.cn

[T11] Kotlin：协程
来源：http://wm.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wq.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://tt.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://ai.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://uv.huanxung.cn

val m = mapOf("a" to 1)
来源：http://bb.shxzskj.cn

[T14] Kotlin：循环
来源：http://iv.gzmigu.cn

for (i in 1..10) println(i)
来源：http://sg.panjiajie.cn

[T15] Kotlin：接口
来源：http://pd.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://gm.shxzukj.cn

[T16] Swift：Hello World
来源：http://yi.colortex.cn

print("Hello")
来源：http://wo.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ny.szxytkj.cn

var a = 1;  let b = 2
来源：http://hz.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ck.yuntaijiaju.cn

"值: \(b)"
来源：http://fu.nszjky.cn

[T19] Swift：可选绑定
来源：http://ko.panjiajie.cn

if let n = opt { print(n) }
来源：http://df.wgjwhj.cn

[T20] Swift：数组操作
来源：http://ps.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://at.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://es.shxzukj.cn

for x in a { print(x) }
来源：http://vq.jianghongdianzi.cn

[T22] Swift：字典
来源：http://en.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lz.huanxung.cn

[T23] Swift：函数
来源：http://ex.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ll.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ht.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vj.huanxung.cn

[T25] Swift：结构体
来源：http://hp.szxytkj.cn

struct P { var x: Int }
来源：http://wp.shxzukj.cn

[T26] Swift：类与重写
来源：http://ls.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://hu.szsharing.cn

[T27] Swift：错误处理
来源：http://fq.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://es.haigaiapp.cn

[T28] Swift：枚举
来源：http://qt.huixinmuqiang.cn

enum Color { case red, green }
来源：http://ua.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://fc.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://on.yuexingan06.cn

[T30] Swift：协议
来源：http://zg.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://rc.shxzukj.cn

[T31] Lua：Hello World
来源：http://wj.chemitech.net.cn

print("Hello")
来源：http://uz.hnjuh.cn

[T32] Lua：局部变量
来源：http://yp.yuntaijiaju.cn

local a = 1
来源：http://wz.newstarts.cn

[T33] Lua：表（数组）
来源：http://hp.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gm.hnjuh.cn

[T34] Lua：遍历表
来源：http://eh.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wu.bookmarksfly.cn

[T35] Lua：字典表
来源：http://na.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://cg.yuexingan06.cn

[T36] Lua：函数
来源：http://ce.nszjky.cn

function add(a, b) return a + b end
来源：http://ad.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://oi.huixinmuqiang.cn

"a" .. "b"
来源：http://ak.szsharing.cn

[T38] Lua：条件
来源：http://bl.colortex.cn

if x > 0 then print("正") end
来源：http://wr.shxzskj.cn

[T39] Lua：模式匹配
来源：http://oe.szxytkj.cn

string.find(s, "%d+")
来源：http://tc.haigaiapp.cn

[T40] Lua：元表
来源：http://gs.szsharing.cn

setmetatable({}, { __index = base })
来源：http://ct.szsharing.cn

[T41] Perl：Hello World
来源：http://le.521024.cn

print "Hello\n";
来源：http://mc.asd995.cn

[T42] Perl：变量类型
来源：http://us.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nd.shxzskj.cn

[T43] Perl：字符串插值
来源：http://so.jianghongdianzi.cn

"值: $a"
来源：http://oy.hahajie.cn

[T44] Perl：条件
来源：http://pz.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://yn.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://vf.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://cy.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://pd.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gz.nszjky.cn

[T47] Perl：正则捕获
来源：http://nj.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dd.yuexingan06.cn

[T48] Perl：正则替换
来源：http://pm.9csxet.cn

$s =~ s/old/new/g;
来源：http://cw.wgjwhj.cn

[T49] Perl：函数
来源：http://qr.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ir.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://sw.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fi.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://gk.szxytkj.cn

[T51] Scala：Hello World
来源：http://pw.gzmigu.cn

println("Hello")
来源：http://xx.bookmarksfly.cn

[T52] Scala：变量
来源：http://ny.szsharing.cn

val a = 1;  var b = 2
来源：http://fz.colortex.cn

[T53] Scala：字符串插值
来源：http://tt.szxytkj.cn

s"值: $b"
来源：http://kr.jctech888.com.cn

[T54] Scala：集合映射
来源：http://hl.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://yx.panjiajie.cn

[T55] Scala：集合过滤
来源：http://hp.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xa.9csxet.cn

[T56] Scala：样例类
来源：http://cc.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ot.shxzskj.cn

[T57] Scala：模式匹配
来源：http://rt.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rt.szxytkj.cn

[T58] Scala：函数定义
来源：http://wv.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lj.521024.cn

[T59] Scala：循环
来源：http://se.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://mi.jctech888.com.cn

[T60] Scala：折叠
来源：http://xs.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nx.huanxung.cn

================================================================================
来源：http://hv.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ub.huanxung.cn

================================================================================
来源：http://xx.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://uo.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nj.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://nv.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://th.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://nn.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cb.asd995.cn

[U04] Py：变量调试打印
来源：http://av.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ws.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://no.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://jt.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://it.szsharing.cn

{**a, **b}
来源：http://rn.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://ds.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://dm.szsharing.cn

[U08] Py：展平二维列表
来源：http://dk.panjiajie.cn

[y for x in nested for y in x]
来源：http://an.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://of.gzmigu.cn

max(d, key=d.get)
来源：http://uq.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://zn.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pu.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://ft.szsharing.cn

(x * 2 for x in arr)
来源：http://wq.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oa.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://kg.panjiajie.cn

[U13] Py：固定长度队列
来源：http://aw.chemitech.net.cn

deque(maxlen=10)
来源：http://in.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://tu.bjjhwx.cn

defaultdict(list)
来源：http://gv.shxzskj.cn

[U15] Py：高精度计时
来源：http://ej.nszjky.cn

t = time.perf_counter()
来源：http://dm.9csxet.cn

[U16] Py：命令行参数解析
来源：http://ab.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oy.hahajie.cn

[U17] Py：初始化日志
来源：http://yf.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://gh.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://os.521024.cn

pat = re.compile(r"\d+")
来源：http://zr.hahajie.cn

[U19] Py：正则替换带回调
来源：http://hc.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xo.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://zg.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://pa.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://mf.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://zo.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://rn.jianghongdianzi.cn

list(zip(*m))
来源：http://zf.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://ld.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dv.shxzukj.cn

[U24] Py：路径操作
来源：http://vr.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lz.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://wq.hnjuh.cn

csv.DictReader(f)
来源：http://yz.gzmigu.cn

[U26] Py：并发下载
来源：http://xu.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kf.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://st.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://iq.521024.cn

[U28] Py：类型别名
来源：http://vf.szxytkj.cn

UserId = int
来源：http://ee.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://nf.szsharing.cn

@property 与 @x.setter 配合
来源：http://en.jctech888.com.cn

[U30] Py：数据类
来源：http://hv.colortex.cn

@dataclass(slots=True)
来源：http://sn.asd995.cn

[U31] Py：单测
来源：http://jp.wgjwhj.cn

python -m pytest -q
来源：http://ff.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://bw.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://cn.szxytkj.cn

[U33] Py：打包发布
来源：http://tw.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://sc.szxytkj.cn

[U34] Py：判断编码
来源：http://eo.newstarts.cn

chardet.detect(raw)
来源：http://uu.muxihuayi.cn

[U35] Py：发送邮件
来源：http://rb.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gc.asd995.cn

[U36] Py：定时任务
来源：http://be.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://gc.szxytkj.cn

[U37] Py：读写 Excel
来源：http://oe.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ck.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://us.shxzskj.cn

Path(__file__).resolve().parent
来源：http://md.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://zy.9csxet.cn

sys.stdout.isatty()
来源：http://ld.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://aa.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://ni.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://xt.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pt.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://it.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dx.newstarts.cn

[U43] PHP：声明命名空间
来源：http://hr.szsharing.cn

namespace App\Http;
来源：http://sb.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://co.hahajie.cn

declare(strict_types=1);
来源：http://mq.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://bk.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eo.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://sr.chemitech.net.cn

?string $name = null
来源：http://ea.nicolike.cn

[U47] PHP：联合类型
来源：http://je.jianghongdianzi.cn

int|string $id
来源：http://lu.panjiajie.cn

[U48] PHP：纯枚举
来源：http://ro.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rq.wgjwhj.cn

[U49] PHP：只读属性
来源：http://fh.gzmigu.cn

public readonly string $name
来源：http://tz.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://pm.szxytkj.cn

public function __construct(private int $id) {}
来源：http://sl.hnjuh.cn

[U51] PHP：数组解构
来源：http://kn.szxytkj.cn

[$a, $b] = $arr;
来源：http://ik.newstarts.cn

[U52] PHP：箭头函数
来源：http://uw.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://nj.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://jz.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://iu.colortex.cn

[U54] PHP：空安全调用
来源：http://ja.szsharing.cn

$obj?->method()
来源：http://xh.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://zh.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dz.wgjwhj.cn

[U56] PHP：命名参数
来源：http://xz.nicolike.cn

f(a: 1, b: 2)
来源：http://wo.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ns.szsharing.cn

"值: {$a}"
来源：http://da.panjiajie.cn

[U58] PHP：数组三件套
来源：http://uk.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yv.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://rb.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xw.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://tt.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://te.chemitech.net.cn

[U61] PHP：正则
来源：http://uv.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ms.shxzskj.cn

[U62] PHP：日期对象
来源：http://bd.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tq.huixiangedu.cn

[U63] PHP：文件读写
来源：http://lv.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sm.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://pp.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://fh.hahajie.cn

[U65] PHP：会话
来源：http://ja.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cc.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://xk.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://af.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://sj.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xz.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://za.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ys.lnxyls.cn


<!-- 参考信息 -->