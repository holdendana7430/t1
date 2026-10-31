代发 wailian999

int size() const noexcept { return n_; }
来源：http://go.muxihuayi.cn

[S53] C++：移动语义
来源：http://fg.521024.cn

std::vector<int> w = std::move(v);
来源：http://vt.bjjhwx.cn

[S54] C++：异常处理
来源：http://nu.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pf.szsharing.cn

[S55] C++：结构化绑定
来源：http://jb.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ow.shxzukj.cn

[S56] C++：optional
来源：http://pu.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ml.nszjky.cn

[S57] C++：编译期常量
来源：http://qr.asd995.cn

constexpr int N = 10;
来源：http://nw.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://uq.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://lt.haigaiapp.cn

[S59] C++：静态断言
来源：http://oi.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zp.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://yh.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zi.huixiangedu.cn

================================================================================
来源：http://ie.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uv.yuntaijiaju.cn

================================================================================
来源：http://ee.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://tk.chemitech.net.cn

println("Hello")
来源：http://od.lnxyls.cn

[T02] Kotlin：变量
来源：http://iy.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kj.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://vx.panjiajie.cn

"值: $b"
来源：http://xw.colortex.cn

[T04] Kotlin：空安全
来源：http://jn.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://vk.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://er.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gb.newstarts.cn

[T06] Kotlin：集合映射
来源：http://lp.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ha.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://dk.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sv.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://yh.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://fv.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://ib.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://qc.szsharing.cn

[T10] Kotlin：默认参数
来源：http://fv.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tz.shtwfgs.cn

[T11] Kotlin：协程
来源：http://sc.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qq.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://xn.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://ty.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://kd.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://dn.shtwfgs.cn

[T14] Kotlin：循环
来源：http://dy.521024.cn

for (i in 1..10) println(i)
来源：http://la.wgjwhj.cn

[T15] Kotlin：接口
来源：http://cm.hahajie.cn

interface Shape { fun area(): Double }
来源：http://ra.chemitech.net.cn

[T16] Swift：Hello World
来源：http://eg.nszjky.cn

print("Hello")
来源：http://hr.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://cv.shtwfgs.cn

var a = 1;  let b = 2
来源：http://jh.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://vz.szxytkj.cn

"值: \(b)"
来源：http://zz.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://fk.szsharing.cn

if let n = opt { print(n) }
来源：http://mv.szxytkj.cn

[T20] Swift：数组操作
来源：http://xq.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gu.haigaiapp.cn

[T21] Swift：遍历
来源：http://qj.9csxet.cn

for x in a { print(x) }
来源：http://fq.muxihuayi.cn

[T22] Swift：字典
来源：http://id.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oy.nszjky.cn

[T23] Swift：函数
来源：http://xt.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ha.shxzskj.cn

[T24] Swift：闭包
来源：http://kw.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jg.shxzukj.cn

[T25] Swift：结构体
来源：http://oq.panjiajie.cn

struct P { var x: Int }
来源：http://yf.haigaiapp.cn

[T26] Swift：类与重写
来源：http://yp.szxytkj.cn

class A: Base { override func f() {} }
来源：http://ub.shxzskj.cn

[T27] Swift：错误处理
来源：http://ga.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://an.szsharing.cn

[T28] Swift：枚举
来源：http://vn.bjjhwx.cn

enum Color { case red, green }
来源：http://yt.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://ol.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://ke.haigaiapp.cn

[T30] Swift：协议
来源：http://eq.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://kx.nicolike.cn

[T31] Lua：Hello World
来源：http://gr.yuexingan06.cn

print("Hello")
来源：http://km.huanxung.cn

[T32] Lua：局部变量
来源：http://yx.hahajie.cn

local a = 1
来源：http://gf.nszjky.cn

[T33] Lua：表（数组）
来源：http://qv.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qo.bjjhwx.cn

[T34] Lua：遍历表
来源：http://ww.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oh.haigaiapp.cn

[T35] Lua：字典表
来源：http://vb.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://eq.shxzukj.cn

[T36] Lua：函数
来源：http://jz.newstarts.cn

function add(a, b) return a + b end
来源：http://jk.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://oq.shxzskj.cn

"a" .. "b"
来源：http://pm.hnjuh.cn

