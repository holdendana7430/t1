代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://he.huixinmuqiang.cn

================================================================================
来源：http://xx.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lx.szxytkj.cn

================================================================================
来源：http://kq.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://zm.muxihuayi.cn

println("Hello")
来源：http://bt.chemitech.net.cn

[T02] Kotlin：变量
来源：http://ad.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bx.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://gh.nszjky.cn

"值: $b"
来源：http://ad.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://wz.521024.cn

val n: String? = null;  n?.length
来源：http://rj.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://wg.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mr.newstarts.cn

[T06] Kotlin：集合映射
来源：http://wc.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ec.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://px.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://td.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://ow.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://ap.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://tk.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://vq.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://tu.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tm.bjjhwx.cn

[T11] Kotlin：协程
来源：http://nw.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iy.szsharing.cn

[T12] Kotlin：解构声明
来源：http://vg.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://wc.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://mi.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://zb.nszjky.cn

[T14] Kotlin：循环
来源：http://nj.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://zj.hnjuh.cn

[T15] Kotlin：接口
来源：http://lj.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://wv.asd995.cn

[T16] Swift：Hello World
来源：http://yp.newstarts.cn

print("Hello")
来源：http://br.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://os.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ug.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://ue.chemitech.net.cn

"值: \(b)"
来源：http://nz.colortex.cn

[T19] Swift：可选绑定
来源：http://zn.521024.cn

if let n = opt { print(n) }
来源：http://ce.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://xb.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oi.shxzukj.cn

[T21] Swift：遍历
来源：http://ob.wgjwhj.cn

for x in a { print(x) }
来源：http://sq.huixinmuqiang.cn

[T22] Swift：字典
来源：http://iz.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jx.bookmarksfly.cn

[T23] Swift：函数
来源：http://lg.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hg.yuexingan06.cn

[T24] Swift：闭包
来源：http://el.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gi.chemitech.net.cn

[T25] Swift：结构体
来源：http://ge.521024.cn

struct P { var x: Int }
来源：http://ll.muxihuayi.cn

[T26] Swift：类与重写
来源：http://xk.newstarts.cn

class A: Base { override func f() {} }
来源：http://cc.nicolike.cn

[T27] Swift：错误处理
来源：http://qi.asd995.cn

do { try f() } catch { print(error) }
来源：http://dl.huanxung.cn

[T28] Swift：枚举
来源：http://um.nicolike.cn

enum Color { case red, green }
来源：http://pd.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://mh.colortex.cn

guard let x = opt else { return }
来源：http://bq.haigaiapp.cn

[T30] Swift：协议
来源：http://dj.asd995.cn

protocol Shape { func area() -> Double }
来源：http://ke.panjiajie.cn

[T31] Lua：Hello World
来源：http://tv.haigaiapp.cn

print("Hello")
来源：http://hz.nszjky.cn

[T32] Lua：局部变量
来源：http://ru.hnjuh.cn

local a = 1
来源：http://om.521024.cn

[T33] Lua：表（数组）
来源：http://qu.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hc.szsharing.cn

[T34] Lua：遍历表
来源：http://ud.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bg.gzmigu.cn

[T35] Lua：字典表
来源：http://mn.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://hw.colortex.cn

[T36] Lua：函数
来源：http://ij.9csxet.cn

function add(a, b) return a + b end
来源：http://wy.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://ik.szxytkj.cn

"a" .. "b"
来源：http://jw.nszjky.cn

[T38] Lua：条件
来源：http://ii.newstarts.cn

if x > 0 then print("正") end
来源：http://xi.huanxung.cn

[T39] Lua：模式匹配
来源：http://fe.bookmarksfly.cn

string.find(s, "%d+")
来源：http://mp.shxzskj.cn

[T40] Lua：元表
来源：http://ox.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://ip.hnjuh.cn

[T41] Perl：Hello World
来源：http://ar.nicolike.cn

print "Hello\n";
来源：http://ba.shxzukj.cn

[T42] Perl：变量类型
来源：http://nc.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nv.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://hp.shtwfgs.cn

