代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ix.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://of.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://pn.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gt.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://jo.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://os.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://wu.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://xo.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://hl.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://xt.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://dy.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://of.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ss.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ah.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://ki.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://qj.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://ci.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://vi.521024.cn

[T14] Kotlin：循环
来源：http://up.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://az.haigaiapp.cn

[T15] Kotlin：接口
来源：http://rx.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://ao.szxytkj.cn

[T16] Swift：Hello World
来源：http://jm.colortex.cn

print("Hello")
来源：http://lz.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://qw.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://yy.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://is.9csxet.cn

"值: \(b)"
来源：http://no.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://nd.shxzukj.cn

if let n = opt { print(n) }
来源：http://aq.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ri.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hm.shxzukj.cn

[T21] Swift：遍历
来源：http://li.haigaiapp.cn

for x in a { print(x) }
来源：http://nu.panjiajie.cn

[T22] Swift：字典
来源：http://to.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jz.colortex.cn

[T23] Swift：函数
来源：http://md.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oz.9csxet.cn

[T24] Swift：闭包
来源：http://oy.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lq.hnjuh.cn

[T25] Swift：结构体
来源：http://ff.newstarts.cn

struct P { var x: Int }
来源：http://bd.huanxung.cn

[T26] Swift：类与重写
来源：http://qv.521024.cn

class A: Base { override func f() {} }
来源：http://nk.shxzukj.cn

[T27] Swift：错误处理
来源：http://pz.huanxung.cn

do { try f() } catch { print(error) }
来源：http://dw.huixiangedu.cn

[T28] Swift：枚举
来源：http://tr.chemitech.net.cn

enum Color { case red, green }
来源：http://sb.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://ha.panjiajie.cn

guard let x = opt else { return }
来源：http://st.szsharing.cn

[T30] Swift：协议
来源：http://yt.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://on.colortex.cn

[T31] Lua：Hello World
来源：http://qi.nicolike.cn

print("Hello")
来源：http://yu.huanxung.cn

[T32] Lua：局部变量
来源：http://vd.newstarts.cn

local a = 1
来源：http://zz.9csxet.cn

[T33] Lua：表（数组）
来源：http://cj.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://im.nicolike.cn

[T34] Lua：遍历表
来源：http://fw.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yl.wgjwhj.cn

[T35] Lua：字典表
来源：http://ps.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://as.lnxyls.cn

[T36] Lua：函数
来源：http://oe.asd995.cn

function add(a, b) return a + b end
来源：http://yu.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://cm.muxihuayi.cn

"a" .. "b"
来源：http://df.nicolike.cn

[T38] Lua：条件
来源：http://nk.newstarts.cn

if x > 0 then print("正") end
来源：http://ne.hnjuh.cn

[T39] Lua：模式匹配
来源：http://zz.yuexingan06.cn

string.find(s, "%d+")
来源：http://in.huixinmuqiang.cn

[T40] Lua：元表
来源：http://rk.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://af.newstarts.cn

[T41] Perl：Hello World
来源：http://gt.wgjwhj.cn

print "Hello\n";
来源：http://mc.haigaiapp.cn

[T42] Perl：变量类型
来源：http://qh.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bh.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://vl.gzmigu.cn

"值: $a"
来源：http://db.haigaiapp.cn

[T44] Perl：条件
来源：http://qa.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://qs.hahajie.cn

[T45] Perl：数组遍历
来源：http://us.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://mh.gzmigu.cn

[T46] Perl：哈希操作
来源：http://ck.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lf.hnjuh.cn

[T47] Perl：正则捕获
来源：http://kq.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fm.gzmigu.cn

[T48] Perl：正则替换
来源：http://bl.colortex.cn

$s =~ s/old/new/g;
来源：http://rm.hnjuh.cn

[T49] Perl：函数
来源：http://uv.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lw.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://xd.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bo.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://re.szxytkj.cn

[T51] Scala：Hello World
来源：http://mg.haigaiapp.cn

println("Hello")
来源：http://ex.9csxet.cn

[T52] Scala：变量
来源：http://lw.huixiangedu.cn

val a = 1;  var b = 2
来源：http://oq.asd995.cn

[T53] Scala：字符串插值
来源：http://lg.shxzskj.cn

s"值: $b"
来源：http://ru.jctech888.com.cn

