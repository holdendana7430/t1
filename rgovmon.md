代发 wailian999

[T09] Kotlin：扩展函数
来源：http://ep.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://yy.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://xz.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jw.haigaiapp.cn

[T11] Kotlin：协程
来源：http://yt.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hn.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://kf.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://qr.colortex.cn

[T13] Kotlin：只读 Map
来源：http://ij.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://qw.szsharing.cn

[T14] Kotlin：循环
来源：http://zl.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://aw.shxzukj.cn

[T15] Kotlin：接口
来源：http://ot.huanxung.cn

interface Shape { fun area(): Double }
来源：http://te.wgjwhj.cn

[T16] Swift：Hello World
来源：http://do.huixiangedu.cn

print("Hello")
来源：http://ed.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://of.wgjwhj.cn

var a = 1;  let b = 2
来源：http://hl.nicolike.cn

[T18] Swift：字符串插值
来源：http://vf.bjjhwx.cn

"值: \(b)"
来源：http://ew.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://er.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://rb.szsharing.cn

[T20] Swift：数组操作
来源：http://zr.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nj.hahajie.cn

[T21] Swift：遍历
来源：http://yc.muxihuayi.cn

for x in a { print(x) }
来源：http://xo.shxzskj.cn

[T22] Swift：字典
来源：http://qa.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hx.huixinmuqiang.cn

[T23] Swift：函数
来源：http://wu.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fg.colortex.cn

[T24] Swift：闭包
来源：http://ix.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dz.panjiajie.cn

[T25] Swift：结构体
来源：http://sw.szsharing.cn

struct P { var x: Int }
来源：http://kt.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://lt.shxzukj.cn

class A: Base { override func f() {} }
来源：http://eu.muxihuayi.cn

[T27] Swift：错误处理
来源：http://ka.szsharing.cn

do { try f() } catch { print(error) }
来源：http://zc.szxytkj.cn

[T28] Swift：枚举
来源：http://fo.bookmarksfly.cn

enum Color { case red, green }
来源：http://km.521024.cn

[T29] Swift：guard 提前返回
来源：http://zo.gzmigu.cn

guard let x = opt else { return }
来源：http://uq.yuntaijiaju.cn

[T30] Swift：协议
来源：http://hf.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://tf.huanxung.cn

[T31] Lua：Hello World
来源：http://hv.jctech888.com.cn

print("Hello")
来源：http://mo.haigaiapp.cn

[T32] Lua：局部变量
来源：http://xr.huixiangedu.cn

local a = 1
来源：http://lj.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://yp.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ex.szxytkj.cn

[T34] Lua：遍历表
来源：http://kj.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://th.haigaiapp.cn

[T35] Lua：字典表
来源：http://le.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://xd.hahajie.cn

[T36] Lua：函数
来源：http://lt.shxzskj.cn

function add(a, b) return a + b end
来源：http://tx.521024.cn

[T37] Lua：字符串拼接
来源：http://hb.bjjhwx.cn

"a" .. "b"
来源：http://wa.asd995.cn

[T38] Lua：条件
来源：http://ec.nszjky.cn

if x > 0 then print("正") end
来源：http://xw.nicolike.cn

[T39] Lua：模式匹配
来源：http://ga.szsharing.cn

string.find(s, "%d+")
来源：http://vo.bjjhwx.cn

[T40] Lua：元表
来源：http://me.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://yl.shtwfgs.cn

[T41] Perl：Hello World
来源：http://lc.szsharing.cn

print "Hello\n";
来源：http://yk.shxzukj.cn

[T42] Perl：变量类型
来源：http://me.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pd.9csxet.cn

[T43] Perl：字符串插值
来源：http://qj.9csxet.cn

"值: $a"
来源：http://io.hnjuh.cn

[T44] Perl：条件
来源：http://oq.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://ns.shxzskj.cn

[T45] Perl：数组遍历
来源：http://vl.colortex.cn

for my $x (@arr) { print $x; }
来源：http://kb.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://jc.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hl.colortex.cn

[T47] Perl：正则捕获
来源：http://ky.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pj.colortex.cn

[T48] Perl：正则替换
来源：http://vi.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://ie.chemitech.net.cn

