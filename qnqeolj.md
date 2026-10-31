代发 wailian999

int size() const noexcept { return n_; }
来源：http://fv.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://rf.521024.cn

std::vector<int> w = std::move(v);
来源：http://qp.lnxyls.cn

[S54] C++：异常处理
来源：http://eg.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://us.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://cn.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qw.bjjhwx.cn

[S56] C++：optional
来源：http://ou.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nk.shtwfgs.cn

[S57] C++：编译期常量
来源：http://wt.hahajie.cn

constexpr int N = 10;
来源：http://ag.nicolike.cn

[S58] C++：命名空间
来源：http://gm.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://wj.shtwfgs.cn

[S59] C++：静态断言
来源：http://gm.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ba.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://fm.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qm.bookmarksfly.cn

================================================================================
来源：http://nt.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zn.asd995.cn

================================================================================
来源：http://ww.szsharing.cn

[T01] Kotlin：Hello World
来源：http://ij.muxihuayi.cn

println("Hello")
来源：http://bs.lnxyls.cn

[T02] Kotlin：变量
来源：http://ym.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ea.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://iw.bookmarksfly.cn

"值: $b"
来源：http://sq.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://fe.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://zt.521024.cn

[T05] Kotlin：when 表达式
来源：http://cl.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://te.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://pb.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wd.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ui.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nt.hnjuh.cn

[T08] Kotlin：数据类
来源：http://az.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://ot.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://tq.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://yp.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://fb.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gk.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://wg.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lo.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://uy.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://pi.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://id.huanxung.cn

val m = mapOf("a" to 1)
来源：http://or.nicolike.cn

[T14] Kotlin：循环
来源：http://tu.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://fy.jctech888.com.cn

[T15] Kotlin：接口
来源：http://hn.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://id.chemitech.net.cn

[T16] Swift：Hello World
来源：http://dg.nicolike.cn

print("Hello")
来源：http://fh.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ci.9csxet.cn

var a = 1;  let b = 2
来源：http://ib.szsharing.cn

[T18] Swift：字符串插值
来源：http://sp.hahajie.cn

"值: \(b)"
来源：http://xr.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://zb.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ps.nszjky.cn

[T20] Swift：数组操作
来源：http://ds.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hs.shtwfgs.cn

[T21] Swift：遍历
来源：http://oo.shxzskj.cn

for x in a { print(x) }
来源：http://kf.jctech888.com.cn

[T22] Swift：字典
来源：http://kd.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rd.huixiangedu.cn

[T23] Swift：函数
来源：http://ae.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rp.wgjwhj.cn

[T24] Swift：闭包
来源：http://rz.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qt.muxihuayi.cn

[T25] Swift：结构体
来源：http://uq.hahajie.cn

struct P { var x: Int }
来源：http://sd.shxzukj.cn

[T26] Swift：类与重写
来源：http://cz.huanxung.cn

class A: Base { override func f() {} }
来源：http://rl.panjiajie.cn

[T27] Swift：错误处理
来源：http://rp.nszjky.cn

do { try f() } catch { print(error) }
来源：http://ji.panjiajie.cn

[T28] Swift：枚举
来源：http://rv.chemitech.net.cn

enum Color { case red, green }
来源：http://zf.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://as.wgjwhj.cn

guard let x = opt else { return }
来源：http://te.yuntaijiaju.cn

[T30] Swift：协议
来源：http://uf.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://dq.huixiangedu.cn

[T31] Lua：Hello World
来源：http://wn.nszjky.cn

print("Hello")
来源：http://qm.asd995.cn

[T32] Lua：局部变量
来源：http://uw.lnxyls.cn

local a = 1
来源：http://ai.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://ah.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rg.muxihuayi.cn

[T34] Lua：遍历表
来源：http://sh.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cp.chemitech.net.cn

[T35] Lua：字典表
来源：http://ra.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://db.gzmigu.cn

[T36] Lua：函数
来源：http://up.nicolike.cn

function add(a, b) return a + b end
来源：http://yp.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://rb.lnxyls.cn

"a" .. "b"
来源：http://nb.yuexingan06.cn

[T38] Lua：条件
来源：http://on.gzmigu.cn

