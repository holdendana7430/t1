代发 wailian999

while (std::getline(in, line)) { }
来源：http://sc.shxzukj.cn

[S49] C++：写文件
来源：http://kq.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fs.yuexingan06.cn

[S50] C++：格式化数字
来源：http://jf.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yk.9csxet.cn

[S51] C++：显式类型转换
来源：http://bn.colortex.cn

static_cast<double>(a) / b
来源：http://dj.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://lw.521024.cn

int size() const noexcept { return n_; }
来源：http://ji.szsharing.cn

[S53] C++：移动语义
来源：http://dj.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://if.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://gp.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://al.szsharing.cn

[S55] C++：结构化绑定
来源：http://of.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ro.shtwfgs.cn

[S56] C++：optional
来源：http://fz.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yr.shtwfgs.cn

[S57] C++：编译期常量
来源：http://gs.nicolike.cn

constexpr int N = 10;
来源：http://fi.newstarts.cn

[S58] C++：命名空间
来源：http://nl.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://ri.szsharing.cn

[S59] C++：静态断言
来源：http://ul.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ie.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://ds.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tm.bjjhwx.cn

================================================================================
来源：http://eh.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rc.hahajie.cn

================================================================================
来源：http://zh.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://cg.gzmigu.cn

println("Hello")
来源：http://zk.nszjky.cn

[T02] Kotlin：变量
来源：http://yi.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sa.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ap.yuexingan06.cn

"值: $b"
来源：http://zq.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://xv.lnxyls.cn

val n: String? = null;  n?.length
来源：http://pb.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://rq.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kc.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://ph.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jh.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ng.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gj.huanxung.cn

[T08] Kotlin：数据类
来源：http://zu.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ce.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://kv.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://zc.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://xv.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vw.huixiangedu.cn

[T11] Kotlin：协程
来源：http://fd.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yt.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://jp.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://lu.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://sc.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ao.nicolike.cn

[T14] Kotlin：循环
来源：http://sj.asd995.cn

for (i in 1..10) println(i)
来源：http://ok.hnjuh.cn

[T15] Kotlin：接口
来源：http://hl.9csxet.cn

interface Shape { fun area(): Double }
来源：http://mk.hnjuh.cn

[T16] Swift：Hello World
来源：http://sj.yuexingan06.cn

print("Hello")
来源：http://ah.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://mo.gzmigu.cn

var a = 1;  let b = 2
来源：http://st.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://ft.nicolike.cn

"值: \(b)"
来源：http://yk.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://hz.521024.cn

if let n = opt { print(n) }
来源：http://uj.haigaiapp.cn

[T20] Swift：数组操作
来源：http://sx.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mm.shxzskj.cn

[T21] Swift：遍历
来源：http://nr.lnxyls.cn

for x in a { print(x) }
来源：http://sv.nicolike.cn

[T22] Swift：字典
来源：http://yx.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ic.haigaiapp.cn

[T23] Swift：函数
来源：http://aq.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nf.shxzukj.cn

[T24] Swift：闭包
来源：http://ec.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hb.panjiajie.cn

[T25] Swift：结构体
来源：http://tq.huixinmuqiang.cn

struct P { var x: Int }
来源：http://tx.shxzskj.cn

[T26] Swift：类与重写
来源：http://at.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://ml.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://ed.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://ts.bjjhwx.cn

[T28] Swift：枚举
来源：http://ar.szsharing.cn

enum Color { case red, green }
来源：http://uq.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://bq.muxihuayi.cn

guard let x = opt else { return }
来源：http://do.yuntaijiaju.cn

[T30] Swift：协议
来源：http://kd.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://tp.jctech888.com.cn

[T31] Lua：Hello World
来源：http://hx.haigaiapp.cn

print("Hello")
来源：http://zk.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://un.shxzskj.cn

local a = 1
来源：http://yf.szxytkj.cn

[T33] Lua：表（数组）
来源：http://to.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bb.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://am.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eu.shtwfgs.cn

[T35] Lua：字典表
来源：http://fk.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://ew.szsharing.cn

[T36] Lua：函数
来源：http://lp.yuexingan06.cn

function add(a, b) return a + b end
来源：http://qp.9csxet.cn

