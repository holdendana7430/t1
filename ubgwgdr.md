代发 wailian999

[S45] C++：lambda
来源：http://yg.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oo.jctech888.com.cn

[S46] C++：函数模板
来源：http://xp.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bf.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://re.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xl.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://nk.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ks.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://qs.gzmigu.cn

[S49] C++：写文件
来源：http://jd.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vf.wgjwhj.cn

[S50] C++：格式化数字
来源：http://yl.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hu.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://oq.bjjhwx.cn

static_cast<double>(a) / b
来源：http://ug.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://xf.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://um.shtwfgs.cn

[S53] C++：移动语义
来源：http://zr.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://ya.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://ng.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fd.nicolike.cn

[S55] C++：结构化绑定
来源：http://ym.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nl.lnxyls.cn

[S56] C++：optional
来源：http://za.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://go.szsharing.cn

[S57] C++：编译期常量
来源：http://op.asd995.cn

constexpr int N = 10;
来源：http://qe.shxzukj.cn

[S58] C++：命名空间
来源：http://zs.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://xy.haigaiapp.cn

[S59] C++：静态断言
来源：http://tu.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jw.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://lr.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://up.bookmarksfly.cn

================================================================================
来源：http://zm.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://um.jianghongdianzi.cn

================================================================================
来源：http://aw.9csxet.cn

[T01] Kotlin：Hello World
来源：http://lr.9csxet.cn

println("Hello")
来源：http://ho.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ki.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vt.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://sf.jctech888.com.cn

"值: $b"
来源：http://xi.9csxet.cn

[T04] Kotlin：空安全
来源：http://hz.hnjuh.cn

val n: String? = null;  n?.length
来源：http://dt.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://ki.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vk.huanxung.cn

[T06] Kotlin：集合映射
来源：http://wv.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gq.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://hv.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lq.asd995.cn

[T08] Kotlin：数据类
来源：http://fh.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://pc.521024.cn

[T09] Kotlin：扩展函数
来源：http://el.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://wi.521024.cn

[T10] Kotlin：默认参数
来源：http://nx.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://df.huanxung.cn

[T11] Kotlin：协程
来源：http://tr.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ac.521024.cn

[T12] Kotlin：解构声明
来源：http://sr.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://nq.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://ma.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://do.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://gn.colortex.cn

for (i in 1..10) println(i)
来源：http://gj.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://lw.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://kt.muxihuayi.cn

[T16] Swift：Hello World
来源：http://kc.yuntaijiaju.cn

print("Hello")
来源：http://ks.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://vh.szxytkj.cn

var a = 1;  let b = 2
来源：http://ve.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://zn.panjiajie.cn

"值: \(b)"
来源：http://cv.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://jc.nicolike.cn

if let n = opt { print(n) }
来源：http://le.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ac.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tf.asd995.cn

[T21] Swift：遍历
来源：http://ub.colortex.cn

for x in a { print(x) }
来源：http://rt.bjjhwx.cn

[T22] Swift：字典
来源：http://dw.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ls.521024.cn

[T23] Swift：函数
来源：http://jy.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ef.huanxung.cn

[T24] Swift：闭包
来源：http://gy.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ai.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://oz.huixinmuqiang.cn

struct P { var x: Int }
来源：http://tc.nicolike.cn

[T26] Swift：类与重写
来源：http://ny.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://ew.wgjwhj.cn

[T27] Swift：错误处理
来源：http://pu.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://ws.asd995.cn

[T28] Swift：枚举
来源：http://pc.jctech888.com.cn

enum Color { case red, green }
来源：http://na.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://ds.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://yj.wgjwhj.cn

[T30] Swift：协议
来源：http://un.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://cf.szsharing.cn

[T31] Lua：Hello World
来源：http://lo.gzmigu.cn

print("Hello")
来源：http://xq.shtwfgs.cn

[T32] Lua：局部变量
来源：http://jf.nszjky.cn

local a = 1
来源：http://gb.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://su.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ey.wgjwhj.cn

[T34] Lua：遍历表
来源：http://up.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://he.shxzukj.cn

[T35] Lua：字典表
来源：http://rc.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://cp.huixinmuqiang.cn

[T36] Lua：函数
来源：http://mz.yuexingan06.cn

