代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://vc.shxzukj.cn

[S59] C++：静态断言
来源：http://ba.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://br.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://io.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pq.szxytkj.cn

================================================================================
来源：http://qo.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fk.9csxet.cn

================================================================================
来源：http://ap.huanxung.cn

[T01] Kotlin：Hello World
来源：http://ys.panjiajie.cn

println("Hello")
来源：http://oe.nszjky.cn

[T02] Kotlin：变量
来源：http://cv.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cg.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://xx.wgjwhj.cn

"值: $b"
来源：http://pk.huanxung.cn

[T04] Kotlin：空安全
来源：http://xe.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://up.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://dz.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bx.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://js.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cw.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://hk.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xa.colortex.cn

[T08] Kotlin：数据类
来源：http://rk.asd995.cn

data class User(val name: String, val age: Int)
来源：http://fj.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://id.asd995.cn

fun String.exclaim() = this + "!"
来源：http://mq.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://sd.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gm.nicolike.cn

[T11] Kotlin：协程
来源：http://hv.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qt.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://rz.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://xz.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://gz.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://pp.nicolike.cn

[T14] Kotlin：循环
来源：http://kk.nszjky.cn

for (i in 1..10) println(i)
来源：http://ts.shxzukj.cn

[T15] Kotlin：接口
来源：http://zp.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://pa.521024.cn

[T16] Swift：Hello World
来源：http://rs.szsharing.cn

print("Hello")
来源：http://zc.521024.cn

[T17] Swift：变量与常量
来源：http://cc.hahajie.cn

var a = 1;  let b = 2
来源：http://ep.newstarts.cn

[T18] Swift：字符串插值
来源：http://lo.lnxyls.cn

"值: \(b)"
来源：http://hn.9csxet.cn

[T19] Swift：可选绑定
来源：http://wc.shxzukj.cn

if let n = opt { print(n) }
来源：http://jl.panjiajie.cn

[T20] Swift：数组操作
来源：http://ri.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sj.nszjky.cn

[T21] Swift：遍历
来源：http://xw.yuntaijiaju.cn

for x in a { print(x) }
来源：http://nw.nicolike.cn

[T22] Swift：字典
来源：http://rq.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mt.hahajie.cn

[T23] Swift：函数
来源：http://eq.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://va.szxytkj.cn

[T24] Swift：闭包
来源：http://va.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qp.panjiajie.cn

[T25] Swift：结构体
来源：http://cm.hnjuh.cn

struct P { var x: Int }
来源：http://qe.panjiajie.cn

[T26] Swift：类与重写
来源：http://nk.colortex.cn

class A: Base { override func f() {} }
来源：http://fg.huanxung.cn

[T27] Swift：错误处理
来源：http://su.nicolike.cn

do { try f() } catch { print(error) }
来源：http://fg.gzmigu.cn

[T28] Swift：枚举
来源：http://yo.shxzukj.cn

enum Color { case red, green }
来源：http://im.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://yx.asd995.cn

guard let x = opt else { return }
来源：http://hh.shxzukj.cn

[T30] Swift：协议
来源：http://yc.asd995.cn

protocol Shape { func area() -> Double }
来源：http://pa.asd995.cn

[T31] Lua：Hello World
来源：http://tp.wgjwhj.cn

print("Hello")
来源：http://kn.chemitech.net.cn

[T32] Lua：局部变量
来源：http://sm.huixiangedu.cn

local a = 1
来源：http://vv.gzmigu.cn

[T33] Lua：表（数组）
来源：http://xq.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xa.huanxung.cn

[T34] Lua：遍历表
来源：http://nr.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xs.lnxyls.cn

[T35] Lua：字典表
来源：http://xv.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://im.asd995.cn

[T36] Lua：函数
来源：http://ca.bjjhwx.cn

function add(a, b) return a + b end
来源：http://ho.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://im.huanxung.cn

"a" .. "b"
来源：http://my.panjiajie.cn

[T38] Lua：条件
来源：http://wj.chemitech.net.cn

if x > 0 then print("正") end
来源：http://nm.hnjuh.cn

[T39] Lua：模式匹配
来源：http://fu.wgjwhj.cn

string.find(s, "%d+")
来源：http://ut.colortex.cn

[T40] Lua：元表
来源：http://ha.521024.cn