[T37] Lua：字符串拼接
来源：http://nc.szsharing.cn

"a" .. "b"
来源：http://hu.nicolike.cn

[T38] Lua：条件
来源：http://bn.hnjuh.cn

if x > 0 then print("正") end
来源：http://dz.colortex.cn

[T39] Lua：模式匹配
来源：http://km.panjiajie.cn

string.find(s, "%d+")
来源：http://li.gzmigu.cn

[T40] Lua：元表
来源：http://js.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://nl.shxzukj.cn

[T41] Perl：Hello World
来源：http://fx.asd995.cn

print "Hello\n";
来源：http://mt.hnjuh.cn

[T42] Perl：变量类型
来源：http://rs.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://si.panjiajie.cn

[T43] Perl：字符串插值
来源：http://xz.nicolike.cn

"值: $a"
来源：http://fz.panjiajie.cn

[T44] Perl：条件
来源：http://jb.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://pp.huanxung.cn

[T45] Perl：数组遍历
来源：http://zz.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://ra.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://wp.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oq.gzmigu.cn

[T47] Perl：正则捕获
来源：http://vv.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zw.gzmigu.cn

[T48] Perl：正则替换
来源：http://uj.shxzskj.cn

$s =~ s/old/new/g;
来源：http://qm.colortex.cn

[T49] Perl：函数
来源：http://ib.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zs.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://ma.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qa.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://nk.colortex.cn

[T51] Scala：Hello World
来源：http://mx.szxytkj.cn

println("Hello")
来源：http://fj.szxytkj.cn

[T52] Scala：变量
来源：http://vw.haigaiapp.cn

val a = 1;  var b = 2
来源：http://cm.lnxyls.cn

[T53] Scala：字符串插值
来源：http://bp.haigaiapp.cn

s"值: $b"
来源：http://lc.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://uv.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://mr.szsharing.cn

[T55] Scala：集合过滤
来源：http://oo.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kj.gzmigu.cn

[T56] Scala：样例类
来源：http://wt.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://qh.lnxyls.cn

[T57] Scala：模式匹配
来源：http://iq.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gk.lnxyls.cn

[T58] Scala：函数定义
来源：http://up.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://as.chemitech.net.cn

[T59] Scala：循环
来源：http://ju.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://mp.gzmigu.cn

[T60] Scala：折叠
来源：http://gu.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jo.szsharing.cn

================================================================================
来源：http://uo.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dy.colortex.cn

================================================================================
来源：http://nr.colortex.cn

[U01] Py：创建虚拟环境
来源：http://wj.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bh.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://dl.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://un.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://jd.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rw.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://iw.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://se.nicolike.cn

[U05] Py：列表去重且保序
来源：http://ft.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://al.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://wr.huixiangedu.cn

{**a, **b}
来源：http://vg.szsharing.cn

[U07] Py：反转字典键值
来源：http://lt.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://hw.nicolike.cn

[U08] Py：展平二维列表
来源：http://oy.shxzskj.cn

[y for x in nested for y in x]
来源：http://jb.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://to.chemitech.net.cn

max(d, key=d.get)
来源：http://jy.shxzukj.cn

[U10] Py：按值排序字典
来源：http://es.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rg.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ew.newstarts.cn

(x * 2 for x in arr)
来源：http://gz.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lg.nszjky.cn

Counter(arr).most_common(3)
来源：http://is.newstarts.cn

[U13] Py：固定长度队列
来源：http://qr.gzmigu.cn

deque(maxlen=10)
来源：http://or.asd995.cn

[U14] Py：分组收集到列表
来源：http://ft.chemitech.net.cn

defaultdict(list)
来源：http://jp.jctech888.com.cn

[U15] Py：高精度计时
来源：http://vb.shtwfgs.cn

t = time.perf_counter()
来源：http://zt.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://rg.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yn.panjiajie.cn

[U17] Py：初始化日志
来源：http://lv.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://vc.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://et.newstarts.cn

pat = re.compile(r"\d+")
来源：http://dp.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://am.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://al.newstarts.cn

[U20] Py：缓存函数结果
来源：http://rn.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://uc.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://hz.shxzukj.cn