[T54] Scala：集合映射
来源：http://vz.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://vz.panjiajie.cn

[T55] Scala：集合过滤
来源：http://sx.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fp.haigaiapp.cn

[T56] Scala：样例类
来源：http://be.panjiajie.cn

case class User(name: String, age: Int)
来源：http://ij.huanxung.cn

[T57] Scala：模式匹配
来源：http://tu.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ny.nicolike.cn

[T58] Scala：函数定义
来源：http://ep.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://we.shtwfgs.cn

[T59] Scala：循环
来源：http://kr.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://pj.nicolike.cn

[T60] Scala：折叠
来源：http://mq.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wv.nicolike.cn

================================================================================
来源：http://jf.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jp.shxzukj.cn

================================================================================
来源：http://ua.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://kg.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vt.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://ez.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vy.asd995.cn

[U03] Py：加载 .env 配置
来源：http://cn.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gx.colortex.cn

[U04] Py：变量调试打印
来源：http://wv.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wu.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://fc.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://st.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://la.yuexingan06.cn

{**a, **b}
来源：http://xo.lnxyls.cn

[U07] Py：反转字典键值
来源：http://nm.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://yd.nicolike.cn

[U08] Py：展平二维列表
来源：http://cl.asd995.cn

[y for x in nested for y in x]
来源：http://at.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://sx.haigaiapp.cn

max(d, key=d.get)
来源：http://wg.hnjuh.cn

[U10] Py：按值排序字典
来源：http://nk.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ox.colortex.cn

[U11] Py：生成器表达式
来源：http://ho.521024.cn

(x * 2 for x in arr)
来源：http://ht.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://le.szxytkj.cn

Counter(arr).most_common(3)
来源：http://vm.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://cg.9csxet.cn

deque(maxlen=10)
来源：http://oh.szsharing.cn

[U14] Py：分组收集到列表
来源：http://dx.shtwfgs.cn

defaultdict(list)
来源：http://gz.jctech888.com.cn

[U15] Py：高精度计时
来源：http://ec.nicolike.cn

t = time.perf_counter()
来源：http://od.colortex.cn

[U16] Py：命令行参数解析
来源：http://zu.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pq.newstarts.cn

[U17] Py：初始化日志
来源：http://oe.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://pj.9csxet.cn

[U18] Py：预编译正则
来源：http://fp.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://qa.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://mf.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gv.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://gt.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://qp.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://lz.nicolike.cn

@contextlib.contextmanager
来源：http://tx.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://qt.nszjky.cn

list(zip(*m))
来源：http://fy.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://an.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jm.9csxet.cn

[U24] Py：路径操作
来源：http://gn.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sz.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://hh.nicolike.cn

csv.DictReader(f)
来源：http://bl.chemitech.net.cn

[U26] Py：并发下载
来源：http://ua.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mh.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://az.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://qm.wgjwhj.cn

[U28] Py：类型别名
来源：http://jh.bjjhwx.cn

UserId = int
来源：http://ta.bjjhwx.cn

[U29] Py：属性校验
来源：http://oe.szsharing.cn

@property 与 @x.setter 配合
来源：http://ly.521024.cn

[U30] Py：数据类
来源：http://vc.hnjuh.cn

@dataclass(slots=True)
来源：http://ug.shtwfgs.cn

[U31] Py：单测
来源：http://qw.nicolike.cn

python -m pytest -q
来源：http://tt.nicolike.cn

[U32] Py：代码格式化
来源：http://jq.colortex.cn

ruff format . && ruff check --fix .
来源：http://nw.newstarts.cn

[U33] Py：打包发布
来源：http://bl.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://uy.asd995.cn

[U34] Py：判断编码
来源：http://fs.yuexingan06.cn

chardet.detect(raw)
来源：http://cj.jctech888.com.cn

[U35] Py：发送邮件
来源：http://wp.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ck.nicolike.cn

[U36] Py：定时任务
来源：http://ry.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://vb.asd995.cn

[U37] Py：读写 Excel
来源：http://an.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gi.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://ne.newstarts.cn

Path(__file__).resolve().parent
来源：http://bd.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://us.nicolike.cn

sys.stdout.isatty()
来源：http://wl.asd995.cn

