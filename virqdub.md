代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ag.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cl.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://qi.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ag.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://zc.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sd.panjiajie.cn

[T08] Kotlin：数据类
来源：http://hj.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://zq.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://ds.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://lq.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://no.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cw.haigaiapp.cn

[T11] Kotlin：协程
来源：http://km.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mb.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://nn.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://pi.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://xr.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://lp.nicolike.cn

[T14] Kotlin：循环
来源：http://ht.szxytkj.cn

for (i in 1..10) println(i)
来源：http://ha.colortex.cn

[T15] Kotlin：接口
来源：http://ql.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://uq.shxzukj.cn

[T16] Swift：Hello World
来源：http://bl.huixiangedu.cn

print("Hello")
来源：http://sa.asd995.cn

[T17] Swift：变量与常量
来源：http://hf.shxzskj.cn

var a = 1;  let b = 2
来源：http://mb.hnjuh.cn

[T18] Swift：字符串插值
来源：http://ut.newstarts.cn

"值: \(b)"
来源：http://fp.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://md.muxihuayi.cn

if let n = opt { print(n) }
来源：http://fg.yuexingan06.cn

[T20] Swift：数组操作
来源：http://eu.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qf.jctech888.com.cn

[T21] Swift：遍历
来源：http://qa.panjiajie.cn

for x in a { print(x) }
来源：http://xf.jctech888.com.cn

[T22] Swift：字典
来源：http://nb.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sg.haigaiapp.cn

[T23] Swift：函数
来源：http://kj.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ys.jctech888.com.cn

[T24] Swift：闭包
来源：http://az.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zd.shxzskj.cn

[T25] Swift：结构体
来源：http://io.huanxung.cn

struct P { var x: Int }
来源：http://fv.wgjwhj.cn

[T26] Swift：类与重写
来源：http://xu.lnxyls.cn

class A: Base { override func f() {} }
来源：http://xv.yuexingan06.cn

[T27] Swift：错误处理
来源：http://iy.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ma.huanxung.cn

[T28] Swift：枚举
来源：http://xq.shxzskj.cn

enum Color { case red, green }
来源：http://et.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://ls.nszjky.cn

guard let x = opt else { return }
来源：http://th.wgjwhj.cn

[T30] Swift：协议
来源：http://eg.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://jo.shxzskj.cn

[T31] Lua：Hello World
来源：http://ur.colortex.cn

print("Hello")
来源：http://oj.bjjhwx.cn

[T32] Lua：局部变量
来源：http://ij.shxzukj.cn

local a = 1
来源：http://bx.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://oj.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://up.haigaiapp.cn

[T34] Lua：遍历表
来源：http://yb.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ew.huanxung.cn

[T35] Lua：字典表
来源：http://im.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://iz.9csxet.cn

[T36] Lua：函数
来源：http://ku.asd995.cn

function add(a, b) return a + b end
来源：http://my.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://qw.shxzukj.cn

"a" .. "b"
来源：http://fv.haigaiapp.cn

[T38] Lua：条件
来源：http://mj.shxzukj.cn

if x > 0 then print("正") end
来源：http://nl.szsharing.cn

[T39] Lua：模式匹配
来源：http://kh.gzmigu.cn

string.find(s, "%d+")
来源：http://dt.jctech888.com.cn

[T40] Lua：元表
来源：http://zg.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://uk.chemitech.net.cn

[T41] Perl：Hello World
来源：http://wy.panjiajie.cn

print "Hello\n";
来源：http://dd.gzmigu.cn

[T42] Perl：变量类型
来源：http://lv.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ua.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://if.haigaiapp.cn

"值: $a"
来源：http://gd.shxzskj.cn

[T44] Perl：条件
来源：http://pd.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://jt.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://zh.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://yb.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://oa.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qo.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://jj.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yw.shtwfgs.cn

[T48] Perl：正则替换
来源：http://ns.asd995.cn

$s =~ s/old/new/g;
来源：http://wz.jianghongdianzi.cn

[T49] Perl：函数
来源：http://hv.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dj.9csxet.cn

[T50] Perl：逐行读文件
来源：http://xd.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ng.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://uh.huanxung.cn

[T51] Scala：Hello World
来源：http://vz.bookmarksfly.cn

