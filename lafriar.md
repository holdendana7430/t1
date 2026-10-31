代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rr.shxzskj.cn

================================================================================
来源：http://jl.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xb.shtwfgs.cn

================================================================================
来源：http://ft.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://pn.shxzukj.cn

println("Hello")
来源：http://kk.colortex.cn

[T02] Kotlin：变量
来源：http://rm.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://po.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://fk.nszjky.cn

"值: $b"
来源：http://da.szxytkj.cn

[T04] Kotlin：空安全
来源：http://sm.shxzskj.cn

val n: String? = null;  n?.length
来源：http://rb.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://wc.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ts.colortex.cn

[T06] Kotlin：集合映射
来源：http://nt.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://af.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://fq.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sc.hnjuh.cn

[T08] Kotlin：数据类
来源：http://uw.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://bd.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://is.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ob.szsharing.cn

[T10] Kotlin：默认参数
来源：http://py.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xx.hnjuh.cn

[T11] Kotlin：协程
来源：http://er.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://li.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://ux.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://rc.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://bl.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://it.panjiajie.cn

[T14] Kotlin：循环
来源：http://hj.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://si.asd995.cn

[T15] Kotlin：接口
来源：http://rl.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://eb.asd995.cn

[T16] Swift：Hello World
来源：http://vn.huixiangedu.cn

print("Hello")
来源：http://pe.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ni.hahajie.cn

var a = 1;  let b = 2
来源：http://ze.asd995.cn

[T18] Swift：字符串插值
来源：http://vu.szxytkj.cn

"值: \(b)"
来源：http://xn.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://jf.szxytkj.cn

if let n = opt { print(n) }
来源：http://py.asd995.cn

[T20] Swift：数组操作
来源：http://ua.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ud.bjjhwx.cn

[T21] Swift：遍历
来源：http://fa.shtwfgs.cn

for x in a { print(x) }
来源：http://pk.bjjhwx.cn

[T22] Swift：字典
来源：http://qq.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ov.hnjuh.cn

[T23] Swift：函数
来源：http://fm.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ao.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://kw.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ck.wgjwhj.cn

[T25] Swift：结构体
来源：http://qd.nicolike.cn

struct P { var x: Int }
来源：http://jb.nicolike.cn

[T26] Swift：类与重写
来源：http://lq.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://fh.asd995.cn

[T27] Swift：错误处理
来源：http://fb.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://st.huanxung.cn

[T28] Swift：枚举
来源：http://wi.wgjwhj.cn

enum Color { case red, green }
来源：http://ye.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://le.colortex.cn

guard let x = opt else { return }
来源：http://ku.hahajie.cn

[T30] Swift：协议
来源：http://wy.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://gt.shxzukj.cn

[T31] Lua：Hello World
来源：http://ly.bookmarksfly.cn

print("Hello")
来源：http://wz.haigaiapp.cn

[T32] Lua：局部变量
来源：http://mj.yuexingan06.cn

local a = 1
来源：http://wt.asd995.cn

[T33] Lua：表（数组）
来源：http://pb.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oo.muxihuayi.cn

[T34] Lua：遍历表
来源：http://px.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wz.521024.cn

[T35] Lua：字典表
来源：http://kw.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://on.bookmarksfly.cn

[T36] Lua：函数
来源：http://yb.shxzukj.cn

function add(a, b) return a + b end
来源：http://dp.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://xt.bjjhwx.cn

"a" .. "b"
来源：http://un.jctech888.com.cn

[T38] Lua：条件
来源：http://ku.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://jx.hahajie.cn

[T39] Lua：模式匹配
来源：http://fm.szsharing.cn

string.find(s, "%d+")
来源：http://hq.hnjuh.cn

[T40] Lua：元表
来源：http://tw.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ns.newstarts.cn

[T41] Perl：Hello World
来源：http://um.nszjky.cn

print "Hello\n";
来源：http://ht.panjiajie.cn

[T42] Perl：变量类型
来源：http://jp.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ud.szxytkj.cn

[T43] Perl：字符串插值
来源：http://kh.lnxyls.cn

