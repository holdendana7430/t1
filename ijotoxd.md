代发 wailian999

int size() const noexcept { return n_; }
来源：http://na.bjjhwx.cn

[S53] C++：移动语义
来源：http://lr.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://nb.huixiangedu.cn

[S54] C++：异常处理
来源：http://mz.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sn.hnjuh.cn

[S55] C++：结构化绑定
来源：http://bn.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mo.gzmigu.cn

[S56] C++：optional
来源：http://am.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://it.colortex.cn

[S57] C++：编译期常量
来源：http://fy.haigaiapp.cn

constexpr int N = 10;
来源：http://ki.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://vp.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://ov.shtwfgs.cn

[S59] C++：静态断言
来源：http://nr.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nl.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://zs.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lq.huixinmuqiang.cn

================================================================================
来源：http://gb.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ak.muxihuayi.cn

================================================================================
来源：http://cp.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://df.muxihuayi.cn

println("Hello")
来源：http://ec.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://pn.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bz.521024.cn

[T03] Kotlin：字符串模板
来源：http://en.lnxyls.cn

"值: $b"
来源：http://xg.newstarts.cn

[T04] Kotlin：空安全
来源：http://jr.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://yq.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://im.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iw.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://lr.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lv.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://mr.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ho.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://da.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://do.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://pz.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://oo.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://du.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nx.hahajie.cn

[T11] Kotlin：协程
来源：http://nj.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ge.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://jh.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://rq.asd995.cn

[T13] Kotlin：只读 Map
来源：http://rt.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://kh.asd995.cn

[T14] Kotlin：循环
来源：http://oz.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://zx.nszjky.cn

[T15] Kotlin：接口
来源：http://wz.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://pd.hnjuh.cn

[T16] Swift：Hello World
来源：http://sc.9csxet.cn

print("Hello")
来源：http://lc.shxzukj.cn

[T17] Swift：变量与常量
来源：http://oi.shtwfgs.cn

var a = 1;  let b = 2
来源：http://re.nicolike.cn

[T18] Swift：字符串插值
来源：http://wn.yuexingan06.cn

"值: \(b)"
来源：http://sb.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://jj.gzmigu.cn

if let n = opt { print(n) }
来源：http://wa.muxihuayi.cn

[T20] Swift：数组操作
来源：http://al.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lk.shxzskj.cn

[T21] Swift：遍历
来源：http://kt.jctech888.com.cn

for x in a { print(x) }
来源：http://dg.asd995.cn

[T22] Swift：字典
来源：http://ms.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hs.yuntaijiaju.cn

[T23] Swift：函数
来源：http://wo.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vq.nszjky.cn

[T24] Swift：闭包
来源：http://dz.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cx.wgjwhj.cn

[T25] Swift：结构体
来源：http://uc.gzmigu.cn

struct P { var x: Int }
来源：http://li.hahajie.cn

[T26] Swift：类与重写
来源：http://zy.nicolike.cn

class A: Base { override func f() {} }
来源：http://er.9csxet.cn

[T27] Swift：错误处理
来源：http://xr.9csxet.cn

do { try f() } catch { print(error) }
来源：http://zs.hnjuh.cn

[T28] Swift：枚举
来源：http://wg.521024.cn

enum Color { case red, green }
来源：http://qm.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://xk.nicolike.cn

guard let x = opt else { return }
来源：http://gp.haigaiapp.cn

[T30] Swift：协议
来源：http://jp.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://fc.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://pf.huixinmuqiang.cn

print("Hello")
来源：http://dz.jctech888.com.cn

[T32] Lua：局部变量
来源：http://wg.jctech888.com.cn

local a = 1
来源：http://ac.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://nt.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xy.gzmigu.cn

[T34] Lua：遍历表
来源：http://hf.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ii.521024.cn

[T35] Lua：字典表
来源：http://db.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://ry.521024.cn

[T36] Lua：函数
来源：http://ac.haigaiapp.cn

function add(a, b) return a + b end
来源：http://wx.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://jm.nszjky.cn

"a" .. "b"
来源：http://bv.haigaiapp.cn