[T49] Perl：函数
来源：http://es.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kf.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://nb.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wz.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://of.shxzukj.cn

[T51] Scala：Hello World
来源：http://xd.hnjuh.cn

println("Hello")
来源：http://lm.hahajie.cn

[T52] Scala：变量
来源：http://bu.hahajie.cn

val a = 1;  var b = 2
来源：http://to.9csxet.cn

[T53] Scala：字符串插值
来源：http://lv.gzmigu.cn

s"值: $b"
来源：http://tm.lnxyls.cn

[T54] Scala：集合映射
来源：http://fw.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://ya.gzmigu.cn

[T55] Scala：集合过滤
来源：http://np.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kq.521024.cn

[T56] Scala：样例类
来源：http://ek.nicolike.cn

case class User(name: String, age: Int)
来源：http://uw.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://hj.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ti.huixiangedu.cn

[T58] Scala：函数定义
来源：http://em.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hy.hahajie.cn

[T59] Scala：循环
来源：http://wu.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://lb.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://yw.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gv.shxzukj.cn

================================================================================
来源：http://sh.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aw.shxzskj.cn

================================================================================
来源：http://dt.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://zf.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ax.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://bp.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qc.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://xi.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rk.asd995.cn

[U04] Py：变量调试打印
来源：http://er.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hv.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://py.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://qy.szsharing.cn

[U06] Py：合并两个字典
来源：http://fh.shtwfgs.cn

{**a, **b}
来源：http://zx.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://gj.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://so.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://dz.gzmigu.cn

[y for x in nested for y in x]
来源：http://es.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://bk.lnxyls.cn

max(d, key=d.get)
来源：http://re.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://nc.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ht.nicolike.cn

[U11] Py：生成器表达式
来源：http://xd.shxzukj.cn

(x * 2 for x in arr)
来源：http://sh.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fb.newstarts.cn

Counter(arr).most_common(3)
来源：http://qz.szsharing.cn

[U13] Py：固定长度队列
来源：http://fu.haigaiapp.cn

deque(maxlen=10)
来源：http://oh.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://nd.wgjwhj.cn

defaultdict(list)
来源：http://ot.521024.cn

[U15] Py：高精度计时
来源：http://nv.muxihuayi.cn

t = time.perf_counter()
来源：http://ra.huanxung.cn

[U16] Py：命令行参数解析
来源：http://sp.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dr.colortex.cn

[U17] Py：初始化日志
来源：http://bv.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://sc.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://lc.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://bf.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://vk.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ii.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://uw.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://yw.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://tr.szsharing.cn

@contextlib.contextmanager
来源：http://ga.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://qy.muxihuayi.cn

list(zip(*m))
来源：http://kj.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://qz.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lx.nicolike.cn

[U24] Py：路径操作
来源：http://tz.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sk.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://va.asd995.cn

csv.DictReader(f)
来源：http://nq.chemitech.net.cn

[U26] Py：并发下载
来源：http://ek.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kw.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://aj.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://th.wgjwhj.cn

[U28] Py：类型别名
来源：http://ll.yuntaijiaju.cn

UserId = int
来源：http://cm.lnxyls.cn

[U29] Py：属性校验
来源：http://ed.colortex.cn

@property 与 @x.setter 配合
来源：http://zk.bookmarksfly.cn

[U30] Py：数据类
来源：http://sp.nszjky.cn

@dataclass(slots=True)
来源：http://mn.hnjuh.cn

[U31] Py：单测
来源：http://ye.colortex.cn

python -m pytest -q
来源：http://zv.shxzukj.cn

[U32] Py：代码格式化
来源：http://ey.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://tn.521024.cn

[U33] Py：打包发布
来源：http://ej.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://zr.yuexingan06.cn

[U34] Py：判断编码
来源：http://uf.yuexingan06.cn

chardet.detect(raw)
来源：http://ef.9csxet.cn

[U35] Py：发送邮件
来源：http://cl.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nr.wgjwhj.cn

[U36] Py：定时任务
来源：http://zr.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://tb.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://qj.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dd.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://vr.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://yf.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://pg.jctech888.com.cn

