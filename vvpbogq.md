代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://qb.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ax.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://sg.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gd.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://hs.asd995.cn

[S49] C++：写文件
来源：http://cf.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cx.huixiangedu.cn

[S50] C++：格式化数字
来源：http://nb.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rk.newstarts.cn

[S51] C++：显式类型转换
来源：http://nd.chemitech.net.cn

static_cast<double>(a) / b
来源：http://va.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://cm.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://xf.9csxet.cn

[S53] C++：移动语义
来源：http://ry.521024.cn

std::vector<int> w = std::move(v);
来源：http://sn.wgjwhj.cn

[S54] C++：异常处理
来源：http://ls.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lg.nszjky.cn

[S55] C++：结构化绑定
来源：http://bl.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rf.huixinmuqiang.cn

[S56] C++：optional
来源：http://dc.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://he.wgjwhj.cn

[S57] C++：编译期常量
来源：http://pi.jctech888.com.cn

constexpr int N = 10;
来源：http://sf.huanxung.cn

[S58] C++：命名空间
来源：http://ud.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://yg.szxytkj.cn

[S59] C++：静态断言
来源：http://bk.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wj.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://wr.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eb.huanxung.cn

================================================================================
来源：http://bz.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://my.gzmigu.cn

================================================================================
来源：http://ja.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://lb.jianghongdianzi.cn

println("Hello")
来源：http://hg.hnjuh.cn

[T02] Kotlin：变量
来源：http://sn.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lf.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://at.bookmarksfly.cn

"值: $b"
来源：http://ws.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ej.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://dq.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://gr.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ko.colortex.cn

[T06] Kotlin：集合映射
来源：http://qz.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qe.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://fx.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tk.colortex.cn

[T08] Kotlin：数据类
来源：http://vv.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://my.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://ci.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://te.newstarts.cn

[T10] Kotlin：默认参数
来源：http://ia.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bh.panjiajie.cn

[T11] Kotlin：协程
来源：http://qh.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ax.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://xm.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://js.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://mx.nszjky.cn

val m = mapOf("a" to 1)
来源：http://or.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ie.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://hh.shtwfgs.cn

[T15] Kotlin：接口
来源：http://xt.asd995.cn

interface Shape { fun area(): Double }
来源：http://fc.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://pu.asd995.cn

print("Hello")
来源：http://in.hahajie.cn

[T17] Swift：变量与常量
来源：http://kd.szxytkj.cn

var a = 1;  let b = 2
来源：http://uc.521024.cn

[T18] Swift：字符串插值
来源：http://nn.bjjhwx.cn

"值: \(b)"
来源：http://cd.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://sc.9csxet.cn

if let n = opt { print(n) }
来源：http://mt.hahajie.cn

[T20] Swift：数组操作
来源：http://mc.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mr.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://jw.huixiangedu.cn

for x in a { print(x) }
来源：http://bz.gzmigu.cn

[T22] Swift：字典
来源：http://ud.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jx.colortex.cn

[T23] Swift：函数
来源：http://gx.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gt.hnjuh.cn

[T24] Swift：闭包
来源：http://ji.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wm.szxytkj.cn

[T25] Swift：结构体
来源：http://xt.521024.cn

struct P { var x: Int }
来源：http://gm.hnjuh.cn

[T26] Swift：类与重写
来源：http://nx.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://dk.gzmigu.cn

[T27] Swift：错误处理
来源：http://ob.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://qr.szsharing.cn

[T28] Swift：枚举
来源：http://gm.bookmarksfly.cn

enum Color { case red, green }
来源：http://yv.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://og.shxzukj.cn

guard let x = opt else { return }
来源：http://cx.9csxet.cn

[T30] Swift：协议
来源：http://of.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://lq.wgjwhj.cn

[T31] Lua：Hello World
来源：http://qw.chemitech.net.cn

print("Hello")
来源：http://es.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://pi.nicolike.cn

local a = 1
来源：http://av.hnjuh.cn

[T33] Lua：表（数组）
来源：http://bm.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zu.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ho.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rl.szsharing.cn

[T35] Lua：字典表
来源：http://vp.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://fe.nicolike.cn

