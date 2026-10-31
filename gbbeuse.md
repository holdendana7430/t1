代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xi.521024.cn

[S51] C++：显式类型转换
来源：http://zr.colortex.cn

static_cast<double>(a) / b
来源：http://zt.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://az.nicolike.cn

int size() const noexcept { return n_; }
来源：http://ix.521024.cn

[S53] C++：移动语义
来源：http://sx.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://ez.yuexingan06.cn

[S54] C++：异常处理
来源：http://mq.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eh.newstarts.cn

[S55] C++：结构化绑定
来源：http://wr.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pi.colortex.cn

[S56] C++：optional
来源：http://ee.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xi.huixiangedu.cn

[S57] C++：编译期常量
来源：http://gr.szsharing.cn

constexpr int N = 10;
来源：http://sw.colortex.cn

[S58] C++：命名空间
来源：http://vy.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://bi.szxytkj.cn

[S59] C++：静态断言
来源：http://pg.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ef.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://qb.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://is.shxzskj.cn

================================================================================
来源：http://gb.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pd.huixinmuqiang.cn

================================================================================
来源：http://zj.521024.cn

[T01] Kotlin：Hello World
来源：http://wz.szsharing.cn

println("Hello")
来源：http://ut.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://eg.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ki.521024.cn

[T03] Kotlin：字符串模板
来源：http://br.bookmarksfly.cn

"值: $b"
来源：http://zr.newstarts.cn

[T04] Kotlin：空安全
来源：http://jh.shxzukj.cn

val n: String? = null;  n?.length
来源：http://kh.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://do.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ff.nicolike.cn

[T06] Kotlin：集合映射
来源：http://zn.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ig.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://em.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dt.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://hj.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://vc.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://cp.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://bk.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://zn.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fb.hnjuh.cn

[T11] Kotlin：协程
来源：http://wq.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wq.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://uc.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://zg.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://zl.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://wi.shtwfgs.cn

[T14] Kotlin：循环
来源：http://rf.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://uc.colortex.cn

[T15] Kotlin：接口
来源：http://rf.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://ah.shxzskj.cn

[T16] Swift：Hello World
来源：http://ul.huanxung.cn

print("Hello")
来源：http://ai.hnjuh.cn

[T17] Swift：变量与常量
来源：http://us.wgjwhj.cn

var a = 1;  let b = 2
来源：http://rh.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://mh.huixiangedu.cn

"值: \(b)"
来源：http://mw.nszjky.cn

[T19] Swift：可选绑定
来源：http://ap.newstarts.cn

if let n = opt { print(n) }
来源：http://af.lnxyls.cn

[T20] Swift：数组操作
来源：http://qu.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yf.bookmarksfly.cn

[T21] Swift：遍历
来源：http://go.shxzukj.cn

for x in a { print(x) }
来源：http://mo.9csxet.cn

[T22] Swift：字典
来源：http://no.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ql.szsharing.cn

[T23] Swift：函数
来源：http://eg.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://on.hahajie.cn

[T24] Swift：闭包
来源：http://zs.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tn.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://jk.muxihuayi.cn

struct P { var x: Int }
来源：http://ce.shxzukj.cn

[T26] Swift：类与重写
来源：http://yt.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://fp.lnxyls.cn

[T27] Swift：错误处理
来源：http://sr.szsharing.cn

do { try f() } catch { print(error) }
来源：http://vx.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://av.muxihuayi.cn

enum Color { case red, green }
来源：http://wh.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://nr.shxzskj.cn

guard let x = opt else { return }
来源：http://nt.wgjwhj.cn

[T30] Swift：协议
来源：http://fn.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ee.shtwfgs.cn

[T31] Lua：Hello World
来源：http://lh.shxzukj.cn

print("Hello")
来源：http://se.shxzskj.cn

[T32] Lua：局部变量
来源：http://gk.yuexingan06.cn

local a = 1
来源：http://kq.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://pc.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ux.521024.cn