[T38] Lua：条件
来源：http://ph.shxzskj.cn

if x > 0 then print("正") end
来源：http://ix.asd995.cn

[T39] Lua：模式匹配
来源：http://mk.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://yk.bookmarksfly.cn

[T40] Lua：元表
来源：http://ix.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://hj.521024.cn

[T41] Perl：Hello World
来源：http://iq.newstarts.cn

print "Hello\n";
来源：http://tc.wgjwhj.cn

[T42] Perl：变量类型
来源：http://ar.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yx.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://ib.muxihuayi.cn

"值: $a"
来源：http://qa.shxzskj.cn

[T44] Perl：条件
来源：http://hd.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://gn.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://dp.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://os.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://he.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kj.panjiajie.cn

[T47] Perl：正则捕获
来源：http://pe.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://po.shxzskj.cn

[T48] Perl：正则替换
来源：http://cx.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://yo.asd995.cn

[T49] Perl：函数
来源：http://fg.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xi.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://oj.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zl.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://qj.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://gy.huixinmuqiang.cn

println("Hello")
来源：http://kb.asd995.cn

[T52] Scala：变量
来源：http://fs.newstarts.cn

val a = 1;  var b = 2
来源：http://xj.panjiajie.cn

[T53] Scala：字符串插值
来源：http://xu.szsharing.cn

s"值: $b"
来源：http://bh.gzmigu.cn

[T54] Scala：集合映射
来源：http://ll.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://qy.gzmigu.cn

[T55] Scala：集合过滤
来源：http://fs.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ni.521024.cn

[T56] Scala：样例类
来源：http://ij.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://me.huanxung.cn

[T57] Scala：模式匹配
来源：http://yv.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pw.gzmigu.cn

[T58] Scala：函数定义
来源：http://xi.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zg.wgjwhj.cn

[T59] Scala：循环
来源：http://ln.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://ww.huanxung.cn

[T60] Scala：折叠
来源：http://qm.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lt.panjiajie.cn

================================================================================
来源：http://dh.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pu.nicolike.cn

================================================================================
来源：http://fo.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://ns.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dq.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://fc.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nc.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://iw.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qk.lnxyls.cn

[U04] Py：变量调试打印
来源：http://vs.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lo.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://bg.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://kq.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://rt.muxihuayi.cn

{**a, **b}
来源：http://fq.hnjuh.cn

[U07] Py：反转字典键值
来源：http://aq.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://mt.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://sj.hnjuh.cn

[y for x in nested for y in x]
来源：http://hn.521024.cn

[U09] Py：字典取最大值的键
来源：http://lu.hnjuh.cn

max(d, key=d.get)
来源：http://vu.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://wu.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kg.hahajie.cn

[U11] Py：生成器表达式
来源：http://ce.newstarts.cn

(x * 2 for x in arr)
来源：http://qd.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wj.panjiajie.cn

Counter(arr).most_common(3)
来源：http://xy.huanxung.cn

[U13] Py：固定长度队列
来源：http://tm.hnjuh.cn

deque(maxlen=10)
来源：http://fw.szsharing.cn

[U14] Py：分组收集到列表
来源：http://rd.newstarts.cn

defaultdict(list)
来源：http://lw.szsharing.cn

[U15] Py：高精度计时
来源：http://un.huixinmuqiang.cn

t = time.perf_counter()
来源：http://oq.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://vt.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vw.shxzskj.cn

[U17] Py：初始化日志
来源：http://ck.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://zq.colortex.cn

[U18] Py：预编译正则
来源：http://gv.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ko.szsharing.cn

[U19] Py：正则替换带回调
来源：http://oa.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://my.huanxung.cn

[U20] Py：缓存函数结果
来源：http://sm.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://vk.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://vv.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://bp.9csxet.cn

[U22] Py：矩阵转置
来源：http://wu.shtwfgs.cn

list(zip(*m))
来源：http://ej.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://yg.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pq.szsharing.cn

[U24] Py：路径操作
来源：http://wt.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ex.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://su.nicolike.cn

csv.DictReader(f)
来源：http://ly.chemitech.net.cn

[U26] Py：并发下载
来源：http://ic.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wi.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://xt.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ou.9csxet.cn

