代发 wailian999

[T07] Kotlin：集合过滤
来源：http://je.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cn.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://wh.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://yy.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://za.521024.cn

fun String.exclaim() = this + "!"
来源：http://ij.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://bq.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ce.9csxet.cn

[T11] Kotlin：协程
来源：http://py.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qd.szsharing.cn

[T12] Kotlin：解构声明
来源：http://xf.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://kb.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://gk.huanxung.cn

val m = mapOf("a" to 1)
来源：http://kp.huanxung.cn

[T14] Kotlin：循环
来源：http://jw.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://ui.jctech888.com.cn

[T15] Kotlin：接口
来源：http://gj.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://cq.haigaiapp.cn

[T16] Swift：Hello World
来源：http://hr.nszjky.cn

print("Hello")
来源：http://ob.szxytkj.cn

[T17] Swift：变量与常量
来源：http://db.hnjuh.cn

var a = 1;  let b = 2
来源：http://ww.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://xg.nicolike.cn

"值: \(b)"
来源：http://mr.nicolike.cn

[T19] Swift：可选绑定
来源：http://cn.hnjuh.cn

if let n = opt { print(n) }
来源：http://gp.shxzukj.cn

[T20] Swift：数组操作
来源：http://nb.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ll.chemitech.net.cn

[T21] Swift：遍历
来源：http://eu.szxytkj.cn

for x in a { print(x) }
来源：http://kb.szsharing.cn

[T22] Swift：字典
来源：http://lx.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wy.huixiangedu.cn

[T23] Swift：函数
来源：http://st.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pg.nicolike.cn

[T24] Swift：闭包
来源：http://kn.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ys.wgjwhj.cn

[T25] Swift：结构体
来源：http://to.huixinmuqiang.cn

struct P { var x: Int }
来源：http://wd.nszjky.cn

[T26] Swift：类与重写
来源：http://ja.asd995.cn

class A: Base { override func f() {} }
来源：http://ra.szxytkj.cn

[T27] Swift：错误处理
来源：http://vs.huanxung.cn

do { try f() } catch { print(error) }
来源：http://ty.asd995.cn

[T28] Swift：枚举
来源：http://yo.9csxet.cn

enum Color { case red, green }
来源：http://lx.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://bk.bjjhwx.cn

guard let x = opt else { return }
来源：http://ta.shxzskj.cn

[T30] Swift：协议
来源：http://nn.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://da.colortex.cn

[T31] Lua：Hello World
来源：http://nl.jianghongdianzi.cn

print("Hello")
来源：http://es.newstarts.cn

[T32] Lua：局部变量
来源：http://hb.jctech888.com.cn

local a = 1
来源：http://ss.asd995.cn

[T33] Lua：表（数组）
来源：http://eq.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lv.wgjwhj.cn

[T34] Lua：遍历表
来源：http://kx.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ec.asd995.cn

[T35] Lua：字典表
来源：http://qc.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://hq.hnjuh.cn

[T36] Lua：函数
来源：http://um.huixiangedu.cn

function add(a, b) return a + b end
来源：http://uj.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://oc.521024.cn

"a" .. "b"
来源：http://vg.bookmarksfly.cn

[T38] Lua：条件
来源：http://gh.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://te.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://dm.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://xj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ne.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://lp.9csxet.cn

[T41] Perl：Hello World
来源：http://ax.9csxet.cn

print "Hello\n";
来源：http://it.hahajie.cn

[T42] Perl：变量类型
来源：http://vt.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tu.nszjky.cn

[T43] Perl：字符串插值
来源：http://ft.gzmigu.cn

"值: $a"
来源：http://tc.jianghongdianzi.cn

[T44] Perl：条件
来源：http://ej.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://fy.szxytkj.cn

[T45] Perl：数组遍历
来源：http://bd.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ih.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://xc.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://do.nicolike.cn

[T47] Perl：正则捕获
来源：http://vy.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mm.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ve.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://zh.jianghongdianzi.cn

[T49] Perl：函数
来源：http://qu.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mr.colortex.cn

[T50] Perl：逐行读文件
来源：http://pa.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wp.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://os.szsharing.cn

[T51] Scala：Hello World
来源：http://ia.huixiangedu.cn

println("Hello")
来源：http://al.hahajie.cn

