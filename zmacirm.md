代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cf.szxytkj.cn

[S51] C++：显式类型转换
来源：http://eo.wgjwhj.cn

static_cast<double>(a) / b
来源：http://ae.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://ng.colortex.cn

int size() const noexcept { return n_; }
来源：http://dp.hahajie.cn

[S53] C++：移动语义
来源：http://tz.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://rf.hahajie.cn

[S54] C++：异常处理
来源：http://vk.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sd.huanxung.cn

[S55] C++：结构化绑定
来源：http://cp.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zw.szsharing.cn

[S56] C++：optional
来源：http://vc.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ga.shxzukj.cn

[S57] C++：编译期常量
来源：http://in.521024.cn

constexpr int N = 10;
来源：http://ye.szxytkj.cn

[S58] C++：命名空间
来源：http://qc.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://xh.huixiangedu.cn

[S59] C++：静态断言
来源：http://us.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sk.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://jl.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hp.shxzukj.cn

================================================================================
来源：http://hn.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.9csxet.cn

================================================================================
来源：http://dx.newstarts.cn

[T01] Kotlin：Hello World
来源：http://vo.bjjhwx.cn

println("Hello")
来源：http://iq.huixiangedu.cn

[T02] Kotlin：变量
来源：http://yj.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://at.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://qt.huixinmuqiang.cn

"值: $b"
来源：http://mo.szxytkj.cn

[T04] Kotlin：空安全
来源：http://zp.shxzukj.cn

val n: String? = null;  n?.length
来源：http://fk.asd995.cn

[T05] Kotlin：when 表达式
来源：http://tn.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://er.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://oe.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://il.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://lc.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pe.9csxet.cn

[T08] Kotlin：数据类
来源：http://ae.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://bc.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://rl.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://qp.nszjky.cn

[T10] Kotlin：默认参数
来源：http://nk.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ja.yuexingan06.cn

[T11] Kotlin：协程
来源：http://ok.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wf.colortex.cn

[T12] Kotlin：解构声明
来源：http://yn.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://kb.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://wk.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://fv.shxzukj.cn

[T14] Kotlin：循环
来源：http://wp.shxzukj.cn

for (i in 1..10) println(i)
来源：http://wg.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://tt.hahajie.cn

interface Shape { fun area(): Double }
来源：http://ab.muxihuayi.cn

[T16] Swift：Hello World
来源：http://lh.bjjhwx.cn

print("Hello")
来源：http://yx.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://wq.haigaiapp.cn

var a = 1;  let b = 2
来源：http://rh.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://ji.gzmigu.cn

"值: \(b)"
来源：http://wx.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://fg.nicolike.cn

if let n = opt { print(n) }
来源：http://ia.yuexingan06.cn

[T20] Swift：数组操作
来源：http://qg.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://km.chemitech.net.cn

[T21] Swift：遍历
来源：http://kw.haigaiapp.cn

for x in a { print(x) }
来源：http://ek.huanxung.cn

[T22] Swift：字典
来源：http://xm.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wv.huanxung.cn

[T23] Swift：函数
来源：http://zw.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hi.huanxung.cn

[T24] Swift：闭包
来源：http://pu.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://av.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://lc.huixinmuqiang.cn

struct P { var x: Int }
来源：http://fl.huixiangedu.cn

[T26] Swift：类与重写
来源：http://ln.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://lu.huanxung.cn

[T27] Swift：错误处理
来源：http://ld.asd995.cn

do { try f() } catch { print(error) }
来源：http://gj.jctech888.com.cn

[T28] Swift：枚举
来源：http://xu.haigaiapp.cn

enum Color { case red, green }
来源：http://ma.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://xp.newstarts.cn

guard let x = opt else { return }
来源：http://db.yuexingan06.cn

[T30] Swift：协议
来源：http://cw.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://mc.gzmigu.cn

[T31] Lua：Hello World
来源：http://xh.muxihuayi.cn

print("Hello")
来源：http://sr.szsharing.cn

[T32] Lua：局部变量
来源：http://ev.bookmarksfly.cn

local a = 1
来源：http://xm.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://dd.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jg.yuexingan06.cn

[T34] Lua：遍历表
来源：http://dp.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.newstarts.cn

