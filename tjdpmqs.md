代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hv.hahajie.cn

[S59] C++：静态断言
来源：http://vi.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xe.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://sl.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nx.lnxyls.cn

================================================================================
来源：http://nd.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nu.hahajie.cn

================================================================================
来源：http://di.szsharing.cn

[T01] Kotlin：Hello World
来源：http://jr.yuexingan06.cn

println("Hello")
来源：http://en.wgjwhj.cn

[T02] Kotlin：变量
来源：http://pt.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eh.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://gt.bjjhwx.cn

"值: $b"
来源：http://ds.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://ic.gzmigu.cn

val n: String? = null;  n?.length
来源：http://cc.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://gv.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sr.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://ft.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bu.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://pi.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jt.lnxyls.cn

[T08] Kotlin：数据类
来源：http://su.colortex.cn

data class User(val name: String, val age: Int)
来源：http://un.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://zg.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://av.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://gh.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ke.hnjuh.cn

[T11] Kotlin：协程
来源：http://sg.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fm.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://xl.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://tr.colortex.cn

[T13] Kotlin：只读 Map
来源：http://vq.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://th.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://pb.nszjky.cn

for (i in 1..10) println(i)
来源：http://zj.huixiangedu.cn

[T15] Kotlin：接口
来源：http://sm.asd995.cn

interface Shape { fun area(): Double }
来源：http://mz.muxihuayi.cn

[T16] Swift：Hello World
来源：http://xb.nszjky.cn

print("Hello")
来源：http://kj.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://st.panjiajie.cn

var a = 1;  let b = 2
来源：http://wd.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://dh.szxytkj.cn

"值: \(b)"
来源：http://di.521024.cn

[T19] Swift：可选绑定
来源：http://xl.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://dr.shxzukj.cn

[T20] Swift：数组操作
来源：http://hi.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ka.hnjuh.cn

[T21] Swift：遍历
来源：http://gf.yuexingan06.cn

for x in a { print(x) }
来源：http://tf.521024.cn

[T22] Swift：字典
来源：http://ut.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ck.wgjwhj.cn

[T23] Swift：函数
来源：http://mv.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://th.muxihuayi.cn

[T24] Swift：闭包
来源：http://wi.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aj.nszjky.cn

[T25] Swift：结构体
来源：http://ck.gzmigu.cn

struct P { var x: Int }
来源：http://az.muxihuayi.cn

[T26] Swift：类与重写
来源：http://ag.521024.cn

class A: Base { override func f() {} }
来源：http://fj.shtwfgs.cn

[T27] Swift：错误处理
来源：http://or.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://qn.nicolike.cn

[T28] Swift：枚举
来源：http://ww.chemitech.net.cn

enum Color { case red, green }
来源：http://bt.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://gx.lnxyls.cn

guard let x = opt else { return }
来源：http://xu.lnxyls.cn

[T30] Swift：协议
来源：http://eo.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ej.hahajie.cn

[T31] Lua：Hello World
来源：http://qt.huixiangedu.cn

print("Hello")
来源：http://au.bjjhwx.cn

[T32] Lua：局部变量
来源：http://ov.shxzskj.cn

local a = 1
来源：http://iq.shxzskj.cn

[T33] Lua：表（数组）
来源：http://hn.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tb.huanxung.cn

[T34] Lua：遍历表
来源：http://wy.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dy.bjjhwx.cn

[T35] Lua：字典表
来源：http://sn.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://xm.haigaiapp.cn

[T36] Lua：函数
来源：http://vq.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://sy.nicolike.cn

[T37] Lua：字符串拼接
来源：http://zf.hnjuh.cn

"a" .. "b"
来源：http://nm.yuexingan06.cn

[T38] Lua：条件
来源：http://zk.szxytkj.cn

if x > 0 then print("正") end
来源：http://zf.huanxung.cn

[T39] Lua：模式匹配
来源：http://ei.9csxet.cn

string.find(s, "%d+")
来源：http://nq.wgjwhj.cn

[T40] Lua：元表
来源：http://rk.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://un.shxzukj.cn

