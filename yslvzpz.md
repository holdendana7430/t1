代发 wailian999

[T01] Kotlin：Hello World
来源：http://yc.szsharing.cn

println("Hello")
来源：http://fa.nszjky.cn

[T02] Kotlin：变量
来源：http://gi.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ff.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://zz.huixiangedu.cn

"值: $b"
来源：http://za.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://ao.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://mc.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://de.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qh.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://oi.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jt.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://mv.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ix.hahajie.cn

[T08] Kotlin：数据类
来源：http://wb.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://bj.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://ne.asd995.cn

fun String.exclaim() = this + "!"
来源：http://tf.colortex.cn

[T10] Kotlin：默认参数
来源：http://ne.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://so.huanxung.cn

[T11] Kotlin：协程
来源：http://jg.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://go.nszjky.cn

[T12] Kotlin：解构声明
来源：http://qo.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://es.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://se.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://su.asd995.cn

[T14] Kotlin：循环
来源：http://nr.newstarts.cn

for (i in 1..10) println(i)
来源：http://ey.nszjky.cn

[T15] Kotlin：接口
来源：http://lr.newstarts.cn

interface Shape { fun area(): Double }
来源：http://co.jctech888.com.cn

[T16] Swift：Hello World
来源：http://dk.521024.cn

print("Hello")
来源：http://ho.521024.cn

[T17] Swift：变量与常量
来源：http://oj.haigaiapp.cn

var a = 1;  let b = 2
来源：http://yx.nszjky.cn

[T18] Swift：字符串插值
来源：http://dd.hahajie.cn

"值: \(b)"
来源：http://cg.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://kx.yuexingan06.cn

if let n = opt { print(n) }
来源：http://kt.gzmigu.cn

[T20] Swift：数组操作
来源：http://cn.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iz.huixiangedu.cn

[T21] Swift：遍历
来源：http://sq.shxzskj.cn

for x in a { print(x) }
来源：http://ig.bookmarksfly.cn

[T22] Swift：字典
来源：http://dt.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tg.nicolike.cn

[T23] Swift：函数
来源：http://ss.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ng.yuexingan06.cn

[T24] Swift：闭包
来源：http://wf.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mr.wgjwhj.cn

[T25] Swift：结构体
来源：http://uu.bookmarksfly.cn

struct P { var x: Int }
来源：http://rh.asd995.cn

[T26] Swift：类与重写
来源：http://zn.asd995.cn

class A: Base { override func f() {} }
来源：http://fe.szsharing.cn

[T27] Swift：错误处理
来源：http://bf.hahajie.cn

do { try f() } catch { print(error) }
来源：http://vt.bjjhwx.cn

[T28] Swift：枚举
来源：http://az.nicolike.cn

enum Color { case red, green }
来源：http://xn.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://xt.shxzukj.cn

guard let x = opt else { return }
来源：http://sz.hahajie.cn

[T30] Swift：协议
来源：http://es.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://pe.9csxet.cn

[T31] Lua：Hello World
来源：http://bf.shxzskj.cn

print("Hello")
来源：http://rf.muxihuayi.cn

[T32] Lua：局部变量
来源：http://cy.521024.cn

local a = 1
来源：http://bm.lnxyls.cn

[T33] Lua：表（数组）
来源：http://fe.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gc.wgjwhj.cn

[T34] Lua：遍历表
来源：http://zl.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ps.9csxet.cn

[T35] Lua：字典表
来源：http://gi.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://uw.panjiajie.cn

[T36] Lua：函数
来源：http://mn.asd995.cn

function add(a, b) return a + b end
来源：http://om.newstarts.cn

[T37] Lua：字符串拼接
来源：http://yt.521024.cn

"a" .. "b"
来源：http://an.haigaiapp.cn

[T38] Lua：条件
来源：http://ur.jctech888.com.cn

if x > 0 then print("正") end
来源：http://qo.panjiajie.cn

[T39] Lua：模式匹配
来源：http://fv.newstarts.cn

string.find(s, "%d+")
来源：http://kb.shxzukj.cn

[T40] Lua：元表
来源：http://vr.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://bq.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://kp.newstarts.cn

print "Hello\n";
来源：http://ab.lnxyls.cn

