代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://va.shxzskj.cn

[S59] C++：静态断言
来源：http://wk.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xu.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://ce.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mc.haigaiapp.cn

================================================================================
来源：http://gn.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cr.shtwfgs.cn

================================================================================
来源：http://bi.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://ry.shtwfgs.cn

println("Hello")
来源：http://gd.gzmigu.cn

[T02] Kotlin：变量
来源：http://xd.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xt.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://oq.bookmarksfly.cn

"值: $b"
来源：http://jw.gzmigu.cn

[T04] Kotlin：空安全
来源：http://vv.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://km.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://rk.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://za.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://jd.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jb.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://hy.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ol.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://hm.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://vj.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://sj.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://fc.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://ul.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sj.chemitech.net.cn

[T11] Kotlin：协程
来源：http://vd.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pu.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://fa.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://kx.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://ik.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://dk.hahajie.cn

[T14] Kotlin：循环
来源：http://dl.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://xl.shxzskj.cn

[T15] Kotlin：接口
来源：http://qr.newstarts.cn

interface Shape { fun area(): Double }
来源：http://ca.haigaiapp.cn

[T16] Swift：Hello World
来源：http://ng.bjjhwx.cn

print("Hello")
来源：http://pt.huanxung.cn

[T17] Swift：变量与常量
来源：http://rj.nszjky.cn

var a = 1;  let b = 2
来源：http://pp.szxytkj.cn

[T18] Swift：字符串插值
来源：http://px.shxzukj.cn

"值: \(b)"
来源：http://xv.nicolike.cn

[T19] Swift：可选绑定
来源：http://dp.shxzskj.cn

if let n = opt { print(n) }
来源：http://vl.nszjky.cn

[T20] Swift：数组操作
来源：http://ta.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yw.hahajie.cn

[T21] Swift：遍历
来源：http://pe.shxzukj.cn

for x in a { print(x) }
来源：http://cr.shtwfgs.cn

[T22] Swift：字典
来源：http://ze.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cd.chemitech.net.cn

[T23] Swift：函数
来源：http://mp.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ue.hahajie.cn

[T24] Swift：闭包
来源：http://wq.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tb.jctech888.com.cn

[T25] Swift：结构体
来源：http://my.panjiajie.cn

struct P { var x: Int }
来源：http://mi.colortex.cn

[T26] Swift：类与重写
来源：http://ki.hahajie.cn

class A: Base { override func f() {} }
来源：http://fn.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://in.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://zc.bookmarksfly.cn

[T28] Swift：枚举
来源：http://kq.wgjwhj.cn

enum Color { case red, green }
来源：http://vp.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ww.nszjky.cn

guard let x = opt else { return }
来源：http://as.shtwfgs.cn

[T30] Swift：协议
来源：http://cf.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://pd.huixiangedu.cn

[T31] Lua：Hello World
来源：http://ac.huixiangedu.cn

print("Hello")
来源：http://bf.gzmigu.cn

[T32] Lua：局部变量
来源：http://ij.jianghongdianzi.cn

local a = 1
来源：http://gh.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://gk.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qz.9csxet.cn

[T34] Lua：遍历表
来源：http://rb.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://un.chemitech.net.cn

[T35] Lua：字典表
来源：http://qf.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://mq.szxytkj.cn

[T36] Lua：函数
来源：http://gh.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://qs.nicolike.cn

[T37] Lua：字符串拼接
来源：http://bk.jianghongdianzi.cn

"a" .. "b"
来源：http://be.huixiangedu.cn

[T38] Lua：条件
来源：http://bj.wgjwhj.cn

if x > 0 then print("正") end
来源：http://ks.hnjuh.cn

[T39] Lua：模式匹配
来源：http://uz.hnjuh.cn

string.find(s, "%d+")
来源：http://av.hnjuh.cn

[T40] Lua：元表
来源：http://yk.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://tg.szsharing.cn

[T41] Perl：Hello World
来源：http://rp.newstarts.cn

print "Hello\n";
来源：http://ix.gzmigu.cn

[T42] Perl：变量类型
来源：http://ql.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ob.nszjky.cn

