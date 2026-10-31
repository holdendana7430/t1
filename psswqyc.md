代发 wailian999

int size() const noexcept { return n_; }
来源：http://bk.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://fq.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://lf.yuexingan06.cn

[S54] C++：异常处理
来源：http://rt.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dh.szsharing.cn

[S55] C++：结构化绑定
来源：http://qm.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pd.bjjhwx.cn

[S56] C++：optional
来源：http://og.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dp.szsharing.cn

[S57] C++：编译期常量
来源：http://tp.lnxyls.cn

constexpr int N = 10;
来源：http://uh.hnjuh.cn

[S58] C++：命名空间
来源：http://gu.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://dq.chemitech.net.cn

[S59] C++：静态断言
来源：http://lr.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cv.colortex.cn

[S60] C++：遍历并删除元素
来源：http://at.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pg.szsharing.cn

================================================================================
来源：http://ts.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jt.asd995.cn

================================================================================
来源：http://jv.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://gz.yuntaijiaju.cn

println("Hello")
来源：http://mm.colortex.cn

[T02] Kotlin：变量
来源：http://km.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vn.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://pa.yuntaijiaju.cn

"值: $b"
来源：http://oy.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://dy.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ho.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://yw.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ia.huanxung.cn

[T06] Kotlin：集合映射
来源：http://ci.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://do.521024.cn

[T07] Kotlin：集合过滤
来源：http://gn.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://or.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://pq.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://oi.asd995.cn

[T09] Kotlin：扩展函数
来源：http://fp.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://pu.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://dl.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fe.shxzukj.cn

[T11] Kotlin：协程
来源：http://vo.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ay.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://ab.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://is.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://ib.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://jq.wgjwhj.cn

[T14] Kotlin：循环
来源：http://cf.szsharing.cn

for (i in 1..10) println(i)
来源：http://ak.nszjky.cn

[T15] Kotlin：接口
来源：http://qt.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://ho.jctech888.com.cn

[T16] Swift：Hello World
来源：http://iz.jianghongdianzi.cn

print("Hello")
来源：http://du.nszjky.cn

[T17] Swift：变量与常量
来源：http://nm.szxytkj.cn

var a = 1;  let b = 2
来源：http://pz.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://oa.bookmarksfly.cn

"值: \(b)"
来源：http://tv.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://wv.huixiangedu.cn

if let n = opt { print(n) }
来源：http://ha.hnjuh.cn

[T20] Swift：数组操作
来源：http://gm.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bm.chemitech.net.cn

[T21] Swift：遍历
来源：http://jd.yuexingan06.cn

for x in a { print(x) }
来源：http://as.hahajie.cn

[T22] Swift：字典
来源：http://rz.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lb.lnxyls.cn

[T23] Swift：函数
来源：http://dh.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jq.szxytkj.cn

[T24] Swift：闭包
来源：http://xx.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tc.huixiangedu.cn

[T25] Swift：结构体
来源：http://sk.hahajie.cn

struct P { var x: Int }
来源：http://on.panjiajie.cn

[T26] Swift：类与重写
来源：http://df.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://hd.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://ox.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://ez.jctech888.com.cn

[T28] Swift：枚举
来源：http://xx.shxzskj.cn

enum Color { case red, green }
来源：http://fw.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://mx.newstarts.cn

guard let x = opt else { return }
来源：http://yk.huixiangedu.cn

[T30] Swift：协议
来源：http://ic.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://fa.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://vn.haigaiapp.cn

print("Hello")
来源：http://us.szxytkj.cn

[T32] Lua：局部变量
来源：http://id.nicolike.cn

local a = 1
来源：http://kw.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://tv.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fe.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ms.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yz.jctech888.com.cn

[T35] Lua：字典表
来源：http://ci.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://hj.hnjuh.cn

[T36] Lua：函数
来源：http://sa.nszjky.cn

function add(a, b) return a + b end
来源：http://zd.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://pz.asd995.cn

"a" .. "b"
来源：http://rc.gzmigu.cn

[T38] Lua：条件
来源：http://kx.shxzukj.cn

if x > 0 then print("正") end
来源：http://cm.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://my.huixiangedu.cn

