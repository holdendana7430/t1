代发 wailian999

[T09] Kotlin：扩展函数
来源：http://st.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://kv.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://kl.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dz.hnjuh.cn

[T11] Kotlin：协程
来源：http://be.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yx.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://zi.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://vs.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://in.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://we.huixiangedu.cn

[T14] Kotlin：循环
来源：http://yu.hnjuh.cn

for (i in 1..10) println(i)
来源：http://ta.huixiangedu.cn

[T15] Kotlin：接口
来源：http://im.colortex.cn

interface Shape { fun area(): Double }
来源：http://lg.huanxung.cn

[T16] Swift：Hello World
来源：http://gy.gzmigu.cn

print("Hello")
来源：http://lx.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://gc.nicolike.cn

var a = 1;  let b = 2
来源：http://qg.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://pg.panjiajie.cn

"值: \(b)"
来源：http://lz.nicolike.cn

[T19] Swift：可选绑定
来源：http://tm.nicolike.cn

if let n = opt { print(n) }
来源：http://en.gzmigu.cn

[T20] Swift：数组操作
来源：http://yx.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://su.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://px.asd995.cn

for x in a { print(x) }
来源：http://uz.asd995.cn

[T22] Swift：字典
来源：http://pv.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nw.yuexingan06.cn

[T23] Swift：函数
来源：http://pl.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://go.shxzskj.cn

[T24] Swift：闭包
来源：http://rj.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tb.wgjwhj.cn

[T25] Swift：结构体
来源：http://wn.jctech888.com.cn

struct P { var x: Int }
来源：http://gb.panjiajie.cn

[T26] Swift：类与重写
来源：http://bk.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://qd.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://cg.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://tr.bookmarksfly.cn

[T28] Swift：枚举
来源：http://cv.chemitech.net.cn

enum Color { case red, green }
来源：http://bt.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://zb.shxzskj.cn

guard let x = opt else { return }
来源：http://ce.521024.cn

[T30] Swift：协议
来源：http://wv.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://lq.panjiajie.cn

[T31] Lua：Hello World
来源：http://fv.jctech888.com.cn

print("Hello")
来源：http://hr.colortex.cn

[T32] Lua：局部变量
来源：http://yd.hnjuh.cn

local a = 1
来源：http://vz.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://lb.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://as.muxihuayi.cn

[T34] Lua：遍历表
来源：http://bd.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tk.huanxung.cn

[T35] Lua：字典表
来源：http://fj.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://rv.lnxyls.cn

[T36] Lua：函数
来源：http://fz.hahajie.cn

function add(a, b) return a + b end
来源：http://wb.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://wu.bjjhwx.cn

"a" .. "b"
来源：http://st.szsharing.cn

[T38] Lua：条件
来源：http://fr.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ty.szsharing.cn

[T39] Lua：模式匹配
来源：http://he.bjjhwx.cn

string.find(s, "%d+")
来源：http://ts.wgjwhj.cn

[T40] Lua：元表
来源：http://lz.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ud.newstarts.cn

[T41] Perl：Hello World
来源：http://fw.haigaiapp.cn

print "Hello\n";
来源：http://dj.shtwfgs.cn

[T42] Perl：变量类型
来源：http://kd.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kn.asd995.cn

[T43] Perl：字符串插值
来源：http://zd.chemitech.net.cn

"值: $a"
来源：http://aj.asd995.cn

[T44] Perl：条件
来源：http://jc.asd995.cn

if ($a > 0) { print "正"; }
来源：http://nh.nszjky.cn

[T45] Perl：数组遍历
来源：http://xz.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://rc.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://xo.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sf.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://nd.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rp.gzmigu.cn

[T48] Perl：正则替换
来源：http://xi.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://en.szxytkj.cn

[T49] Perl：函数
来源：http://mr.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zx.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://dx.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qc.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ew.nicolike.cn

[T51] Scala：Hello World
来源：http://wq.szxytkj.cn

println("Hello")
来源：http://li.huanxung.cn

[T52] Scala：变量
来源：http://gn.haigaiapp.cn

val a = 1;  var b = 2
来源：http://if.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://bs.chemitech.net.cn

