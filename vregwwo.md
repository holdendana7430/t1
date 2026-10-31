代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kg.shxzukj.cn

[S55] C++：结构化绑定
来源：http://ko.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wy.jianghongdianzi.cn

[S56] C++：optional
来源：http://ve.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lf.jctech888.com.cn

[S57] C++：编译期常量
来源：http://sw.chemitech.net.cn

constexpr int N = 10;
来源：http://dy.newstarts.cn

[S58] C++：命名空间
来源：http://zm.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://yq.bjjhwx.cn

[S59] C++：静态断言
来源：http://dn.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tw.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://rs.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hc.newstarts.cn

================================================================================
来源：http://dh.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zv.nicolike.cn

================================================================================
来源：http://sh.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://xk.hahajie.cn

println("Hello")
来源：http://xe.newstarts.cn

[T02] Kotlin：变量
来源：http://fa.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ip.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://rd.9csxet.cn

"值: $b"
来源：http://tt.521024.cn

[T04] Kotlin：空安全
来源：http://br.hahajie.cn

val n: String? = null;  n?.length
来源：http://my.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://jy.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dx.colortex.cn

[T06] Kotlin：集合映射
来源：http://wo.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bd.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://kw.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mq.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ud.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://hz.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://lz.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://sn.newstarts.cn

[T10] Kotlin：默认参数
来源：http://vm.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ge.bjjhwx.cn

[T11] Kotlin：协程
来源：http://ix.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cx.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://dx.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://sk.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://ty.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://pq.9csxet.cn

[T14] Kotlin：循环
来源：http://df.asd995.cn

for (i in 1..10) println(i)
来源：http://sc.panjiajie.cn

[T15] Kotlin：接口
来源：http://fc.nicolike.cn

interface Shape { fun area(): Double }
来源：http://th.gzmigu.cn

[T16] Swift：Hello World
来源：http://dg.haigaiapp.cn

print("Hello")
来源：http://nw.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ln.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://np.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://cs.lnxyls.cn

"值: \(b)"
来源：http://jx.shxzukj.cn

[T19] Swift：可选绑定
来源：http://xp.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://xa.shxzukj.cn

[T20] Swift：数组操作
来源：http://ju.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iv.huixiangedu.cn

[T21] Swift：遍历
来源：http://xi.shtwfgs.cn

for x in a { print(x) }
来源：http://po.muxihuayi.cn

[T22] Swift：字典
来源：http://qw.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kl.colortex.cn

[T23] Swift：函数
来源：http://td.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nn.colortex.cn

[T24] Swift：闭包
来源：http://pt.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rw.nszjky.cn

[T25] Swift：结构体
来源：http://rt.nicolike.cn

struct P { var x: Int }
来源：http://gy.nicolike.cn

[T26] Swift：类与重写
来源：http://dc.nszjky.cn

class A: Base { override func f() {} }
来源：http://ke.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://gy.hahajie.cn

do { try f() } catch { print(error) }
来源：http://wi.hahajie.cn

[T28] Swift：枚举
来源：http://pa.chemitech.net.cn

enum Color { case red, green }
来源：http://vp.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://rp.haigaiapp.cn

guard let x = opt else { return }
来源：http://as.huixiangedu.cn

[T30] Swift：协议
来源：http://fx.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://bn.newstarts.cn

[T31] Lua：Hello World
来源：http://ra.nszjky.cn

print("Hello")
来源：http://zp.hnjuh.cn

[T32] Lua：局部变量
来源：http://su.bookmarksfly.cn

local a = 1
来源：http://qp.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://mx.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jr.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://xu.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ml.shxzskj.cn

[T35] Lua：字典表
来源：http://hl.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://kt.jianghongdianzi.cn

[T36] Lua：函数
来源：http://ky.newstarts.cn

function add(a, b) return a + b end
来源：http://hm.asd995.cn

[T37] Lua：字符串拼接
来源：http://vc.shtwfgs.cn

"a" .. "b"
来源：http://dy.hahajie.cn

[T38] Lua：条件
来源：http://vf.nicolike.cn

if x > 0 then print("正") end
来源：http://sk.9csxet.cn

[T39] Lua：模式匹配
来源：http://rh.hahajie.cn

string.find(s, "%d+")
来源：http://dm.jctech888.com.cn