[U28] Py：类型别名
来源：http://wc.lnxyls.cn

UserId = int
来源：http://ea.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://oh.panjiajie.cn

@property 与 @x.setter 配合
来源：http://fj.shxzskj.cn

[U30] Py：数据类
来源：http://fm.shxzukj.cn

@dataclass(slots=True)
来源：http://oy.muxihuayi.cn

[U31] Py：单测
来源：http://hj.huixinmuqiang.cn

python -m pytest -q
来源：http://yb.shxzskj.cn

[U32] Py：代码格式化
来源：http://sj.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://jr.wgjwhj.cn

[U33] Py：打包发布
来源：http://ec.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://dh.nszjky.cn

[U34] Py：判断编码
来源：http://za.szxytkj.cn

chardet.detect(raw)
来源：http://bu.hnjuh.cn

[U35] Py：发送邮件
来源：http://mq.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mw.chemitech.net.cn

[U36] Py：定时任务
来源：http://pn.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://ow.colortex.cn

[U37] Py：读写 Excel
来源：http://fy.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yv.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://lc.colortex.cn

Path(__file__).resolve().parent
来源：http://wz.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://hx.szsharing.cn

sys.stdout.isatty()
来源：http://qq.nicolike.cn

[U40] Py：打印到标准错误
来源：http://xv.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://og.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://zk.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tz.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ns.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aa.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://uv.bjjhwx.cn

namespace App\Http;
来源：http://gl.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://wq.yuntaijiaju.cn

declare(strict_types=1);
来源：http://yk.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://hx.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mz.muxihuayi.cn

[U46] PHP：可空类型
来源：http://mn.huanxung.cn

?string $name = null
来源：http://ys.haigaiapp.cn

[U47] PHP：联合类型
来源：http://qa.bjjhwx.cn

int|string $id
来源：http://mj.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://jb.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cd.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://ev.hnjuh.cn

public readonly string $name
来源：http://pn.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://le.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://uj.haigaiapp.cn

[U51] PHP：数组解构
来源：http://nm.nszjky.cn

[$a, $b] = $arr;
来源：http://nh.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://gs.521024.cn

$double = fn($x) => $x * 2;
来源：http://sp.nicolike.cn

[U53] PHP：空合并运算符
来源：http://cn.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://cs.szxytkj.cn

[U54] PHP：空安全调用
来源：http://pn.jctech888.com.cn

$obj?->method()
来源：http://ed.shxzukj.cn

[U55] PHP：match 表达式
来源：http://zx.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qz.szxytkj.cn

[U56] PHP：命名参数
来源：http://xx.newstarts.cn

f(a: 1, b: 2)
来源：http://zj.gzmigu.cn

[U57] PHP：字符串插值
来源：http://pk.huanxung.cn

"值: {$a}"
来源：http://dr.hnjuh.cn

[U58] PHP：数组三件套
来源：http://xp.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://er.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://yx.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gr.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://uh.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oj.panjiajie.cn

[U61] PHP：正则
来源：http://ir.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ll.asd995.cn

[U62] PHP：日期对象
来源：http://je.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rz.nszjky.cn

[U63] PHP：文件读写
来源：http://gr.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xr.szsharing.cn

[U64] PHP：目录遍历
来源：http://bf.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://xy.muxihuayi.cn

[U65] PHP：会话
来源：http://aj.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bz.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://lf.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qo.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://rw.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yw.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://ff.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ul.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://lp.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ay.nicolike.cn

[U70] PHP：PDO 事务
来源：http://qk.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ib.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://cs.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://iw.521024.cn

[U72] PHP：写错误日志
来源：http://pq.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://ot.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://ua.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://fq.huanxung.cn

[U74] PHP：读取环境变量
来源：http://gy.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://rt.521024.cn

[U75] PHP：依赖注入
来源：http://la.nszjky.cn

composer require psr/container
来源：http://zn.shxzskj.cn

[U76] PHP：简单路由
来源：http://ps.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ia.nszjky.cn

[U77] PHP：模板渲染
来源：http://wh.huixinmuqiang.cn

composer require twig/twig
来源：http://ej.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ko.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://fq.bookmarksfly.cn


<!-- 参考信息 -->