[T36] Lua：函数
来源：http://zj.huanxung.cn

function add(a, b) return a + b end
来源：http://yk.huanxung.cn

[T37] Lua：字符串拼接
来源：http://pe.9csxet.cn

"a" .. "b"
来源：http://qy.jctech888.com.cn

[T38] Lua：条件
来源：http://wa.szsharing.cn

if x > 0 then print("正") end
来源：http://qp.nszjky.cn

[T39] Lua：模式匹配
来源：http://oi.jctech888.com.cn

string.find(s, "%d+")
来源：http://kz.yuntaijiaju.cn

[T40] Lua：元表
来源：http://pt.asd995.cn

setmetatable({}, { __index = base })
来源：http://te.shxzukj.cn

[T41] Perl：Hello World
来源：http://ke.hahajie.cn

print "Hello\n";
来源：http://jb.hnjuh.cn

[T42] Perl：变量类型
来源：http://qw.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mz.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://sc.huixiangedu.cn

"值: $a"
来源：http://pi.haigaiapp.cn

[T44] Perl：条件
来源：http://oi.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://yy.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://ev.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://ti.huanxung.cn

[T46] Perl：哈希操作
来源：http://nd.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bw.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://kl.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://km.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://dh.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://zv.panjiajie.cn

[T49] Perl：函数
来源：http://ab.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zo.huanxung.cn

[T50] Perl：逐行读文件
来源：http://he.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uv.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://kb.yuexingan06.cn

[T51] Scala：Hello World
来源：http://zk.chemitech.net.cn

println("Hello")
来源：http://se.hnjuh.cn

[T52] Scala：变量
来源：http://lh.521024.cn

val a = 1;  var b = 2
来源：http://op.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://nj.haigaiapp.cn

s"值: $b"
来源：http://ay.bjjhwx.cn

[T54] Scala：集合映射
来源：http://bf.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://tr.hnjuh.cn

[T55] Scala：集合过滤
来源：http://ft.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vx.colortex.cn

[T56] Scala：样例类
来源：http://dt.szxytkj.cn

case class User(name: String, age: Int)
来源：http://mp.panjiajie.cn

[T57] Scala：模式匹配
来源：http://nw.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ar.huixiangedu.cn

[T58] Scala：函数定义
来源：http://vz.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://da.asd995.cn

[T59] Scala：循环
来源：http://qz.521024.cn

for (i <- 1 to 10) println(i)
来源：http://ud.gzmigu.cn

[T60] Scala：折叠
来源：http://wi.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tf.nszjky.cn

================================================================================
来源：http://um.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pn.asd995.cn

================================================================================
来源：http://uq.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://vv.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dw.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://zp.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://or.asd995.cn

[U03] Py：加载 .env 配置
来源：http://ma.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ky.shxzskj.cn

[U04] Py：变量调试打印
来源：http://nw.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vc.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://sh.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://wb.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://nw.9csxet.cn

{**a, **b}
来源：http://jg.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://xc.szsharing.cn

{v: k for k, v in d.items()}
来源：http://es.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://ld.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://ss.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://zm.asd995.cn

max(d, key=d.get)
来源：http://py.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://kj.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ll.asd995.cn

[U11] Py：生成器表达式
来源：http://gv.newstarts.cn

(x * 2 for x in arr)
来源：http://az.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jz.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://fo.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://kl.hnjuh.cn

deque(maxlen=10)
来源：http://yq.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://wg.9csxet.cn

defaultdict(list)
来源：http://th.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://pn.9csxet.cn

t = time.perf_counter()
来源：http://pj.9csxet.cn

[U16] Py：命令行参数解析
来源：http://or.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ix.wgjwhj.cn

[U17] Py：初始化日志
来源：http://yg.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ry.jctech888.com.cn

[U18] Py：预编译正则
来源：http://ti.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://up.szsharing.cn

[U19] Py：正则替换带回调
来源：http://lk.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oa.colortex.cn

[U20] Py：缓存函数结果
来源：http://ux.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://hr.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://ud.bjjhwx.cn

@contextlib.contextmanager
来源：http://ar.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://rz.szsharing.cn