println("Hello")
来源：http://ie.lnxyls.cn

[T52] Scala：变量
来源：http://vr.shxzskj.cn

val a = 1;  var b = 2
来源：http://gm.shxzukj.cn

[T53] Scala：字符串插值
来源：http://of.bjjhwx.cn

s"值: $b"
来源：http://hr.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://vu.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://xo.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://mw.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://os.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://wd.hnjuh.cn

case class User(name: String, age: Int)
来源：http://qu.szsharing.cn

[T57] Scala：模式匹配
来源：http://gd.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ht.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://ei.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bj.chemitech.net.cn

[T59] Scala：循环
来源：http://jn.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://nd.yuexingan06.cn

[T60] Scala：折叠
来源：http://hu.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wq.haigaiapp.cn

================================================================================
来源：http://wz.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fg.huanxung.cn

================================================================================
来源：http://xo.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://ri.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gn.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://lk.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gt.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://kn.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dn.hahajie.cn

[U04] Py：变量调试打印
来源：http://sa.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zb.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://tp.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://mf.shxzukj.cn

[U06] Py：合并两个字典
来源：http://ws.panjiajie.cn

{**a, **b}
来源：http://el.szxytkj.cn

[U07] Py：反转字典键值
来源：http://ax.colortex.cn

{v: k for k, v in d.items()}
来源：http://ja.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://jz.9csxet.cn

[y for x in nested for y in x]
来源：http://bk.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ei.yuexingan06.cn

max(d, key=d.get)
来源：http://tr.nszjky.cn

[U10] Py：按值排序字典
来源：http://kl.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qg.szsharing.cn

[U11] Py：生成器表达式
来源：http://pj.hnjuh.cn

(x * 2 for x in arr)
来源：http://ho.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yj.asd995.cn

Counter(arr).most_common(3)
来源：http://rw.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://pe.shtwfgs.cn

deque(maxlen=10)
来源：http://va.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://tx.shxzskj.cn

defaultdict(list)
来源：http://pc.huanxung.cn

[U15] Py：高精度计时
来源：http://hz.huixinmuqiang.cn

t = time.perf_counter()
来源：http://fr.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://fv.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ca.yuexingan06.cn

[U17] Py：初始化日志
来源：http://vd.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://wj.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://cc.hahajie.cn

pat = re.compile(r"\d+")
来源：http://vn.newstarts.cn

[U19] Py：正则替换带回调
来源：http://lm.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lt.asd995.cn

[U20] Py：缓存函数结果
来源：http://id.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://th.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://zx.hahajie.cn

@contextlib.contextmanager
来源：http://pw.521024.cn

[U22] Py：矩阵转置
来源：http://wq.shxzukj.cn

list(zip(*m))
来源：http://av.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://fr.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sk.szsharing.cn

[U24] Py：路径操作
来源：http://em.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ka.asd995.cn

[U25] Py：CSV 按字典读
来源：http://ss.huanxung.cn

csv.DictReader(f)
来源：http://rw.szxytkj.cn

[U26] Py：并发下载
来源：http://hm.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ku.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://hx.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://rv.jctech888.com.cn

[U28] Py：类型别名
来源：http://gq.shtwfgs.cn

UserId = int
来源：http://go.nicolike.cn

[U29] Py：属性校验
来源：http://li.shxzukj.cn

@property 与 @x.setter 配合
来源：http://vv.huixiangedu.cn

[U30] Py：数据类
来源：http://ky.hahajie.cn

@dataclass(slots=True)
来源：http://ki.521024.cn

[U31] Py：单测
来源：http://lo.hnjuh.cn

python -m pytest -q
来源：http://os.wgjwhj.cn

[U32] Py：代码格式化
来源：http://tv.nszjky.cn

ruff format . && ruff check --fix .
来源：http://lm.shxzskj.cn

[U33] Py：打包发布
来源：http://zh.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://gm.bjjhwx.cn

[U34] Py：判断编码
来源：http://xa.9csxet.cn

chardet.detect(raw)
来源：http://gb.muxihuayi.cn

[U35] Py：发送邮件
来源：http://ro.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wu.szsharing.cn

[U36] Py：定时任务
来源：http://uu.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ew.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://vw.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qh.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://nc.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://aj.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://lr.szxytkj.cn

