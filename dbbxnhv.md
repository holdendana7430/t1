代发 wailian999

[S45] C++：lambda
来源：http://kl.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bd.yuexingan06.cn

[S46] C++：函数模板
来源：http://wd.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cp.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://pe.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ch.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://tu.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://be.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://ua.newstarts.cn

[S49] C++：写文件
来源：http://lt.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ay.huixiangedu.cn

[S50] C++：格式化数字
来源：http://tw.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gt.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://dl.huanxung.cn

static_cast<double>(a) / b
来源：http://br.521024.cn

[S52] C++：const 与 noexcept
来源：http://va.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://pr.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://zn.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ii.lnxyls.cn

[S54] C++：异常处理
来源：http://xp.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vr.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://jd.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://os.yuexingan06.cn

[S56] C++：optional
来源：http://md.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nd.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://lr.panjiajie.cn

constexpr int N = 10;
来源：http://vo.hnjuh.cn

[S58] C++：命名空间
来源：http://zm.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://dx.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://se.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fk.asd995.cn

[S60] C++：遍历并删除元素
来源：http://en.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dc.huixinmuqiang.cn

================================================================================
来源：http://vi.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mn.nicolike.cn

================================================================================
来源：http://wh.521024.cn

[T01] Kotlin：Hello World
来源：http://yd.shxzskj.cn

println("Hello")
来源：http://sg.haigaiapp.cn

[T02] Kotlin：变量
来源：http://gh.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://by.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://hy.haigaiapp.cn

"值: $b"
来源：http://vv.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://pw.asd995.cn

val n: String? = null;  n?.length
来源：http://zz.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://vv.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nh.521024.cn

[T06] Kotlin：集合映射
来源：http://ol.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://be.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://dm.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gt.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ol.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://ka.521024.cn

[T09] Kotlin：扩展函数
来源：http://ce.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://bl.newstarts.cn

[T10] Kotlin：默认参数
来源：http://yz.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rz.panjiajie.cn

[T11] Kotlin：协程
来源：http://gi.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://td.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://kj.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://fh.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://ex.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://tj.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ir.asd995.cn

for (i in 1..10) println(i)
来源：http://ip.gzmigu.cn

[T15] Kotlin：接口
来源：http://ef.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://wv.chemitech.net.cn

[T16] Swift：Hello World
来源：http://xc.panjiajie.cn

print("Hello")
来源：http://wp.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://lm.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://qh.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://zs.huixiangedu.cn

"值: \(b)"
来源：http://ku.hnjuh.cn

[T19] Swift：可选绑定
来源：http://zs.szxytkj.cn

if let n = opt { print(n) }
来源：http://nx.shtwfgs.cn

[T20] Swift：数组操作
来源：http://pm.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xl.szxytkj.cn

[T21] Swift：遍历
来源：http://av.yuexingan06.cn

for x in a { print(x) }
来源：http://hy.chemitech.net.cn

[T22] Swift：字典
来源：http://gu.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gj.gzmigu.cn

[T23] Swift：函数
来源：http://xp.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mq.9csxet.cn

[T24] Swift：闭包
来源：http://oy.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cr.gzmigu.cn

[T25] Swift：结构体
来源：http://dz.chemitech.net.cn

struct P { var x: Int }
来源：http://di.panjiajie.cn

[T26] Swift：类与重写
来源：http://dv.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://zm.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://dc.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://zz.haigaiapp.cn

[T28] Swift：枚举
来源：http://px.huixiangedu.cn

enum Color { case red, green }
来源：http://rj.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://dm.521024.cn

guard let x = opt else { return }
来源：http://wm.asd995.cn

[T30] Swift：协议
来源：http://qz.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://yq.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://ne.shxzukj.cn

print("Hello")
来源：http://oc.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://xz.colortex.cn

local a = 1
来源：http://zh.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ij.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gw.jctech888.com.cn

[T34] Lua：遍历表
来源：http://nu.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xg.muxihuayi.cn

[T35] Lua：字典表
来源：http://ta.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://mc.jctech888.com.cn