[T42] Perl：变量类型
来源：http://gy.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rt.hnjuh.cn

[T43] Perl：字符串插值
来源：http://zk.nicolike.cn

"值: $a"
来源：http://dk.newstarts.cn

[T44] Perl：条件
来源：http://uv.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://mv.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://yu.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://gc.szsharing.cn

[T46] Perl：哈希操作
来源：http://ud.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ep.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://sq.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ss.shtwfgs.cn

[T48] Perl：正则替换
来源：http://go.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://bt.huanxung.cn

[T49] Perl：函数
来源：http://hm.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lt.9csxet.cn

[T50] Perl：逐行读文件
来源：http://us.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tz.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://pe.bjjhwx.cn

[T51] Scala：Hello World
来源：http://rt.huixinmuqiang.cn

println("Hello")
来源：http://rg.shxzskj.cn

[T52] Scala：变量
来源：http://ti.wgjwhj.cn

val a = 1;  var b = 2
来源：http://af.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://fe.chemitech.net.cn

s"值: $b"
来源：http://dv.9csxet.cn

[T54] Scala：集合映射
来源：http://qj.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://od.huanxung.cn

[T55] Scala：集合过滤
来源：http://vc.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ck.huanxung.cn

[T56] Scala：样例类
来源：http://jx.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://xt.newstarts.cn

[T57] Scala：模式匹配
来源：http://vg.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ck.asd995.cn

[T58] Scala：函数定义
来源：http://mb.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://no.hahajie.cn

[T59] Scala：循环
来源：http://zn.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://oq.hnjuh.cn

[T60] Scala：折叠
来源：http://sd.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cq.hnjuh.cn

================================================================================
来源：http://xa.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nc.huanxung.cn

================================================================================
来源：http://sy.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://eh.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ds.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ao.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ja.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://pu.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mh.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://mo.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://st.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://gz.nicolike.cn

list(dict.fromkeys(arr))
来源：http://ob.gzmigu.cn

[U06] Py：合并两个字典
来源：http://fq.nszjky.cn

{**a, **b}
来源：http://al.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://cs.hahajie.cn

{v: k for k, v in d.items()}
来源：http://hp.hnjuh.cn

[U08] Py：展平二维列表
来源：http://rg.chemitech.net.cn

[y for x in nested for y in x]
来源：http://pp.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://zn.lnxyls.cn

max(d, key=d.get)
来源：http://do.hnjuh.cn

[U10] Py：按值排序字典
来源：http://po.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ns.shxzskj.cn

[U11] Py：生成器表达式
来源：http://vc.muxihuayi.cn

(x * 2 for x in arr)
来源：http://dh.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xk.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://bp.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://zb.chemitech.net.cn

deque(maxlen=10)
来源：http://ru.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://sv.colortex.cn

defaultdict(list)
来源：http://hd.yuexingan06.cn

[U15] Py：高精度计时
来源：http://ol.yuexingan06.cn

t = time.perf_counter()
来源：http://nq.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://zq.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cx.hahajie.cn

[U17] Py：初始化日志
来源：http://jk.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tt.bjjhwx.cn

[U18] Py：预编译正则
来源：http://qv.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://jf.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://pn.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zx.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://gj.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://dv.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://tl.521024.cn

@contextlib.contextmanager
来源：http://iw.shxzukj.cn

[U22] Py：矩阵转置
来源：http://uu.shxzukj.cn

list(zip(*m))
来源：http://ao.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://bw.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ot.haigaiapp.cn

[U24] Py：路径操作
来源：http://wf.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nk.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://oe.yuntaijiaju.cn

csv.DictReader(f)
来源：http://es.hnjuh.cn

[U26] Py：并发下载
来源：http://xv.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qt.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://jg.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://hd.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://zp.szxytkj.cn

UserId = int
来源：http://ki.shxzskj.cn

[U29] Py：属性校验
来源：http://kz.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://om.521024.cn

[U30] Py：数据类
来源：http://od.panjiajie.cn

@dataclass(slots=True)
来源：http://km.hahajie.cn

[U31] Py：单测
来源：http://gq.nicolike.cn

python -m pytest -q
来源：http://ai.panjiajie.cn

