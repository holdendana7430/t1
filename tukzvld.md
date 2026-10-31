代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://os.huanxung.cn

================================================================================
来源：http://zk.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ss.hnjuh.cn

================================================================================
来源：http://fn.huanxung.cn

[T01] Kotlin：Hello World
来源：http://ke.panjiajie.cn

println("Hello")
来源：http://da.huanxung.cn

[T02] Kotlin：变量
来源：http://gn.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eh.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://ro.bookmarksfly.cn

"值: $b"
来源：http://lu.panjiajie.cn

[T04] Kotlin：空安全
来源：http://rs.shxzskj.cn

val n: String? = null;  n?.length
来源：http://km.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://nh.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fx.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://dd.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jy.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://yr.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tq.hahajie.cn

[T08] Kotlin：数据类
来源：http://ip.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://mw.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://fm.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://cy.asd995.cn

[T10] Kotlin：默认参数
来源：http://vv.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://un.haigaiapp.cn

[T11] Kotlin：协程
来源：http://ti.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fy.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://xc.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://hc.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://go.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://il.huixiangedu.cn

[T14] Kotlin：循环
来源：http://zh.lnxyls.cn

for (i in 1..10) println(i)
来源：http://bs.shxzukj.cn

[T15] Kotlin：接口
来源：http://vn.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://yn.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://rc.chemitech.net.cn

print("Hello")
来源：http://wk.hahajie.cn

[T17] Swift：变量与常量
来源：http://ld.shtwfgs.cn

var a = 1;  let b = 2
来源：http://is.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://mv.shxzskj.cn

"值: \(b)"
来源：http://te.szxytkj.cn

[T19] Swift：可选绑定
来源：http://jp.szxytkj.cn

if let n = opt { print(n) }
来源：http://ho.muxihuayi.cn

[T20] Swift：数组操作
来源：http://bk.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iq.szxytkj.cn

[T21] Swift：遍历
来源：http://cb.bookmarksfly.cn

for x in a { print(x) }
来源：http://ky.colortex.cn

[T22] Swift：字典
来源：http://rz.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jd.szsharing.cn

[T23] Swift：函数
来源：http://lf.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://og.bjjhwx.cn

[T24] Swift：闭包
来源：http://no.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xc.gzmigu.cn

[T25] Swift：结构体
来源：http://pz.colortex.cn

struct P { var x: Int }
来源：http://xb.521024.cn

[T26] Swift：类与重写
来源：http://ly.nszjky.cn

class A: Base { override func f() {} }
来源：http://rb.9csxet.cn

[T27] Swift：错误处理
来源：http://dm.asd995.cn

do { try f() } catch { print(error) }
来源：http://xp.huanxung.cn

[T28] Swift：枚举
来源：http://ak.shxzukj.cn

enum Color { case red, green }
来源：http://xi.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://lc.hahajie.cn

guard let x = opt else { return }
来源：http://le.colortex.cn

[T30] Swift：协议
来源：http://gu.asd995.cn

protocol Shape { func area() -> Double }
来源：http://il.jctech888.com.cn

[T31] Lua：Hello World
来源：http://zz.jctech888.com.cn

print("Hello")
来源：http://xr.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://qi.newstarts.cn

local a = 1
来源：http://qt.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://dd.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vc.9csxet.cn

[T34] Lua：遍历表
来源：http://tp.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ot.wgjwhj.cn

[T35] Lua：字典表
来源：http://ge.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://yx.asd995.cn

[T36] Lua：函数
来源：http://hi.hnjuh.cn

function add(a, b) return a + b end
来源：http://cz.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://my.lnxyls.cn

"a" .. "b"
来源：http://vb.lnxyls.cn

[T38] Lua：条件
来源：http://mm.nszjky.cn

if x > 0 then print("正") end
来源：http://pt.hahajie.cn

[T39] Lua：模式匹配
来源：http://rt.521024.cn

string.find(s, "%d+")
来源：http://ec.szsharing.cn

[T40] Lua：元表
来源：http://jf.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://fq.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://em.yuntaijiaju.cn

print "Hello\n";
来源：http://jg.newstarts.cn

[T42] Perl：变量类型
来源：http://om.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fh.szxytkj.cn

[T43] Perl：字符串插值
来源：http://va.huixinmuqiang.cn