[T36] Lua：函数
来源：http://xq.jctech888.com.cn

function add(a, b) return a + b end
来源：http://fv.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://ro.nicolike.cn

"a" .. "b"
来源：http://yf.shxzukj.cn

[T38] Lua：条件
来源：http://hp.521024.cn

if x > 0 then print("正") end
来源：http://aw.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://ua.521024.cn

string.find(s, "%d+")
来源：http://bb.colortex.cn

[T40] Lua：元表
来源：http://rn.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://vf.yuexingan06.cn

[T41] Perl：Hello World
来源：http://te.nicolike.cn

print "Hello\n";
来源：http://ug.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://zw.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uu.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://wr.hnjuh.cn

"值: $a"
来源：http://ea.jianghongdianzi.cn

[T44] Perl：条件
来源：http://ef.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://gl.shxzskj.cn

[T45] Perl：数组遍历
来源：http://sz.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://fh.nszjky.cn

[T46] Perl：哈希操作
来源：http://ap.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://an.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://sp.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://si.colortex.cn

[T48] Perl：正则替换
来源：http://ok.panjiajie.cn

$s =~ s/old/new/g;
来源：http://jd.bookmarksfly.cn

[T49] Perl：函数
来源：http://vu.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oy.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://mo.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ss.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://um.panjiajie.cn

[T51] Scala：Hello World
来源：http://tt.muxihuayi.cn

println("Hello")
来源：http://wd.haigaiapp.cn

[T52] Scala：变量
来源：http://jf.lnxyls.cn

val a = 1;  var b = 2
来源：http://nv.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://fv.hnjuh.cn

s"值: $b"
来源：http://dv.gzmigu.cn

[T54] Scala：集合映射
来源：http://tt.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://fb.shxzskj.cn

[T55] Scala：集合过滤
来源：http://zw.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nm.nicolike.cn

[T56] Scala：样例类
来源：http://sd.521024.cn

case class User(name: String, age: Int)
来源：http://qi.newstarts.cn

[T57] Scala：模式匹配
来源：http://xl.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://af.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://lo.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ni.muxihuayi.cn

[T59] Scala：循环
来源：http://jo.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://uh.yuexingan06.cn

[T60] Scala：折叠
来源：http://gx.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ki.gzmigu.cn

================================================================================
来源：http://ap.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xc.colortex.cn

================================================================================
来源：http://cr.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://zz.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ec.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://qv.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qc.asd995.cn

[U03] Py：加载 .env 配置
来源：http://ge.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://me.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://gl.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://su.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://iv.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://hz.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ix.nszjky.cn

{**a, **b}
来源：http://ae.szxytkj.cn

[U07] Py：反转字典键值
来源：http://gu.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://ci.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://ge.shxzskj.cn

[y for x in nested for y in x]
来源：http://nq.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://iz.lnxyls.cn

max(d, key=d.get)
来源：http://ek.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://fv.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ld.huanxung.cn

[U11] Py：生成器表达式
来源：http://np.shxzukj.cn

(x * 2 for x in arr)
来源：http://ck.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://no.9csxet.cn

Counter(arr).most_common(3)
来源：http://vw.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://dr.haigaiapp.cn

deque(maxlen=10)
来源：http://lf.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://qc.yuexingan06.cn

defaultdict(list)
来源：http://iv.nszjky.cn

[U15] Py：高精度计时
来源：http://yy.yuexingan06.cn

t = time.perf_counter()
来源：http://zw.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://qm.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gs.wgjwhj.cn

[U17] Py：初始化日志
来源：http://nk.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://qw.gzmigu.cn

[U18] Py：预编译正则
来源：http://yk.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://ja.huanxung.cn

[U19] Py：正则替换带回调
来源：http://do.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ll.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://ii.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://cb.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://cd.521024.cn

@contextlib.contextmanager
来源：http://wf.gzmigu.cn

[U22] Py：矩阵转置
来源：http://nz.bookmarksfly.cn