sys.stdout.isatty()
来源：http://oi.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ey.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://po.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://yj.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bm.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://xj.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qf.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://fv.colortex.cn

namespace App\Http;
来源：http://kg.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://tr.asd995.cn

declare(strict_types=1);
来源：http://ti.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://hy.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ml.bjjhwx.cn

[U46] PHP：可空类型
来源：http://pp.shtwfgs.cn

?string $name = null
来源：http://vn.jctech888.com.cn

[U47] PHP：联合类型
来源：http://zq.nszjky.cn

int|string $id
来源：http://bg.nszjky.cn

[U48] PHP：纯枚举
来源：http://hw.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oa.szsharing.cn

[U49] PHP：只读属性
来源：http://yn.asd995.cn

public readonly string $name
来源：http://ub.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://jt.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ys.asd995.cn

[U51] PHP：数组解构
来源：http://li.muxihuayi.cn

[$a, $b] = $arr;
来源：http://fy.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://cm.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://mr.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://dn.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://cq.hnjuh.cn

[U54] PHP：空安全调用
来源：http://du.panjiajie.cn

$obj?->method()
来源：http://rv.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://hy.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ej.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://zs.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://pv.colortex.cn

[U57] PHP：字符串插值
来源：http://hp.haigaiapp.cn

"值: {$a}"
来源：http://rw.szxytkj.cn

[U58] PHP：数组三件套
来源：http://we.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://es.panjiajie.cn

[U59] PHP：自定义排序
来源：http://cn.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vb.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://xe.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dg.wgjwhj.cn

[U61] PHP：正则
来源：http://kg.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dh.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://hr.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cx.521024.cn

[U63] PHP：文件读写
来源：http://px.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sx.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://zb.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://bv.wgjwhj.cn

[U65] PHP：会话
来源：http://em.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yd.521024.cn

[U66] PHP：设置 Cookie
来源：http://fj.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jb.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://ud.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://re.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://cu.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tc.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://rz.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ur.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://jl.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vi.huanxung.cn

[U71] PHP：抛出异常
来源：http://ux.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://xj.hnjuh.cn

[U72] PHP：写错误日志
来源：http://gy.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://jw.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://tl.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://el.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://ty.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://ah.huanxung.cn

[U75] PHP：依赖注入
来源：http://bh.bjjhwx.cn

composer require psr/container
来源：http://mk.521024.cn

[U76] PHP：简单路由
来源：http://hf.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rh.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://gf.jianghongdianzi.cn

composer require twig/twig
来源：http://zr.shtwfgs.cn

[U78] PHP：单元测试
来源：http://np.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://vi.szxytkj.cn

[U79] PHP：静态分析
来源：http://hp.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://rn.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://fn.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://se.newstarts.cn

[U81] JS：初始化项目
来源：http://jf.hnjuh.cn

npm init -y;  npm i express
来源：http://mt.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://qj.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yf.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://af.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ui.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://im.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://di.muxihuayi.cn

[U85] JS：可选链
来源：http://mf.bjjhwx.cn

a?.b?.c
来源：http://nu.9csxet.cn

[U86] JS：空值合并
来源：http://xh.nicolike.cn

a ?? b
来源：http://as.muxihuayi.cn

[U87] JS：解构默认值
来源：http://xt.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://zt.hnjuh.cn

[U88] JS：对象展开合并
来源：http://qw.shxzukj.cn

{ ...a, ...b }
来源：http://zu.nszjky.cn

[U89] JS：数组去重
来源：http://rh.shxzskj.cn

[...new Set(arr)]
来源：http://xq.hnjuh.cn

[U90] JS：数字数组排序
来源：http://hs.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ql.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://fg.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sl.nszjky.cn

[U92] JS：深拷贝
来源：http://ld.szxytkj.cn

structuredClone(obj)
来源：http://dp.huanxung.cn

[U93] JS：模板字符串
来源：http://dn.bjjhwx.cn

`共 ${n} 条`
来源：http://ri.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://gl.bookmarksfly.cn

const double = x => x * 2;
来源：http://io.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://as.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://qr.hahajie.cn

[U96] JS：async/await 与异常
来源：http://jv.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tr.colortex.cn


<!-- 参考信息 -->