s"值: $b"
来源：http://ed.lnxyls.cn

[T54] Scala：集合映射
来源：http://mi.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://hg.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://xn.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ve.wgjwhj.cn

[T56] Scala：样例类
来源：http://bc.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://rj.nicolike.cn

[T57] Scala：模式匹配
来源：http://jy.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vf.hahajie.cn

[T58] Scala：函数定义
来源：http://wb.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rh.wgjwhj.cn

[T59] Scala：循环
来源：http://ce.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://ui.jctech888.com.cn

[T60] Scala：折叠
来源：http://im.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qu.9csxet.cn

================================================================================
来源：http://pw.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ex.huanxung.cn

================================================================================
来源：http://ka.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://qt.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fp.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://hy.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jj.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://nx.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fe.hahajie.cn

[U04] Py：变量调试打印
来源：http://qn.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bh.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://vx.colortex.cn

list(dict.fromkeys(arr))
来源：http://pg.lnxyls.cn

[U06] Py：合并两个字典
来源：http://vp.yuexingan06.cn

{**a, **b}
来源：http://gf.nicolike.cn

[U07] Py：反转字典键值
来源：http://qg.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://ru.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://jh.szxytkj.cn

[y for x in nested for y in x]
来源：http://pm.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://bs.muxihuayi.cn

max(d, key=d.get)
来源：http://tj.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://dx.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fw.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://zg.gzmigu.cn

(x * 2 for x in arr)
来源：http://gq.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qz.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://xe.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ph.shtwfgs.cn

deque(maxlen=10)
来源：http://vp.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://wm.asd995.cn

defaultdict(list)
来源：http://fp.9csxet.cn

[U15] Py：高精度计时
来源：http://ee.szxytkj.cn

t = time.perf_counter()
来源：http://ya.nicolike.cn

[U16] Py：命令行参数解析
来源：http://te.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://go.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://rr.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://br.jctech888.com.cn

[U18] Py：预编译正则
来源：http://on.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://bw.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://rj.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fh.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://eu.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://gk.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://rz.huanxung.cn

@contextlib.contextmanager
来源：http://zc.hnjuh.cn

[U22] Py：矩阵转置
来源：http://bm.huixinmuqiang.cn

list(zip(*m))
来源：http://nk.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://tc.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://su.hahajie.cn

[U24] Py：路径操作
来源：http://dc.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sr.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://hz.jctech888.com.cn

csv.DictReader(f)
来源：http://lh.nicolike.cn

[U26] Py：并发下载
来源：http://dq.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wz.hahajie.cn

[U27] Py：异步 HTTP
来源：http://wc.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://bp.hnjuh.cn

[U28] Py：类型别名
来源：http://jm.yuexingan06.cn

UserId = int
来源：http://rx.huanxung.cn

[U29] Py：属性校验
来源：http://sr.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://rk.colortex.cn

[U30] Py：数据类
来源：http://vc.newstarts.cn

@dataclass(slots=True)
来源：http://dy.nszjky.cn

[U31] Py：单测
来源：http://vb.shxzskj.cn

python -m pytest -q
来源：http://ij.szxytkj.cn

[U32] Py：代码格式化
来源：http://cn.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://mw.shxzukj.cn

[U33] Py：打包发布
来源：http://vn.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://xv.huanxung.cn

[U34] Py：判断编码
来源：http://ck.hahajie.cn

chardet.detect(raw)
来源：http://ip.shxzukj.cn

[U35] Py：发送邮件
来源：http://do.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pp.shtwfgs.cn

[U36] Py：定时任务
来源：http://wb.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://kl.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://si.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bb.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://cv.521024.cn

Path(__file__).resolve().parent
来源：http://hu.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://se.shxzskj.cn

sys.stdout.isatty()
来源：http://ew.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://am.asd995.cn

print("err", file=sys.stderr)
来源：http://di.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://qs.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://py.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://fu.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xt.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://mr.shtwfgs.cn

namespace App\Http;
来源：http://tv.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://yl.9csxet.cn

declare(strict_types=1);
来源：http://vw.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://yw.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bt.shtwfgs.cn

[U46] PHP：可空类型
来源：http://sq.hahajie.cn

