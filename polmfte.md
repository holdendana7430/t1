代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ig.9csxet.cn

================================================================================
来源：http://rr.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fq.jianghongdianzi.cn

================================================================================
来源：http://dc.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://xa.haigaiapp.cn

println("Hello")
来源：http://ye.shtwfgs.cn

[T02] Kotlin：变量
来源：http://jc.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ui.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://uv.yuntaijiaju.cn

"值: $b"
来源：http://yg.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://qp.nicolike.cn

val n: String? = null;  n?.length
来源：http://uf.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://gq.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bp.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://ng.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kd.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://wj.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yz.asd995.cn

[T08] Kotlin：数据类
来源：http://hx.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ih.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://nr.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://ue.521024.cn

[T10] Kotlin：默认参数
来源：http://jc.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hm.jctech888.com.cn

[T11] Kotlin：协程
来源：http://nz.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ik.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://pm.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://ur.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ie.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://az.huanxung.cn

[T14] Kotlin：循环
来源：http://ba.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://it.yuexingan06.cn

[T15] Kotlin：接口
来源：http://xv.colortex.cn

interface Shape { fun area(): Double }
来源：http://lb.lnxyls.cn

[T16] Swift：Hello World
来源：http://cz.szsharing.cn

print("Hello")
来源：http://jt.newstarts.cn

[T17] Swift：变量与常量
来源：http://et.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://hm.colortex.cn

[T18] Swift：字符串插值
来源：http://rt.9csxet.cn

"值: \(b)"
来源：http://ka.huanxung.cn

[T19] Swift：可选绑定
来源：http://qx.bjjhwx.cn

if let n = opt { print(n) }
来源：http://kw.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://wg.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qg.muxihuayi.cn

[T21] Swift：遍历
来源：http://fm.bjjhwx.cn

for x in a { print(x) }
来源：http://am.nszjky.cn

[T22] Swift：字典
来源：http://ua.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ub.jianghongdianzi.cn

[T23] Swift：函数
来源：http://vv.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ra.jctech888.com.cn

[T24] Swift：闭包
来源：http://vh.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ob.9csxet.cn

[T25] Swift：结构体
来源：http://vy.wgjwhj.cn

struct P { var x: Int }
来源：http://jg.nicolike.cn

[T26] Swift：类与重写
来源：http://vh.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://lv.newstarts.cn

[T27] Swift：错误处理
来源：http://nc.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://qs.shxzskj.cn

[T28] Swift：枚举
来源：http://ai.bjjhwx.cn

enum Color { case red, green }
来源：http://jt.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://en.huanxung.cn

guard let x = opt else { return }
来源：http://vp.shxzskj.cn

[T30] Swift：协议
来源：http://rk.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://vd.nicolike.cn

[T31] Lua：Hello World
来源：http://ey.muxihuayi.cn

print("Hello")
来源：http://mc.chemitech.net.cn

[T32] Lua：局部变量
来源：http://qy.gzmigu.cn

local a = 1
来源：http://sn.gzmigu.cn

[T33] Lua：表（数组）
来源：http://dj.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vl.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://vu.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gu.shxzskj.cn

[T35] Lua：字典表
来源：http://yd.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://ul.colortex.cn

[T36] Lua：函数
来源：http://jr.nszjky.cn

function add(a, b) return a + b end
来源：http://me.nszjky.cn

[T37] Lua：字符串拼接
来源：http://qb.panjiajie.cn

"a" .. "b"
来源：http://yj.hnjuh.cn

[T38] Lua：条件
来源：http://dt.shtwfgs.cn

if x > 0 then print("正") end
来源：http://yj.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://da.lnxyls.cn

string.find(s, "%d+")
来源：http://da.haigaiapp.cn

[T40] Lua：元表
来源：http://kc.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://ui.hahajie.cn

[T41] Perl：Hello World
来源：http://ys.chemitech.net.cn

print "Hello\n";
来源：http://lz.9csxet.cn

[T42] Perl：变量类型
来源：http://nf.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wv.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://xh.haigaiapp.cn

"值: $a"
来源：http://wy.9csxet.cn

[T44] Perl：条件
来源：http://cg.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://ih.huanxung.cn

[T45] Perl：数组遍历
来源：http://aj.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://xr.panjiajie.cn

