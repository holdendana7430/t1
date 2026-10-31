代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://rl.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qg.shxzukj.cn

[S48] C++：逐行读文件
来源：http://bj.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pn.nszjky.cn

while (std::getline(in, line)) { }
来源：http://wv.haigaiapp.cn

[S49] C++：写文件
来源：http://fq.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mt.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://gg.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yt.asd995.cn

[S51] C++：显式类型转换
来源：http://mg.yuexingan06.cn

static_cast<double>(a) / b
来源：http://td.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://jw.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://kp.bookmarksfly.cn

[S53] C++：移动语义
来源：http://mb.asd995.cn

std::vector<int> w = std::move(v);
来源：http://xt.nszjky.cn

[S54] C++：异常处理
来源：http://wh.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vg.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://gu.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uh.muxihuayi.cn

[S56] C++：optional
来源：http://vg.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nx.gzmigu.cn

[S57] C++：编译期常量
来源：http://vf.haigaiapp.cn

constexpr int N = 10;
来源：http://nl.shxzukj.cn

[S58] C++：命名空间
来源：http://cq.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://kq.szxytkj.cn

[S59] C++：静态断言
来源：http://tl.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://el.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://hv.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mj.bjjhwx.cn

================================================================================
来源：http://cb.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gy.haigaiapp.cn

================================================================================
来源：http://dv.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://dq.wgjwhj.cn

println("Hello")
来源：http://hq.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://bt.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sc.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://my.lnxyls.cn

"值: $b"
来源：http://ye.shxzskj.cn

[T04] Kotlin：空安全
来源：http://pv.hahajie.cn

val n: String? = null;  n?.length
来源：http://kp.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://xo.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pl.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://nv.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tu.colortex.cn

[T07] Kotlin：集合过滤
来源：http://fn.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bq.asd995.cn

[T08] Kotlin：数据类
来源：http://ij.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://iw.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://yu.colortex.cn

fun String.exclaim() = this + "!"
来源：http://ko.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ep.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yi.asd995.cn

[T11] Kotlin：协程
来源：http://cz.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://me.colortex.cn

[T12] Kotlin：解构声明
来源：http://hk.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://am.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://xy.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://xc.szxytkj.cn

[T14] Kotlin：循环
来源：http://rh.shxzukj.cn

for (i in 1..10) println(i)
来源：http://ml.asd995.cn

[T15] Kotlin：接口
来源：http://wh.nicolike.cn

interface Shape { fun area(): Double }
来源：http://sp.yuexingan06.cn

[T16] Swift：Hello World
来源：http://fx.shxzukj.cn

print("Hello")
来源：http://ni.huanxung.cn

[T17] Swift：变量与常量
来源：http://uv.jctech888.com.cn

var a = 1;  let b = 2
来源：http://nk.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://wu.szxytkj.cn

"值: \(b)"
来源：http://dm.521024.cn

[T19] Swift：可选绑定
来源：http://fl.haigaiapp.cn

if let n = opt { print(n) }
来源：http://cp.muxihuayi.cn

[T20] Swift：数组操作
来源：http://kj.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pe.newstarts.cn

[T21] Swift：遍历
来源：http://yq.shxzukj.cn

for x in a { print(x) }
来源：http://gp.newstarts.cn

[T22] Swift：字典
来源：http://hf.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mm.wgjwhj.cn

[T23] Swift：函数
来源：http://el.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kg.szsharing.cn

[T24] Swift：闭包
来源：http://aj.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tf.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://qe.wgjwhj.cn

struct P { var x: Int }
来源：http://ba.gzmigu.cn

[T26] Swift：类与重写
来源：http://rh.521024.cn

class A: Base { override func f() {} }
来源：http://fn.muxihuayi.cn

[T27] Swift：错误处理
来源：http://oh.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://av.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://fb.haigaiapp.cn

enum Color { case red, green }
来源：http://cu.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://lo.jctech888.com.cn

guard let x = opt else { return }
来源：http://mv.yuexingan06.cn

[T30] Swift：协议
来源：http://ih.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://zd.hnjuh.cn

[T31] Lua：Hello World
来源：http://xh.hahajie.cn