sys.stdout.isatty()
来源：http://jz.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://km.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ow.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://jf.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pc.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://pw.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yh.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://uj.panjiajie.cn

namespace App\Http;
来源：http://mf.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://bo.jctech888.com.cn

declare(strict_types=1);
来源：http://pj.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://xq.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qa.chemitech.net.cn

[U46] PHP：可空类型
来源：http://kx.shxzskj.cn

?string $name = null
来源：http://lx.szsharing.cn

[U47] PHP：联合类型
来源：http://ji.asd995.cn

int|string $id
来源：http://hu.huanxung.cn

[U48] PHP：纯枚举
来源：http://pn.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gb.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://iq.hahajie.cn

public readonly string $name
来源：http://bn.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://od.521024.cn

public function __construct(private int $id) {}
来源：http://fu.wgjwhj.cn

[U51] PHP：数组解构
来源：http://ft.wgjwhj.cn

[$a, $b] = $arr;
来源：http://cj.huanxung.cn

[U52] PHP：箭头函数
来源：http://du.asd995.cn

$double = fn($x) => $x * 2;
来源：http://mu.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://cp.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://cs.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://lj.chemitech.net.cn

$obj?->method()
来源：http://gv.521024.cn

[U55] PHP：match 表达式
来源：http://wo.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://am.szsharing.cn

[U56] PHP：命名参数
来源：http://db.colortex.cn

f(a: 1, b: 2)
来源：http://ps.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://ue.shxzskj.cn

"值: {$a}"
来源：http://ds.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://oz.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qx.asd995.cn

[U59] PHP：自定义排序
来源：http://ut.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sy.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://rq.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zs.jianghongdianzi.cn

[U61] PHP：正则
来源：http://my.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eh.haigaiapp.cn

[U62] PHP：日期对象
来源：http://ga.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vr.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://hq.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://or.hnjuh.cn

[U64] PHP：目录遍历
来源：http://fi.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://uy.huanxung.cn

[U65] PHP：会话
来源：http://nx.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zh.521024.cn

[U66] PHP：设置 Cookie
来源：http://tt.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vo.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://ok.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mh.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://ge.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jc.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://eu.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gn.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://vb.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xz.hahajie.cn

[U71] PHP：抛出异常
来源：http://js.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://sr.9csxet.cn

[U72] PHP：写错误日志
来源：http://ve.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://vu.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://is.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://tz.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://zl.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://ea.shxzukj.cn

[U75] PHP：依赖注入
来源：http://rg.bjjhwx.cn

composer require psr/container
来源：http://sk.szxytkj.cn

[U76] PHP：简单路由
来源：http://an.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://an.shxzukj.cn

[U77] PHP：模板渲染
来源：http://xu.shxzukj.cn

composer require twig/twig
来源：http://aq.wgjwhj.cn

[U78] PHP：单元测试
来源：http://aw.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://oq.colortex.cn

[U79] PHP：静态分析
来源：http://sh.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://zj.szsharing.cn

[U80] PHP：代码规范修复
来源：http://po.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ec.haigaiapp.cn

[U81] JS：初始化项目
来源：http://gf.nszjky.cn

npm init -y;  npm i express
来源：http://cq.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://ns.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dq.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://qh.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mo.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://lu.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rh.jctech888.com.cn

[U85] JS：可选链
来源：http://zn.yuexingan06.cn

a?.b?.c
来源：http://dv.9csxet.cn

[U86] JS：空值合并
来源：http://ih.bjjhwx.cn

a ?? b
来源：http://uf.newstarts.cn

[U87] JS：解构默认值
来源：http://ka.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://cs.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://hq.newstarts.cn

{ ...a, ...b }
来源：http://hs.bookmarksfly.cn

[U89] JS：数组去重
来源：http://vu.huanxung.cn

[...new Set(arr)]
来源：http://uv.nszjky.cn

[U90] JS：数字数组排序
来源：http://fn.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://ha.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://sc.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dq.huixiangedu.cn

[U92] JS：深拷贝
来源：http://uc.yuntaijiaju.cn

structuredClone(obj)
来源：http://vn.szsharing.cn


<!-- 参考信息 -->