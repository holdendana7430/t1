代发 wailian999

[T05] Kotlin：when 表达式
来源：http://oc.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pq.nszjky.cn

[T06] Kotlin：集合映射
来源：http://xm.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ea.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://zm.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qa.asd995.cn

[T08] Kotlin：数据类
来源：http://yi.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://dl.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://mx.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://jb.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://by.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vq.shtwfgs.cn

[T11] Kotlin：协程
来源：http://nu.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dt.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ji.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://bo.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://wj.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://dl.nicolike.cn

[T14] Kotlin：循环
来源：http://dr.nszjky.cn

for (i in 1..10) println(i)
来源：http://re.colortex.cn

[T15] Kotlin：接口
来源：http://yz.nszjky.cn

interface Shape { fun area(): Double }
来源：http://bi.wgjwhj.cn

[T16] Swift：Hello World
来源：http://jc.huixiangedu.cn

print("Hello")
来源：http://tf.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://qg.9csxet.cn

var a = 1;  let b = 2
来源：http://jc.521024.cn

[T18] Swift：字符串插值
来源：http://sq.hnjuh.cn

"值: \(b)"
来源：http://hm.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ai.huixiangedu.cn

if let n = opt { print(n) }
来源：http://co.huixiangedu.cn

[T20] Swift：数组操作
来源：http://aa.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ac.newstarts.cn

[T21] Swift：遍历
来源：http://hs.hnjuh.cn

for x in a { print(x) }
来源：http://zm.szsharing.cn

[T22] Swift：字典
来源：http://qz.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zg.hnjuh.cn

[T23] Swift：函数
来源：http://pv.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cw.nicolike.cn

[T24] Swift：闭包
来源：http://nw.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vp.521024.cn

[T25] Swift：结构体
来源：http://fd.szxytkj.cn

struct P { var x: Int }
来源：http://ez.jctech888.com.cn

[T26] Swift：类与重写
来源：http://qu.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ht.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://nt.asd995.cn

do { try f() } catch { print(error) }
来源：http://nq.bookmarksfly.cn

[T28] Swift：枚举
来源：http://ur.szsharing.cn

enum Color { case red, green }
来源：http://vb.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://sf.huanxung.cn

guard let x = opt else { return }
来源：http://rs.bookmarksfly.cn

[T30] Swift：协议
来源：http://gr.colortex.cn

protocol Shape { func area() -> Double }
来源：http://gh.huixiangedu.cn

[T31] Lua：Hello World
来源：http://zy.bookmarksfly.cn

print("Hello")
来源：http://rl.haigaiapp.cn

[T32] Lua：局部变量
来源：http://on.bookmarksfly.cn

local a = 1
来源：http://nf.9csxet.cn

[T33] Lua：表（数组）
来源：http://ye.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nt.colortex.cn

[T34] Lua：遍历表
来源：http://gv.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://so.bookmarksfly.cn

[T35] Lua：字典表
来源：http://yp.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://th.shtwfgs.cn

[T36] Lua：函数
来源：http://xy.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://cq.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://wt.haigaiapp.cn

"a" .. "b"
来源：http://wg.panjiajie.cn

[T38] Lua：条件
来源：http://lm.muxihuayi.cn

if x > 0 then print("正") end
来源：http://jn.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://gp.521024.cn

string.find(s, "%d+")
来源：http://jb.gzmigu.cn

[T40] Lua：元表
来源：http://fw.hahajie.cn

setmetatable({}, { __index = base })
来源：http://xf.bjjhwx.cn

[T41] Perl：Hello World
来源：http://xa.shxzukj.cn

print "Hello\n";
来源：http://fu.shtwfgs.cn

[T42] Perl：变量类型
来源：http://pf.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nt.szxytkj.cn

[T43] Perl：字符串插值
来源：http://wi.colortex.cn

"值: $a"
来源：http://oc.bjjhwx.cn

[T44] Perl：条件
来源：http://kz.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://bq.szxytkj.cn

[T45] Perl：数组遍历
来源：http://wg.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://dm.521024.cn

[T46] Perl：哈希操作
来源：http://ky.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rb.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://hh.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zc.muxihuayi.cn

[T48] Perl：正则替换
来源：http://yi.szxytkj.cn

