代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://te.panjiajie.cn

================================================================================
来源：http://ja.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tk.yuntaijiaju.cn

================================================================================
来源：http://rb.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://as.szxytkj.cn

println("Hello")
来源：http://ah.9csxet.cn

[T02] Kotlin：变量
来源：http://hj.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ti.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://xq.chemitech.net.cn

"值: $b"
来源：http://nv.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://nw.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://fd.colortex.cn

[T05] Kotlin：when 表达式
来源：http://nc.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wm.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://iz.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aa.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://zh.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oq.shxzukj.cn

[T08] Kotlin：数据类
来源：http://nk.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://rw.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://aw.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://im.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://zj.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pk.shtwfgs.cn

[T11] Kotlin：协程
来源：http://zu.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jw.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://hm.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://zq.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://fs.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://nw.nszjky.cn

[T14] Kotlin：循环
来源：http://lx.newstarts.cn

for (i in 1..10) println(i)
来源：http://mo.newstarts.cn

[T15] Kotlin：接口
来源：http://is.asd995.cn

interface Shape { fun area(): Double }
来源：http://nz.shtwfgs.cn

[T16] Swift：Hello World
来源：http://oh.gzmigu.cn

print("Hello")
来源：http://bi.colortex.cn

[T17] Swift：变量与常量
来源：http://ga.szxytkj.cn

var a = 1;  let b = 2
来源：http://wf.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://xn.chemitech.net.cn

"值: \(b)"
来源：http://jd.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://lc.chemitech.net.cn

if let n = opt { print(n) }
来源：http://te.chemitech.net.cn

[T20] Swift：数组操作
来源：http://vr.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zl.nszjky.cn

[T21] Swift：遍历
来源：http://uo.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ne.huixiangedu.cn

[T22] Swift：字典
来源：http://cv.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zc.gzmigu.cn

[T23] Swift：函数
来源：http://ci.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zj.wgjwhj.cn

[T24] Swift：闭包
来源：http://ht.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ep.521024.cn

[T25] Swift：结构体
来源：http://kr.szsharing.cn

struct P { var x: Int }
来源：http://jo.colortex.cn

[T26] Swift：类与重写
来源：http://mk.shxzskj.cn

class A: Base { override func f() {} }
来源：http://rz.szxytkj.cn

[T27] Swift：错误处理
来源：http://fj.colortex.cn

do { try f() } catch { print(error) }
来源：http://yo.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://wo.newstarts.cn

enum Color { case red, green }
来源：http://gq.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://aw.wgjwhj.cn

guard let x = opt else { return }
来源：http://vg.asd995.cn

[T30] Swift：协议
来源：http://ue.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://vh.9csxet.cn

[T31] Lua：Hello World
来源：http://gy.hnjuh.cn

print("Hello")
来源：http://ou.haigaiapp.cn

[T32] Lua：局部变量
来源：http://vn.jctech888.com.cn

local a = 1
来源：http://mf.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://oe.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://of.szsharing.cn

[T34] Lua：遍历表
来源：http://gy.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hk.szsharing.cn

[T35] Lua：字典表
来源：http://gw.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://az.521024.cn

[T36] Lua：函数
来源：http://tn.hnjuh.cn

function add(a, b) return a + b end
来源：http://om.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://qt.hahajie.cn

"a" .. "b"
来源：http://tz.huixiangedu.cn

[T38] Lua：条件
来源：http://dn.shtwfgs.cn

if x > 0 then print("正") end
来源：http://mb.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://rj.9csxet.cn

string.find(s, "%d+")
来源：http://yu.bjjhwx.cn

[T40] Lua：元表
来源：http://iu.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://ll.szxytkj.cn

[T41] Perl：Hello World
来源：http://gf.colortex.cn

print "Hello\n";
来源：http://ld.nicolike.cn

[T42] Perl：变量类型
来源：http://cb.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bt.asd995.cn

[T43] Perl：字符串插值
来源：http://et.jctech888.com.cn