setmetatable({}, { __index = base })
来源：http://xb.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://kc.nszjky.cn

print "Hello\n";
来源：http://lq.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://zt.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sr.szxytkj.cn

[T43] Perl：字符串插值
来源：http://qd.haigaiapp.cn

"值: $a"
来源：http://pt.szxytkj.cn

[T44] Perl：条件
来源：http://fs.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://ac.9csxet.cn

[T45] Perl：数组遍历
来源：http://ct.asd995.cn

for my $x (@arr) { print $x; }
来源：http://dg.9csxet.cn

[T46] Perl：哈希操作
来源：http://tx.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mq.asd995.cn

[T47] Perl：正则捕获
来源：http://yh.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://we.yuexingan06.cn

[T48] Perl：正则替换
来源：http://bw.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://qh.huixinmuqiang.cn

[T49] Perl：函数
来源：http://le.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hi.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://tl.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ud.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://jl.gzmigu.cn

[T51] Scala：Hello World
来源：http://jc.szsharing.cn

println("Hello")
来源：http://ia.shxzukj.cn

[T52] Scala：变量
来源：http://va.asd995.cn

val a = 1;  var b = 2
来源：http://xd.newstarts.cn

[T53] Scala：字符串插值
来源：http://zi.hnjuh.cn

s"值: $b"
来源：http://qj.jctech888.com.cn

[T54] Scala：集合映射
来源：http://bp.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://to.9csxet.cn

[T55] Scala：集合过滤
来源：http://mh.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kz.bjjhwx.cn

[T56] Scala：样例类
来源：http://mg.nszjky.cn

case class User(name: String, age: Int)
来源：http://gr.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://df.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kq.chemitech.net.cn

[T58] Scala：函数定义
来源：http://lg.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zb.wgjwhj.cn

[T59] Scala：循环
来源：http://sb.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://wo.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ot.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zh.huixinmuqiang.cn

================================================================================
来源：http://lb.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xu.9csxet.cn

================================================================================
来源：http://sl.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://dj.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hw.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://ch.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bw.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://sb.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fj.gzmigu.cn

[U04] Py：变量调试打印
来源：http://hm.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ah.huanxung.cn

[U05] Py：列表去重且保序
来源：http://zk.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://oc.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://li.hahajie.cn

{**a, **b}
来源：http://ch.gzmigu.cn

[U07] Py：反转字典键值
来源：http://eb.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://gf.szxytkj.cn

[U08] Py：展平二维列表
来源：http://jb.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://yp.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://vd.lnxyls.cn

max(d, key=d.get)
来源：http://dz.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://os.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zi.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://uf.hnjuh.cn

(x * 2 for x in arr)
来源：http://jl.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://px.nszjky.cn

Counter(arr).most_common(3)
来源：http://nw.nicolike.cn

[U13] Py：固定长度队列
来源：http://tl.lnxyls.cn

deque(maxlen=10)
来源：http://nd.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://ax.wgjwhj.cn

defaultdict(list)
来源：http://oe.szxytkj.cn

[U15] Py：高精度计时
来源：http://fz.gzmigu.cn

t = time.perf_counter()
来源：http://vz.colortex.cn

[U16] Py：命令行参数解析
来源：http://nx.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mw.nicolike.cn

[U17] Py：初始化日志
来源：http://tj.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://ml.panjiajie.cn

[U18] Py：预编译正则
来源：http://sw.asd995.cn

pat = re.compile(r"\d+")
来源：http://yt.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://ug.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gf.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://qp.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://ja.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://pz.lnxyls.cn

@contextlib.contextmanager
来源：http://nn.colortex.cn

[U22] Py：矩阵转置
来源：http://am.huixiangedu.cn

list(zip(*m))
来源：http://vf.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://hs.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qu.asd995.cn

[U24] Py：路径操作
来源：http://cw.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fp.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://is.newstarts.cn

csv.DictReader(f)
来源：http://xq.wgjwhj.cn

[U26] Py：并发下载
来源：http://sd.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fk.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ly.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://rb.newstarts.cn

[U28] Py：类型别名
来源：http://mq.gzmigu.cn

UserId = int
来源：http://yi.wgjwhj.cn

[U29] Py：属性校验
来源：http://ww.521024.cn

@property 与 @x.setter 配合
来源：http://nh.huanxung.cn