$s =~ s/old/new/g;
来源：http://rw.asd995.cn

[T49] Perl：函数
来源：http://rh.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zg.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://bt.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mv.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://oi.huixiangedu.cn

[T51] Scala：Hello World
来源：http://eg.panjiajie.cn

println("Hello")
来源：http://zs.newstarts.cn

[T52] Scala：变量
来源：http://bs.521024.cn

val a = 1;  var b = 2
来源：http://fn.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://wn.hnjuh.cn

s"值: $b"
来源：http://pd.szsharing.cn

[T54] Scala：集合映射
来源：http://us.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://hi.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://pd.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bn.9csxet.cn

[T56] Scala：样例类
来源：http://cw.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://nc.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://as.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ad.hnjuh.cn

[T58] Scala：函数定义
来源：http://dw.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nq.yuntaijiaju.cn

[T59] Scala：循环
来源：http://tc.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://vi.szsharing.cn

[T60] Scala：折叠
来源：http://yk.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jd.jianghongdianzi.cn

================================================================================
来源：http://on.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://is.gzmigu.cn

================================================================================
来源：http://tv.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://cb.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oj.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://gr.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qi.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://zf.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://od.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://ca.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://id.colortex.cn

[U05] Py：列表去重且保序
来源：http://vj.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://sz.huanxung.cn

[U06] Py：合并两个字典
来源：http://dy.shxzukj.cn

{**a, **b}
来源：http://gk.9csxet.cn

[U07] Py：反转字典键值
来源：http://yg.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://xk.gzmigu.cn

[U08] Py：展平二维列表
来源：http://js.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ip.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://xr.huanxung.cn

max(d, key=d.get)
来源：http://my.panjiajie.cn

[U10] Py：按值排序字典
来源：http://xg.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rq.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://oe.chemitech.net.cn

(x * 2 for x in arr)
来源：http://df.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zf.lnxyls.cn

Counter(arr).most_common(3)
来源：http://qs.nszjky.cn

[U13] Py：固定长度队列
来源：http://hm.9csxet.cn

deque(maxlen=10)
来源：http://hg.asd995.cn

[U14] Py：分组收集到列表
来源：http://xl.colortex.cn

defaultdict(list)
来源：http://qi.huanxung.cn

[U15] Py：高精度计时
来源：http://fe.szsharing.cn

t = time.perf_counter()
来源：http://tm.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://lv.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fh.shxzskj.cn

[U17] Py：初始化日志
来源：http://sj.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://ih.panjiajie.cn

[U18] Py：预编译正则
来源：http://cn.521024.cn

pat = re.compile(r"\d+")
来源：http://hq.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://rr.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nc.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://wg.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://pb.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://oc.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://zx.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://nv.shtwfgs.cn

list(zip(*m))
来源：http://of.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://tm.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xb.colortex.cn

[U24] Py：路径操作
来源：http://ib.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dn.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ms.asd995.cn

csv.DictReader(f)
来源：http://vd.521024.cn

[U26] Py：并发下载
来源：http://kh.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ui.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://jw.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://eg.nszjky.cn

[U28] Py：类型别名
来源：http://le.gzmigu.cn

UserId = int
来源：http://fu.bjjhwx.cn

[U29] Py：属性校验
来源：http://sp.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://oj.huanxung.cn

[U30] Py：数据类
来源：http://ru.521024.cn

@dataclass(slots=True)
来源：http://eq.chemitech.net.cn

[U31] Py：单测
来源：http://iq.szsharing.cn

python -m pytest -q
来源：http://eq.bjjhwx.cn

[U32] Py：代码格式化
来源：http://ok.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://xg.szsharing.cn

[U33] Py：打包发布
来源：http://he.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ml.bjjhwx.cn

[U34] Py：判断编码
来源：http://px.panjiajie.cn

chardet.detect(raw)
来源：http://gv.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ei.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sb.chemitech.net.cn

[U36] Py：定时任务
来源：http://ks.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://py.9csxet.cn

[U37] Py：读写 Excel
来源：http://cp.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yk.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://do.huanxung.cn

Path(__file__).resolve().parent
来源：http://dz.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://or.huanxung.cn

sys.stdout.isatty()
来源：http://fy.huanxung.cn