[T35] Lua：字典表
来源：http://xj.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://ph.huixinmuqiang.cn

[T36] Lua：函数
来源：http://pk.shxzukj.cn

function add(a, b) return a + b end
来源：http://cb.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://pf.9csxet.cn

"a" .. "b"
来源：http://zp.lnxyls.cn

[T38] Lua：条件
来源：http://ie.gzmigu.cn

if x > 0 then print("正") end
来源：http://fd.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ub.hahajie.cn

string.find(s, "%d+")
来源：http://ie.chemitech.net.cn

[T40] Lua：元表
来源：http://lh.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://nq.hahajie.cn

[T41] Perl：Hello World
来源：http://yn.9csxet.cn

print "Hello\n";
来源：http://eg.szxytkj.cn

[T42] Perl：变量类型
来源：http://ol.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gw.asd995.cn

[T43] Perl：字符串插值
来源：http://ww.panjiajie.cn

"值: $a"
来源：http://ho.hnjuh.cn

[T44] Perl：条件
来源：http://ln.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://le.szsharing.cn

[T45] Perl：数组遍历
来源：http://za.colortex.cn

for my $x (@arr) { print $x; }
来源：http://aj.hnjuh.cn

[T46] Perl：哈希操作
来源：http://rs.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cs.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://am.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oo.gzmigu.cn

[T48] Perl：正则替换
来源：http://jy.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://xx.jctech888.com.cn

[T49] Perl：函数
来源：http://hd.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hv.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://ys.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lo.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://vb.yuexingan06.cn

[T51] Scala：Hello World
来源：http://zn.newstarts.cn

println("Hello")
来源：http://vt.jctech888.com.cn

[T52] Scala：变量
来源：http://dy.yuexingan06.cn

val a = 1;  var b = 2
来源：http://jk.hahajie.cn

[T53] Scala：字符串插值
来源：http://an.huixinmuqiang.cn

s"值: $b"
来源：http://li.lnxyls.cn

[T54] Scala：集合映射
来源：http://qg.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://nw.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://ni.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kx.huixiangedu.cn

[T56] Scala：样例类
来源：http://tq.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://rw.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://rn.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://km.hahajie.cn

[T58] Scala：函数定义
来源：http://bq.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wf.521024.cn

[T59] Scala：循环
来源：http://fd.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://zy.jctech888.com.cn

[T60] Scala：折叠
来源：http://jg.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hv.jctech888.com.cn

================================================================================
来源：http://rm.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fd.panjiajie.cn

================================================================================
来源：http://tx.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://vg.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ml.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://yb.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sm.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://ei.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ue.huanxung.cn

[U04] Py：变量调试打印
来源：http://qx.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ac.asd995.cn

[U05] Py：列表去重且保序
来源：http://uc.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ur.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://iy.nicolike.cn

{**a, **b}
来源：http://ep.hahajie.cn

[U07] Py：反转字典键值
来源：http://op.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://op.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://wx.muxihuayi.cn

[y for x in nested for y in x]
来源：http://pk.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://pb.newstarts.cn

max(d, key=d.get)
来源：http://iy.panjiajie.cn

[U10] Py：按值排序字典
来源：http://js.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lb.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://oy.521024.cn

(x * 2 for x in arr)
来源：http://oe.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xh.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://cb.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://it.huixiangedu.cn

deque(maxlen=10)
来源：http://gn.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://gd.shtwfgs.cn

defaultdict(list)
来源：http://op.chemitech.net.cn

[U15] Py：高精度计时
来源：http://rf.szsharing.cn

t = time.perf_counter()
来源：http://ew.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://bs.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hd.lnxyls.cn

[U17] Py：初始化日志
来源：http://cn.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://mj.asd995.cn

[U18] Py：预编译正则
来源：http://sr.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://rb.521024.cn

[U19] Py：正则替换带回调
来源：http://lf.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ln.szsharing.cn

[U20] Py：缓存函数结果
来源：http://tf.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://jf.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://js.shxzukj.cn

@contextlib.contextmanager
来源：http://ku.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://lm.szxytkj.cn

list(zip(*m))
来源：http://om.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://wm.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xb.asd995.cn