function add(a, b) return a + b end
来源：http://cz.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://tu.huanxung.cn

"a" .. "b"
来源：http://kw.szsharing.cn

[T38] Lua：条件
来源：http://pd.nszjky.cn

if x > 0 then print("正") end
来源：http://fa.newstarts.cn

[T39] Lua：模式匹配
来源：http://wr.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://rj.lnxyls.cn

[T40] Lua：元表
来源：http://pe.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://bs.wgjwhj.cn

[T41] Perl：Hello World
来源：http://tb.jianghongdianzi.cn

print "Hello\n";
来源：http://bv.hnjuh.cn

[T42] Perl：变量类型
来源：http://vx.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wm.521024.cn

[T43] Perl：字符串插值
来源：http://jr.chemitech.net.cn

"值: $a"
来源：http://eo.asd995.cn

[T44] Perl：条件
来源：http://ej.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://hy.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://zq.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://zg.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://us.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sp.9csxet.cn

[T47] Perl：正则捕获
来源：http://vi.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rg.9csxet.cn

[T48] Perl：正则替换
来源：http://rd.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://gx.huixiangedu.cn

[T49] Perl：函数
来源：http://mm.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xw.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://kk.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qo.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://tw.lnxyls.cn

[T51] Scala：Hello World
来源：http://wx.9csxet.cn

println("Hello")
来源：http://pe.huixinmuqiang.cn

[T52] Scala：变量
来源：http://wx.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://tk.gzmigu.cn

[T53] Scala：字符串插值
来源：http://zm.hnjuh.cn

s"值: $b"
来源：http://nd.jctech888.com.cn

[T54] Scala：集合映射
来源：http://lr.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://kt.szxytkj.cn

[T55] Scala：集合过滤
来源：http://lc.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ba.szsharing.cn

[T56] Scala：样例类
来源：http://sl.hnjuh.cn

case class User(name: String, age: Int)
来源：http://gg.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://zx.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ou.asd995.cn

[T58] Scala：函数定义
来源：http://xj.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qo.bjjhwx.cn

[T59] Scala：循环
来源：http://iv.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://vo.nicolike.cn

[T60] Scala：折叠
来源：http://oh.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bw.yuexingan06.cn

================================================================================
来源：http://eg.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jt.jianghongdianzi.cn

================================================================================
来源：http://ha.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://pn.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oc.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://fg.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://is.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://la.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xi.521024.cn

[U04] Py：变量调试打印
来源：http://he.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ya.nszjky.cn

[U05] Py：列表去重且保序
来源：http://gx.hahajie.cn

list(dict.fromkeys(arr))
来源：http://pb.nszjky.cn

[U06] Py：合并两个字典
来源：http://so.shtwfgs.cn

{**a, **b}
来源：http://fm.shxzukj.cn

[U07] Py：反转字典键值
来源：http://rt.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://me.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://ag.yuexingan06.cn

[y for x in nested for y in x]
来源：http://vl.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://km.shxzukj.cn

max(d, key=d.get)
来源：http://yg.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://va.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cq.gzmigu.cn

[U11] Py：生成器表达式
来源：http://nx.gzmigu.cn

(x * 2 for x in arr)
来源：http://aj.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zh.9csxet.cn

Counter(arr).most_common(3)
来源：http://fv.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ko.haigaiapp.cn

deque(maxlen=10)
来源：http://yq.521024.cn

[U14] Py：分组收集到列表
来源：http://nm.gzmigu.cn

defaultdict(list)
来源：http://ug.muxihuayi.cn

[U15] Py：高精度计时
来源：http://tj.bjjhwx.cn

t = time.perf_counter()
来源：http://kl.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://bi.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ry.newstarts.cn

[U17] Py：初始化日志
来源：http://hh.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://lf.haigaiapp.cn

[U18] Py：预编译正则
来源：http://xz.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://xr.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://bm.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cr.newstarts.cn

[U20] Py：缓存函数结果
来源：http://lr.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://vj.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://bc.wgjwhj.cn

@contextlib.contextmanager
来源：http://rl.szxytkj.cn

[U22] Py：矩阵转置
来源：http://yl.521024.cn

list(zip(*m))
来源：http://sy.nszjky.cn