[T41] Perl：Hello World
来源：http://fw.nszjky.cn

print "Hello\n";
来源：http://ee.chemitech.net.cn

[T42] Perl：变量类型
来源：http://pb.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cs.shxzukj.cn

[T43] Perl：字符串插值
来源：http://gu.jctech888.com.cn

"值: $a"
来源：http://ud.nszjky.cn

[T44] Perl：条件
来源：http://dz.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://vg.nszjky.cn

[T45] Perl：数组遍历
来源：http://et.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://fh.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://kw.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ux.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://mx.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://af.shxzskj.cn

[T48] Perl：正则替换
来源：http://ve.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://vw.gzmigu.cn

[T49] Perl：函数
来源：http://oe.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yo.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://kp.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kq.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://di.muxihuayi.cn

[T51] Scala：Hello World
来源：http://kl.chemitech.net.cn

println("Hello")
来源：http://zr.yuexingan06.cn

[T52] Scala：变量
来源：http://hy.shxzukj.cn

val a = 1;  var b = 2
来源：http://lc.szsharing.cn

[T53] Scala：字符串插值
来源：http://wf.haigaiapp.cn

s"值: $b"
来源：http://vh.521024.cn

[T54] Scala：集合映射
来源：http://gs.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://eg.szsharing.cn

[T55] Scala：集合过滤
来源：http://qy.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bm.521024.cn

[T56] Scala：样例类
来源：http://gr.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://pl.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://hp.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yx.hahajie.cn

[T58] Scala：函数定义
来源：http://rg.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tk.szxytkj.cn

[T59] Scala：循环
来源：http://hg.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://bd.shtwfgs.cn

[T60] Scala：折叠
来源：http://uw.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kw.asd995.cn

================================================================================
来源：http://jo.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xs.hnjuh.cn

================================================================================
来源：http://ai.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://ea.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qw.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://rr.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ee.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://wp.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xa.gzmigu.cn

[U04] Py：变量调试打印
来源：http://hg.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ak.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://rq.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://vn.9csxet.cn

[U06] Py：合并两个字典
来源：http://wo.shxzskj.cn

{**a, **b}
来源：http://lb.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://kz.nicolike.cn

{v: k for k, v in d.items()}
来源：http://ob.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://nc.muxihuayi.cn

[y for x in nested for y in x]
来源：http://kt.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://av.jianghongdianzi.cn

max(d, key=d.get)
来源：http://xw.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://oc.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hr.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://sj.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://er.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dt.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://lj.521024.cn

[U13] Py：固定长度队列
来源：http://mf.nicolike.cn

deque(maxlen=10)
来源：http://wv.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://ur.huanxung.cn

defaultdict(list)
来源：http://eu.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://bj.shtwfgs.cn

t = time.perf_counter()
来源：http://ju.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://nf.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yq.9csxet.cn

[U17] Py：初始化日志
来源：http://xy.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://wl.haigaiapp.cn

[U18] Py：预编译正则
来源：http://wh.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://nr.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://xr.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xd.colortex.cn

[U20] Py：缓存函数结果
来源：http://nt.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://gu.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://yq.asd995.cn

@contextlib.contextmanager
来源：http://sb.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://rq.nicolike.cn

list(zip(*m))
来源：http://tn.colortex.cn

[U23] Py：分块读取大文件
来源：http://wt.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sr.haigaiapp.cn

[U24] Py：路径操作
来源：http://qh.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hb.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://wc.haigaiapp.cn

csv.DictReader(f)
来源：http://si.panjiajie.cn

[U26] Py：并发下载
来源：http://pr.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zv.asd995.cn

[U27] Py：异步 HTTP
来源：http://bp.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://qo.9csxet.cn

[U28] Py：类型别名
来源：http://jh.hnjuh.cn

UserId = int
来源：http://ev.gzmigu.cn

[U29] Py：属性校验
来源：http://va.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://lp.hahajie.cn

[U30] Py：数据类
来源：http://tw.shtwfgs.cn

@dataclass(slots=True)
来源：http://vp.shtwfgs.cn

[U31] Py：单测
来源：http://gp.9csxet.cn

