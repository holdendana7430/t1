代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kn.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://kb.huanxung.cn

static_cast<double>(a) / b
来源：http://vi.521024.cn

[S52] C++：const 与 noexcept
来源：http://wc.9csxet.cn

int size() const noexcept { return n_; }
来源：http://wi.gzmigu.cn

[S53] C++：移动语义
来源：http://gz.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://wv.shtwfgs.cn

[S54] C++：异常处理
来源：http://fv.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qr.szsharing.cn

[S55] C++：结构化绑定
来源：http://xq.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cj.chemitech.net.cn

[S56] C++：optional
来源：http://ry.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://da.521024.cn

[S57] C++：编译期常量
来源：http://fy.nszjky.cn

constexpr int N = 10;
来源：http://fl.hnjuh.cn

[S58] C++：命名空间
来源：http://jb.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://yn.haigaiapp.cn

[S59] C++：静态断言
来源：http://st.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cm.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://sk.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bn.bjjhwx.cn

================================================================================
来源：http://pc.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kx.huixinmuqiang.cn

================================================================================
来源：http://xv.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://uu.huixiangedu.cn

println("Hello")
来源：http://zm.521024.cn

[T02] Kotlin：变量
来源：http://nd.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cs.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://hn.gzmigu.cn

"值: $b"
来源：http://ar.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://ih.gzmigu.cn

val n: String? = null;  n?.length
来源：http://lg.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://wr.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uz.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://rf.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xs.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://gp.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aq.521024.cn

[T08] Kotlin：数据类
来源：http://bw.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ws.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://gf.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://qu.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://bv.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://et.szsharing.cn

[T11] Kotlin：协程
来源：http://nf.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yv.colortex.cn

[T12] Kotlin：解构声明
来源：http://tk.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://bz.colortex.cn

[T13] Kotlin：只读 Map
来源：http://vk.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://qr.jctech888.com.cn

[T14] Kotlin：循环
来源：http://wn.shxzukj.cn

for (i in 1..10) println(i)
来源：http://dh.nszjky.cn

[T15] Kotlin：接口
来源：http://ck.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://ct.shxzskj.cn

[T16] Swift：Hello World
来源：http://ik.muxihuayi.cn

print("Hello")
来源：http://fn.asd995.cn

[T17] Swift：变量与常量
来源：http://tq.szsharing.cn

var a = 1;  let b = 2
来源：http://kh.521024.cn

[T18] Swift：字符串插值
来源：http://sf.huixiangedu.cn

"值: \(b)"
来源：http://yn.lnxyls.cn

[T19] Swift：可选绑定
来源：http://dp.asd995.cn

if let n = opt { print(n) }
来源：http://ih.haigaiapp.cn

[T20] Swift：数组操作
来源：http://nn.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yy.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://rp.muxihuayi.cn

for x in a { print(x) }
来源：http://hh.bjjhwx.cn

[T22] Swift：字典
来源：http://ln.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ck.shtwfgs.cn

[T23] Swift：函数
来源：http://re.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://op.haigaiapp.cn

[T24] Swift：闭包
来源：http://tj.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cs.muxihuayi.cn

[T25] Swift：结构体
来源：http://is.huanxung.cn

struct P { var x: Int }
来源：http://ji.shtwfgs.cn

[T26] Swift：类与重写
来源：http://qy.szxytkj.cn

class A: Base { override func f() {} }
来源：http://ge.haigaiapp.cn

[T27] Swift：错误处理
来源：http://bx.szsharing.cn

do { try f() } catch { print(error) }
来源：http://bm.huanxung.cn

[T28] Swift：枚举
来源：http://yp.chemitech.net.cn

enum Color { case red, green }
来源：http://nn.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://bw.hnjuh.cn

guard let x = opt else { return }
来源：http://dm.nszjky.cn

[T30] Swift：协议
来源：http://gg.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://bo.muxihuayi.cn

[T31] Lua：Hello World
来源：http://uy.asd995.cn

print("Hello")
来源：http://yv.lnxyls.cn

[T32] Lua：局部变量
来源：http://cc.haigaiapp.cn

local a = 1
来源：http://kk.hnjuh.cn

[T33] Lua：表（数组）
来源：http://xp.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bu.9csxet.cn

[T34] Lua：遍历表
来源：http://ty.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cb.muxihuayi.cn

