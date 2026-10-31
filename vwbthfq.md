代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lx.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://st.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kf.asd995.cn

[S56] C++：optional
来源：http://ul.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ao.yuexingan06.cn

[S57] C++：编译期常量
来源：http://jy.yuntaijiaju.cn

constexpr int N = 10;
来源：http://gj.shtwfgs.cn

[S58] C++：命名空间
来源：http://zp.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://ih.newstarts.cn

[S59] C++：静态断言
来源：http://lf.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aw.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://bh.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://im.yuntaijiaju.cn

================================================================================
来源：http://ly.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vh.9csxet.cn

================================================================================
来源：http://yy.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://ui.huixiangedu.cn

println("Hello")
来源：http://yv.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://hl.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zf.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://qj.haigaiapp.cn

"值: $b"
来源：http://ns.panjiajie.cn

[T04] Kotlin：空安全
来源：http://lp.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://zx.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://lq.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jj.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://se.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://is.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://cb.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uh.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://qv.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://zp.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://kl.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://no.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://su.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bl.haigaiapp.cn

[T11] Kotlin：协程
来源：http://bj.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qi.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ua.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://ml.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://cw.colortex.cn

val m = mapOf("a" to 1)
来源：http://nf.szxytkj.cn

[T14] Kotlin：循环
来源：http://tl.nicolike.cn

for (i in 1..10) println(i)
来源：http://dg.szsharing.cn

[T15] Kotlin：接口
来源：http://mc.nicolike.cn

interface Shape { fun area(): Double }
来源：http://ch.huixiangedu.cn

[T16] Swift：Hello World
来源：http://vp.chemitech.net.cn

print("Hello")
来源：http://mn.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://as.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ul.colortex.cn

[T18] Swift：字符串插值
来源：http://ub.jianghongdianzi.cn

"值: \(b)"
来源：http://td.panjiajie.cn

[T19] Swift：可选绑定
来源：http://xy.hnjuh.cn

if let n = opt { print(n) }
来源：http://td.nszjky.cn

[T20] Swift：数组操作
来源：http://eh.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://en.bjjhwx.cn

[T21] Swift：遍历
来源：http://vq.lnxyls.cn

for x in a { print(x) }
来源：http://tj.gzmigu.cn

[T22] Swift：字典
来源：http://ov.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fh.bookmarksfly.cn

[T23] Swift：函数
来源：http://vk.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ov.bjjhwx.cn

[T24] Swift：闭包
来源：http://ar.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ah.hnjuh.cn

[T25] Swift：结构体
来源：http://mv.wgjwhj.cn

struct P { var x: Int }
来源：http://eb.panjiajie.cn

[T26] Swift：类与重写
来源：http://dp.panjiajie.cn

class A: Base { override func f() {} }
来源：http://py.jctech888.com.cn

[T27] Swift：错误处理
来源：http://ow.hahajie.cn

do { try f() } catch { print(error) }
来源：http://tb.bookmarksfly.cn

[T28] Swift：枚举
来源：http://bc.shxzukj.cn

enum Color { case red, green }
来源：http://ke.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://px.huixiangedu.cn

guard let x = opt else { return }
来源：http://pp.huixiangedu.cn

[T30] Swift：协议
来源：http://iz.colortex.cn

protocol Shape { func area() -> Double }
来源：http://ki.hahajie.cn

[T31] Lua：Hello World
来源：http://yp.haigaiapp.cn

print("Hello")
来源：http://np.huanxung.cn

[T32] Lua：局部变量
来源：http://ou.szxytkj.cn

local a = 1
来源：http://bk.colortex.cn

[T33] Lua：表（数组）
来源：http://ca.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wy.bjjhwx.cn

[T34] Lua：遍历表
来源：http://le.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ln.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://vp.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://bv.szsharing.cn

[T36] Lua：函数
来源：http://wa.nszjky.cn

function add(a, b) return a + b end
来源：http://tg.colortex.cn

[T37] Lua：字符串拼接
来源：http://pc.shtwfgs.cn

"a" .. "b"
来源：http://hn.muxihuayi.cn

[T38] Lua：条件
来源：http://uf.nicolike.cn

if x > 0 then print("正") end
来源：http://ej.nszjky.cn