[U23] Py：分块读取大文件
来源：http://ib.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sg.9csxet.cn

[U24] Py：路径操作
来源：http://cy.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mw.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://io.haigaiapp.cn

csv.DictReader(f)
来源：http://uf.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://dw.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yq.huanxung.cn

[U27] Py：异步 HTTP
来源：http://dc.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://aa.chemitech.net.cn

[U28] Py：类型别名
来源：http://ym.hnjuh.cn

UserId = int
来源：http://mw.huixiangedu.cn

[U29] Py：属性校验
来源：http://ak.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://pp.newstarts.cn

[U30] Py：数据类
来源：http://py.bookmarksfly.cn

@dataclass(slots=True)
来源：http://yf.szxytkj.cn

[U31] Py：单测
来源：http://zv.huixinmuqiang.cn

python -m pytest -q
来源：http://cc.bjjhwx.cn

[U32] Py：代码格式化
来源：http://wj.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://wz.muxihuayi.cn

[U33] Py：打包发布
来源：http://yg.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ul.szsharing.cn

[U34] Py：判断编码
来源：http://uo.szxytkj.cn

chardet.detect(raw)
来源：http://mv.huanxung.cn

[U35] Py：发送邮件
来源：http://ms.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uj.wgjwhj.cn

[U36] Py：定时任务
来源：http://og.521024.cn

schedule.every(10).minutes.do(job)
来源：http://ud.nszjky.cn

[U37] Py：读写 Excel
来源：http://af.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wv.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://rg.lnxyls.cn

Path(__file__).resolve().parent
来源：http://xa.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://eg.muxihuayi.cn

sys.stdout.isatty()
来源：http://wp.nicolike.cn

[U40] Py：打印到标准错误
来源：http://lz.gzmigu.cn

print("err", file=sys.stderr)
来源：http://zs.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ua.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ny.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://uu.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://be.hahajie.cn

[U43] PHP：声明命名空间
来源：http://mo.szxytkj.cn

namespace App\Http;
来源：http://kz.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ue.lnxyls.cn

declare(strict_types=1);
来源：http://vr.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://sz.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://te.shxzukj.cn

[U46] PHP：可空类型
来源：http://qr.yuntaijiaju.cn

?string $name = null
来源：http://hu.newstarts.cn

[U47] PHP：联合类型
来源：http://rn.hnjuh.cn

int|string $id
来源：http://fe.szxytkj.cn

[U48] PHP：纯枚举
来源：http://vd.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bd.bjjhwx.cn

[U49] PHP：只读属性
来源：http://ax.gzmigu.cn

public readonly string $name
来源：http://eb.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://br.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://sn.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ta.nicolike.cn

[$a, $b] = $arr;
来源：http://dq.panjiajie.cn

[U52] PHP：箭头函数
来源：http://qc.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ds.szsharing.cn

[U53] PHP：空合并运算符
来源：http://hr.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://sn.521024.cn

[U54] PHP：空安全调用
来源：http://dv.yuexingan06.cn

$obj?->method()
来源：http://ur.asd995.cn

[U55] PHP：match 表达式
来源：http://eb.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vz.bjjhwx.cn

[U56] PHP：命名参数
来源：http://ie.lnxyls.cn

f(a: 1, b: 2)
来源：http://rx.huanxung.cn

[U57] PHP：字符串插值
来源：http://sb.huixinmuqiang.cn

"值: {$a}"
来源：http://sc.shxzukj.cn

[U58] PHP：数组三件套
来源：http://wj.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tm.newstarts.cn

[U59] PHP：自定义排序
来源：http://he.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qh.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://xa.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cp.haigaiapp.cn

[U61] PHP：正则
来源：http://fq.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vx.lnxyls.cn

[U62] PHP：日期对象
来源：http://hm.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://en.nicolike.cn

[U63] PHP：文件读写
来源：http://ls.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jj.hahajie.cn

[U64] PHP：目录遍历
来源：http://ou.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://df.shtwfgs.cn

[U65] PHP：会话
来源：http://ks.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gi.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://tt.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pu.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://gr.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://av.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://hz.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xi.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://tr.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bk.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://kr.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zb.shtwfgs.cn


<!-- 参考信息 -->