string.find(s, "%d+")
来源：http://cw.shxzskj.cn

[T40] Lua：元表
来源：http://vk.nszjky.cn

setmetatable({}, { __index = base })
来源：http://iq.chemitech.net.cn

[T41] Perl：Hello World
来源：http://oi.shxzskj.cn

print "Hello\n";
来源：http://pg.huanxung.cn

[T42] Perl：变量类型
来源：http://xp.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vg.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://gf.muxihuayi.cn

"值: $a"
来源：http://bs.haigaiapp.cn

[T44] Perl：条件
来源：http://zf.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://wa.colortex.cn

[T45] Perl：数组遍历
来源：http://uo.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://gq.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://kx.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://of.9csxet.cn

[T47] Perl：正则捕获
来源：http://on.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lj.jctech888.com.cn

[T48] Perl：正则替换
来源：http://jn.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://mm.bjjhwx.cn

[T49] Perl：函数
来源：http://fe.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pa.asd995.cn

[T50] Perl：逐行读文件
来源：http://nx.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nn.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://lw.jctech888.com.cn

[T51] Scala：Hello World
来源：http://uz.bookmarksfly.cn

println("Hello")
来源：http://fo.huanxung.cn

[T52] Scala：变量
来源：http://qi.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ce.gzmigu.cn

[T53] Scala：字符串插值
来源：http://jf.9csxet.cn

s"值: $b"
来源：http://dv.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://yv.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://lz.huanxung.cn

[T55] Scala：集合过滤
来源：http://sa.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ej.hahajie.cn

[T56] Scala：样例类
来源：http://wm.panjiajie.cn

case class User(name: String, age: Int)
来源：http://hf.szxytkj.cn

[T57] Scala：模式匹配
来源：http://zt.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ta.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://qw.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ja.shxzskj.cn

[T59] Scala：循环
来源：http://df.521024.cn

for (i <- 1 to 10) println(i)
来源：http://iv.huixiangedu.cn

[T60] Scala：折叠
来源：http://ds.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pg.nszjky.cn

================================================================================
来源：http://sm.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xm.hnjuh.cn

================================================================================
来源：http://ey.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://bo.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wc.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://qr.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ww.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://ml.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://to.hnjuh.cn

[U04] Py：变量调试打印
来源：http://gg.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nh.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://za.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://ex.hahajie.cn

[U06] Py：合并两个字典
来源：http://nu.jianghongdianzi.cn

{**a, **b}
来源：http://en.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://tt.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://no.shxzskj.cn

[U08] Py：展平二维列表
来源：http://fp.haigaiapp.cn

[y for x in nested for y in x]
来源：http://fu.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://va.huixinmuqiang.cn

max(d, key=d.get)
来源：http://op.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://rs.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kp.colortex.cn

[U11] Py：生成器表达式
来源：http://dg.nicolike.cn

(x * 2 for x in arr)
来源：http://re.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ud.gzmigu.cn

Counter(arr).most_common(3)
来源：http://fj.szxytkj.cn

[U13] Py：固定长度队列
来源：http://li.huixinmuqiang.cn

deque(maxlen=10)
来源：http://cu.colortex.cn

[U14] Py：分组收集到列表
来源：http://oq.lnxyls.cn

defaultdict(list)
来源：http://er.haigaiapp.cn

[U15] Py：高精度计时
来源：http://yf.chemitech.net.cn

t = time.perf_counter()
来源：http://vg.szsharing.cn

[U16] Py：命令行参数解析
来源：http://ie.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tn.wgjwhj.cn

[U17] Py：初始化日志
来源：http://dv.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nu.jctech888.com.cn

[U18] Py：预编译正则
来源：http://kj.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://sv.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://ma.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sq.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://cj.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://eu.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://qp.521024.cn

@contextlib.contextmanager
来源：http://hw.9csxet.cn

[U22] Py：矩阵转置
来源：http://ud.lnxyls.cn

list(zip(*m))
来源：http://na.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://vk.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nu.jctech888.com.cn

[U24] Py：路径操作
来源：http://sk.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://le.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://im.hahajie.cn

csv.DictReader(f)
来源：http://te.huanxung.cn