"值: $a"
来源：http://gv.huixinmuqiang.cn

[T44] Perl：条件
来源：http://vp.asd995.cn

if ($a > 0) { print "正"; }
来源：http://kr.gzmigu.cn

[T45] Perl：数组遍历
来源：http://ev.colortex.cn

for my $x (@arr) { print $x; }
来源：http://oj.hnjuh.cn

[T46] Perl：哈希操作
来源：http://ib.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fv.szsharing.cn

[T47] Perl：正则捕获
来源：http://ue.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://br.shxzukj.cn

[T48] Perl：正则替换
来源：http://jg.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://to.bjjhwx.cn

[T49] Perl：函数
来源：http://se.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://op.521024.cn

[T50] Perl：逐行读文件
来源：http://xw.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qk.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://md.bjjhwx.cn

[T51] Scala：Hello World
来源：http://xv.chemitech.net.cn

println("Hello")
来源：http://ha.shtwfgs.cn

[T52] Scala：变量
来源：http://ou.gzmigu.cn

val a = 1;  var b = 2
来源：http://lw.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://ib.gzmigu.cn

s"值: $b"
来源：http://ph.colortex.cn

[T54] Scala：集合映射
来源：http://qc.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://lu.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://ys.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tj.nicolike.cn

[T56] Scala：样例类
来源：http://hg.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://fr.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://ro.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://av.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://om.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zl.bookmarksfly.cn

[T59] Scala：循环
来源：http://yf.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://mg.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://cx.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fn.shtwfgs.cn

================================================================================
来源：http://zt.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qm.szsharing.cn

================================================================================
来源：http://pf.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://vn.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wb.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://pr.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ok.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://mr.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uz.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://vg.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sz.huanxung.cn

[U05] Py：列表去重且保序
来源：http://yg.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://id.nszjky.cn

[U06] Py：合并两个字典
来源：http://cw.lnxyls.cn

{**a, **b}
来源：http://dw.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ew.szsharing.cn

{v: k for k, v in d.items()}
来源：http://st.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://ag.yuexingan06.cn

[y for x in nested for y in x]
来源：http://ka.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://yn.newstarts.cn

max(d, key=d.get)
来源：http://ns.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://ia.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qt.shxzskj.cn

[U11] Py：生成器表达式
来源：http://hh.jctech888.com.cn

(x * 2 for x in arr)
来源：http://ib.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fa.hahajie.cn

Counter(arr).most_common(3)
来源：http://kt.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://lh.asd995.cn

deque(maxlen=10)
来源：http://ej.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://iz.huanxung.cn

defaultdict(list)
来源：http://rs.szsharing.cn

[U15] Py：高精度计时
来源：http://ny.muxihuayi.cn

t = time.perf_counter()
来源：http://ck.nicolike.cn

[U16] Py：命令行参数解析
来源：http://pg.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pq.hnjuh.cn

[U17] Py：初始化日志
来源：http://lw.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://qz.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://hg.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://gq.huanxung.cn

[U19] Py：正则替换带回调
来源：http://fg.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oy.521024.cn

[U20] Py：缓存函数结果
来源：http://ru.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://ky.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://or.szxytkj.cn

@contextlib.contextmanager
来源：http://qc.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://tm.jctech888.com.cn

list(zip(*m))
来源：http://yv.asd995.cn

[U23] Py：分块读取大文件
来源：http://ba.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qb.wgjwhj.cn

[U24] Py：路径操作
来源：http://dc.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zu.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://ru.muxihuayi.cn

csv.DictReader(f)
来源：http://nb.wgjwhj.cn

[U26] Py：并发下载
来源：http://qv.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cn.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://kk.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://rk.shxzukj.cn

[U28] Py：类型别名
来源：http://jm.szsharing.cn

UserId = int
来源：http://fa.gzmigu.cn

[U29] Py：属性校验
来源：http://yz.gzmigu.cn

@property 与 @x.setter 配合
来源：http://ag.haigaiapp.cn

[U30] Py：数据类
来源：http://gt.yuexingan06.cn

@dataclass(slots=True)
来源：http://tg.muxihuayi.cn