"值: $a"
来源：http://mz.haigaiapp.cn

[T44] Perl：条件
来源：http://cz.colortex.cn

if ($a > 0) { print "正"; }
来源：http://pn.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://cg.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://mz.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://hz.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pj.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://qk.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iv.asd995.cn

[T48] Perl：正则替换
来源：http://qg.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://og.wgjwhj.cn

[T49] Perl：函数
来源：http://zs.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qd.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://nk.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gq.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://tr.szxytkj.cn

[T51] Scala：Hello World
来源：http://hu.jianghongdianzi.cn

println("Hello")
来源：http://rs.yuntaijiaju.cn

[T52] Scala：变量
来源：http://xh.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://jx.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://ts.bookmarksfly.cn

s"值: $b"
来源：http://jp.shtwfgs.cn

[T54] Scala：集合映射
来源：http://zl.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://ob.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://qd.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qf.lnxyls.cn

[T56] Scala：样例类
来源：http://iq.asd995.cn

case class User(name: String, age: Int)
来源：http://gl.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://bw.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zj.lnxyls.cn

[T58] Scala：函数定义
来源：http://th.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pc.chemitech.net.cn

[T59] Scala：循环
来源：http://pb.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://un.gzmigu.cn

[T60] Scala：折叠
来源：http://ow.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://my.panjiajie.cn

================================================================================
来源：http://dd.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://da.jianghongdianzi.cn

================================================================================
来源：http://up.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://je.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qf.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://hy.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://io.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://xn.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zp.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://gz.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fo.huanxung.cn

[U05] Py：列表去重且保序
来源：http://dc.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://wr.asd995.cn

[U06] Py：合并两个字典
来源：http://qr.wgjwhj.cn

{**a, **b}
来源：http://sg.gzmigu.cn

[U07] Py：反转字典键值
来源：http://fk.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://db.lnxyls.cn

[U08] Py：展平二维列表
来源：http://au.bjjhwx.cn

[y for x in nested for y in x]
来源：http://li.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://po.yuexingan06.cn

max(d, key=d.get)
来源：http://xs.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://ku.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://va.huanxung.cn

[U11] Py：生成器表达式
来源：http://dv.newstarts.cn

(x * 2 for x in arr)
来源：http://pj.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iw.gzmigu.cn

Counter(arr).most_common(3)
来源：http://ps.9csxet.cn

[U13] Py：固定长度队列
来源：http://ma.bjjhwx.cn

deque(maxlen=10)
来源：http://sh.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://mx.wgjwhj.cn

defaultdict(list)
来源：http://td.shxzukj.cn

[U15] Py：高精度计时
来源：http://vm.nszjky.cn

t = time.perf_counter()
来源：http://ss.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://cj.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rn.haigaiapp.cn

[U17] Py：初始化日志
来源：http://kq.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nt.shtwfgs.cn

[U18] Py：预编译正则
来源：http://py.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://cm.nszjky.cn

[U19] Py：正则替换带回调
来源：http://dd.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wk.9csxet.cn

[U20] Py：缓存函数结果
来源：http://my.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://tv.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://tc.shtwfgs.cn

@contextlib.contextmanager
来源：http://gc.shxzukj.cn

[U22] Py：矩阵转置
来源：http://ym.szsharing.cn

list(zip(*m))
来源：http://ub.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://kv.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qk.gzmigu.cn

[U24] Py：路径操作
来源：http://nr.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kw.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://oe.lnxyls.cn

csv.DictReader(f)
来源：http://hu.haigaiapp.cn

[U26] Py：并发下载
来源：http://nu.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xo.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://aa.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://bh.haigaiapp.cn

[U28] Py：类型别名
来源：http://gj.huixiangedu.cn

UserId = int
来源：http://cf.colortex.cn

[U29] Py：属性校验
来源：http://kc.nszjky.cn

@property 与 @x.setter 配合
来源：http://jb.haigaiapp.cn

[U30] Py：数据类
来源：http://ao.shtwfgs.cn

