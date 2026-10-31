代发 wailian999

while (std::getline(in, line)) { }
来源：http://tr.yuexingan06.cn

[S49] C++：写文件
来源：http://vl.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uk.shxzskj.cn

[S50] C++：格式化数字
来源：http://zr.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cu.szsharing.cn

[S51] C++：显式类型转换
来源：http://yb.jctech888.com.cn

static_cast<double>(a) / b
来源：http://nc.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://cp.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://sw.gzmigu.cn

[S53] C++：移动语义
来源：http://yy.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://ix.nszjky.cn

[S54] C++：异常处理
来源：http://ox.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tp.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ou.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ep.huanxung.cn

[S56] C++：optional
来源：http://pg.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zt.huixiangedu.cn

[S57] C++：编译期常量
来源：http://zs.panjiajie.cn

constexpr int N = 10;
来源：http://kc.szsharing.cn

[S58] C++：命名空间
来源：http://gi.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://ui.panjiajie.cn

[S59] C++：静态断言
来源：http://xw.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gg.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://dm.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yr.gzmigu.cn

================================================================================
来源：http://pv.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qq.szsharing.cn

================================================================================
来源：http://lv.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://aj.newstarts.cn

println("Hello")
来源：http://kw.nicolike.cn

[T02] Kotlin：变量
来源：http://ka.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yb.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://do.gzmigu.cn

"值: $b"
来源：http://it.nszjky.cn

[T04] Kotlin：空安全
来源：http://ck.gzmigu.cn

val n: String? = null;  n?.length
来源：http://wl.colortex.cn

[T05] Kotlin：when 表达式
来源：http://tx.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bx.newstarts.cn

[T06] Kotlin：集合映射
来源：http://ys.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ze.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://oh.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oh.asd995.cn

[T08] Kotlin：数据类
来源：http://pk.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://qn.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://pi.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://pk.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://jt.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jr.hahajie.cn

[T11] Kotlin：协程
来源：http://zl.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cf.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ze.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://lz.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://mr.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://ys.huanxung.cn

[T14] Kotlin：循环
来源：http://cy.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://bs.huanxung.cn

[T15] Kotlin：接口
来源：http://jr.9csxet.cn

interface Shape { fun area(): Double }
来源：http://vz.huanxung.cn

[T16] Swift：Hello World
来源：http://ym.huixiangedu.cn

print("Hello")
来源：http://bg.gzmigu.cn

[T17] Swift：变量与常量
来源：http://cn.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://lx.nicolike.cn

[T18] Swift：字符串插值
来源：http://mz.lnxyls.cn

"值: \(b)"
来源：http://vs.asd995.cn

[T19] Swift：可选绑定
来源：http://wm.colortex.cn

if let n = opt { print(n) }
来源：http://ts.9csxet.cn

[T20] Swift：数组操作
来源：http://oa.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pq.nszjky.cn

[T21] Swift：遍历
来源：http://mc.huixiangedu.cn

for x in a { print(x) }
来源：http://qt.szxytkj.cn

[T22] Swift：字典
来源：http://jf.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ft.nicolike.cn

[T23] Swift：函数
来源：http://we.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zf.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://iv.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gj.jctech888.com.cn

[T25] Swift：结构体
来源：http://jv.9csxet.cn

struct P { var x: Int }
来源：http://mp.huixiangedu.cn

[T26] Swift：类与重写
来源：http://pw.lnxyls.cn

class A: Base { override func f() {} }
来源：http://ds.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ig.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://nr.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://xw.muxihuayi.cn

enum Color { case red, green }
来源：http://af.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://jk.hahajie.cn

guard let x = opt else { return }
来源：http://vi.huixiangedu.cn

[T30] Swift：协议
来源：http://yh.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://fw.shtwfgs.cn

[T31] Lua：Hello World
来源：http://to.gzmigu.cn

print("Hello")
来源：http://ha.521024.cn

[T32] Lua：局部变量
来源：http://wd.huixinmuqiang.cn

local a = 1
来源：http://ei.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://dx.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ji.hnjuh.cn

[T34] Lua：遍历表
来源：http://cn.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vg.shtwfgs.cn