[U31] Py：单测
来源：http://lw.asd995.cn

python -m pytest -q
来源：http://gy.9csxet.cn

[U32] Py：代码格式化
来源：http://gz.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://pa.hahajie.cn

[U33] Py：打包发布
来源：http://hd.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://br.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://rt.muxihuayi.cn

chardet.detect(raw)
来源：http://un.muxihuayi.cn

[U35] Py：发送邮件
来源：http://po.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ms.nicolike.cn

[U36] Py：定时任务
来源：http://gq.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://ct.newstarts.cn

[U37] Py：读写 Excel
来源：http://tt.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ww.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://ld.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://ec.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://ht.gzmigu.cn

sys.stdout.isatty()
来源：http://jw.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://gn.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://be.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://rg.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hb.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://ii.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sg.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://wp.newstarts.cn

namespace App\Http;
来源：http://iw.9csxet.cn

[U44] PHP：开启严格类型
来源：http://jw.gzmigu.cn

declare(strict_types=1);
来源：http://cq.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://dr.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xi.chemitech.net.cn

[U46] PHP：可空类型
来源：http://of.huanxung.cn

?string $name = null
来源：http://uf.panjiajie.cn

[U47] PHP：联合类型
来源：http://tm.huixiangedu.cn

int|string $id
来源：http://xs.9csxet.cn

[U48] PHP：纯枚举
来源：http://jg.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bc.asd995.cn

[U49] PHP：只读属性
来源：http://dh.hahajie.cn

public readonly string $name
来源：http://yi.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://oj.szxytkj.cn

public function __construct(private int $id) {}
来源：http://go.muxihuayi.cn

[U51] PHP：数组解构
来源：http://xv.yuexingan06.cn

[$a, $b] = $arr;
来源：http://os.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://bz.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://jc.huanxung.cn

[U53] PHP：空合并运算符
来源：http://ts.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://kq.huanxung.cn

[U54] PHP：空安全调用
来源：http://bf.jianghongdianzi.cn

$obj?->method()
来源：http://mm.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://fn.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://to.asd995.cn

[U56] PHP：命名参数
来源：http://ze.9csxet.cn

f(a: 1, b: 2)
来源：http://ib.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ny.gzmigu.cn

"值: {$a}"
来源：http://hx.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ha.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qn.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://tz.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vm.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://th.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ic.jctech888.com.cn

[U61] PHP：正则
来源：http://be.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hj.nicolike.cn

[U62] PHP：日期对象
来源：http://xu.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qk.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ue.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nc.asd995.cn

[U64] PHP：目录遍历
来源：http://qk.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://jp.yuntaijiaju.cn

[U65] PHP：会话
来源：http://xq.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qp.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://ng.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://op.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://yo.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ww.nicolike.cn

[U68] PHP：PDO 连接
来源：http://vr.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jy.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://zu.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ds.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ym.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rq.hahajie.cn

[U71] PHP：抛出异常
来源：http://vp.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://ez.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://td.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ff.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://zz.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://fl.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://nn.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://tf.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://zq.nszjky.cn

composer require psr/container
来源：http://hx.muxihuayi.cn

[U76] PHP：简单路由
来源：http://bb.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xk.panjiajie.cn

[U77] PHP：模板渲染
来源：http://ov.colortex.cn

composer require twig/twig
来源：http://mn.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://ed.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ya.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ac.colortex.cn

composer require --dev phpstan/phpstan
来源：http://ul.nicolike.cn

[U80] PHP：代码规范修复
来源：http://us.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lg.yuexingan06.cn

[U81] JS：初始化项目
来源：http://mg.shxzskj.cn

npm init -y;  npm i express
来源：http://fs.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://ny.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pt.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://mr.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://je.521024.cn

[U84] JS：CommonJS 写法
来源：http://dd.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ln.hahajie.cn

[U85] JS：可选链
来源：http://xv.yuntaijiaju.cn

a?.b?.c
来源：http://ls.521024.cn

[U86] JS：空值合并
来源：http://gd.muxihuayi.cn

a ?? b
来源：http://pw.newstarts.cn


<!-- 参考信息 -->