[T46] Perl：哈希操作
来源：http://zx.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nv.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://af.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://al.colortex.cn

[T48] Perl：正则替换
来源：http://sp.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://lo.jctech888.com.cn

[T49] Perl：函数
来源：http://oi.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gp.huanxung.cn

[T50] Perl：逐行读文件
来源：http://eh.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zi.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://mj.lnxyls.cn

[T51] Scala：Hello World
来源：http://ay.colortex.cn

println("Hello")
来源：http://dr.hahajie.cn

[T52] Scala：变量
来源：http://oo.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://wh.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://ue.hahajie.cn

s"值: $b"
来源：http://ae.chemitech.net.cn

[T54] Scala：集合映射
来源：http://db.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://xf.9csxet.cn

[T55] Scala：集合过滤
来源：http://ze.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://il.nicolike.cn

[T56] Scala：样例类
来源：http://hu.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://tw.521024.cn

[T57] Scala：模式匹配
来源：http://bw.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hs.colortex.cn

[T58] Scala：函数定义
来源：http://ae.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://za.yuexingan06.cn

[T59] Scala：循环
来源：http://nx.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://he.521024.cn

[T60] Scala：折叠
来源：http://wf.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ei.521024.cn

================================================================================
来源：http://ap.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ff.nszjky.cn

================================================================================
来源：http://ex.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://jr.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tm.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://aq.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pp.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://nq.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yz.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://qh.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zg.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://wm.newstarts.cn

list(dict.fromkeys(arr))
来源：http://fe.nszjky.cn

[U06] Py：合并两个字典
来源：http://lx.szxytkj.cn

{**a, **b}
来源：http://gd.521024.cn

[U07] Py：反转字典键值
来源：http://jk.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://mg.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://vd.panjiajie.cn

[y for x in nested for y in x]
来源：http://hf.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://of.521024.cn

max(d, key=d.get)
来源：http://tv.9csxet.cn

[U10] Py：按值排序字典
来源：http://fg.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tm.9csxet.cn

[U11] Py：生成器表达式
来源：http://kb.colortex.cn

(x * 2 for x in arr)
来源：http://mz.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bq.shxzskj.cn

Counter(arr).most_common(3)
来源：http://lv.huanxung.cn

[U13] Py：固定长度队列
来源：http://ja.shxzukj.cn

deque(maxlen=10)
来源：http://ug.nszjky.cn

[U14] Py：分组收集到列表
来源：http://ic.newstarts.cn

defaultdict(list)
来源：http://nn.gzmigu.cn

[U15] Py：高精度计时
来源：http://hz.muxihuayi.cn

t = time.perf_counter()
来源：http://bl.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://ry.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oj.bjjhwx.cn

[U17] Py：初始化日志
来源：http://co.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://iy.hahajie.cn

[U18] Py：预编译正则
来源：http://vw.nszjky.cn

pat = re.compile(r"\d+")
来源：http://wi.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ra.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qo.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://fj.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://vf.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://sp.9csxet.cn

@contextlib.contextmanager
来源：http://nw.colortex.cn

[U22] Py：矩阵转置
来源：http://lq.chemitech.net.cn

list(zip(*m))
来源：http://pf.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://mn.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ki.newstarts.cn

[U24] Py：路径操作
来源：http://dr.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ni.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://pr.haigaiapp.cn

csv.DictReader(f)
来源：http://ej.colortex.cn

[U26] Py：并发下载
来源：http://qt.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jy.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://zs.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://qu.haigaiapp.cn

[U28] Py：类型别名
来源：http://on.yuntaijiaju.cn

UserId = int
来源：http://st.bjjhwx.cn

[U29] Py：属性校验
来源：http://tr.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://er.bjjhwx.cn

[U30] Py：数据类
来源：http://xl.hahajie.cn

@dataclass(slots=True)
来源：http://xr.9csxet.cn

[U31] Py：单测
来源：http://xe.wgjwhj.cn

python -m pytest -q
来源：http://uj.huanxung.cn

[U32] Py：代码格式化
来源：http://nm.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://hp.yuexingan06.cn

[U33] Py：打包发布
来源：http://vb.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://jf.huanxung.cn

[U34] Py：判断编码
来源：http://rg.hnjuh.cn