if x > 0 then print("正") end
来源：http://sx.hnjuh.cn

[T39] Lua：模式匹配
来源：http://og.bookmarksfly.cn

string.find(s, "%d+")
来源：http://wp.hahajie.cn

[T40] Lua：元表
来源：http://ys.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://ix.muxihuayi.cn

[T41] Perl：Hello World
来源：http://mz.yuntaijiaju.cn

print "Hello\n";
来源：http://tz.9csxet.cn

[T42] Perl：变量类型
来源：http://mn.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kl.9csxet.cn

[T43] Perl：字符串插值
来源：http://wq.hahajie.cn

"值: $a"
来源：http://ok.bookmarksfly.cn

[T44] Perl：条件
来源：http://mj.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://fb.panjiajie.cn

[T45] Perl：数组遍历
来源：http://xd.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://lv.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://uj.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cs.lnxyls.cn

[T47] Perl：正则捕获
来源：http://dv.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ug.colortex.cn

[T48] Perl：正则替换
来源：http://cx.shxzskj.cn

$s =~ s/old/new/g;
来源：http://of.gzmigu.cn

[T49] Perl：函数
来源：http://bq.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mc.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://gt.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gv.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ll.hnjuh.cn

[T51] Scala：Hello World
来源：http://zx.bookmarksfly.cn

println("Hello")
来源：http://ms.chemitech.net.cn

[T52] Scala：变量
来源：http://jf.521024.cn

val a = 1;  var b = 2
来源：http://ob.panjiajie.cn

[T53] Scala：字符串插值
来源：http://dn.szxytkj.cn

s"值: $b"
来源：http://zu.colortex.cn

[T54] Scala：集合映射
来源：http://xr.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ey.szsharing.cn

[T55] Scala：集合过滤
来源：http://fh.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oc.yuexingan06.cn

[T56] Scala：样例类
来源：http://yl.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://em.hahajie.cn

[T57] Scala：模式匹配
来源：http://dr.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hh.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://uz.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rx.chemitech.net.cn

[T59] Scala：循环
来源：http://vg.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://sd.lnxyls.cn

[T60] Scala：折叠
来源：http://wj.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fp.haigaiapp.cn

================================================================================
来源：http://wv.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gk.nszjky.cn

================================================================================
来源：http://jv.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://lb.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ol.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://fu.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kb.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://gp.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wy.shxzukj.cn

[U04] Py：变量调试打印
来源：http://dv.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kq.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://ir.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://es.nszjky.cn

[U06] Py：合并两个字典
来源：http://uq.bjjhwx.cn

{**a, **b}
来源：http://tn.szxytkj.cn

[U07] Py：反转字典键值
来源：http://zt.nicolike.cn

{v: k for k, v in d.items()}
来源：http://jg.asd995.cn

[U08] Py：展平二维列表
来源：http://oo.asd995.cn

[y for x in nested for y in x]
来源：http://oj.521024.cn

[U09] Py：字典取最大值的键
来源：http://wr.huanxung.cn

max(d, key=d.get)
来源：http://pl.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://ss.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tq.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://vr.nicolike.cn

(x * 2 for x in arr)
来源：http://yo.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zi.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ai.szsharing.cn

[U13] Py：固定长度队列
来源：http://ra.asd995.cn

deque(maxlen=10)
来源：http://ar.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://mc.colortex.cn

defaultdict(list)
来源：http://cd.asd995.cn

[U15] Py：高精度计时
来源：http://sv.huixiangedu.cn

t = time.perf_counter()
来源：http://vy.nszjky.cn

[U16] Py：命令行参数解析
来源：http://ma.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://td.lnxyls.cn

[U17] Py：初始化日志
来源：http://oh.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://md.huixiangedu.cn

[U18] Py：预编译正则
来源：http://gg.nicolike.cn

pat = re.compile(r"\d+")
来源：http://wq.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://xn.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tm.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://nv.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://nj.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://ne.9csxet.cn

@contextlib.contextmanager
来源：http://xw.hnjuh.cn

[U22] Py：矩阵转置
来源：http://kr.wgjwhj.cn

list(zip(*m))
来源：http://mt.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://ln.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dq.panjiajie.cn

[U24] Py：路径操作
来源：http://ml.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vy.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://gs.yuntaijiaju.cn