@contextlib.contextmanager
来源：http://lu.szxytkj.cn

[U22] Py：矩阵转置
来源：http://sh.chemitech.net.cn

list(zip(*m))
来源：http://gi.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://pl.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lf.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://mp.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://is.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://mz.nszjky.cn

csv.DictReader(f)
来源：http://sz.hahajie.cn

[U26] Py：并发下载
来源：http://my.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hs.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://bp.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://xi.szsharing.cn

[U28] Py：类型别名
来源：http://fp.chemitech.net.cn

UserId = int
来源：http://vh.9csxet.cn

[U29] Py：属性校验
来源：http://ri.nicolike.cn

@property 与 @x.setter 配合
来源：http://ml.nicolike.cn

[U30] Py：数据类
来源：http://mh.shxzukj.cn

@dataclass(slots=True)
来源：http://yy.colortex.cn

[U31] Py：单测
来源：http://kf.muxihuayi.cn

python -m pytest -q
来源：http://gd.wgjwhj.cn

[U32] Py：代码格式化
来源：http://ws.szsharing.cn

ruff format . && ruff check --fix .
来源：http://cc.lnxyls.cn

[U33] Py：打包发布
来源：http://ya.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://xv.huixiangedu.cn

[U34] Py：判断编码
来源：http://ne.jianghongdianzi.cn

chardet.detect(raw)
来源：http://sg.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://pg.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://be.wgjwhj.cn

[U36] Py：定时任务
来源：http://ab.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://xo.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://am.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://td.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://ay.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://nc.521024.cn

[U39] Py：判断是否在交互环境
来源：http://os.521024.cn

sys.stdout.isatty()
来源：http://lj.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://xr.newstarts.cn

print("err", file=sys.stderr)
来源：http://li.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rs.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lk.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://cx.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dn.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://az.newstarts.cn

namespace App\Http;
来源：http://nk.newstarts.cn

[U44] PHP：开启严格类型
来源：http://di.jctech888.com.cn

declare(strict_types=1);
来源：http://sb.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://hm.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.hnjuh.cn

[U46] PHP：可空类型
来源：http://zx.hahajie.cn

?string $name = null
来源：http://gr.shxzskj.cn

[U47] PHP：联合类型
来源：http://fp.521024.cn

int|string $id
来源：http://vi.asd995.cn

[U48] PHP：纯枚举
来源：http://rz.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yt.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://hb.jianghongdianzi.cn

public readonly string $name
来源：http://xt.521024.cn

[U50] PHP：构造器属性提升
来源：http://vo.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://rb.jctech888.com.cn

[U51] PHP：数组解构
来源：http://jo.521024.cn

[$a, $b] = $arr;
来源：http://el.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://ql.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://eh.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://kv.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://cc.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://kk.newstarts.cn

$obj?->method()
来源：http://sj.nicolike.cn

[U55] PHP：match 表达式
来源：http://is.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qu.huanxung.cn

[U56] PHP：命名参数
来源：http://aq.bjjhwx.cn

f(a: 1, b: 2)
来源：http://zy.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://bl.newstarts.cn

"值: {$a}"
来源：http://rd.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ml.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://um.colortex.cn

[U59] PHP：自定义排序
来源：http://dv.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://au.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://yf.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cm.haigaiapp.cn

[U61] PHP：正则
来源：http://hn.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pu.shxzskj.cn

[U62] PHP：日期对象
来源：http://yt.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cs.jctech888.com.cn

[U63] PHP：文件读写
来源：http://fy.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pd.hnjuh.cn

[U64] PHP：目录遍历
来源：http://mi.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ug.shxzskj.cn

[U65] PHP：会话
来源：http://ws.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wm.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://iw.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aj.szsharing.cn

[U67] PHP：处理文件上传
来源：http://py.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zg.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://ll.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ig.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://xz.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ut.521024.cn

[U70] PHP：PDO 事务
来源：http://jf.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fj.nicolike.cn

[U71] PHP：抛出异常
来源：http://so.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://ku.newstarts.cn

[U72] PHP：写错误日志
来源：http://ng.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://lw.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://gz.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://qs.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://pn.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://vm.muxihuayi.cn


<!-- 参考信息 -->