python -m pytest -q
来源：http://ls.nszjky.cn

[U32] Py：代码格式化
来源：http://uu.newstarts.cn

ruff format . && ruff check --fix .
来源：http://uw.nicolike.cn

[U33] Py：打包发布
来源：http://nv.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://zg.bjjhwx.cn

[U34] Py：判断编码
来源：http://pn.wgjwhj.cn

chardet.detect(raw)
来源：http://oa.wgjwhj.cn

[U35] Py：发送邮件
来源：http://tw.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vn.szxytkj.cn

[U36] Py：定时任务
来源：http://mm.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://ia.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://be.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rx.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://qp.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ba.521024.cn

[U39] Py：判断是否在交互环境
来源：http://bo.wgjwhj.cn

sys.stdout.isatty()
来源：http://pb.nszjky.cn

[U40] Py：打印到标准错误
来源：http://kb.hnjuh.cn

print("err", file=sys.stderr)
来源：http://im.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://fa.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sf.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://so.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hm.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://kd.bjjhwx.cn

namespace App\Http;
来源：http://fk.huanxung.cn

[U44] PHP：开启严格类型
来源：http://fi.panjiajie.cn

declare(strict_types=1);
来源：http://mg.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://iw.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mx.huanxung.cn

[U46] PHP：可空类型
来源：http://ix.gzmigu.cn

?string $name = null
来源：http://il.bjjhwx.cn

[U47] PHP：联合类型
来源：http://vp.shxzskj.cn

int|string $id
来源：http://zq.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://qy.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dr.haigaiapp.cn

[U49] PHP：只读属性
来源：http://ck.asd995.cn

public readonly string $name
来源：http://ve.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://qu.szsharing.cn

public function __construct(private int $id) {}
来源：http://lz.hahajie.cn

[U51] PHP：数组解构
来源：http://sn.colortex.cn

[$a, $b] = $arr;
来源：http://kp.hahajie.cn

[U52] PHP：箭头函数
来源：http://kr.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://pc.hahajie.cn

[U53] PHP：空合并运算符
来源：http://ya.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://ui.asd995.cn

[U54] PHP：空安全调用
来源：http://xh.gzmigu.cn

$obj?->method()
来源：http://wo.asd995.cn

[U55] PHP：match 表达式
来源：http://gb.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dh.colortex.cn

[U56] PHP：命名参数
来源：http://au.panjiajie.cn

f(a: 1, b: 2)
来源：http://aq.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://jq.panjiajie.cn

"值: {$a}"
来源：http://dc.shxzukj.cn

[U58] PHP：数组三件套
来源：http://oo.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://du.nicolike.cn

[U59] PHP：自定义排序
来源：http://gc.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ku.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://bv.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gb.muxihuayi.cn

[U61] PHP：正则
来源：http://ih.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gf.huanxung.cn

[U62] PHP：日期对象
来源：http://ur.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tf.gzmigu.cn

[U63] PHP：文件读写
来源：http://nk.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ev.nicolike.cn

[U64] PHP：目录遍历
来源：http://qs.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://kh.colortex.cn

[U65] PHP：会话
来源：http://qj.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kg.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://lc.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pv.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://ei.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ox.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://tl.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kg.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://io.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yj.asd995.cn

[U70] PHP：PDO 事务
来源：http://rd.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dv.gzmigu.cn

[U71] PHP：抛出异常
来源：http://xz.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://iz.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://os.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://ar.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://rf.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://nc.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://du.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://cu.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://be.yuntaijiaju.cn

composer require psr/container
来源：http://ba.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://ay.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://og.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://js.521024.cn

composer require twig/twig
来源：http://hy.asd995.cn

[U78] PHP：单元测试
来源：http://my.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://ox.nszjky.cn

[U79] PHP：静态分析
来源：http://aw.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://iz.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://el.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vc.yuexingan06.cn

[U81] JS：初始化项目
来源：http://bi.asd995.cn

npm init -y;  npm i express
来源：http://pd.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://fw.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lc.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://ca.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ax.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://vm.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gv.szsharing.cn


<!-- 参考信息 -->