@dataclass(slots=True)
来源：http://no.bjjhwx.cn

[U31] Py：单测
来源：http://ws.haigaiapp.cn

python -m pytest -q
来源：http://cq.jctech888.com.cn

[U32] Py：代码格式化
来源：http://cq.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://rn.nicolike.cn

[U33] Py：打包发布
来源：http://nr.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://eu.szxytkj.cn

[U34] Py：判断编码
来源：http://kn.wgjwhj.cn

chardet.detect(raw)
来源：http://ea.lnxyls.cn

[U35] Py：发送邮件
来源：http://pu.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yl.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://nz.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://ph.huanxung.cn

[U37] Py：读写 Excel
来源：http://tw.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dm.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://mw.huanxung.cn

Path(__file__).resolve().parent
来源：http://hh.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://bd.wgjwhj.cn

sys.stdout.isatty()
来源：http://id.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://bw.asd995.cn

print("err", file=sys.stderr)
来源：http://fy.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://hi.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mp.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://sw.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://np.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://nn.shxzskj.cn

namespace App\Http;
来源：http://ob.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://tl.panjiajie.cn

declare(strict_types=1);
来源：http://mv.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://hh.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hd.szsharing.cn

[U46] PHP：可空类型
来源：http://mp.lnxyls.cn

?string $name = null
来源：http://kv.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://js.shtwfgs.cn

int|string $id
来源：http://lt.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://fa.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jw.shtwfgs.cn

[U49] PHP：只读属性
来源：http://rw.haigaiapp.cn

public readonly string $name
来源：http://ce.colortex.cn

[U50] PHP：构造器属性提升
来源：http://ix.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://sk.shxzskj.cn

[U51] PHP：数组解构
来源：http://ho.nszjky.cn

[$a, $b] = $arr;
来源：http://db.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://xq.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://kv.colortex.cn

[U53] PHP：空合并运算符
来源：http://bh.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://hq.shxzskj.cn

[U54] PHP：空安全调用
来源：http://ok.gzmigu.cn

$obj?->method()
来源：http://cf.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://sf.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gm.szxytkj.cn

[U56] PHP：命名参数
来源：http://vs.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://od.lnxyls.cn

[U57] PHP：字符串插值
来源：http://ag.szxytkj.cn

"值: {$a}"
来源：http://us.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://lb.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ue.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://mx.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://do.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://ho.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://db.chemitech.net.cn

[U61] PHP：正则
来源：http://gq.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kp.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://fr.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lb.shxzukj.cn

[U63] PHP：文件读写
来源：http://gh.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nb.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://nm.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://yv.shtwfgs.cn

[U65] PHP：会话
来源：http://vp.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fo.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://ox.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dk.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://yf.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://de.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://ik.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vl.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://ph.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gi.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://af.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qo.hnjuh.cn

[U71] PHP：抛出异常
来源：http://gq.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://ea.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://xq.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://ij.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://cb.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://yu.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://vm.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://qh.shxzskj.cn

[U75] PHP：依赖注入
来源：http://mg.nicolike.cn

composer require psr/container
来源：http://xq.szxytkj.cn

[U76] PHP：简单路由
来源：http://qc.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jd.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://qe.hahajie.cn

composer require twig/twig
来源：http://ia.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://js.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://ar.yuexingan06.cn

[U79] PHP：静态分析
来源：http://jy.521024.cn

composer require --dev phpstan/phpstan
来源：http://el.521024.cn

[U80] PHP：代码规范修复
来源：http://ab.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sw.lnxyls.cn

[U81] JS：初始化项目
来源：http://ir.jctech888.com.cn

npm init -y;  npm i express
来源：http://nj.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://tn.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ds.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://gf.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lf.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://zu.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qy.9csxet.cn

[U85] JS：可选链
来源：http://ku.szsharing.cn

a?.b?.c
来源：http://mb.shxzskj.cn

[U86] JS：空值合并
来源：http://co.hahajie.cn

a ?? b
来源：http://ad.colortex.cn


<!-- 参考信息 -->