print("Hello")
来源：http://rq.hnjuh.cn

[T32] Lua：局部变量
来源：http://bq.shxzukj.cn

local a = 1
来源：http://tx.nicolike.cn

[T33] Lua：表（数组）
来源：http://ae.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uu.9csxet.cn

[T34] Lua：遍历表
来源：http://bl.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gr.gzmigu.cn

[T35] Lua：字典表
来源：http://qf.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://gl.colortex.cn

[T36] Lua：函数
来源：http://lu.bjjhwx.cn

function add(a, b) return a + b end
来源：http://pm.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://rb.521024.cn

"a" .. "b"
来源：http://ti.panjiajie.cn

[T38] Lua：条件
来源：http://yv.wgjwhj.cn

if x > 0 then print("正") end
来源：http://mp.9csxet.cn

[T39] Lua：模式匹配
来源：http://ql.huanxung.cn

string.find(s, "%d+")
来源：http://qh.szxytkj.cn

[T40] Lua：元表
来源：http://dp.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://qs.lnxyls.cn

[T41] Perl：Hello World
来源：http://fe.shxzskj.cn

print "Hello\n";
来源：http://bh.bjjhwx.cn

[T42] Perl：变量类型
来源：http://sa.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vk.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://ko.nszjky.cn

"值: $a"
来源：http://an.shxzskj.cn

[T44] Perl：条件
来源：http://ml.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://pc.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://ud.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://jd.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://lc.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kg.hahajie.cn

[T47] Perl：正则捕获
来源：http://lw.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wn.szsharing.cn

[T48] Perl：正则替换
来源：http://yy.nicolike.cn

$s =~ s/old/new/g;
来源：http://eh.muxihuayi.cn

[T49] Perl：函数
来源：http://ok.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kb.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://tc.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gm.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://kl.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://gc.szsharing.cn

println("Hello")
来源：http://zj.shxzskj.cn

[T52] Scala：变量
来源：http://it.asd995.cn

val a = 1;  var b = 2
来源：http://sg.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ye.colortex.cn

s"值: $b"
来源：http://fo.hahajie.cn

[T54] Scala：集合映射
来源：http://nk.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://ma.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ug.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rf.521024.cn

[T56] Scala：样例类
来源：http://tg.szsharing.cn

case class User(name: String, age: Int)
来源：http://sg.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://pp.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bl.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://rx.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ec.jianghongdianzi.cn

[T59] Scala：循环
来源：http://wg.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://po.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://uf.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ul.yuexingan06.cn

================================================================================
来源：http://kf.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vo.muxihuayi.cn

================================================================================
来源：http://zk.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://av.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bi.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://mv.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fa.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://wr.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qg.newstarts.cn

[U04] Py：变量调试打印
来源：http://pz.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nl.newstarts.cn

[U05] Py：列表去重且保序
来源：http://ji.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ap.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://gf.shxzukj.cn

{**a, **b}
来源：http://he.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://kl.szsharing.cn

{v: k for k, v in d.items()}
来源：http://fq.nicolike.cn

[U08] Py：展平二维列表
来源：http://ex.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ab.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://qm.hnjuh.cn

max(d, key=d.get)
来源：http://gu.shxzukj.cn

[U10] Py：按值排序字典
来源：http://db.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qc.colortex.cn

[U11] Py：生成器表达式
来源：http://xp.shtwfgs.cn

(x * 2 for x in arr)
来源：http://xc.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qw.panjiajie.cn

Counter(arr).most_common(3)
来源：http://kw.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://vj.wgjwhj.cn

deque(maxlen=10)
来源：http://ks.newstarts.cn

[U14] Py：分组收集到列表
来源：http://ab.colortex.cn

defaultdict(list)
来源：http://xf.haigaiapp.cn

[U15] Py：高精度计时
来源：http://cv.szsharing.cn

t = time.perf_counter()
来源：http://rn.newstarts.cn

[U16] Py：命令行参数解析
来源：http://op.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yg.haigaiapp.cn

[U17] Py：初始化日志
来源：http://jv.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://cp.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ow.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://pk.asd995.cn