"值: $a"
来源：http://ev.haigaiapp.cn

[T44] Perl：条件
来源：http://ux.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://go.huanxung.cn

[T45] Perl：数组遍历
来源：http://te.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://le.huanxung.cn

[T46] Perl：哈希操作
来源：http://yv.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dx.colortex.cn

[T47] Perl：正则捕获
来源：http://ti.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sz.hnjuh.cn

[T48] Perl：正则替换
来源：http://pa.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://zc.hnjuh.cn

[T49] Perl：函数
来源：http://wy.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ru.nszjky.cn

[T50] Perl：逐行读文件
来源：http://tg.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jc.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://qw.asd995.cn

[T51] Scala：Hello World
来源：http://ro.huixinmuqiang.cn

println("Hello")
来源：http://mh.huanxung.cn

[T52] Scala：变量
来源：http://ko.hahajie.cn

val a = 1;  var b = 2
来源：http://it.asd995.cn

[T53] Scala：字符串插值
来源：http://pt.lnxyls.cn

s"值: $b"
来源：http://aq.wgjwhj.cn

[T54] Scala：集合映射
来源：http://dz.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://zy.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://lg.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tq.colortex.cn

[T56] Scala：样例类
来源：http://sn.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://kx.nicolike.cn

[T57] Scala：模式匹配
来源：http://ru.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dg.hnjuh.cn

[T58] Scala：函数定义
来源：http://pu.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wd.9csxet.cn

[T59] Scala：循环
来源：http://rj.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://nj.colortex.cn

[T60] Scala：折叠
来源：http://wn.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iw.haigaiapp.cn

================================================================================
来源：http://as.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cq.colortex.cn

================================================================================
来源：http://ud.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://gs.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lh.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://uc.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dg.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://oc.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xd.9csxet.cn

[U04] Py：变量调试打印
来源：http://ln.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ac.hahajie.cn

[U05] Py：列表去重且保序
来源：http://ci.colortex.cn

list(dict.fromkeys(arr))
来源：http://ax.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://tn.huixinmuqiang.cn

{**a, **b}
来源：http://eh.521024.cn

[U07] Py：反转字典键值
来源：http://ba.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://zl.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://ht.muxihuayi.cn

[y for x in nested for y in x]
来源：http://wy.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://sw.yuntaijiaju.cn

max(d, key=d.get)
来源：http://ld.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://yu.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ge.521024.cn

[U11] Py：生成器表达式
来源：http://qf.szsharing.cn

(x * 2 for x in arr)
来源：http://hr.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hb.lnxyls.cn

Counter(arr).most_common(3)
来源：http://ym.gzmigu.cn

[U13] Py：固定长度队列
来源：http://lr.szxytkj.cn

deque(maxlen=10)
来源：http://un.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://np.521024.cn

defaultdict(list)
来源：http://aj.haigaiapp.cn

[U15] Py：高精度计时
来源：http://ev.shxzskj.cn

t = time.perf_counter()
来源：http://sf.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://dm.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rv.521024.cn

[U17] Py：初始化日志
来源：http://qg.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://hj.gzmigu.cn

[U18] Py：预编译正则
来源：http://wt.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://so.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://tv.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yy.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ri.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://jv.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://re.wgjwhj.cn

@contextlib.contextmanager
来源：http://qp.huanxung.cn

[U22] Py：矩阵转置
来源：http://xm.nicolike.cn

list(zip(*m))
来源：http://cd.nicolike.cn

[U23] Py：分块读取大文件
来源：http://en.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yv.shtwfgs.cn

[U24] Py：路径操作
来源：http://gl.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ma.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://kc.haigaiapp.cn

csv.DictReader(f)
来源：http://vx.bookmarksfly.cn

[U26] Py：并发下载
来源：http://xo.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yf.colortex.cn

[U27] Py：异步 HTTP
来源：http://ib.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://gi.jctech888.com.cn

[U28] Py：类型别名
来源：http://dv.jctech888.com.cn

UserId = int
来源：http://ml.szsharing.cn

[U29] Py：属性校验
来源：http://dn.shxzskj.cn

@property 与 @x.setter 配合
来源：http://po.shxzukj.cn

[U30] Py：数据类
来源：http://wh.bookmarksfly.cn

@dataclass(slots=True)
来源：http://vn.newstarts.cn