[T34] Lua：遍历表
来源：http://ni.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sq.gzmigu.cn

[T35] Lua：字典表
来源：http://td.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://wr.chemitech.net.cn

[T36] Lua：函数
来源：http://es.lnxyls.cn

function add(a, b) return a + b end
来源：http://iw.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://qt.colortex.cn

"a" .. "b"
来源：http://lb.nicolike.cn

[T38] Lua：条件
来源：http://ey.newstarts.cn

if x > 0 then print("正") end
来源：http://ex.nicolike.cn

[T39] Lua：模式匹配
来源：http://fv.9csxet.cn

string.find(s, "%d+")
来源：http://ml.szxytkj.cn

[T40] Lua：元表
来源：http://xn.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://xw.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ro.szsharing.cn

print "Hello\n";
来源：http://iy.muxihuayi.cn

[T42] Perl：变量类型
来源：http://ko.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pv.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://us.9csxet.cn

"值: $a"
来源：http://vc.nicolike.cn

[T44] Perl：条件
来源：http://lj.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://fy.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://jr.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://vz.asd995.cn

[T46] Perl：哈希操作
来源：http://ss.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ka.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://xq.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rn.panjiajie.cn

[T48] Perl：正则替换
来源：http://yj.colortex.cn

$s =~ s/old/new/g;
来源：http://nd.521024.cn

[T49] Perl：函数
来源：http://pf.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://px.nszjky.cn

[T50] Perl：逐行读文件
来源：http://md.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jf.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://pv.szsharing.cn

[T51] Scala：Hello World
来源：http://he.jctech888.com.cn

println("Hello")
来源：http://ku.bookmarksfly.cn

[T52] Scala：变量
来源：http://yy.shxzukj.cn

val a = 1;  var b = 2
来源：http://am.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://rr.9csxet.cn

s"值: $b"
来源：http://rq.bjjhwx.cn

[T54] Scala：集合映射
来源：http://gx.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://nz.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://iu.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qu.szsharing.cn

[T56] Scala：样例类
来源：http://qm.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://qx.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://aq.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ym.bjjhwx.cn

[T58] Scala：函数定义
来源：http://mq.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://di.szsharing.cn

[T59] Scala：循环
来源：http://os.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://zl.521024.cn

[T60] Scala：折叠
来源：http://iv.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ut.hahajie.cn

================================================================================
来源：http://mh.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kp.521024.cn

================================================================================
来源：http://rb.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://th.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bm.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://sz.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lb.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://wv.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uq.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://ed.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yy.newstarts.cn

[U05] Py：列表去重且保序
来源：http://hz.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://rl.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://jd.shxzukj.cn

{**a, **b}
来源：http://fu.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://pt.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://cf.shxzskj.cn

[U08] Py：展平二维列表
来源：http://zf.colortex.cn

[y for x in nested for y in x]
来源：http://jy.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://yk.huixinmuqiang.cn

max(d, key=d.get)
来源：http://ym.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://gl.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jc.szsharing.cn

[U11] Py：生成器表达式
来源：http://ds.szxytkj.cn

(x * 2 for x in arr)
来源：http://cj.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mi.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://re.shxzukj.cn

[U13] Py：固定长度队列
来源：http://ar.huixinmuqiang.cn

deque(maxlen=10)
来源：http://kw.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://iq.wgjwhj.cn

defaultdict(list)
来源：http://zw.9csxet.cn

[U15] Py：高精度计时
来源：http://hn.bookmarksfly.cn

t = time.perf_counter()
来源：http://mx.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://fh.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tq.lnxyls.cn

[U17] Py：初始化日志
来源：http://it.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://eu.hahajie.cn

[U18] Py：预编译正则
来源：http://ny.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://ty.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://ro.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ol.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://su.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://ah.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://tj.yuexingan06.cn

@contextlib.contextmanager
来源：http://sg.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://uk.asd995.cn

list(zip(*m))
来源：http://xa.nszjky.cn