csv.DictReader(f)
来源：http://ij.hnjuh.cn

[U26] Py：并发下载
来源：http://az.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yv.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://pu.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://fe.521024.cn

[U28] Py：类型别名
来源：http://ok.haigaiapp.cn

UserId = int
来源：http://rz.haigaiapp.cn

[U29] Py：属性校验
来源：http://cw.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://zy.chemitech.net.cn

[U30] Py：数据类
来源：http://vi.lnxyls.cn

@dataclass(slots=True)
来源：http://fe.newstarts.cn

[U31] Py：单测
来源：http://bo.shxzukj.cn

python -m pytest -q
来源：http://ox.haigaiapp.cn

[U32] Py：代码格式化
来源：http://tr.huanxung.cn

ruff format . && ruff check --fix .
来源：http://oh.shtwfgs.cn

[U33] Py：打包发布
来源：http://is.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://po.panjiajie.cn

[U34] Py：判断编码
来源：http://xg.nszjky.cn

chardet.detect(raw)
来源：http://kb.lnxyls.cn

[U35] Py：发送邮件
来源：http://xs.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://me.muxihuayi.cn

[U36] Py：定时任务
来源：http://no.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://bf.hnjuh.cn

[U37] Py：读写 Excel
来源：http://qp.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://um.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://pg.huanxung.cn

Path(__file__).resolve().parent
来源：http://jz.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://vd.shxzskj.cn

sys.stdout.isatty()
来源：http://xq.9csxet.cn

[U40] Py：打印到标准错误
来源：http://kl.shxzukj.cn

print("err", file=sys.stderr)
来源：http://hc.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://yf.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gm.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://rs.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://md.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://sa.shxzukj.cn

namespace App\Http;
来源：http://et.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://kz.shxzukj.cn

declare(strict_types=1);
来源：http://ui.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://wa.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ys.lnxyls.cn

[U46] PHP：可空类型
来源：http://na.yuntaijiaju.cn

?string $name = null
来源：http://cq.muxihuayi.cn

[U47] PHP：联合类型
来源：http://rm.nicolike.cn

int|string $id
来源：http://pg.asd995.cn

[U48] PHP：纯枚举
来源：http://ig.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://db.shxzskj.cn

[U49] PHP：只读属性
来源：http://wj.shxzskj.cn

public readonly string $name
来源：http://ta.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://up.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://ff.huixiangedu.cn

[U51] PHP：数组解构
来源：http://am.jctech888.com.cn

[$a, $b] = $arr;
来源：http://hf.asd995.cn

[U52] PHP：箭头函数
来源：http://kq.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://xm.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://mo.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://if.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://hm.shtwfgs.cn

$obj?->method()
来源：http://se.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://wi.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vo.muxihuayi.cn

[U56] PHP：命名参数
来源：http://nn.panjiajie.cn

f(a: 1, b: 2)
来源：http://lc.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://ch.gzmigu.cn

"值: {$a}"
来源：http://td.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://kp.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gd.9csxet.cn

[U59] PHP：自定义排序
来源：http://cx.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oy.521024.cn

[U60] PHP：JSON 编解码
来源：http://ra.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zs.jianghongdianzi.cn

[U61] PHP：正则
来源：http://hp.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oq.szxytkj.cn

[U62] PHP：日期对象
来源：http://vu.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ny.shxzukj.cn

[U63] PHP：文件读写
来源：http://lh.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qv.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://pi.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://kg.jianghongdianzi.cn

[U65] PHP：会话
来源：http://fs.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pr.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://rw.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tp.521024.cn

[U67] PHP：处理文件上传
来源：http://ar.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jr.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://uk.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cy.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://jt.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mm.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://ax.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zf.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ag.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://en.hahajie.cn

[U72] PHP：写错误日志
来源：http://en.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ea.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://yu.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://fm.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://qd.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://zd.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://nb.huanxung.cn

composer require psr/container
来源：http://ts.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://fq.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vh.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://ug.haigaiapp.cn

composer require twig/twig
来源：http://px.newstarts.cn

[U78] PHP：单元测试
来源：http://cz.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://dj.gzmigu.cn


<!-- 参考信息 -->