[U30] Py：数据类
来源：http://lu.shtwfgs.cn

@dataclass(slots=True)
来源：http://us.521024.cn

[U31] Py：单测
来源：http://ll.yuexingan06.cn

python -m pytest -q
来源：http://ll.521024.cn

[U32] Py：代码格式化
来源：http://wo.huanxung.cn

ruff format . && ruff check --fix .
来源：http://fq.521024.cn

[U33] Py：打包发布
来源：http://oc.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://yo.bookmarksfly.cn

[U34] Py：判断编码
来源：http://jz.szsharing.cn

chardet.detect(raw)
来源：http://vm.huixiangedu.cn

[U35] Py：发送邮件
来源：http://ix.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xr.hnjuh.cn

[U36] Py：定时任务
来源：http://yl.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://wq.9csxet.cn

[U37] Py：读写 Excel
来源：http://eg.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vr.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://cu.nicolike.cn

Path(__file__).resolve().parent
来源：http://ci.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://rz.panjiajie.cn

sys.stdout.isatty()
来源：http://fa.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://an.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://bv.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://gq.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gz.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://hx.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mn.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://zn.huanxung.cn

namespace App\Http;
来源：http://go.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://je.bjjhwx.cn

declare(strict_types=1);
来源：http://ow.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://ww.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.521024.cn

[U46] PHP：可空类型
来源：http://to.nszjky.cn

?string $name = null
来源：http://oy.chemitech.net.cn

[U47] PHP：联合类型
来源：http://lu.bookmarksfly.cn

int|string $id
来源：http://ju.gzmigu.cn

[U48] PHP：纯枚举
来源：http://el.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jd.panjiajie.cn

[U49] PHP：只读属性
来源：http://tj.panjiajie.cn

public readonly string $name
来源：http://so.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://ym.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://ss.nicolike.cn

[U51] PHP：数组解构
来源：http://vk.newstarts.cn

[$a, $b] = $arr;
来源：http://rh.panjiajie.cn

[U52] PHP：箭头函数
来源：http://an.colortex.cn

$double = fn($x) => $x * 2;
来源：http://xz.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://cl.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://zu.lnxyls.cn

[U54] PHP：空安全调用
来源：http://ws.shxzskj.cn

$obj?->method()
来源：http://li.huanxung.cn

[U55] PHP：match 表达式
来源：http://hm.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ol.shxzskj.cn

[U56] PHP：命名参数
来源：http://cb.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://qx.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://kp.szxytkj.cn

"值: {$a}"
来源：http://lt.nszjky.cn

[U58] PHP：数组三件套
来源：http://sm.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ye.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ah.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wh.521024.cn

[U60] PHP：JSON 编解码
来源：http://sj.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gt.hnjuh.cn

[U61] PHP：正则
来源：http://wc.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pg.newstarts.cn

[U62] PHP：日期对象
来源：http://jd.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://od.panjiajie.cn

[U63] PHP：文件读写
来源：http://ff.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ku.gzmigu.cn

[U64] PHP：目录遍历
来源：http://fb.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://vb.haigaiapp.cn

[U65] PHP：会话
来源：http://yj.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://np.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://qz.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fs.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://zz.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nf.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://td.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://og.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://pq.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xc.nszjky.cn

[U70] PHP：PDO 事务
来源：http://pi.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ro.lnxyls.cn

[U71] PHP：抛出异常
来源：http://bz.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://op.shxzskj.cn

[U72] PHP：写错误日志
来源：http://ga.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://gi.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://ns.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://ei.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://qm.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://uj.asd995.cn

[U75] PHP：依赖注入
来源：http://hr.yuexingan06.cn

composer require psr/container
来源：http://rv.nicolike.cn

[U76] PHP：简单路由
来源：http://qb.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gx.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://ag.9csxet.cn

composer require twig/twig
来源：http://gg.9csxet.cn

[U78] PHP：单元测试
来源：http://sa.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://ye.shxzskj.cn

[U79] PHP：静态分析
来源：http://jj.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://qs.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://zt.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lg.shtwfgs.cn

[U81] JS：初始化项目
来源：http://ck.shxzskj.cn

npm init -y;  npm i express
来源：http://bt.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://ar.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tp.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://iz.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vk.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://du.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://el.chemitech.net.cn


<!-- 参考信息 -->