[T39] Lua：模式匹配
来源：http://wp.nszjky.cn

string.find(s, "%d+")
来源：http://hw.colortex.cn

[T40] Lua：元表
来源：http://td.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://ey.asd995.cn

[T41] Perl：Hello World
来源：http://kp.9csxet.cn

print "Hello\n";
来源：http://zd.nszjky.cn

[T42] Perl：变量类型
来源：http://xh.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tu.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://cw.jianghongdianzi.cn

"值: $a"
来源：http://dg.9csxet.cn

[T44] Perl：条件
来源：http://lw.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://gv.hahajie.cn

[T45] Perl：数组遍历
来源：http://uh.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://ey.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://hu.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xv.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ry.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yv.chemitech.net.cn

[T48] Perl：正则替换
来源：http://ck.lnxyls.cn

$s =~ s/old/new/g;
来源：http://yq.nicolike.cn

[T49] Perl：函数
来源：http://qu.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mh.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://wl.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lz.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://dx.nszjky.cn

[T51] Scala：Hello World
来源：http://qg.asd995.cn

println("Hello")
来源：http://pt.panjiajie.cn

[T52] Scala：变量
来源：http://os.shxzskj.cn

val a = 1;  var b = 2
来源：http://ov.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://lf.yuntaijiaju.cn

s"值: $b"
来源：http://tb.haigaiapp.cn

[T54] Scala：集合映射
来源：http://kk.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://el.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://xz.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xc.szxytkj.cn

[T56] Scala：样例类
来源：http://gw.nszjky.cn

case class User(name: String, age: Int)
来源：http://ir.gzmigu.cn

[T57] Scala：模式匹配
来源：http://ax.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sb.shxzukj.cn

[T58] Scala：函数定义
来源：http://yq.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zl.hahajie.cn

[T59] Scala：循环
来源：http://la.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://ox.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://zc.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://da.jianghongdianzi.cn

================================================================================
来源：http://rj.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wj.hahajie.cn

================================================================================
来源：http://sw.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://vo.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hf.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://kx.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gf.asd995.cn

[U03] Py：加载 .env 配置
来源：http://ud.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cy.asd995.cn

[U04] Py：变量调试打印
来源：http://ia.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dy.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://pi.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://bm.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ld.huixinmuqiang.cn

{**a, **b}
来源：http://ok.panjiajie.cn

[U07] Py：反转字典键值
来源：http://pn.newstarts.cn

{v: k for k, v in d.items()}
来源：http://ea.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://eu.haigaiapp.cn

[y for x in nested for y in x]
来源：http://up.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://is.yuexingan06.cn

max(d, key=d.get)
来源：http://rv.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://gv.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sv.nicolike.cn

[U11] Py：生成器表达式
来源：http://dl.colortex.cn

(x * 2 for x in arr)
来源：http://yo.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xz.huanxung.cn

Counter(arr).most_common(3)
来源：http://jd.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://oz.yuntaijiaju.cn

deque(maxlen=10)
来源：http://yo.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://sh.hahajie.cn

defaultdict(list)
来源：http://is.9csxet.cn

[U15] Py：高精度计时
来源：http://nw.jianghongdianzi.cn

t = time.perf_counter()
来源：http://us.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://ra.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lm.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://nh.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://lu.lnxyls.cn

[U18] Py：预编译正则
来源：http://tt.asd995.cn

pat = re.compile(r"\d+")
来源：http://nt.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://iz.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xz.nszjky.cn

[U20] Py：缓存函数结果
来源：http://zt.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://jy.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://xc.muxihuayi.cn

@contextlib.contextmanager
来源：http://jq.hnjuh.cn

[U22] Py：矩阵转置
来源：http://wm.bjjhwx.cn

list(zip(*m))
来源：http://wn.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://tp.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qr.9csxet.cn

[U24] Py：路径操作
来源：http://zq.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zb.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://ax.bjjhwx.cn

csv.DictReader(f)
来源：http://xw.hahajie.cn

[U26] Py：并发下载
来源：http://ju.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zz.9csxet.cn

[U27] Py：异步 HTTP
来源：http://oo.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://bz.jctech888.com.cn

[U28] Py：类型别名
来源：http://oy.9csxet.cn