[U23] Py：分块读取大文件
来源：http://oj.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ie.newstarts.cn

[U24] Py：路径操作
来源：http://kg.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bs.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://ap.haigaiapp.cn

csv.DictReader(f)
来源：http://no.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://oa.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ks.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://fk.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://pd.hnjuh.cn

[U28] Py：类型别名
来源：http://fn.yuntaijiaju.cn

UserId = int
来源：http://jv.shtwfgs.cn

[U29] Py：属性校验
来源：http://mw.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://gk.huanxung.cn

[U30] Py：数据类
来源：http://qg.gzmigu.cn

@dataclass(slots=True)
来源：http://ed.huanxung.cn

[U31] Py：单测
来源：http://nt.huixinmuqiang.cn

python -m pytest -q
来源：http://xj.shxzskj.cn

[U32] Py：代码格式化
来源：http://cx.nicolike.cn

ruff format . && ruff check --fix .
来源：http://ee.szsharing.cn

[U33] Py：打包发布
来源：http://nm.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://pg.lnxyls.cn

[U34] Py：判断编码
来源：http://kk.hnjuh.cn

chardet.detect(raw)
来源：http://cl.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ta.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jt.yuexingan06.cn

[U36] Py：定时任务
来源：http://ph.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://yd.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://zu.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lk.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://hp.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://cb.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://cf.colortex.cn

sys.stdout.isatty()
来源：http://ad.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://rp.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://vp.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://wz.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zj.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://vn.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://di.huanxung.cn

[U43] PHP：声明命名空间
来源：http://mz.nicolike.cn

namespace App\Http;
来源：http://gr.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://xl.yuntaijiaju.cn

declare(strict_types=1);
来源：http://ao.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://yn.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ik.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://hx.hahajie.cn

?string $name = null
来源：http://lx.shxzskj.cn

[U47] PHP：联合类型
来源：http://lf.shtwfgs.cn

int|string $id
来源：http://xg.huanxung.cn

[U48] PHP：纯枚举
来源：http://cw.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nm.haigaiapp.cn

[U49] PHP：只读属性
来源：http://rf.gzmigu.cn

public readonly string $name
来源：http://tg.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://jt.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://oy.hahajie.cn

[U51] PHP：数组解构
来源：http://cl.lnxyls.cn

[$a, $b] = $arr;
来源：http://jz.gzmigu.cn

[U52] PHP：箭头函数
来源：http://fw.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://kw.asd995.cn

[U53] PHP：空合并运算符
来源：http://qn.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://xf.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://xn.szsharing.cn

$obj?->method()
来源：http://op.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ge.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://so.lnxyls.cn

[U56] PHP：命名参数
来源：http://mm.huixiangedu.cn

f(a: 1, b: 2)
来源：http://qh.lnxyls.cn

[U57] PHP：字符串插值
来源：http://jf.yuntaijiaju.cn

"值: {$a}"
来源：http://hq.hahajie.cn

[U58] PHP：数组三件套
来源：http://nf.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://em.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://xv.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gm.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://se.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zj.asd995.cn

[U61] PHP：正则
来源：http://bm.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fg.asd995.cn

[U62] PHP：日期对象
来源：http://ro.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rv.colortex.cn

[U63] PHP：文件读写
来源：http://mh.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rk.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://es.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://az.newstarts.cn

[U65] PHP：会话
来源：http://ha.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://js.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://ly.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://in.huanxung.cn

[U67] PHP：处理文件上传
来源：http://qv.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://og.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://mv.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tf.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://ux.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ft.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://sl.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://os.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://ny.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://gy.shxzskj.cn

[U72] PHP：写错误日志
来源：http://hm.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://po.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://yf.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://hn.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://vh.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://fa.gzmigu.cn

[U75] PHP：依赖注入
来源：http://em.nicolike.cn

composer require psr/container
来源：http://jk.asd995.cn

[U76] PHP：简单路由
来源：http://dh.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://es.shtwfgs.cn


<!-- 参考信息 -->