[T40] Lua：元表
来源：http://ys.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://ly.bjjhwx.cn

[T41] Perl：Hello World
来源：http://lv.jianghongdianzi.cn

print "Hello\n";
来源：http://zn.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://rr.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nu.asd995.cn

[T43] Perl：字符串插值
来源：http://sb.nszjky.cn

"值: $a"
来源：http://iq.bjjhwx.cn

[T44] Perl：条件
来源：http://qj.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://lw.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://zb.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://gt.nicolike.cn

[T46] Perl：哈希操作
来源：http://ln.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qm.gzmigu.cn

[T47] Perl：正则捕获
来源：http://ah.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dv.nicolike.cn

[T48] Perl：正则替换
来源：http://jc.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://pd.lnxyls.cn

[T49] Perl：函数
来源：http://ox.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gt.huanxung.cn

[T50] Perl：逐行读文件
来源：http://id.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://du.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://fi.colortex.cn

[T51] Scala：Hello World
来源：http://xt.521024.cn

println("Hello")
来源：http://uu.bjjhwx.cn

[T52] Scala：变量
来源：http://he.szsharing.cn

val a = 1;  var b = 2
来源：http://gj.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://be.szsharing.cn

s"值: $b"
来源：http://ic.9csxet.cn

[T54] Scala：集合映射
来源：http://mw.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://lj.newstarts.cn

[T55] Scala：集合过滤
来源：http://js.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tj.colortex.cn

[T56] Scala：样例类
来源：http://kv.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://vq.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://on.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pb.yuexingan06.cn

[T58] Scala：函数定义
来源：http://zx.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sg.yuntaijiaju.cn

[T59] Scala：循环
来源：http://iz.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://da.hnjuh.cn

[T60] Scala：折叠
来源：http://yr.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pk.szsharing.cn

================================================================================
来源：http://dc.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://se.bjjhwx.cn

================================================================================
来源：http://ys.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://cq.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fr.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://go.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://st.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://ph.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lv.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://ih.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://st.colortex.cn

[U05] Py：列表去重且保序
来源：http://de.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://te.nicolike.cn

[U06] Py：合并两个字典
来源：http://pz.jctech888.com.cn

{**a, **b}
来源：http://td.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://xh.colortex.cn

{v: k for k, v in d.items()}
来源：http://nn.szxytkj.cn

[U08] Py：展平二维列表
来源：http://vw.haigaiapp.cn

[y for x in nested for y in x]
来源：http://wy.521024.cn

[U09] Py：字典取最大值的键
来源：http://us.shxzskj.cn

max(d, key=d.get)
来源：http://bh.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://he.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fl.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://sm.chemitech.net.cn

(x * 2 for x in arr)
来源：http://kw.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ab.hahajie.cn

Counter(arr).most_common(3)
来源：http://po.nszjky.cn

[U13] Py：固定长度队列
来源：http://vw.huixiangedu.cn

deque(maxlen=10)
来源：http://fu.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://is.hnjuh.cn

defaultdict(list)
来源：http://td.newstarts.cn

[U15] Py：高精度计时
来源：http://lx.jctech888.com.cn

t = time.perf_counter()
来源：http://lf.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://ow.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ai.asd995.cn

[U17] Py：初始化日志
来源：http://vb.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://of.chemitech.net.cn

[U18] Py：预编译正则
来源：http://hk.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://mn.nicolike.cn

[U19] Py：正则替换带回调
来源：http://ka.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ul.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://rg.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://ps.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://dm.yuexingan06.cn

@contextlib.contextmanager
来源：http://ch.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://zq.9csxet.cn

list(zip(*m))
来源：http://wo.9csxet.cn

[U23] Py：分块读取大文件
来源：http://lu.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ro.muxihuayi.cn

[U24] Py：路径操作
来源：http://ar.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jb.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://hd.hnjuh.cn

csv.DictReader(f)
来源：http://yq.bookmarksfly.cn

[U26] Py：并发下载
来源：http://am.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xh.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ru.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://ze.9csxet.cn

[U28] Py：类型别名
来源：http://ws.hnjuh.cn

UserId = int
来源：http://xn.521024.cn

[U29] Py：属性校验
来源：http://iy.gzmigu.cn

@property 与 @x.setter 配合
来源：http://dw.wgjwhj.cn