[T43] Perl：字符串插值
来源：http://zn.nicolike.cn

"值: $a"
来源：http://yh.asd995.cn

[T44] Perl：条件
来源：http://ur.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://wo.gzmigu.cn

[T45] Perl：数组遍历
来源：http://hq.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ed.shxzskj.cn

[T46] Perl：哈希操作
来源：http://yg.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eo.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://em.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wq.521024.cn

[T48] Perl：正则替换
来源：http://hy.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://wh.jianghongdianzi.cn

[T49] Perl：函数
来源：http://gj.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zy.szsharing.cn

[T50] Perl：逐行读文件
来源：http://ru.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bz.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://bl.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://ny.colortex.cn

println("Hello")
来源：http://ht.yuexingan06.cn

[T52] Scala：变量
来源：http://re.521024.cn

val a = 1;  var b = 2
来源：http://vq.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://ph.hnjuh.cn

s"值: $b"
来源：http://mh.521024.cn

[T54] Scala：集合映射
来源：http://fq.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://no.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://so.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zz.shxzskj.cn

[T56] Scala：样例类
来源：http://ds.hahajie.cn

case class User(name: String, age: Int)
来源：http://rp.szxytkj.cn

[T57] Scala：模式匹配
来源：http://sn.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://he.yuexingan06.cn

[T58] Scala：函数定义
来源：http://ai.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qq.bookmarksfly.cn

[T59] Scala：循环
来源：http://yy.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://qd.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://nm.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cm.hnjuh.cn

================================================================================
来源：http://kh.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oi.nszjky.cn

================================================================================
来源：http://ut.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://sy.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pn.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://ox.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://df.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://mo.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pb.nszjky.cn

[U04] Py：变量调试打印
来源：http://gg.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wq.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://sj.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://hu.nicolike.cn

[U06] Py：合并两个字典
来源：http://kw.hnjuh.cn

{**a, **b}
来源：http://sg.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://jn.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://rc.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://oc.shxzukj.cn

[y for x in nested for y in x]
来源：http://nh.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://bx.521024.cn

max(d, key=d.get)
来源：http://ik.newstarts.cn

[U10] Py：按值排序字典
来源：http://gz.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wi.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://xh.yuexingan06.cn

(x * 2 for x in arr)
来源：http://tl.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aj.newstarts.cn

Counter(arr).most_common(3)
来源：http://ij.shxzskj.cn

[U13] Py：固定长度队列
来源：http://ft.wgjwhj.cn

deque(maxlen=10)
来源：http://uu.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ix.panjiajie.cn

defaultdict(list)
来源：http://cl.nicolike.cn

[U15] Py：高精度计时
来源：http://ft.jianghongdianzi.cn

t = time.perf_counter()
来源：http://tx.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://pp.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tw.shtwfgs.cn

[U17] Py：初始化日志
来源：http://gg.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://nh.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://uo.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://gi.nicolike.cn

[U19] Py：正则替换带回调
来源：http://ru.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hu.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://xc.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://lu.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ot.shtwfgs.cn

@contextlib.contextmanager
来源：http://qi.nicolike.cn

[U22] Py：矩阵转置
来源：http://uj.shxzskj.cn

list(zip(*m))
来源：http://od.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://bp.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cz.szxytkj.cn

[U24] Py：路径操作
来源：http://am.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://je.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://ee.muxihuayi.cn

csv.DictReader(f)
来源：http://to.huixiangedu.cn

[U26] Py：并发下载
来源：http://jt.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cd.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://yh.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://pf.szxytkj.cn

[U28] Py：类型别名
来源：http://jl.chemitech.net.cn

UserId = int
来源：http://vm.huixiangedu.cn

[U29] Py：属性校验
来源：http://cw.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://wc.hnjuh.cn

[U30] Py：数据类
来源：http://mz.nicolike.cn

@dataclass(slots=True)
来源：http://jm.muxihuayi.cn

[U31] Py：单测
来源：http://cx.lnxyls.cn

python -m pytest -q
来源：http://jh.jctech888.com.cn