[U24] Py：路径操作
来源：http://kl.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hq.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://en.shxzskj.cn

csv.DictReader(f)
来源：http://da.shxzskj.cn

[U26] Py：并发下载
来源：http://oq.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dk.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://cw.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://vm.colortex.cn

[U28] Py：类型别名
来源：http://os.gzmigu.cn

UserId = int
来源：http://lt.haigaiapp.cn

[U29] Py：属性校验
来源：http://gk.asd995.cn

@property 与 @x.setter 配合
来源：http://yo.shxzskj.cn

[U30] Py：数据类
来源：http://jt.nszjky.cn

@dataclass(slots=True)
来源：http://og.bookmarksfly.cn

[U31] Py：单测
来源：http://si.9csxet.cn

python -m pytest -q
来源：http://ks.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://zu.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://pf.huixiangedu.cn

[U33] Py：打包发布
来源：http://dg.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://yo.gzmigu.cn

[U34] Py：判断编码
来源：http://sc.panjiajie.cn

chardet.detect(raw)
来源：http://lf.shtwfgs.cn

[U35] Py：发送邮件
来源：http://pj.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ty.shtwfgs.cn

[U36] Py：定时任务
来源：http://tm.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://ng.nszjky.cn

[U37] Py：读写 Excel
来源：http://eq.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tm.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://yj.szsharing.cn

Path(__file__).resolve().parent
来源：http://cx.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://lh.9csxet.cn

sys.stdout.isatty()
来源：http://hn.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://iy.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://zp.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://tj.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ss.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://gy.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vw.szsharing.cn

[U43] PHP：声明命名空间
来源：http://xx.hnjuh.cn

namespace App\Http;
来源：http://eu.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://id.jctech888.com.cn

declare(strict_types=1);
来源：http://ot.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://hu.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ml.shxzukj.cn

[U46] PHP：可空类型
来源：http://cm.colortex.cn

?string $name = null
来源：http://xo.521024.cn

[U47] PHP：联合类型
来源：http://cr.9csxet.cn

int|string $id
来源：http://po.shxzskj.cn

[U48] PHP：纯枚举
来源：http://dc.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qk.nszjky.cn

[U49] PHP：只读属性
来源：http://rg.huanxung.cn

public readonly string $name
来源：http://mn.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://zm.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ho.colortex.cn

[U51] PHP：数组解构
来源：http://mb.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ln.gzmigu.cn

[U52] PHP：箭头函数
来源：http://pq.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://zc.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://fh.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://di.asd995.cn

[U54] PHP：空安全调用
来源：http://zy.shxzskj.cn

$obj?->method()
来源：http://rv.colortex.cn

[U55] PHP：match 表达式
来源：http://hs.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gl.shxzskj.cn

[U56] PHP：命名参数
来源：http://qx.bjjhwx.cn

f(a: 1, b: 2)
来源：http://jh.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://ls.panjiajie.cn

"值: {$a}"
来源：http://rk.szsharing.cn

[U58] PHP：数组三件套
来源：http://ok.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ze.hnjuh.cn

[U59] PHP：自定义排序
来源：http://of.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hl.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://dm.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gc.szxytkj.cn

[U61] PHP：正则
来源：http://ch.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pw.lnxyls.cn

[U62] PHP：日期对象
来源：http://nd.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ej.haigaiapp.cn

[U63] PHP：文件读写
来源：http://gn.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://at.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://dg.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://lq.newstarts.cn

[U65] PHP：会话
来源：http://et.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gi.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://ya.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://py.nszjky.cn

[U67] PHP：处理文件上传
来源：http://cf.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://im.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://dq.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lw.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://lj.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wx.nicolike.cn

[U70] PHP：PDO 事务
来源：http://gd.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mx.shxzukj.cn

[U71] PHP：抛出异常
来源：http://hu.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://pi.huanxung.cn

[U72] PHP：写错误日志
来源：http://cc.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://fm.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://jc.asd995.cn

parse_ini_file("config.ini", true)
来源：http://ew.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://ez.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://ce.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://fj.wgjwhj.cn

composer require psr/container
来源：http://cd.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://oo.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qy.chemitech.net.cn


<!-- 参考信息 -->