[U30] Py：数据类
来源：http://fw.shxzukj.cn

@dataclass(slots=True)
来源：http://mv.gzmigu.cn

[U31] Py：单测
来源：http://mn.chemitech.net.cn

python -m pytest -q
来源：http://bh.szxytkj.cn

[U32] Py：代码格式化
来源：http://wu.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://jm.gzmigu.cn

[U33] Py：打包发布
来源：http://oi.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://bo.bjjhwx.cn

[U34] Py：判断编码
来源：http://ew.wgjwhj.cn

chardet.detect(raw)
来源：http://cm.wgjwhj.cn

[U35] Py：发送邮件
来源：http://qo.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gzmigu.cn

[U36] Py：定时任务
来源：http://yx.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ks.huanxung.cn

[U37] Py：读写 Excel
来源：http://zj.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lh.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://hi.shxzukj.cn

Path(__file__).resolve().parent
来源：http://pc.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://nl.shtwfgs.cn

sys.stdout.isatty()
来源：http://uj.521024.cn

[U40] Py：打印到标准错误
来源：http://ke.panjiajie.cn

print("err", file=sys.stderr)
来源：http://pb.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://tn.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://an.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://qo.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vt.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://xx.9csxet.cn

namespace App\Http;
来源：http://os.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://uj.hahajie.cn

declare(strict_types=1);
来源：http://ae.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://zr.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tf.wgjwhj.cn

[U46] PHP：可空类型
来源：http://qu.yuexingan06.cn

?string $name = null
来源：http://rf.gzmigu.cn

[U47] PHP：联合类型
来源：http://qb.hahajie.cn

int|string $id
来源：http://ew.asd995.cn

[U48] PHP：纯枚举
来源：http://fu.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lt.hnjuh.cn

[U49] PHP：只读属性
来源：http://vo.muxihuayi.cn

public readonly string $name
来源：http://zv.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://hu.newstarts.cn

public function __construct(private int $id) {}
来源：http://ty.wgjwhj.cn

[U51] PHP：数组解构
来源：http://om.9csxet.cn

[$a, $b] = $arr;
来源：http://hl.gzmigu.cn

[U52] PHP：箭头函数
来源：http://cb.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://oq.hahajie.cn

[U53] PHP：空合并运算符
来源：http://ui.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ys.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://ol.bjjhwx.cn

$obj?->method()
来源：http://rf.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://pz.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lm.haigaiapp.cn

[U56] PHP：命名参数
来源：http://lz.hnjuh.cn

f(a: 1, b: 2)
来源：http://xn.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://xc.bjjhwx.cn

"值: {$a}"
来源：http://sx.colortex.cn

[U58] PHP：数组三件套
来源：http://bv.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fs.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://pe.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qm.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://qr.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://na.asd995.cn

[U61] PHP：正则
来源：http://nh.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ul.szsharing.cn

[U62] PHP：日期对象
来源：http://jz.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hs.nszjky.cn

[U63] PHP：文件读写
来源：http://ji.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ek.asd995.cn

[U64] PHP：目录遍历
来源：http://xx.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://af.haigaiapp.cn

[U65] PHP：会话
来源：http://gf.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bh.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://cd.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wg.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://dp.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ji.szsharing.cn

[U68] PHP：PDO 连接
来源：http://hj.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zo.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://rg.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gx.asd995.cn

[U70] PHP：PDO 事务
来源：http://xk.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kr.hnjuh.cn

[U71] PHP：抛出异常
来源：http://wc.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://so.szxytkj.cn

[U72] PHP：写错误日志
来源：http://kj.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://ak.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://yz.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://pd.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://oh.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://kk.shxzukj.cn

[U75] PHP：依赖注入
来源：http://gp.shxzukj.cn

composer require psr/container
来源：http://fd.panjiajie.cn

[U76] PHP：简单路由
来源：http://jj.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cr.shxzskj.cn

[U77] PHP：模板渲染
来源：http://of.jianghongdianzi.cn

composer require twig/twig
来源：http://bb.chemitech.net.cn

[U78] PHP：单元测试
来源：http://yj.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://ab.szsharing.cn

[U79] PHP：静态分析
来源：http://vv.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://al.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://bh.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dl.hnjuh.cn


<!-- 参考信息 -->