[U32] Py：代码格式化
来源：http://ph.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://ct.bjjhwx.cn

[U33] Py：打包发布
来源：http://gm.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://vj.huixiangedu.cn

[U34] Py：判断编码
来源：http://uf.muxihuayi.cn

chardet.detect(raw)
来源：http://wv.shxzukj.cn

[U35] Py：发送邮件
来源：http://kn.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hs.lnxyls.cn

[U36] Py：定时任务
来源：http://rz.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://ny.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://qo.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xb.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://qn.panjiajie.cn

Path(__file__).resolve().parent
来源：http://hq.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://bw.huixiangedu.cn

sys.stdout.isatty()
来源：http://un.szsharing.cn

[U40] Py：打印到标准错误
来源：http://gh.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://jw.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://bb.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rh.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://wb.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jn.newstarts.cn

[U43] PHP：声明命名空间
来源：http://rt.bjjhwx.cn

namespace App\Http;
来源：http://tt.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ml.bookmarksfly.cn

declare(strict_types=1);
来源：http://kw.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://ph.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lv.gzmigu.cn

[U46] PHP：可空类型
来源：http://ao.hahajie.cn

?string $name = null
来源：http://zb.hnjuh.cn

[U47] PHP：联合类型
来源：http://fu.521024.cn

int|string $id
来源：http://cf.gzmigu.cn

[U48] PHP：纯枚举
来源：http://cr.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vi.muxihuayi.cn

[U49] PHP：只读属性
来源：http://zn.hahajie.cn

public readonly string $name
来源：http://nq.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://te.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://tk.yuexingan06.cn

[U51] PHP：数组解构
来源：http://gq.asd995.cn

[$a, $b] = $arr;
来源：http://vf.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://hg.colortex.cn

$double = fn($x) => $x * 2;
来源：http://fq.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ds.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://th.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://ob.chemitech.net.cn

$obj?->method()
来源：http://rn.szxytkj.cn

[U55] PHP：match 表达式
来源：http://mj.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iq.nicolike.cn

[U56] PHP：命名参数
来源：http://jr.huixiangedu.cn

f(a: 1, b: 2)
来源：http://mv.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://xi.nszjky.cn

"值: {$a}"
来源：http://xn.521024.cn

[U58] PHP：数组三件套
来源：http://jl.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://he.hahajie.cn

[U59] PHP：自定义排序
来源：http://jp.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fm.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://wr.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ua.haigaiapp.cn

[U61] PHP：正则
来源：http://lk.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ns.9csxet.cn

[U62] PHP：日期对象
来源：http://cn.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fb.nicolike.cn

[U63] PHP：文件读写
来源：http://ww.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nc.szxytkj.cn

[U64] PHP：目录遍历
来源：http://eh.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://wg.yuexingan06.cn

[U65] PHP：会话
来源：http://ci.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xt.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://le.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pp.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://yd.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cr.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://de.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ys.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://es.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iv.nszjky.cn

[U70] PHP：PDO 事务
来源：http://cf.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dc.hnjuh.cn

[U71] PHP：抛出异常
来源：http://cn.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://dp.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://av.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://ux.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://yx.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://wi.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://kc.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://fh.9csxet.cn

[U75] PHP：依赖注入
来源：http://qd.wgjwhj.cn

composer require psr/container
来源：http://of.szsharing.cn

[U76] PHP：简单路由
来源：http://fw.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ps.gzmigu.cn

[U77] PHP：模板渲染
来源：http://zd.haigaiapp.cn

composer require twig/twig
来源：http://qv.muxihuayi.cn

[U78] PHP：单元测试
来源：http://iu.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://ao.nicolike.cn

[U79] PHP：静态分析
来源：http://hn.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://na.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://vx.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ig.nszjky.cn

[U81] JS：初始化项目
来源：http://zs.hahajie.cn

npm init -y;  npm i express
来源：http://bn.hahajie.cn

[U82] JS：package.json 脚本
来源：http://uk.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dl.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://cu.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ay.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://av.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lk.jctech888.com.cn


<!-- 参考信息 -->