[T35] Lua：字典表
来源：http://nq.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ko.shtwfgs.cn

[T36] Lua：函数
来源：http://xt.haigaiapp.cn

function add(a, b) return a + b end
来源：http://wu.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://ht.chemitech.net.cn

"a" .. "b"
来源：http://im.szsharing.cn

[T38] Lua：条件
来源：http://zh.9csxet.cn

if x > 0 then print("正") end
来源：http://do.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://ty.asd995.cn

string.find(s, "%d+")
来源：http://wt.nicolike.cn

[T40] Lua：元表
来源：http://gh.huanxung.cn

setmetatable({}, { __index = base })
来源：http://ei.panjiajie.cn

[T41] Perl：Hello World
来源：http://jm.muxihuayi.cn

print "Hello\n";
来源：http://pq.newstarts.cn

[T42] Perl：变量类型
来源：http://ud.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sg.colortex.cn

[T43] Perl：字符串插值
来源：http://pk.9csxet.cn

"值: $a"
来源：http://er.lnxyls.cn

[T44] Perl：条件
来源：http://nq.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://hs.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://ed.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://ed.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://hk.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xl.lnxyls.cn

[T47] Perl：正则捕获
来源：http://cg.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yd.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://jg.hahajie.cn

$s =~ s/old/new/g;
来源：http://bi.shtwfgs.cn

[T49] Perl：函数
来源：http://vy.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wg.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://bm.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jd.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://fc.newstarts.cn

[T51] Scala：Hello World
来源：http://cp.gzmigu.cn

println("Hello")
来源：http://cr.shxzskj.cn

[T52] Scala：变量
来源：http://ra.shxzskj.cn

val a = 1;  var b = 2
来源：http://na.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://mw.huixiangedu.cn

s"值: $b"
来源：http://bn.hnjuh.cn

[T54] Scala：集合映射
来源：http://ts.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ip.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ob.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ww.newstarts.cn

[T56] Scala：样例类
来源：http://qp.asd995.cn

case class User(name: String, age: Int)
来源：http://bi.521024.cn

[T57] Scala：模式匹配
来源：http://ay.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nc.muxihuayi.cn

[T58] Scala：函数定义
来源：http://xp.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pg.jianghongdianzi.cn

[T59] Scala：循环
来源：http://yz.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://ya.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://qu.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cf.shxzukj.cn

================================================================================
来源：http://py.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lc.huanxung.cn

================================================================================
来源：http://zt.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://pp.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sp.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://ya.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wk.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://rs.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jy.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://wu.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ow.szsharing.cn

[U05] Py：列表去重且保序
来源：http://ez.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://gx.colortex.cn

[U06] Py：合并两个字典
来源：http://fp.nicolike.cn

{**a, **b}
来源：http://sj.9csxet.cn

[U07] Py：反转字典键值
来源：http://om.szsharing.cn

{v: k for k, v in d.items()}
来源：http://uo.521024.cn

[U08] Py：展平二维列表
来源：http://gp.shxzukj.cn

[y for x in nested for y in x]
来源：http://fv.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://zm.521024.cn

max(d, key=d.get)
来源：http://ar.asd995.cn

[U10] Py：按值排序字典
来源：http://ll.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xd.huanxung.cn

[U11] Py：生成器表达式
来源：http://do.yuexingan06.cn

(x * 2 for x in arr)
来源：http://bi.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://io.hnjuh.cn

Counter(arr).most_common(3)
来源：http://zc.9csxet.cn

[U13] Py：固定长度队列
来源：http://bx.szxytkj.cn

deque(maxlen=10)
来源：http://vz.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://qd.asd995.cn

defaultdict(list)
来源：http://jh.szxytkj.cn

[U15] Py：高精度计时
来源：http://ms.wgjwhj.cn

t = time.perf_counter()
来源：http://ki.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://nn.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ub.gzmigu.cn

[U17] Py：初始化日志
来源：http://qv.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://ej.chemitech.net.cn

[U18] Py：预编译正则
来源：http://uo.colortex.cn