[T52] Scala：变量
来源：http://hm.9csxet.cn

val a = 1;  var b = 2
来源：http://oz.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://rs.haigaiapp.cn

s"值: $b"
来源：http://ko.huixiangedu.cn

[T54] Scala：集合映射
来源：http://aj.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://il.szxytkj.cn

[T55] Scala：集合过滤
来源：http://em.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iv.yuexingan06.cn

[T56] Scala：样例类
来源：http://dm.9csxet.cn

case class User(name: String, age: Int)
来源：http://st.szxytkj.cn

[T57] Scala：模式匹配
来源：http://vq.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gi.huixiangedu.cn

[T58] Scala：函数定义
来源：http://wg.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ke.shxzukj.cn

[T59] Scala：循环
来源：http://cy.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://vj.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://ix.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tz.jctech888.com.cn

================================================================================
来源：http://sx.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sx.hnjuh.cn

================================================================================
来源：http://wr.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://hl.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://la.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://ll.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nq.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://qp.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iz.colortex.cn

[U04] Py：变量调试打印
来源：http://um.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vg.hahajie.cn

[U05] Py：列表去重且保序
来源：http://or.nicolike.cn

list(dict.fromkeys(arr))
来源：http://id.huanxung.cn

[U06] Py：合并两个字典
来源：http://jz.521024.cn

{**a, **b}
来源：http://lt.shxzskj.cn

[U07] Py：反转字典键值
来源：http://fw.asd995.cn

{v: k for k, v in d.items()}
来源：http://kc.asd995.cn

[U08] Py：展平二维列表
来源：http://kw.9csxet.cn

[y for x in nested for y in x]
来源：http://ph.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://oh.haigaiapp.cn

max(d, key=d.get)
来源：http://kc.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://so.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oh.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://kr.huanxung.cn

(x * 2 for x in arr)
来源：http://gg.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gq.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://eu.gzmigu.cn

[U13] Py：固定长度队列
来源：http://sb.bookmarksfly.cn

deque(maxlen=10)
来源：http://mh.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://zw.colortex.cn

defaultdict(list)
来源：http://gs.shtwfgs.cn

[U15] Py：高精度计时
来源：http://pg.bjjhwx.cn

t = time.perf_counter()
来源：http://mv.colortex.cn

[U16] Py：命令行参数解析
来源：http://sv.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yg.yuexingan06.cn

[U17] Py：初始化日志
来源：http://ut.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://ib.gzmigu.cn

[U18] Py：预编译正则
来源：http://kx.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://xn.colortex.cn

[U19] Py：正则替换带回调
来源：http://pm.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wi.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://pu.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://vm.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://fu.hahajie.cn

@contextlib.contextmanager
来源：http://ky.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://bi.shtwfgs.cn

list(zip(*m))
来源：http://ww.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://kw.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vq.jctech888.com.cn

[U24] Py：路径操作
来源：http://nv.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tx.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://ug.shxzukj.cn

csv.DictReader(f)
来源：http://ef.9csxet.cn

[U26] Py：并发下载
来源：http://tk.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ux.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://sn.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://wo.521024.cn

[U28] Py：类型别名
来源：http://lf.huixinmuqiang.cn

UserId = int
来源：http://ym.shxzskj.cn

[U29] Py：属性校验
来源：http://et.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://sq.hahajie.cn

[U30] Py：数据类
来源：http://we.yuexingan06.cn

@dataclass(slots=True)
来源：http://dq.chemitech.net.cn

[U31] Py：单测
来源：http://cw.asd995.cn

python -m pytest -q
来源：http://sx.panjiajie.cn

[U32] Py：代码格式化
来源：http://zs.hahajie.cn

ruff format . && ruff check --fix .
来源：http://tf.szsharing.cn

[U33] Py：打包发布
来源：http://ag.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://kr.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://sr.nszjky.cn

chardet.detect(raw)
来源：http://ep.shxzskj.cn

[U35] Py：发送邮件
来源：http://zk.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://am.szxytkj.cn

[U36] Py：定时任务
来源：http://pb.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://rg.shxzskj.cn

[U37] Py：读写 Excel
来源：http://se.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xw.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://ns.gzmigu.cn

Path(__file__).resolve().parent
来源：http://fe.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://dz.shxzskj.cn