list(zip(*m))
来源：http://ht.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://cr.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iq.yuexingan06.cn

[U24] Py：路径操作
来源：http://cy.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dd.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://eq.panjiajie.cn

csv.DictReader(f)
来源：http://ln.haigaiapp.cn

[U26] Py：并发下载
来源：http://kk.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oz.asd995.cn

[U27] Py：异步 HTTP
来源：http://ky.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://vp.haigaiapp.cn

[U28] Py：类型别名
来源：http://zs.9csxet.cn

UserId = int
来源：http://ou.wgjwhj.cn

[U29] Py：属性校验
来源：http://un.newstarts.cn

@property 与 @x.setter 配合
来源：http://ic.haigaiapp.cn

[U30] Py：数据类
来源：http://zt.newstarts.cn

@dataclass(slots=True)
来源：http://mi.shxzskj.cn

[U31] Py：单测
来源：http://by.chemitech.net.cn

python -m pytest -q
来源：http://hb.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ie.huanxung.cn

ruff format . && ruff check --fix .
来源：http://bw.colortex.cn

[U33] Py：打包发布
来源：http://wq.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ey.shxzukj.cn

[U34] Py：判断编码
来源：http://tf.chemitech.net.cn

chardet.detect(raw)
来源：http://ap.shtwfgs.cn

[U35] Py：发送邮件
来源：http://hz.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ue.muxihuayi.cn

[U36] Py：定时任务
来源：http://te.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://kb.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://bc.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yq.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://ss.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://rd.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://sw.shtwfgs.cn

sys.stdout.isatty()
来源：http://bn.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://tt.szsharing.cn

print("err", file=sys.stderr)
来源：http://uc.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://wf.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yd.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://mn.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kv.hahajie.cn

[U43] PHP：声明命名空间
来源：http://np.wgjwhj.cn

namespace App\Http;
来源：http://yx.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ae.shxzskj.cn

declare(strict_types=1);
来源：http://oc.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://mu.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pe.wgjwhj.cn

[U46] PHP：可空类型
来源：http://gs.wgjwhj.cn

?string $name = null
来源：http://ch.gzmigu.cn

[U47] PHP：联合类型
来源：http://zr.9csxet.cn

int|string $id
来源：http://rf.szsharing.cn

[U48] PHP：纯枚举
来源：http://ks.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aj.panjiajie.cn

[U49] PHP：只读属性
来源：http://mt.haigaiapp.cn

public readonly string $name
来源：http://zw.521024.cn

[U50] PHP：构造器属性提升
来源：http://ou.colortex.cn

public function __construct(private int $id) {}
来源：http://gn.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://fx.hahajie.cn

[$a, $b] = $arr;
来源：http://hu.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://bt.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://ys.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://vo.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://zw.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://nr.gzmigu.cn

$obj?->method()
来源：http://ma.nszjky.cn

[U55] PHP：match 表达式
来源：http://ar.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ld.colortex.cn

[U56] PHP：命名参数
来源：http://tx.shtwfgs.cn

f(a: 1, b: 2)
来源：http://jh.newstarts.cn

[U57] PHP：字符串插值
来源：http://bo.jianghongdianzi.cn

"值: {$a}"
来源：http://es.newstarts.cn

[U58] PHP：数组三件套
来源：http://re.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hn.521024.cn

[U59] PHP：自定义排序
来源：http://my.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ev.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://vy.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lu.gzmigu.cn

[U61] PHP：正则
来源：http://oy.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xv.shxzskj.cn

[U62] PHP：日期对象
来源：http://oq.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pz.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://gg.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dh.hnjuh.cn

[U64] PHP：目录遍历
来源：http://xm.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://ph.jctech888.com.cn

[U65] PHP：会话
来源：http://mw.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ve.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://qa.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yz.szsharing.cn

[U67] PHP：处理文件上传
来源：http://xi.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ue.colortex.cn

[U68] PHP：PDO 连接
来源：http://pc.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lf.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://xi.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nx.szsharing.cn

[U70] PHP：PDO 事务
来源：http://lk.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xp.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://fd.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://hb.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://ks.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://fy.nszjky.cn


<!-- 参考信息 -->