[T35] Lua：字典表
来源：http://wq.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://yi.bjjhwx.cn

[T36] Lua：函数
来源：http://lg.nicolike.cn

function add(a, b) return a + b end
来源：http://en.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://li.9csxet.cn

"a" .. "b"
来源：http://rs.shtwfgs.cn

[T38] Lua：条件
来源：http://qs.wgjwhj.cn

if x > 0 then print("正") end
来源：http://an.lnxyls.cn

[T39] Lua：模式匹配
来源：http://sz.szsharing.cn

string.find(s, "%d+")
来源：http://ev.nicolike.cn

[T40] Lua：元表
来源：http://sp.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://ox.shtwfgs.cn

[T41] Perl：Hello World
来源：http://bd.nicolike.cn

print "Hello\n";
来源：http://xr.hnjuh.cn

[T42] Perl：变量类型
来源：http://rw.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jm.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://sl.chemitech.net.cn

"值: $a"
来源：http://xa.yuexingan06.cn

[T44] Perl：条件
来源：http://aj.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://dl.shxzskj.cn

[T45] Perl：数组遍历
来源：http://wb.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://dh.hnjuh.cn

[T46] Perl：哈希操作
来源：http://fa.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nu.shxzskj.cn

[T47] Perl：正则捕获
来源：http://bg.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xd.haigaiapp.cn

[T48] Perl：正则替换
来源：http://tf.9csxet.cn

$s =~ s/old/new/g;
来源：http://uv.huixiangedu.cn

[T49] Perl：函数
来源：http://zg.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nc.9csxet.cn

[T50] Perl：逐行读文件
来源：http://wh.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sd.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://ab.chemitech.net.cn

[T51] Scala：Hello World
来源：http://hn.lnxyls.cn

println("Hello")
来源：http://qa.colortex.cn

[T52] Scala：变量
来源：http://cx.521024.cn

val a = 1;  var b = 2
来源：http://ap.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://cm.bjjhwx.cn

s"值: $b"
来源：http://zc.lnxyls.cn

[T54] Scala：集合映射
来源：http://tr.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://ya.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://wl.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qp.shxzskj.cn

[T56] Scala：样例类
来源：http://is.newstarts.cn

case class User(name: String, age: Int)
来源：http://te.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://vg.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cg.jctech888.com.cn

[T58] Scala：函数定义
来源：http://wt.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://my.hnjuh.cn

[T59] Scala：循环
来源：http://ao.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://he.hnjuh.cn

[T60] Scala：折叠
来源：http://ry.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lr.bookmarksfly.cn

================================================================================
来源：http://pb.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qg.yuexingan06.cn

================================================================================
来源：http://rx.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ug.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cs.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://nd.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fa.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://hf.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rz.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://km.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cl.huanxung.cn

[U05] Py：列表去重且保序
来源：http://jb.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://rt.521024.cn

[U06] Py：合并两个字典
来源：http://dm.9csxet.cn

{**a, **b}
来源：http://tx.shxzukj.cn

[U07] Py：反转字典键值
来源：http://lb.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://lz.panjiajie.cn

[U08] Py：展平二维列表
来源：http://ub.muxihuayi.cn

[y for x in nested for y in x]
来源：http://wm.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://yr.newstarts.cn

max(d, key=d.get)
来源：http://pj.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://nj.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bj.panjiajie.cn

[U11] Py：生成器表达式
来源：http://pd.shtwfgs.cn

(x * 2 for x in arr)
来源：http://kw.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://va.panjiajie.cn

Counter(arr).most_common(3)
来源：http://tj.lnxyls.cn

[U13] Py：固定长度队列
来源：http://ig.shxzskj.cn

deque(maxlen=10)
来源：http://gp.newstarts.cn

[U14] Py：分组收集到列表
来源：http://gx.muxihuayi.cn

defaultdict(list)
来源：http://zu.colortex.cn

[U15] Py：高精度计时
来源：http://nl.bookmarksfly.cn

t = time.perf_counter()
来源：http://ru.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://jz.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ye.szsharing.cn

[U17] Py：初始化日志
来源：http://ea.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://ut.shxzukj.cn

[U18] Py：预编译正则
来源：http://vt.huanxung.cn

pat = re.compile(r"\d+")
来源：http://gu.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://gl.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rk.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://iw.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://uq.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://db.shtwfgs.cn