sys.stdout.isatty()
来源：http://fn.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://zi.hnjuh.cn

print("err", file=sys.stderr)
来源：http://wl.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://sx.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fb.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://wd.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bi.newstarts.cn

[U43] PHP：声明命名空间
来源：http://fk.haigaiapp.cn

namespace App\Http;
来源：http://xn.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://tv.yuntaijiaju.cn

declare(strict_types=1);
来源：http://do.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://qw.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dp.lnxyls.cn

[U46] PHP：可空类型
来源：http://ve.asd995.cn

?string $name = null
来源：http://ol.shtwfgs.cn

[U47] PHP：联合类型
来源：http://oa.jctech888.com.cn

int|string $id
来源：http://wj.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://zg.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xi.huanxung.cn

[U49] PHP：只读属性
来源：http://wt.newstarts.cn

public readonly string $name
来源：http://bm.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://gr.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://eg.colortex.cn

[U51] PHP：数组解构
来源：http://ml.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://vb.szxytkj.cn

[U52] PHP：箭头函数
来源：http://ry.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://xf.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://xr.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://uq.9csxet.cn

[U54] PHP：空安全调用
来源：http://oq.huanxung.cn

$obj?->method()
来源：http://qu.newstarts.cn

[U55] PHP：match 表达式
来源：http://zh.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jk.bjjhwx.cn

[U56] PHP：命名参数
来源：http://zv.chemitech.net.cn

f(a: 1, b: 2)
来源：http://kb.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://fo.gzmigu.cn

"值: {$a}"
来源：http://xx.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://og.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ud.521024.cn

[U59] PHP：自定义排序
来源：http://xl.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bq.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://ah.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ns.chemitech.net.cn

[U61] PHP：正则
来源：http://jr.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://px.hnjuh.cn

[U62] PHP：日期对象
来源：http://jr.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fu.shxzukj.cn

[U63] PHP：文件读写
来源：http://qd.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ak.521024.cn

[U64] PHP：目录遍历
来源：http://ea.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://rd.shtwfgs.cn

[U65] PHP：会话
来源：http://sz.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pw.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ay.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ya.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://wq.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fu.colortex.cn

[U68] PHP：PDO 连接
来源：http://xu.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yp.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://jm.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bh.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://hw.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ng.hahajie.cn

[U71] PHP：抛出异常
来源：http://oi.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://li.huanxung.cn

[U72] PHP：写错误日志
来源：http://mn.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://lu.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://dr.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://mw.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://nx.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://vk.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://rj.gzmigu.cn

composer require psr/container
来源：http://oy.gzmigu.cn

[U76] PHP：简单路由
来源：http://wp.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mk.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://ba.bookmarksfly.cn

composer require twig/twig
来源：http://qc.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ia.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://sf.jctech888.com.cn

[U79] PHP：静态分析
来源：http://ef.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://cr.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ll.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jr.newstarts.cn

[U81] JS：初始化项目
来源：http://rb.521024.cn

npm init -y;  npm i express
来源：http://iw.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://pc.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mw.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://lf.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cc.521024.cn

[U84] JS：CommonJS 写法
来源：http://gn.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ym.jianghongdianzi.cn

[U85] JS：可选链
来源：http://rp.521024.cn

a?.b?.c
来源：http://ph.gzmigu.cn

[U86] JS：空值合并
来源：http://no.chemitech.net.cn

a ?? b
来源：http://xx.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://nx.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://bv.szsharing.cn

[U88] JS：对象展开合并
来源：http://ja.nicolike.cn

{ ...a, ...b }
来源：http://zt.521024.cn

[U89] JS：数组去重
来源：http://fv.jctech888.com.cn

[...new Set(arr)]
来源：http://eu.asd995.cn

[U90] JS：数字数组排序
来源：http://qe.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://xp.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://se.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lh.huanxung.cn

[U92] JS：深拷贝
来源：http://fm.nicolike.cn

structuredClone(obj)
来源：http://rw.chemitech.net.cn

[U93] JS：模板字符串
来源：http://ya.asd995.cn

`共 ${n} 条`
来源：http://wq.asd995.cn

[U94] JS：箭头函数
来源：http://ka.yuntaijiaju.cn

const double = x => x * 2;
来源：http://wn.nicolike.cn


<!-- 参考信息 -->