"值: $a"
来源：http://af.gzmigu.cn

[T44] Perl：条件
来源：http://nw.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://cn.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://ox.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://hx.szsharing.cn

[T46] Perl：哈希操作
来源：http://cf.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bd.hnjuh.cn

[T47] Perl：正则捕获
来源：http://kn.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cv.colortex.cn

[T48] Perl：正则替换
来源：http://rk.colortex.cn

$s =~ s/old/new/g;
来源：http://ez.9csxet.cn

[T49] Perl：函数
来源：http://oe.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ip.9csxet.cn

[T50] Perl：逐行读文件
来源：http://jd.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yb.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://km.gzmigu.cn

[T51] Scala：Hello World
来源：http://cq.nicolike.cn

println("Hello")
来源：http://au.shxzskj.cn

[T52] Scala：变量
来源：http://an.haigaiapp.cn

val a = 1;  var b = 2
来源：http://ka.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://xy.521024.cn

s"值: $b"
来源：http://qg.chemitech.net.cn

[T54] Scala：集合映射
来源：http://rj.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://mi.521024.cn

[T55] Scala：集合过滤
来源：http://xl.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lt.shxzukj.cn

[T56] Scala：样例类
来源：http://qp.szsharing.cn

case class User(name: String, age: Int)
来源：http://me.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://hd.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dt.shtwfgs.cn

[T58] Scala：函数定义
来源：http://tp.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ue.huixinmuqiang.cn

[T59] Scala：循环
来源：http://hf.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://tv.bookmarksfly.cn

[T60] Scala：折叠
来源：http://vv.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bb.chemitech.net.cn

================================================================================
来源：http://vb.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://va.shtwfgs.cn

================================================================================
来源：http://mi.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://bc.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cb.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://wb.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ak.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://br.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fw.521024.cn

[U04] Py：变量调试打印
来源：http://ig.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hm.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://ok.huanxung.cn

list(dict.fromkeys(arr))
来源：http://sm.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://en.asd995.cn

{**a, **b}
来源：http://sm.9csxet.cn

[U07] Py：反转字典键值
来源：http://fj.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://qh.521024.cn

[U08] Py：展平二维列表
来源：http://dc.panjiajie.cn

[y for x in nested for y in x]
来源：http://bu.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://cz.lnxyls.cn

max(d, key=d.get)
来源：http://gt.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://jq.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pm.9csxet.cn

[U11] Py：生成器表达式
来源：http://uw.wgjwhj.cn

(x * 2 for x in arr)
来源：http://rr.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tc.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://fx.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://lh.wgjwhj.cn

deque(maxlen=10)
来源：http://jj.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://zf.jctech888.com.cn

defaultdict(list)
来源：http://hw.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://ml.bjjhwx.cn

t = time.perf_counter()
来源：http://zu.newstarts.cn

[U16] Py：命令行参数解析
来源：http://mh.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xu.yuexingan06.cn

[U17] Py：初始化日志
来源：http://xm.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://pv.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://yu.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://xw.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ye.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eq.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://fv.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://er.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://mm.521024.cn

@contextlib.contextmanager
来源：http://dx.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://jq.shxzukj.cn

list(zip(*m))
来源：http://zt.colortex.cn

[U23] Py：分块读取大文件
来源：http://pp.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gr.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://qv.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pj.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://rd.lnxyls.cn

csv.DictReader(f)
来源：http://na.521024.cn

[U26] Py：并发下载
来源：http://nf.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://av.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://io.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://df.jctech888.com.cn

[U28] Py：类型别名
来源：http://er.yuntaijiaju.cn

UserId = int
来源：http://tp.muxihuayi.cn

[U29] Py：属性校验
来源：http://ie.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://ul.colortex.cn

[U30] Py：数据类
来源：http://kw.wgjwhj.cn

@dataclass(slots=True)
来源：http://zv.shxzskj.cn

[U31] Py：单测
来源：http://jx.colortex.cn

python -m pytest -q
来源：http://dx.szsharing.cn