[T38] Lua：条件
来源：http://ua.shtwfgs.cn

if x > 0 then print("正") end
来源：http://ox.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://gj.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://fk.shtwfgs.cn

[T40] Lua：元表
来源：http://gq.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://rj.521024.cn

[T41] Perl：Hello World
来源：http://ng.yuexingan06.cn

print "Hello\n";
来源：http://xv.nicolike.cn

[T42] Perl：变量类型
来源：http://ob.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cf.asd995.cn

[T43] Perl：字符串插值
来源：http://yb.yuexingan06.cn

"值: $a"
来源：http://pb.shtwfgs.cn

[T44] Perl：条件
来源：http://bh.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://my.panjiajie.cn

[T45] Perl：数组遍历
来源：http://xh.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://kb.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://jv.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://na.colortex.cn

[T47] Perl：正则捕获
来源：http://bq.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aw.gzmigu.cn

[T48] Perl：正则替换
来源：http://gm.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ix.lnxyls.cn

[T49] Perl：函数
来源：http://ql.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ze.newstarts.cn

[T50] Perl：逐行读文件
来源：http://ql.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ny.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://ke.nszjky.cn

[T51] Scala：Hello World
来源：http://ln.huixiangedu.cn

println("Hello")
来源：http://kd.muxihuayi.cn

[T52] Scala：变量
来源：http://no.szsharing.cn

val a = 1;  var b = 2
来源：http://do.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://eh.hahajie.cn

s"值: $b"
来源：http://zg.szxytkj.cn

[T54] Scala：集合映射
来源：http://oy.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://tb.szsharing.cn

[T55] Scala：集合过滤
来源：http://lk.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://he.shxzukj.cn

[T56] Scala：样例类
来源：http://gg.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://sz.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://yl.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ph.asd995.cn

[T58] Scala：函数定义
来源：http://xr.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dw.bookmarksfly.cn

[T59] Scala：循环
来源：http://kr.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://wz.bjjhwx.cn

[T60] Scala：折叠
来源：http://zg.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ea.muxihuayi.cn

================================================================================
来源：http://hx.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cp.shxzukj.cn

================================================================================
来源：http://be.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://br.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ax.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://wf.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bs.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://uw.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ws.gzmigu.cn

[U04] Py：变量调试打印
来源：http://hd.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mx.szsharing.cn

[U05] Py：列表去重且保序
来源：http://pu.9csxet.cn

list(dict.fromkeys(arr))
来源：http://ei.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://zj.yuexingan06.cn

{**a, **b}
来源：http://lb.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://do.colortex.cn

{v: k for k, v in d.items()}
来源：http://hn.szsharing.cn

[U08] Py：展平二维列表
来源：http://la.chemitech.net.cn

[y for x in nested for y in x]
来源：http://kx.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://ro.wgjwhj.cn

max(d, key=d.get)
来源：http://or.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://gn.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ct.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://fi.szxytkj.cn

(x * 2 for x in arr)
来源：http://qz.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://if.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://aq.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://of.shtwfgs.cn

deque(maxlen=10)
来源：http://hf.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://tj.yuntaijiaju.cn

defaultdict(list)
来源：http://sd.shxzukj.cn

[U15] Py：高精度计时
来源：http://gk.colortex.cn

t = time.perf_counter()
来源：http://ce.nszjky.cn

[U16] Py：命令行参数解析
来源：http://ik.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ux.szxytkj.cn

[U17] Py：初始化日志
来源：http://cx.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://rj.haigaiapp.cn

[U18] Py：预编译正则
来源：http://ca.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://qd.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://ex.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xw.nszjky.cn

[U20] Py：缓存函数结果
来源：http://ny.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://wp.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://gl.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://er.colortex.cn

[U22] Py：矩阵转置
来源：http://zq.nicolike.cn

list(zip(*m))
来源：http://ml.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://yv.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ty.huixiangedu.cn

[U24] Py：路径操作
来源：http://aw.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yk.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://bl.panjiajie.cn

csv.DictReader(f)
来源：http://pz.colortex.cn

[U26] Py：并发下载
来源：http://tk.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jl.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://ep.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://qi.shxzskj.cn