[U40] Py：打印到标准错误
来源：http://qb.asd995.cn

print("err", file=sys.stderr)
来源：http://xe.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://by.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://el.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ss.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eq.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://kg.yuexingan06.cn

namespace App\Http;
来源：http://xu.nicolike.cn

[U44] PHP：开启严格类型
来源：http://wu.haigaiapp.cn

declare(strict_types=1);
来源：http://en.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ak.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://op.colortex.cn

[U46] PHP：可空类型
来源：http://lx.huixiangedu.cn

?string $name = null
来源：http://ri.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://wd.nicolike.cn

int|string $id
来源：http://kv.szsharing.cn

[U48] PHP：纯枚举
来源：http://ry.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fb.hahajie.cn

[U49] PHP：只读属性
来源：http://qt.chemitech.net.cn

public readonly string $name
来源：http://ae.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://nq.9csxet.cn

public function __construct(private int $id) {}
来源：http://pw.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://os.muxihuayi.cn

[$a, $b] = $arr;
来源：http://dr.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://zk.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://dm.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://te.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://dk.lnxyls.cn

[U54] PHP：空安全调用
来源：http://zo.jianghongdianzi.cn

$obj?->method()
来源：http://gx.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://cf.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://em.yuexingan06.cn

[U56] PHP：命名参数
来源：http://fo.gzmigu.cn

f(a: 1, b: 2)
来源：http://us.gzmigu.cn

[U57] PHP：字符串插值
来源：http://xx.huixiangedu.cn

"值: {$a}"
来源：http://uz.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://ko.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pu.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://nb.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ml.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://ju.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ec.yuntaijiaju.cn

[U61] PHP：正则
来源：http://zs.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ln.panjiajie.cn

[U62] PHP：日期对象
来源：http://cb.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uf.haigaiapp.cn

[U63] PHP：文件读写
来源：http://ii.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ww.lnxyls.cn

[U64] PHP：目录遍历
来源：http://lk.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://cr.chemitech.net.cn

[U65] PHP：会话
来源：http://jv.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pm.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://ks.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yy.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://ti.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fv.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://gx.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://co.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://qv.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jk.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://rq.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hd.9csxet.cn

[U71] PHP：抛出异常
来源：http://vk.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://un.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://tb.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://xx.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://hz.colortex.cn

parse_ini_file("config.ini", true)
来源：http://zd.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://mt.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://fk.panjiajie.cn

[U75] PHP：依赖注入
来源：http://px.newstarts.cn

composer require psr/container
来源：http://qf.shxzukj.cn

[U76] PHP：简单路由
来源：http://vo.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kt.gzmigu.cn

[U77] PHP：模板渲染
来源：http://ms.muxihuayi.cn

composer require twig/twig
来源：http://rt.jctech888.com.cn

[U78] PHP：单元测试
来源：http://my.colortex.cn

composer require --dev phpunit/phpunit
来源：http://rn.huanxung.cn

[U79] PHP：静态分析
来源：http://vs.asd995.cn

composer require --dev phpstan/phpstan
来源：http://wd.huanxung.cn

[U80] PHP：代码规范修复
来源：http://um.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eo.szsharing.cn

[U81] JS：初始化项目
来源：http://ju.gzmigu.cn

npm init -y;  npm i express
来源：http://ih.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://jj.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ny.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://ht.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ac.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://um.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ps.panjiajie.cn

[U85] JS：可选链
来源：http://qy.szsharing.cn

a?.b?.c
来源：http://lp.lnxyls.cn

[U86] JS：空值合并
来源：http://ix.yuexingan06.cn

a ?? b
来源：http://xs.colortex.cn

[U87] JS：解构默认值
来源：http://pc.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://rh.asd995.cn

[U88] JS：对象展开合并
来源：http://ga.bookmarksfly.cn

{ ...a, ...b }
来源：http://cl.nicolike.cn

[U89] JS：数组去重
来源：http://qh.yuexingan06.cn

[...new Set(arr)]
来源：http://vt.newstarts.cn

[U90] JS：数字数组排序
来源：http://gi.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ed.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://sn.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fv.panjiajie.cn

[U92] JS：深拷贝
来源：http://el.haigaiapp.cn

structuredClone(obj)
来源：http://uk.yuntaijiaju.cn


<!-- 参考信息 -->