?string $name = null
来源：http://bi.lnxyls.cn

[U47] PHP：联合类型
来源：http://xd.szxytkj.cn

int|string $id
来源：http://sj.hahajie.cn

[U48] PHP：纯枚举
来源：http://ht.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zm.yuexingan06.cn

[U49] PHP：只读属性
来源：http://hf.newstarts.cn

public readonly string $name
来源：http://oo.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://ig.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://fh.shxzukj.cn

[U51] PHP：数组解构
来源：http://er.bjjhwx.cn

[$a, $b] = $arr;
来源：http://zi.hahajie.cn

[U52] PHP：箭头函数
来源：http://op.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://uh.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://at.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://th.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://co.bookmarksfly.cn

$obj?->method()
来源：http://so.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://ps.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://as.muxihuayi.cn

[U56] PHP：命名参数
来源：http://xl.huanxung.cn

f(a: 1, b: 2)
来源：http://me.nicolike.cn

[U57] PHP：字符串插值
来源：http://fj.asd995.cn

"值: {$a}"
来源：http://zb.szsharing.cn

[U58] PHP：数组三件套
来源：http://gk.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gg.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://vt.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ac.colortex.cn

[U60] PHP：JSON 编解码
来源：http://hs.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ol.yuntaijiaju.cn

[U61] PHP：正则
来源：http://nx.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dz.muxihuayi.cn

[U62] PHP：日期对象
来源：http://uh.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nb.bjjhwx.cn

[U63] PHP：文件读写
来源：http://ea.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jw.shxzukj.cn

[U64] PHP：目录遍历
来源：http://ww.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://sw.muxihuayi.cn

[U65] PHP：会话
来源：http://gr.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kr.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://cn.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ie.521024.cn

[U67] PHP：处理文件上传
来源：http://wm.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ek.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://op.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ms.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://wt.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zw.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://ha.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jr.newstarts.cn

[U71] PHP：抛出异常
来源：http://xp.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://sw.huanxung.cn

[U72] PHP：写错误日志
来源：http://ct.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://lm.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://jo.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://oy.asd995.cn

[U74] PHP：读取环境变量
来源：http://ik.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://zq.panjiajie.cn

[U75] PHP：依赖注入
来源：http://yh.chemitech.net.cn

composer require psr/container
来源：http://tk.szxytkj.cn

[U76] PHP：简单路由
来源：http://bc.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kw.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://lv.chemitech.net.cn

composer require twig/twig
来源：http://dt.panjiajie.cn

[U78] PHP：单元测试
来源：http://gn.asd995.cn

composer require --dev phpunit/phpunit
来源：http://il.szxytkj.cn

[U79] PHP：静态分析
来源：http://oc.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://nb.asd995.cn

[U80] PHP：代码规范修复
来源：http://gt.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gv.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ou.9csxet.cn

npm init -y;  npm i express
来源：http://ou.newstarts.cn

[U82] JS：package.json 脚本
来源：http://zo.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sk.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ah.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ro.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://yk.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eq.muxihuayi.cn

[U85] JS：可选链
来源：http://kw.huanxung.cn

a?.b?.c
来源：http://sr.nszjky.cn

[U86] JS：空值合并
来源：http://ao.szxytkj.cn

a ?? b
来源：http://ym.9csxet.cn

[U87] JS：解构默认值
来源：http://dc.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://wt.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://zp.hahajie.cn

{ ...a, ...b }
来源：http://rg.chemitech.net.cn

[U89] JS：数组去重
来源：http://ny.jctech888.com.cn

[...new Set(arr)]
来源：http://tg.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://bw.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://rl.521024.cn

[U91] JS：对象键值遍历
来源：http://cz.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bc.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ew.colortex.cn

structuredClone(obj)
来源：http://sn.muxihuayi.cn

[U93] JS：模板字符串
来源：http://yf.bookmarksfly.cn

`共 ${n} 条`
来源：http://sn.szsharing.cn

[U94] JS：箭头函数
来源：http://cs.hahajie.cn

const double = x => x * 2;
来源：http://nm.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://er.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://bx.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://qa.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hs.yuntaijiaju.cn


<!-- 参考信息 -->