[U28] Py：类型别名
来源：http://yu.gzmigu.cn

UserId = int
来源：http://kl.jctech888.com.cn

[U29] Py：属性校验
来源：http://cu.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://qe.wgjwhj.cn

[U30] Py：数据类
来源：http://kc.jctech888.com.cn

@dataclass(slots=True)
来源：http://vv.bjjhwx.cn

[U31] Py：单测
来源：http://ma.huixiangedu.cn

python -m pytest -q
来源：http://zj.panjiajie.cn

[U32] Py：代码格式化
来源：http://us.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://jw.jctech888.com.cn

[U33] Py：打包发布
来源：http://is.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://ms.yuexingan06.cn

[U34] Py：判断编码
来源：http://jr.shxzskj.cn

chardet.detect(raw)
来源：http://jh.chemitech.net.cn

[U35] Py：发送邮件
来源：http://sn.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://om.bookmarksfly.cn

[U36] Py：定时任务
来源：http://sz.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://bb.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://er.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oq.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://xa.asd995.cn

Path(__file__).resolve().parent
来源：http://zd.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://fv.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://gf.nicolike.cn

[U40] Py：打印到标准错误
来源：http://qn.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://on.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://aq.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vr.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vg.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ye.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://ba.yuexingan06.cn

namespace App\Http;
来源：http://bu.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ig.hnjuh.cn

declare(strict_types=1);
来源：http://ju.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://lz.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.wgjwhj.cn

[U46] PHP：可空类型
来源：http://zc.panjiajie.cn

?string $name = null
来源：http://ow.szxytkj.cn

[U47] PHP：联合类型
来源：http://im.asd995.cn

int|string $id
来源：http://ye.szsharing.cn

[U48] PHP：纯枚举
来源：http://ls.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://me.shxzukj.cn

[U49] PHP：只读属性
来源：http://ec.wgjwhj.cn

public readonly string $name
来源：http://ak.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://lh.colortex.cn

public function __construct(private int $id) {}
来源：http://rx.nicolike.cn

[U51] PHP：数组解构
来源：http://ew.gzmigu.cn

[$a, $b] = $arr;
来源：http://od.colortex.cn

[U52] PHP：箭头函数
来源：http://ng.asd995.cn

$double = fn($x) => $x * 2;
来源：http://lf.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://xq.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://nv.shxzskj.cn

[U54] PHP：空安全调用
来源：http://fo.shxzukj.cn

$obj?->method()
来源：http://lo.hahajie.cn

[U55] PHP：match 表达式
来源：http://xp.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jx.huixiangedu.cn

[U56] PHP：命名参数
来源：http://xz.jctech888.com.cn

f(a: 1, b: 2)
来源：http://fu.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://zg.panjiajie.cn

"值: {$a}"
来源：http://da.521024.cn

[U58] PHP：数组三件套
来源：http://kk.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eu.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://xy.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sd.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://jk.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mh.nszjky.cn

[U61] PHP：正则
来源：http://je.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zj.jctech888.com.cn

[U62] PHP：日期对象
来源：http://vw.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jd.wgjwhj.cn

[U63] PHP：文件读写
来源：http://fi.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zm.gzmigu.cn

[U64] PHP：目录遍历
来源：http://fj.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ig.muxihuayi.cn

[U65] PHP：会话
来源：http://ur.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ar.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://em.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oo.9csxet.cn

[U67] PHP：处理文件上传
来源：http://qb.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rt.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://ke.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://li.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://tq.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://li.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://js.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://na.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://pm.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://aa.huanxung.cn

[U72] PHP：写错误日志
来源：http://di.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://te.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://yl.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://vz.szsharing.cn

[U74] PHP：读取环境变量
来源：http://cj.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://oq.521024.cn

[U75] PHP：依赖注入
来源：http://tg.huanxung.cn

composer require psr/container
来源：http://pl.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://an.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ho.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://zy.shtwfgs.cn

composer require twig/twig
来源：http://nv.chemitech.net.cn

[U78] PHP：单元测试
来源：http://mv.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://jt.haigaiapp.cn


<!-- 参考信息 -->