[U19] Py：正则替换带回调
来源：http://kt.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://be.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ve.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://wu.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ai.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://tq.panjiajie.cn

[U22] Py：矩阵转置
来源：http://cd.nszjky.cn

list(zip(*m))
来源：http://rm.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://rl.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vp.asd995.cn

[U24] Py：路径操作
来源：http://qn.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vq.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://qt.huanxung.cn

csv.DictReader(f)
来源：http://qc.nszjky.cn

[U26] Py：并发下载
来源：http://wl.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ba.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://cj.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://gz.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://js.9csxet.cn

UserId = int
来源：http://lu.nszjky.cn

[U29] Py：属性校验
来源：http://fi.panjiajie.cn

@property 与 @x.setter 配合
来源：http://uv.shxzukj.cn

[U30] Py：数据类
来源：http://qp.szsharing.cn

@dataclass(slots=True)
来源：http://vw.huixiangedu.cn

[U31] Py：单测
来源：http://al.bjjhwx.cn

python -m pytest -q
来源：http://ga.huixiangedu.cn

[U32] Py：代码格式化
来源：http://ce.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://ta.jctech888.com.cn

[U33] Py：打包发布
来源：http://cr.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ey.huanxung.cn

[U34] Py：判断编码
来源：http://pu.shxzskj.cn

chardet.detect(raw)
来源：http://bl.shxzskj.cn

[U35] Py：发送邮件
来源：http://jj.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ks.521024.cn

[U36] Py：定时任务
来源：http://gc.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://ua.szsharing.cn

[U37] Py：读写 Excel
来源：http://fk.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sc.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://pj.asd995.cn

Path(__file__).resolve().parent
来源：http://ex.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://wg.shxzskj.cn

sys.stdout.isatty()
来源：http://hn.colortex.cn

[U40] Py：打印到标准错误
来源：http://qy.panjiajie.cn

print("err", file=sys.stderr)
来源：http://bv.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://wb.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ov.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://cn.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tp.9csxet.cn

[U43] PHP：声明命名空间
来源：http://cf.colortex.cn

namespace App\Http;
来源：http://ov.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ck.9csxet.cn

declare(strict_types=1);
来源：http://uk.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://sh.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hp.haigaiapp.cn

[U46] PHP：可空类型
来源：http://bm.huanxung.cn

?string $name = null
来源：http://ob.9csxet.cn

[U47] PHP：联合类型
来源：http://kq.hahajie.cn

int|string $id
来源：http://ag.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://kb.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gd.wgjwhj.cn

[U49] PHP：只读属性
来源：http://cb.colortex.cn

public readonly string $name
来源：http://bp.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://at.panjiajie.cn

public function __construct(private int $id) {}
来源：http://le.shxzskj.cn

[U51] PHP：数组解构
来源：http://to.chemitech.net.cn

[$a, $b] = $arr;
来源：http://fc.hnjuh.cn

[U52] PHP：箭头函数
来源：http://vm.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://sd.huanxung.cn

[U53] PHP：空合并运算符
来源：http://fw.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://qg.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://ey.haigaiapp.cn

$obj?->method()
来源：http://di.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://ny.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lr.panjiajie.cn

[U56] PHP：命名参数
来源：http://qg.szsharing.cn

f(a: 1, b: 2)
来源：http://st.panjiajie.cn

[U57] PHP：字符串插值
来源：http://cl.lnxyls.cn

"值: {$a}"
来源：http://ng.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://ot.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://su.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://ef.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://md.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://mx.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oe.chemitech.net.cn

[U61] PHP：正则
来源：http://ro.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://nx.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ey.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://yb.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mm.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://yn.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://tr.bookmarksfly.cn

[U65] PHP：会话
来源：http://tz.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qv.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://ot.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cw.newstarts.cn

[U67] PHP：处理文件上传
来源：http://mt.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cz.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ar.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ll.521024.cn

[U69] PHP：PDO 预处理
来源：http://hs.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pl.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://em.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yz.521024.cn

[U71] PHP：抛出异常
来源：http://fg.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://mh.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://dx.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://jg.shxzukj.cn


<!-- 参考信息 -->