chardet.detect(raw)
来源：http://xh.nicolike.cn

[U35] Py：发送邮件
来源：http://wf.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jz.haigaiapp.cn

[U36] Py：定时任务
来源：http://al.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://yv.hahajie.cn

[U37] Py：读写 Excel
来源：http://ov.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jf.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://tn.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://oa.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://fc.panjiajie.cn

sys.stdout.isatty()
来源：http://qp.hahajie.cn

[U40] Py：打印到标准错误
来源：http://re.asd995.cn

print("err", file=sys.stderr)
来源：http://ew.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ir.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qt.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vf.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://un.521024.cn

[U43] PHP：声明命名空间
来源：http://bn.nszjky.cn

namespace App\Http;
来源：http://eu.colortex.cn

[U44] PHP：开启严格类型
来源：http://ar.lnxyls.cn

declare(strict_types=1);
来源：http://ez.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://wz.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xo.521024.cn

[U46] PHP：可空类型
来源：http://dv.asd995.cn

?string $name = null
来源：http://pw.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://rc.asd995.cn

int|string $id
来源：http://rf.9csxet.cn

[U48] PHP：纯枚举
来源：http://gn.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ts.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://tv.huanxung.cn

public readonly string $name
来源：http://nr.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://rn.hnjuh.cn

public function __construct(private int $id) {}
来源：http://rz.bjjhwx.cn

[U51] PHP：数组解构
来源：http://qa.newstarts.cn

[$a, $b] = $arr;
来源：http://yb.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://pm.colortex.cn

$double = fn($x) => $x * 2;
来源：http://pr.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://eu.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://uo.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://vl.gzmigu.cn

$obj?->method()
来源：http://rx.newstarts.cn

[U55] PHP：match 表达式
来源：http://fi.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jb.yuexingan06.cn

[U56] PHP：命名参数
来源：http://ws.nszjky.cn

f(a: 1, b: 2)
来源：http://tt.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://tk.shtwfgs.cn

"值: {$a}"
来源：http://nf.hahajie.cn

[U58] PHP：数组三件套
来源：http://ka.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zc.panjiajie.cn

[U59] PHP：自定义排序
来源：http://by.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cn.asd995.cn

[U60] PHP：JSON 编解码
来源：http://le.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://de.panjiajie.cn

[U61] PHP：正则
来源：http://bx.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lt.bjjhwx.cn

[U62] PHP：日期对象
来源：http://jo.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yy.gzmigu.cn

[U63] PHP：文件读写
来源：http://ma.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kz.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://wg.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://yc.newstarts.cn

[U65] PHP：会话
来源：http://cl.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fu.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://ia.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rz.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://yw.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mq.szsharing.cn

[U68] PHP：PDO 连接
来源：http://ye.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://su.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://mp.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gh.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://sk.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://il.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://ap.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://fi.gzmigu.cn

[U72] PHP：写错误日志
来源：http://oe.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://dz.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://jx.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://jb.asd995.cn

[U74] PHP：读取环境变量
来源：http://jv.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://xs.szsharing.cn

[U75] PHP：依赖注入
来源：http://iv.lnxyls.cn

composer require psr/container
来源：http://ha.newstarts.cn

[U76] PHP：简单路由
来源：http://ai.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gp.nszjky.cn

[U77] PHP：模板渲染
来源：http://uv.shtwfgs.cn

composer require twig/twig
来源：http://dw.hnjuh.cn

[U78] PHP：单元测试
来源：http://td.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://zh.yuexingan06.cn

[U79] PHP：静态分析
来源：http://ot.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://gx.hahajie.cn

[U80] PHP：代码规范修复
来源：http://yb.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oj.bjjhwx.cn

[U81] JS：初始化项目
来源：http://mg.szxytkj.cn

npm init -y;  npm i express
来源：http://ey.colortex.cn

[U82] JS：package.json 脚本
来源：http://xe.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hw.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://dm.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yi.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://jn.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://um.hnjuh.cn

[U85] JS：可选链
来源：http://qw.9csxet.cn

a?.b?.c
来源：http://bu.szxytkj.cn

[U86] JS：空值合并
来源：http://wd.nicolike.cn

a ?? b
来源：http://yd.shxzukj.cn


<!-- 参考信息 -->