[U32] Py：代码格式化
来源：http://ew.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ez.bookmarksfly.cn

[U33] Py：打包发布
来源：http://wb.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://yb.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://ep.newstarts.cn

chardet.detect(raw)
来源：http://mm.hahajie.cn

[U35] Py：发送邮件
来源：http://jw.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hs.haigaiapp.cn

[U36] Py：定时任务
来源：http://sa.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://zb.huanxung.cn

[U37] Py：读写 Excel
来源：http://ma.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iw.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://tu.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://ui.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://vz.wgjwhj.cn

sys.stdout.isatty()
来源：http://lf.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://vb.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://gw.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://wt.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ix.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://aw.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oe.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://jy.huixiangedu.cn

namespace App\Http;
来源：http://pi.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://sk.gzmigu.cn

declare(strict_types=1);
来源：http://pn.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://oe.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cz.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://nb.asd995.cn

?string $name = null
来源：http://bz.haigaiapp.cn

[U47] PHP：联合类型
来源：http://zn.jctech888.com.cn

int|string $id
来源：http://gj.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://pb.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oq.nszjky.cn

[U49] PHP：只读属性
来源：http://mu.9csxet.cn

public readonly string $name
来源：http://go.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://qj.lnxyls.cn

public function __construct(private int $id) {}
来源：http://uu.colortex.cn

[U51] PHP：数组解构
来源：http://zo.asd995.cn

[$a, $b] = $arr;
来源：http://is.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://qs.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://af.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://rz.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://er.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://uv.lnxyls.cn

$obj?->method()
来源：http://ot.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ed.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tn.szxytkj.cn

[U56] PHP：命名参数
来源：http://ye.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://as.9csxet.cn

[U57] PHP：字符串插值
来源：http://hu.huixinmuqiang.cn

"值: {$a}"
来源：http://zb.szsharing.cn

[U58] PHP：数组三件套
来源：http://yr.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ry.szsharing.cn

[U59] PHP：自定义排序
来源：http://mu.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://he.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://wn.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fw.yuexingan06.cn

[U61] PHP：正则
来源：http://ec.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eb.muxihuayi.cn

[U62] PHP：日期对象
来源：http://ua.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sj.chemitech.net.cn

[U63] PHP：文件读写
来源：http://bj.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nx.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://uy.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ma.jianghongdianzi.cn

[U65] PHP：会话
来源：http://vt.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kd.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://ta.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wn.colortex.cn

[U67] PHP：处理文件上传
来源：http://cd.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ez.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://zb.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rx.colortex.cn

[U69] PHP：PDO 预处理
来源：http://bx.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ze.szsharing.cn

[U70] PHP：PDO 事务
来源：http://da.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://my.shxzukj.cn

[U71] PHP：抛出异常
来源：http://xw.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://us.nicolike.cn

[U72] PHP：写错误日志
来源：http://fe.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://tu.521024.cn

[U73] PHP：读取 ini 配置
来源：http://ki.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://ce.521024.cn

[U74] PHP：读取环境变量
来源：http://xv.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://ro.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://ig.chemitech.net.cn

composer require psr/container
来源：http://pa.jctech888.com.cn

[U76] PHP：简单路由
来源：http://yc.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kk.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://pm.shxzukj.cn

composer require twig/twig
来源：http://to.huixiangedu.cn

[U78] PHP：单元测试
来源：http://pf.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://ak.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://yc.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://ro.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://km.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ek.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://mr.bjjhwx.cn

npm init -y;  npm i express
来源：http://cs.nszjky.cn

[U82] JS：package.json 脚本
来源：http://cc.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://el.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://ty.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sw.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://ed.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://se.bjjhwx.cn

[U85] JS：可选链
来源：http://xf.521024.cn

a?.b?.c
来源：http://jy.gzmigu.cn

[U86] JS：空值合并
来源：http://gk.jctech888.com.cn

a ?? b
来源：http://kh.panjiajie.cn


<!-- 参考信息 -->