@contextlib.contextmanager
来源：http://ie.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://he.shxzukj.cn

list(zip(*m))
来源：http://rs.asd995.cn

[U23] Py：分块读取大文件
来源：http://er.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fm.lnxyls.cn

[U24] Py：路径操作
来源：http://wc.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ep.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://wd.newstarts.cn

csv.DictReader(f)
来源：http://ww.gzmigu.cn

[U26] Py：并发下载
来源：http://uq.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dc.colortex.cn

[U27] Py：异步 HTTP
来源：http://qv.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://hv.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://vt.wgjwhj.cn

UserId = int
来源：http://ql.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://ps.huanxung.cn

@property 与 @x.setter 配合
来源：http://hw.yuntaijiaju.cn

[U30] Py：数据类
来源：http://ou.asd995.cn

@dataclass(slots=True)
来源：http://fa.szsharing.cn

[U31] Py：单测
来源：http://wi.shxzskj.cn

python -m pytest -q
来源：http://gy.gzmigu.cn

[U32] Py：代码格式化
来源：http://xu.asd995.cn

ruff format . && ruff check --fix .
来源：http://ew.shxzskj.cn

[U33] Py：打包发布
来源：http://sb.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://yi.haigaiapp.cn

[U34] Py：判断编码
来源：http://ye.huixiangedu.cn

chardet.detect(raw)
来源：http://fw.wgjwhj.cn

[U35] Py：发送邮件
来源：http://in.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://as.hnjuh.cn

[U36] Py：定时任务
来源：http://zv.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://za.hahajie.cn

[U37] Py：读写 Excel
来源：http://vo.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://un.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://fc.nicolike.cn

Path(__file__).resolve().parent
来源：http://bl.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://vh.wgjwhj.cn

sys.stdout.isatty()
来源：http://td.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://yl.huanxung.cn

print("err", file=sys.stderr)
来源：http://to.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://rq.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xr.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://sg.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ds.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://ix.shxzskj.cn

namespace App\Http;
来源：http://sp.huanxung.cn

[U44] PHP：开启严格类型
来源：http://iy.asd995.cn

declare(strict_types=1);
来源：http://oy.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://nq.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fi.shxzskj.cn

[U46] PHP：可空类型
来源：http://ve.gzmigu.cn

?string $name = null
来源：http://fj.szsharing.cn

[U47] PHP：联合类型
来源：http://in.nszjky.cn

int|string $id
来源：http://cz.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://tq.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yr.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ip.yuexingan06.cn

public readonly string $name
来源：http://sp.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://lo.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://jl.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://yl.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://kd.shxzukj.cn

[U52] PHP：箭头函数
来源：http://au.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://qw.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://jb.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://lz.shxzskj.cn

[U54] PHP：空安全调用
来源：http://db.huixinmuqiang.cn

$obj?->method()
来源：http://nc.lnxyls.cn

[U55] PHP：match 表达式
来源：http://sf.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ts.panjiajie.cn

[U56] PHP：命名参数
来源：http://oi.wgjwhj.cn

f(a: 1, b: 2)
来源：http://tz.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ez.szsharing.cn

"值: {$a}"
来源：http://uz.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://ko.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bg.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://al.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fi.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://rr.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://le.bjjhwx.cn

[U61] PHP：正则
来源：http://wn.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lg.shxzskj.cn

[U62] PHP：日期对象
来源：http://gd.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qe.lnxyls.cn

[U63] PHP：文件读写
来源：http://wi.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hd.hnjuh.cn

[U64] PHP：目录遍历
来源：http://az.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://gc.wgjwhj.cn

[U65] PHP：会话
来源：http://hd.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nf.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ai.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wo.asd995.cn

[U67] PHP：处理文件上传
来源：http://bl.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jf.9csxet.cn

[U68] PHP：PDO 连接
来源：http://ch.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nt.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://jx.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ya.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://bj.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wc.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://zc.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://bv.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://to.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://qb.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://if.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://js.9csxet.cn

[U74] PHP：读取环境变量
来源：http://oq.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://cj.521024.cn

[U75] PHP：依赖注入
来源：http://wi.newstarts.cn

composer require psr/container
来源：http://rr.shtwfgs.cn

[U76] PHP：简单路由
来源：http://kn.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://br.jianghongdianzi.cn


<!-- 参考信息 -->