[U31] Py：单测
来源：http://ri.shxzukj.cn

python -m pytest -q
来源：http://wa.521024.cn

[U32] Py：代码格式化
来源：http://zq.nicolike.cn

ruff format . && ruff check --fix .
来源：http://id.chemitech.net.cn

[U33] Py：打包发布
来源：http://gw.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://gs.jctech888.com.cn

[U34] Py：判断编码
来源：http://wz.9csxet.cn

chardet.detect(raw)
来源：http://do.newstarts.cn

[U35] Py：发送邮件
来源：http://sy.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fh.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ri.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://ls.colortex.cn

[U37] Py：读写 Excel
来源：http://uh.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yb.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://tk.hnjuh.cn

Path(__file__).resolve().parent
来源：http://lb.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://qm.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ha.szsharing.cn

[U40] Py：打印到标准错误
来源：http://qw.nicolike.cn

print("err", file=sys.stderr)
来源：http://pi.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://sc.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dk.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://fm.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sd.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://uy.521024.cn

namespace App\Http;
来源：http://do.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ny.huanxung.cn

declare(strict_types=1);
来源：http://gz.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://ba.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fk.chemitech.net.cn

[U46] PHP：可空类型
来源：http://zf.yuexingan06.cn

?string $name = null
来源：http://go.haigaiapp.cn

[U47] PHP：联合类型
来源：http://pv.panjiajie.cn

int|string $id
来源：http://pf.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://gw.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nj.wgjwhj.cn

[U49] PHP：只读属性
来源：http://nd.9csxet.cn

public readonly string $name
来源：http://bl.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://ik.panjiajie.cn

public function __construct(private int $id) {}
来源：http://vp.szxytkj.cn

[U51] PHP：数组解构
来源：http://oh.521024.cn

[$a, $b] = $arr;
来源：http://td.szsharing.cn

[U52] PHP：箭头函数
来源：http://fq.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://yg.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://vj.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://bq.9csxet.cn

[U54] PHP：空安全调用
来源：http://fi.huixinmuqiang.cn

$obj?->method()
来源：http://gh.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://cc.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sp.asd995.cn

[U56] PHP：命名参数
来源：http://hw.9csxet.cn

f(a: 1, b: 2)
来源：http://uo.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://ni.yuexingan06.cn

"值: {$a}"
来源：http://ug.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://we.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rr.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://hm.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ub.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://nd.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vp.huanxung.cn

[U61] PHP：正则
来源：http://if.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://df.yuexingan06.cn

[U62] PHP：日期对象
来源：http://ek.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://md.chemitech.net.cn

[U63] PHP：文件读写
来源：http://lp.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rp.hnjuh.cn

[U64] PHP：目录遍历
来源：http://yy.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://kx.jianghongdianzi.cn

[U65] PHP：会话
来源：http://ge.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lg.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://xu.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nx.hahajie.cn

[U67] PHP：处理文件上传
来源：http://jd.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mj.huanxung.cn

[U68] PHP：PDO 连接
来源：http://er.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zm.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://pb.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://in.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://oy.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sq.hahajie.cn

[U71] PHP：抛出异常
来源：http://go.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://mb.asd995.cn

[U72] PHP：写错误日志
来源：http://da.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://dn.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://to.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://vh.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://qg.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://vj.hnjuh.cn

[U75] PHP：依赖注入
来源：http://sy.nicolike.cn

composer require psr/container
来源：http://yj.gzmigu.cn

[U76] PHP：简单路由
来源：http://an.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nq.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://jh.shxzskj.cn

composer require twig/twig
来源：http://hd.nszjky.cn

[U78] PHP：单元测试
来源：http://gm.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://xb.9csxet.cn

[U79] PHP：静态分析
来源：http://ek.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://un.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://nu.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hf.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://sw.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://vc.nicolike.cn

[U82] JS：package.json 脚本
来源：http://gp.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mt.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://ls.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tr.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://hn.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zv.muxihuayi.cn

[U85] JS：可选链
来源：http://qi.jianghongdianzi.cn

a?.b?.c
来源：http://wr.szxytkj.cn

[U86] JS：空值合并
来源：http://vh.hnjuh.cn

a ?? b
来源：http://du.hahajie.cn


<!-- 参考信息 -->