list(zip(*m))
来源：http://gc.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://vx.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fs.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ug.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ay.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://it.shxzskj.cn

csv.DictReader(f)
来源：http://md.yuexingan06.cn

[U26] Py：并发下载
来源：http://ae.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://un.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://rj.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://lp.huixiangedu.cn

[U28] Py：类型别名
来源：http://ag.colortex.cn

UserId = int
来源：http://zq.521024.cn

[U29] Py：属性校验
来源：http://ti.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://ik.huixinmuqiang.cn

[U30] Py：数据类
来源：http://rq.shxzukj.cn

@dataclass(slots=True)
来源：http://mi.9csxet.cn

[U31] Py：单测
来源：http://iy.hnjuh.cn

python -m pytest -q
来源：http://cd.nicolike.cn

[U32] Py：代码格式化
来源：http://ir.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://ns.muxihuayi.cn

[U33] Py：打包发布
来源：http://ti.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://yx.shxzskj.cn

[U34] Py：判断编码
来源：http://rp.panjiajie.cn

chardet.detect(raw)
来源：http://nh.shxzskj.cn

[U35] Py：发送邮件
来源：http://qf.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qo.nszjky.cn

[U36] Py：定时任务
来源：http://il.521024.cn

schedule.every(10).minutes.do(job)
来源：http://td.gzmigu.cn

[U37] Py：读写 Excel
来源：http://wg.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fr.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://fy.lnxyls.cn

Path(__file__).resolve().parent
来源：http://zi.521024.cn

[U39] Py：判断是否在交互环境
来源：http://zf.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://zn.nszjky.cn

[U40] Py：打印到标准错误
来源：http://jh.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://jv.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://cb.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ee.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://xf.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lq.nicolike.cn

[U43] PHP：声明命名空间
来源：http://qh.bookmarksfly.cn

namespace App\Http;
来源：http://bz.newstarts.cn

[U44] PHP：开启严格类型
来源：http://bc.jianghongdianzi.cn

declare(strict_types=1);
来源：http://eo.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://xp.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zh.yuexingan06.cn

[U46] PHP：可空类型
来源：http://hy.szxytkj.cn

?string $name = null
来源：http://ql.hnjuh.cn

[U47] PHP：联合类型
来源：http://xu.jctech888.com.cn

int|string $id
来源：http://po.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://gv.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qh.hnjuh.cn

[U49] PHP：只读属性
来源：http://jm.yuexingan06.cn

public readonly string $name
来源：http://ls.521024.cn

[U50] PHP：构造器属性提升
来源：http://ux.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://du.nicolike.cn

[U51] PHP：数组解构
来源：http://vr.bjjhwx.cn

[$a, $b] = $arr;
来源：http://gy.521024.cn

[U52] PHP：箭头函数
来源：http://lr.asd995.cn

$double = fn($x) => $x * 2;
来源：http://bc.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://oj.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://cl.gzmigu.cn

[U54] PHP：空安全调用
来源：http://yf.huixinmuqiang.cn

$obj?->method()
来源：http://nz.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://fb.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mp.shxzukj.cn

[U56] PHP：命名参数
来源：http://we.bjjhwx.cn

f(a: 1, b: 2)
来源：http://zd.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://mm.huixiangedu.cn

"值: {$a}"
来源：http://qj.hnjuh.cn

[U58] PHP：数组三件套
来源：http://cj.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pd.shxzskj.cn

[U59] PHP：自定义排序
来源：http://zk.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mr.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://el.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ne.huanxung.cn

[U61] PHP：正则
来源：http://os.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yw.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://yh.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mk.lnxyls.cn

[U63] PHP：文件读写
来源：http://ri.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nx.newstarts.cn

[U64] PHP：目录遍历
来源：http://pg.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://yt.hahajie.cn

[U65] PHP：会话
来源：http://qn.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cu.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://au.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oy.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://pp.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oz.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://vw.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cb.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://oe.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iz.asd995.cn

[U70] PHP：PDO 事务
来源：http://jm.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pj.wgjwhj.cn


<!-- 参考信息 -->