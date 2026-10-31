代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://if.yuexingan06.cn

[S57] C++：编译期常量
来源：http://qy.nszjky.cn

constexpr int N = 10;
来源：http://wn.521024.cn

[S58] C++：命名空间
来源：http://gt.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://dh.jctech888.com.cn

[S59] C++：静态断言
来源：http://ed.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tb.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://yo.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uy.hahajie.cn

================================================================================
来源：http://zz.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://on.wgjwhj.cn

================================================================================
来源：http://mr.szsharing.cn

[T01] Kotlin：Hello World
来源：http://pg.jctech888.com.cn

println("Hello")
来源：http://ba.asd995.cn

[T02] Kotlin：变量
来源：http://iq.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ut.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://gs.jianghongdianzi.cn

"值: $b"
来源：http://zi.gzmigu.cn

[T04] Kotlin：空安全
来源：http://rc.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://lk.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://rq.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ap.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://ag.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kk.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://bz.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bu.521024.cn

[T08] Kotlin：数据类
来源：http://nt.colortex.cn

data class User(val name: String, val age: Int)
来源：http://oq.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://qj.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://hg.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://bb.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://te.9csxet.cn

[T11] Kotlin：协程
来源：http://ms.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wt.asd995.cn

[T12] Kotlin：解构声明
来源：http://xc.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://yh.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://of.nszjky.cn

val m = mapOf("a" to 1)
来源：http://xo.wgjwhj.cn

[T14] Kotlin：循环
来源：http://oz.gzmigu.cn

for (i in 1..10) println(i)
来源：http://rn.huixiangedu.cn

[T15] Kotlin：接口
来源：http://bz.hahajie.cn

interface Shape { fun area(): Double }
来源：http://eb.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ne.newstarts.cn

print("Hello")
来源：http://ac.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://xt.huanxung.cn

var a = 1;  let b = 2
来源：http://jd.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://sf.asd995.cn

"值: \(b)"
来源：http://dw.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://yk.hahajie.cn

if let n = opt { print(n) }
来源：http://ih.gzmigu.cn

[T20] Swift：数组操作
来源：http://qb.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pb.szxytkj.cn

[T21] Swift：遍历
来源：http://gi.haigaiapp.cn

for x in a { print(x) }
来源：http://wq.lnxyls.cn

[T22] Swift：字典
来源：http://rr.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ab.huixinmuqiang.cn

[T23] Swift：函数
来源：http://of.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bc.hahajie.cn

[T24] Swift：闭包
来源：http://lv.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://st.szxytkj.cn

[T25] Swift：结构体
来源：http://ib.jctech888.com.cn

struct P { var x: Int }
来源：http://bj.bjjhwx.cn

[T26] Swift：类与重写
来源：http://jm.hnjuh.cn

class A: Base { override func f() {} }
来源：http://xx.gzmigu.cn

[T27] Swift：错误处理
来源：http://ym.nszjky.cn

do { try f() } catch { print(error) }
来源：http://lh.yuexingan06.cn

[T28] Swift：枚举
来源：http://mn.shxzukj.cn

enum Color { case red, green }
来源：http://uo.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://in.shxzukj.cn

guard let x = opt else { return }
来源：http://vm.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ys.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://ie.shxzskj.cn

[T31] Lua：Hello World
来源：http://ii.szsharing.cn

print("Hello")
来源：http://ba.9csxet.cn

[T32] Lua：局部变量
来源：http://xk.bjjhwx.cn

local a = 1
来源：http://lp.521024.cn

[T33] Lua：表（数组）
来源：http://tl.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ua.colortex.cn

[T34] Lua：遍历表
来源：http://me.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ac.colortex.cn

[T35] Lua：字典表
来源：http://ga.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://lj.chemitech.net.cn

[T36] Lua：函数
来源：http://dm.chemitech.net.cn

function add(a, b) return a + b end
来源：http://xa.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://wa.newstarts.cn

"a" .. "b"
来源：http://ur.muxihuayi.cn

[T38] Lua：条件
来源：http://df.muxihuayi.cn

if x > 0 then print("正") end
来源：http://yj.nicolike.cn

[T39] Lua：模式匹配
来源：http://kk.chemitech.net.cn