pat = re.compile(r"\d+")
来源：http://uc.szsharing.cn

[U19] Py：正则替换带回调
来源：http://le.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ou.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://ws.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://ht.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://mg.shxzukj.cn

@contextlib.contextmanager
来源：http://ho.colortex.cn

[U22] Py：矩阵转置
来源：http://qr.panjiajie.cn

list(zip(*m))
来源：http://zn.huanxung.cn

[U23] Py：分块读取大文件
来源：http://oa.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qn.hahajie.cn

[U24] Py：路径操作
来源：http://at.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://an.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://hh.huixiangedu.cn

csv.DictReader(f)
来源：http://ez.shtwfgs.cn

[U26] Py：并发下载
来源：http://so.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ec.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://rr.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://nf.chemitech.net.cn

[U28] Py：类型别名
来源：http://tn.lnxyls.cn

UserId = int
来源：http://db.bjjhwx.cn

[U29] Py：属性校验
来源：http://id.nicolike.cn

@property 与 @x.setter 配合
来源：http://wv.bookmarksfly.cn

[U30] Py：数据类
来源：http://zh.hahajie.cn

@dataclass(slots=True)
来源：http://tv.521024.cn

[U31] Py：单测
来源：http://uo.muxihuayi.cn

python -m pytest -q
来源：http://el.9csxet.cn

[U32] Py：代码格式化
来源：http://ok.asd995.cn

ruff format . && ruff check --fix .
来源：http://nv.muxihuayi.cn

[U33] Py：打包发布
来源：http://no.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://al.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://mu.shxzukj.cn

chardet.detect(raw)
来源：http://pj.521024.cn

[U35] Py：发送邮件
来源：http://qy.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pf.9csxet.cn

[U36] Py：定时任务
来源：http://ji.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ha.nszjky.cn

[U37] Py：读写 Excel
来源：http://ef.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ug.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://pm.nicolike.cn

Path(__file__).resolve().parent
来源：http://qq.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://bi.huixiangedu.cn

sys.stdout.isatty()
来源：http://cd.szsharing.cn

[U40] Py：打印到标准错误
来源：http://vr.521024.cn

print("err", file=sys.stderr)
来源：http://dx.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://nx.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cp.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://sd.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bv.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://qv.jctech888.com.cn

namespace App\Http;
来源：http://rw.asd995.cn

[U44] PHP：开启严格类型
来源：http://lr.lnxyls.cn

declare(strict_types=1);
来源：http://io.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://kf.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nc.gzmigu.cn

[U46] PHP：可空类型
来源：http://qt.muxihuayi.cn

?string $name = null
来源：http://gu.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://eu.hahajie.cn

int|string $id
来源：http://es.lnxyls.cn

[U48] PHP：纯枚举
来源：http://ov.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uv.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://dc.521024.cn

public readonly string $name
来源：http://ej.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://cj.nszjky.cn

public function __construct(private int $id) {}
来源：http://td.jctech888.com.cn

[U51] PHP：数组解构
来源：http://ol.shxzukj.cn

[$a, $b] = $arr;
来源：http://vj.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ty.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://vf.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://om.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://ba.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://pp.jianghongdianzi.cn

$obj?->method()
来源：http://xx.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ac.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zq.9csxet.cn

[U56] PHP：命名参数
来源：http://jc.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://ct.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://dr.nszjky.cn

"值: {$a}"
来源：http://ul.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://uo.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ug.shxzukj.cn

[U59] PHP：自定义排序
来源：http://kq.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ux.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://js.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dp.huixiangedu.cn

[U61] PHP：正则
来源：http://tk.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ie.hahajie.cn

[U62] PHP：日期对象
来源：http://kr.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vw.lnxyls.cn

[U63] PHP：文件读写
来源：http://kt.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yv.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://th.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://yx.huixiangedu.cn

[U65] PHP：会话
来源：http://id.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lc.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://dl.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ps.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://ra.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rd.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://yc.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jo.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://jr.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xq.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ay.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dx.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://bk.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://jt.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://gh.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://iz.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://xk.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://dz.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://ki.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://hs.9csxet.cn


<!-- 参考信息 -->