[U40] Py：打印到标准错误
来源：http://aw.shxzskj.cn

print("err", file=sys.stderr)
来源：http://sm.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://nj.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sb.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://cx.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tu.huanxung.cn

[U43] PHP：声明命名空间
来源：http://be.shxzukj.cn

namespace App\Http;
来源：http://xd.nicolike.cn

[U44] PHP：开启严格类型
来源：http://tm.panjiajie.cn

declare(strict_types=1);
来源：http://ip.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://pm.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hj.521024.cn

[U46] PHP：可空类型
来源：http://nz.yuntaijiaju.cn

?string $name = null
来源：http://wb.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://wr.shxzukj.cn

int|string $id
来源：http://je.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://es.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kq.jctech888.com.cn

[U49] PHP：只读属性
来源：http://lx.yuexingan06.cn

public readonly string $name
来源：http://em.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://rh.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://ea.szxytkj.cn

[U51] PHP：数组解构
来源：http://zz.jctech888.com.cn

[$a, $b] = $arr;
来源：http://hb.lnxyls.cn

[U52] PHP：箭头函数
来源：http://fb.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://kv.hahajie.cn

[U53] PHP：空合并运算符
来源：http://gb.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://pj.szxytkj.cn

[U54] PHP：空安全调用
来源：http://hc.hahajie.cn

$obj?->method()
来源：http://cz.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ow.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bk.shxzukj.cn

[U56] PHP：命名参数
来源：http://dx.panjiajie.cn

f(a: 1, b: 2)
来源：http://ye.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://fp.hnjuh.cn

"值: {$a}"
来源：http://qk.521024.cn

[U58] PHP：数组三件套
来源：http://jk.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tc.nicolike.cn

[U59] PHP：自定义排序
来源：http://gp.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tr.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://nq.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yp.haigaiapp.cn

[U61] PHP：正则
来源：http://fp.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vn.shxzukj.cn

[U62] PHP：日期对象
来源：http://zr.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vy.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://mg.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dc.521024.cn

[U64] PHP：目录遍历
来源：http://ls.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://sp.shxzskj.cn

[U65] PHP：会话
来源：http://sk.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ml.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://ut.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://he.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://ua.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ig.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://qz.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gp.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://px.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cy.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://im.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://js.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ff.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ej.huanxung.cn

[U72] PHP：写错误日志
来源：http://gc.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://oy.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://yz.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://lu.huanxung.cn

[U74] PHP：读取环境变量
来源：http://rj.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://jv.panjiajie.cn

[U75] PHP：依赖注入
来源：http://ww.yuexingan06.cn

composer require psr/container
来源：http://yo.nicolike.cn

[U76] PHP：简单路由
来源：http://ys.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zf.lnxyls.cn

[U77] PHP：模板渲染
来源：http://vs.haigaiapp.cn

composer require twig/twig
来源：http://wr.yuexingan06.cn

[U78] PHP：单元测试
来源：http://gn.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://hr.hahajie.cn

[U79] PHP：静态分析
来源：http://ne.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://ii.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://mq.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ip.gzmigu.cn

[U81] JS：初始化项目
来源：http://jy.szsharing.cn

npm init -y;  npm i express
来源：http://sx.huanxung.cn

[U82] JS：package.json 脚本
来源：http://ko.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://as.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://fg.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hp.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://yk.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dg.bookmarksfly.cn

[U85] JS：可选链
来源：http://oz.wgjwhj.cn

a?.b?.c
来源：http://qm.colortex.cn

[U86] JS：空值合并
来源：http://ps.521024.cn

a ?? b
来源：http://em.huanxung.cn

[U87] JS：解构默认值
来源：http://bd.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://mo.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://zi.wgjwhj.cn

{ ...a, ...b }
来源：http://ti.9csxet.cn

[U89] JS：数组去重
来源：http://up.asd995.cn

[...new Set(arr)]
来源：http://up.nicolike.cn

[U90] JS：数字数组排序
来源：http://hh.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://ao.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://us.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zh.muxihuayi.cn

[U92] JS：深拷贝
来源：http://no.colortex.cn

structuredClone(obj)
来源：http://ny.panjiajie.cn


<!-- 参考信息 -->