string.find(s, "%d+")
来源：http://ej.jctech888.com.cn

[T40] Lua：元表
来源：http://zk.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://pb.521024.cn

[T41] Perl：Hello World
来源：http://yy.chemitech.net.cn

print "Hello\n";
来源：http://mm.bjjhwx.cn

[T42] Perl：变量类型
来源：http://km.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eu.hahajie.cn

[T43] Perl：字符串插值
来源：http://qr.chemitech.net.cn

"值: $a"
来源：http://fc.szsharing.cn

[T44] Perl：条件
来源：http://zp.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://lw.asd995.cn

[T45] Perl：数组遍历
来源：http://dw.colortex.cn

for my $x (@arr) { print $x; }
来源：http://sy.nicolike.cn

[T46] Perl：哈希操作
来源：http://lj.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://la.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://el.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qn.bjjhwx.cn

[T48] Perl：正则替换
来源：http://kx.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://np.panjiajie.cn

[T49] Perl：函数
来源：http://ds.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xm.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://dl.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jn.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://wi.wgjwhj.cn

[T51] Scala：Hello World
来源：http://my.panjiajie.cn

println("Hello")
来源：http://pr.huanxung.cn

[T52] Scala：变量
来源：http://wb.gzmigu.cn

val a = 1;  var b = 2
来源：http://vm.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://mi.521024.cn

s"值: $b"
来源：http://vo.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://ba.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://qi.huanxung.cn

[T55] Scala：集合过滤
来源：http://or.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gz.chemitech.net.cn

[T56] Scala：样例类
来源：http://xu.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://up.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://tg.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ik.hnjuh.cn

[T58] Scala：函数定义
来源：http://vy.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wt.shxzskj.cn

[T59] Scala：循环
来源：http://md.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://xh.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://lu.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sb.huixinmuqiang.cn

================================================================================
来源：http://lt.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rb.jianghongdianzi.cn

================================================================================
来源：http://qb.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://pg.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mk.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://jv.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jf.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://rh.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hp.panjiajie.cn

[U04] Py：变量调试打印
来源：http://vq.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://le.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://rr.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://eh.shxzskj.cn

[U06] Py：合并两个字典
来源：http://wm.colortex.cn

{**a, **b}
来源：http://kh.521024.cn

[U07] Py：反转字典键值
来源：http://do.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://wf.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ux.hahajie.cn

[y for x in nested for y in x]
来源：http://xr.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://er.shxzukj.cn

max(d, key=d.get)
来源：http://xu.szxytkj.cn

[U10] Py：按值排序字典
来源：http://gg.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://az.lnxyls.cn

[U11] Py：生成器表达式
来源：http://fp.wgjwhj.cn

(x * 2 for x in arr)
来源：http://gk.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ri.szxytkj.cn

Counter(arr).most_common(3)
来源：http://uz.shxzskj.cn

[U13] Py：固定长度队列
来源：http://to.colortex.cn

deque(maxlen=10)
来源：http://eq.huanxung.cn

[U14] Py：分组收集到列表
来源：http://sw.nicolike.cn

defaultdict(list)
来源：http://ve.panjiajie.cn

[U15] Py：高精度计时
来源：http://bb.szsharing.cn

t = time.perf_counter()
来源：http://gz.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://rz.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zc.muxihuayi.cn

[U17] Py：初始化日志
来源：http://jo.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://jw.wgjwhj.cn

[U18] Py：预编译正则
来源：http://ne.nszjky.cn

pat = re.compile(r"\d+")
来源：http://ew.asd995.cn

[U19] Py：正则替换带回调
来源：http://ro.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fq.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://bc.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://rm.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://fd.hahajie.cn

@contextlib.contextmanager
来源：http://ho.asd995.cn

[U22] Py：矩阵转置
来源：http://el.huanxung.cn

list(zip(*m))
来源：http://au.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://kp.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jf.muxihuayi.cn

[U24] Py：路径操作
来源：http://ue.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://as.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://fw.hahajie.cn

csv.DictReader(f)
来源：http://ui.hahajie.cn

[U26] Py：并发下载
来源：http://kk.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://an.9csxet.cn

[U27] Py：异步 HTTP
来源：http://qg.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://xt.lnxyls.cn