UserId = int
来源：http://df.nicolike.cn

[U29] Py：属性校验
来源：http://he.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://lp.hahajie.cn

[U30] Py：数据类
来源：http://tl.hnjuh.cn

@dataclass(slots=True)
来源：http://zn.colortex.cn

[U31] Py：单测
来源：http://yc.jianghongdianzi.cn

python -m pytest -q
来源：http://fu.wgjwhj.cn

[U32] Py：代码格式化
来源：http://xx.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://zl.huixiangedu.cn

[U33] Py：打包发布
来源：http://vc.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ic.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://kg.haigaiapp.cn

chardet.detect(raw)
来源：http://cc.hahajie.cn

[U35] Py：发送邮件
来源：http://ky.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gw.yuexingan06.cn

[U36] Py：定时任务
来源：http://rd.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://gc.gzmigu.cn

[U37] Py：读写 Excel
来源：http://fw.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xg.521024.cn

[U38] Py：获取脚本所在目录
来源：http://df.panjiajie.cn

Path(__file__).resolve().parent
来源：http://pm.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://ed.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://oo.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://gy.nszjky.cn

print("err", file=sys.stderr)
来源：http://cr.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://ua.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gb.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://xp.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zu.nszjky.cn

[U43] PHP：声明命名空间
来源：http://os.asd995.cn

namespace App\Http;
来源：http://qy.9csxet.cn

[U44] PHP：开启严格类型
来源：http://np.asd995.cn

declare(strict_types=1);
来源：http://qg.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://mq.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oo.szsharing.cn

[U46] PHP：可空类型
来源：http://ae.jianghongdianzi.cn

?string $name = null
来源：http://zq.jctech888.com.cn

[U47] PHP：联合类型
来源：http://yr.asd995.cn

int|string $id
来源：http://mu.9csxet.cn

[U48] PHP：纯枚举
来源：http://zg.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://am.hnjuh.cn

[U49] PHP：只读属性
来源：http://bc.hahajie.cn

public readonly string $name
来源：http://yw.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://xu.szsharing.cn

public function __construct(private int $id) {}
来源：http://kd.asd995.cn

[U51] PHP：数组解构
来源：http://ul.bjjhwx.cn

[$a, $b] = $arr;
来源：http://at.shxzukj.cn

[U52] PHP：箭头函数
来源：http://ms.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://hz.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://ln.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://xi.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://pj.szxytkj.cn

$obj?->method()
来源：http://pg.nszjky.cn

[U55] PHP：match 表达式
来源：http://nl.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hv.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://ee.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://av.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://uy.jctech888.com.cn

"值: {$a}"
来源：http://vm.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://cd.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kp.shxzskj.cn

[U59] PHP：自定义排序
来源：http://sd.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fv.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://ao.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://by.gzmigu.cn

[U61] PHP：正则
来源：http://kb.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ba.muxihuayi.cn

[U62] PHP：日期对象
来源：http://ih.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bs.chemitech.net.cn

[U63] PHP：文件读写
来源：http://wd.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uh.szsharing.cn

[U64] PHP：目录遍历
来源：http://hc.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://dq.lnxyls.cn

[U65] PHP：会话
来源：http://uc.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ph.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://ew.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zm.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://bo.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tx.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://wo.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zz.521024.cn

[U69] PHP：PDO 预处理
来源：http://ga.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ua.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://nq.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ny.hahajie.cn

[U71] PHP：抛出异常
来源：http://zy.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://dy.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://ly.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://wf.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://xq.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://bk.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://wj.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://os.panjiajie.cn

[U75] PHP：依赖注入
来源：http://sm.asd995.cn

composer require psr/container
来源：http://jt.asd995.cn

[U76] PHP：简单路由
来源：http://gv.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ly.gzmigu.cn

[U77] PHP：模板渲染
来源：http://ed.asd995.cn

composer require twig/twig
来源：http://yo.nszjky.cn

[U78] PHP：单元测试
来源：http://eg.colortex.cn

composer require --dev phpunit/phpunit
来源：http://sm.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://hi.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://bl.colortex.cn

[U80] PHP：代码规范修复
来源：http://av.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nr.asd995.cn


<!-- 参考信息 -->