[U32] Py：代码格式化
来源：http://bx.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://ht.huixiangedu.cn

[U33] Py：打包发布
来源：http://ar.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://sa.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://pw.szsharing.cn

chardet.detect(raw)
来源：http://vg.panjiajie.cn

[U35] Py：发送邮件
来源：http://ex.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ty.wgjwhj.cn

[U36] Py：定时任务
来源：http://mq.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://of.asd995.cn

[U37] Py：读写 Excel
来源：http://rc.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://un.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://fg.nicolike.cn

Path(__file__).resolve().parent
来源：http://hq.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://ob.newstarts.cn

sys.stdout.isatty()
来源：http://ce.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://wp.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://iq.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://pl.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wo.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://za.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rs.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://wf.asd995.cn

namespace App\Http;
来源：http://mh.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://wu.jctech888.com.cn

declare(strict_types=1);
来源：http://qq.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://ij.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lv.hahajie.cn

[U46] PHP：可空类型
来源：http://fw.huixinmuqiang.cn

?string $name = null
来源：http://eb.shtwfgs.cn

[U47] PHP：联合类型
来源：http://qn.bjjhwx.cn

int|string $id
来源：http://sx.shxzukj.cn

[U48] PHP：纯枚举
来源：http://xd.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dm.hnjuh.cn

[U49] PHP：只读属性
来源：http://wr.newstarts.cn

public readonly string $name
来源：http://id.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://qm.huanxung.cn

public function __construct(private int $id) {}
来源：http://tg.panjiajie.cn

[U51] PHP：数组解构
来源：http://io.huixiangedu.cn

[$a, $b] = $arr;
来源：http://py.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://ok.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://fy.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://aq.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://xx.szxytkj.cn

[U54] PHP：空安全调用
来源：http://sj.nszjky.cn

$obj?->method()
来源：http://vi.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://mo.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://md.colortex.cn

[U56] PHP：命名参数
来源：http://ko.muxihuayi.cn

f(a: 1, b: 2)
来源：http://gl.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://kq.9csxet.cn

"值: {$a}"
来源：http://nm.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://od.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pj.lnxyls.cn

[U59] PHP：自定义排序
来源：http://mv.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rk.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://yi.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lf.hahajie.cn

[U61] PHP：正则
来源：http://vo.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nx.newstarts.cn

[U62] PHP：日期对象
来源：http://hk.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zv.asd995.cn

[U63] PHP：文件读写
来源：http://gn.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dg.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://vi.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://pc.hnjuh.cn

[U65] PHP：会话
来源：http://ce.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pf.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://vk.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qo.nszjky.cn

[U67] PHP：处理文件上传
来源：http://ui.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cp.huanxung.cn

[U68] PHP：PDO 连接
来源：http://rl.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kn.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://bd.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ma.asd995.cn

[U70] PHP：PDO 事务
来源：http://kn.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uo.shxzskj.cn

[U71] PHP：抛出异常
来源：http://hn.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://hc.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://th.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://sh.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://nk.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://rb.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://vi.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://id.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://pq.521024.cn

composer require psr/container
来源：http://jy.nszjky.cn

[U76] PHP：简单路由
来源：http://jx.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://up.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://bs.hahajie.cn

composer require twig/twig
来源：http://vw.haigaiapp.cn

[U78] PHP：单元测试
来源：http://lc.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://zx.jctech888.com.cn

[U79] PHP：静态分析
来源：http://vp.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://df.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://hi.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ce.huixiangedu.cn

[U81] JS：初始化项目
来源：http://md.lnxyls.cn

npm init -y;  npm i express
来源：http://uk.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://ia.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://da.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://zc.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://if.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://sx.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hy.colortex.cn

[U85] JS：可选链
来源：http://qd.wgjwhj.cn

a?.b?.c
来源：http://jd.huanxung.cn

[U86] JS：空值合并
来源：http://cz.gzmigu.cn

a ?? b
来源：http://bx.szsharing.cn

[U87] JS：解构默认值
来源：http://mh.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://vx.newstarts.cn

[U88] JS：对象展开合并
来源：http://gk.jctech888.com.cn

{ ...a, ...b }
来源：http://vd.huixinmuqiang.cn


<!-- 参考信息 -->