[U28] Py：类型别名
来源：http://qk.jctech888.com.cn

UserId = int
来源：http://tx.chemitech.net.cn

[U29] Py：属性校验
来源：http://nt.shxzskj.cn

@property 与 @x.setter 配合
来源：http://lc.shxzukj.cn

[U30] Py：数据类
来源：http://hy.hahajie.cn

@dataclass(slots=True)
来源：http://jq.521024.cn

[U31] Py：单测
来源：http://vm.huixiangedu.cn

python -m pytest -q
来源：http://il.huanxung.cn

[U32] Py：代码格式化
来源：http://jo.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://dn.szxytkj.cn

[U33] Py：打包发布
来源：http://il.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://dv.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://vp.gzmigu.cn

chardet.detect(raw)
来源：http://qd.9csxet.cn

[U35] Py：发送邮件
来源：http://cd.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yl.hnjuh.cn

[U36] Py：定时任务
来源：http://tx.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://me.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://ci.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dp.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://in.shxzskj.cn

Path(__file__).resolve().parent
来源：http://uu.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://im.huanxung.cn

sys.stdout.isatty()
来源：http://hx.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://dx.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://gt.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://wn.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yf.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://nf.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wi.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://dz.asd995.cn

namespace App\Http;
来源：http://vb.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://lm.shxzukj.cn

declare(strict_types=1);
来源：http://ey.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://uv.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.jctech888.com.cn

[U46] PHP：可空类型
来源：http://vd.bookmarksfly.cn

?string $name = null
来源：http://wv.newstarts.cn

[U47] PHP：联合类型
来源：http://yt.yuntaijiaju.cn

int|string $id
来源：http://nv.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://iy.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hl.gzmigu.cn

[U49] PHP：只读属性
来源：http://os.huixinmuqiang.cn

public readonly string $name
来源：http://bx.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://ed.asd995.cn

public function __construct(private int $id) {}
来源：http://nt.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://cq.szxytkj.cn

[$a, $b] = $arr;
来源：http://up.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ca.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://hk.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://bi.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://ee.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://ul.szsharing.cn

$obj?->method()
来源：http://cu.panjiajie.cn

[U55] PHP：match 表达式
来源：http://mr.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gf.haigaiapp.cn

[U56] PHP：命名参数
来源：http://xn.jctech888.com.cn

f(a: 1, b: 2)
来源：http://pv.asd995.cn

[U57] PHP：字符串插值
来源：http://gm.9csxet.cn

"值: {$a}"
来源：http://ra.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://aj.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ou.hnjuh.cn

[U59] PHP：自定义排序
来源：http://ft.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oe.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://ne.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sv.hahajie.cn

[U61] PHP：正则
来源：http://wa.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xg.huanxung.cn

[U62] PHP：日期对象
来源：http://ib.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mu.szxytkj.cn

[U63] PHP：文件读写
来源：http://fs.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tm.9csxet.cn

[U64] PHP：目录遍历
来源：http://ub.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://yc.yuexingan06.cn

[U65] PHP：会话
来源：http://aa.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qo.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://to.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jq.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://bt.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kq.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://zl.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cw.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://zi.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uu.newstarts.cn

[U70] PHP：PDO 事务
来源：http://ll.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jh.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://dj.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://ko.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://ec.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://eu.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://fy.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://qh.nszjky.cn

[U74] PHP：读取环境变量
来源：http://uk.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://be.szxytkj.cn

[U75] PHP：依赖注入
来源：http://cy.muxihuayi.cn

composer require psr/container
来源：http://ze.lnxyls.cn

[U76] PHP：简单路由
来源：http://pp.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kp.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://nr.nszjky.cn

composer require twig/twig
来源：http://tz.colortex.cn

[U78] PHP：单元测试
来源：http://pj.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://fi.nicolike.cn

[U79] PHP：静态分析
来源：http://to.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://ew.newstarts.cn

[U80] PHP：代码规范修复
来源：http://zv.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fq.yuexingan06.cn

[U81] JS：初始化项目
来源：http://cw.panjiajie.cn

npm init -y;  npm i express
来源：http://fd.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://hk.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gb.panjiajie.cn


<!-- 参考信息 -->