[U26] Py：并发下载
来源：http://nb.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wc.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://pa.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://az.asd995.cn

[U28] Py：类型别名
来源：http://ik.huixinmuqiang.cn

UserId = int
来源：http://oj.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://vv.panjiajie.cn

@property 与 @x.setter 配合
来源：http://pp.nicolike.cn

[U30] Py：数据类
来源：http://qy.chemitech.net.cn

@dataclass(slots=True)
来源：http://hy.nszjky.cn

[U31] Py：单测
来源：http://rg.newstarts.cn

python -m pytest -q
来源：http://sx.hahajie.cn

[U32] Py：代码格式化
来源：http://jo.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://jp.jctech888.com.cn

[U33] Py：打包发布
来源：http://ae.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://lf.nicolike.cn

[U34] Py：判断编码
来源：http://jk.yuexingan06.cn

chardet.detect(raw)
来源：http://sa.nicolike.cn

[U35] Py：发送邮件
来源：http://ae.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hh.newstarts.cn

[U36] Py：定时任务
来源：http://tv.521024.cn

schedule.every(10).minutes.do(job)
来源：http://ng.szxytkj.cn

[U37] Py：读写 Excel
来源：http://xf.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://da.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://al.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ig.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://nj.shxzskj.cn

sys.stdout.isatty()
来源：http://og.nszjky.cn

[U40] Py：打印到标准错误
来源：http://jd.huanxung.cn

print("err", file=sys.stderr)
来源：http://hi.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://dg.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bz.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://mm.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gy.hahajie.cn

[U43] PHP：声明命名空间
来源：http://tp.huixinmuqiang.cn

namespace App\Http;
来源：http://th.521024.cn

[U44] PHP：开启严格类型
来源：http://yn.newstarts.cn

declare(strict_types=1);
来源：http://nk.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://nq.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ex.yuexingan06.cn

[U46] PHP：可空类型
来源：http://jw.nicolike.cn

?string $name = null
来源：http://sn.shxzskj.cn

[U47] PHP：联合类型
来源：http://ce.huanxung.cn

int|string $id
来源：http://jv.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://fz.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uy.521024.cn

[U49] PHP：只读属性
来源：http://ny.lnxyls.cn

public readonly string $name
来源：http://cq.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://tp.lnxyls.cn

public function __construct(private int $id) {}
来源：http://fv.9csxet.cn

[U51] PHP：数组解构
来源：http://vq.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://pw.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://ja.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://am.9csxet.cn

[U53] PHP：空合并运算符
来源：http://la.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://fu.lnxyls.cn

[U54] PHP：空安全调用
来源：http://ab.newstarts.cn

$obj?->method()
来源：http://mu.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://dy.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kc.hnjuh.cn

[U56] PHP：命名参数
来源：http://zy.nszjky.cn

f(a: 1, b: 2)
来源：http://xn.panjiajie.cn

[U57] PHP：字符串插值
来源：http://wj.shtwfgs.cn

"值: {$a}"
来源：http://ed.szsharing.cn

[U58] PHP：数组三件套
来源：http://dp.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vc.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://mw.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ft.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://xl.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qm.shxzukj.cn

[U61] PHP：正则
来源：http://rd.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://po.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://aw.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://or.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://lr.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iq.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://zn.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://sw.bjjhwx.cn

[U65] PHP：会话
来源：http://tc.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qu.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://oe.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ux.newstarts.cn

[U67] PHP：处理文件上传
来源：http://zn.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pt.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ko.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nx.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://hy.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ma.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://wl.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wo.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://kc.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://yu.asd995.cn

[U72] PHP：写错误日志
来源：http://ch.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://wd.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://vw.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://li.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://nb.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://cm.hahajie.cn

[U75] PHP：依赖注入
来源：http://fb.521024.cn

composer require psr/container
来源：http://kv.nicolike.cn

[U76] PHP：简单路由
来源：http://oq.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vq.colortex.cn

[U77] PHP：模板渲染
来源：http://ek.newstarts.cn

composer require twig/twig
来源：http://tf.panjiajie.cn

[U78] PHP：单元测试
来源：http://rz.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://sk.bjjhwx.cn


<!-- 参考信息 -->