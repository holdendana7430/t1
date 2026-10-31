代发 wailian999

[T09] Kotlin：扩展函数
来源：http://in.asd995.cn

fun String.exclaim() = this + "!"
来源：http://nh.asd995.cn

[T10] Kotlin：默认参数
来源：http://yx.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uj.asd995.cn

[T11] Kotlin：协程
来源：http://ie.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rw.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ru.521024.cn

val (a, b) = Pair(1, 2)
来源：http://tm.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://ol.hahajie.cn

val m = mapOf("a" to 1)
来源：http://ac.muxihuayi.cn

[T14] Kotlin：循环
来源：http://wh.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://wp.521024.cn

[T15] Kotlin：接口
来源：http://us.huanxung.cn

interface Shape { fun area(): Double }
来源：http://nr.bjjhwx.cn

[T16] Swift：Hello World
来源：http://un.szxytkj.cn

print("Hello")
来源：http://yk.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://fk.nicolike.cn

var a = 1;  let b = 2
来源：http://gs.shxzskj.cn

[T18] Swift：字符串插值
来源：http://af.szxytkj.cn

"值: \(b)"
来源：http://jb.huanxung.cn

[T19] Swift：可选绑定
来源：http://ni.nszjky.cn

if let n = opt { print(n) }
来源：http://fh.chemitech.net.cn

[T20] Swift：数组操作
来源：http://rg.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ft.huixiangedu.cn

[T21] Swift：遍历
来源：http://or.huixiangedu.cn

for x in a { print(x) }
来源：http://sg.hahajie.cn

[T22] Swift：字典
来源：http://pz.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mg.shtwfgs.cn

[T23] Swift：函数
来源：http://pn.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lm.9csxet.cn

[T24] Swift：闭包
来源：http://ek.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qd.huixiangedu.cn

[T25] Swift：结构体
来源：http://yt.yuntaijiaju.cn

struct P { var x: Int }
来源：http://po.shxzukj.cn

[T26] Swift：类与重写
来源：http://an.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://hl.huanxung.cn

[T27] Swift：错误处理
来源：http://sh.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://lg.chemitech.net.cn

[T28] Swift：枚举
来源：http://ps.newstarts.cn

enum Color { case red, green }
来源：http://zv.asd995.cn

[T29] Swift：guard 提前返回
来源：http://ys.nicolike.cn

guard let x = opt else { return }
来源：http://lc.bookmarksfly.cn

[T30] Swift：协议
来源：http://sj.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ti.haigaiapp.cn

[T31] Lua：Hello World
来源：http://hz.nicolike.cn

print("Hello")
来源：http://wk.nszjky.cn

[T32] Lua：局部变量
来源：http://lf.bjjhwx.cn

local a = 1
来源：http://wi.nicolike.cn

[T33] Lua：表（数组）
来源：http://ht.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xp.nszjky.cn

[T34] Lua：遍历表
来源：http://vd.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qr.panjiajie.cn

[T35] Lua：字典表
来源：http://js.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://ut.panjiajie.cn

[T36] Lua：函数
来源：http://ku.shxzukj.cn

function add(a, b) return a + b end
来源：http://bm.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://rx.szxytkj.cn

"a" .. "b"
来源：http://no.gzmigu.cn

[T38] Lua：条件
来源：http://gc.szsharing.cn

if x > 0 then print("正") end
来源：http://lc.newstarts.cn

[T39] Lua：模式匹配
来源：http://ev.wgjwhj.cn

string.find(s, "%d+")
来源：http://oj.shxzukj.cn

[T40] Lua：元表
来源：http://ut.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://nd.huixiangedu.cn

[T41] Perl：Hello World
来源：http://xr.colortex.cn

print "Hello\n";
来源：http://ia.nicolike.cn

[T42] Perl：变量类型
来源：http://hb.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ei.lnxyls.cn

[T43] Perl：字符串插值
来源：http://uv.szxytkj.cn

"值: $a"
来源：http://jo.9csxet.cn

[T44] Perl：条件
来源：http://jq.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://yj.shxzskj.cn

[T45] Perl：数组遍历
来源：http://uu.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://rl.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://pz.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vo.colortex.cn

[T47] Perl：正则捕获
来源：http://ar.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ex.colortex.cn

[T48] Perl：正则替换
来源：http://un.shxzukj.cn

$s =~ s/old/new/g;
来源：http://mv.nicolike.cn

[T49] Perl：函数
来源：http://zt.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lc.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://dv.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jp.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://fq.shxzskj.cn

[T51] Scala：Hello World
来源：http://fz.bjjhwx.cn

println("Hello")
来源：http://wq.shxzukj.cn

[T52] Scala：变量
来源：http://fr.szsharing.cn

val a = 1;  var b = 2
来源：http://yl.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://zt.haigaiapp.cn

s"值: $b"
来源：http://zm.szxytkj.cn

[T54] Scala：集合映射
来源：http://aw.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://ef.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://bv.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://es.nszjky.cn

[T56] Scala：样例类
来源：http://xd.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://sm.panjiajie.cn

[T57] Scala：模式匹配
来源：http://wq.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ed.shtwfgs.cn

[T58] Scala：函数定义
来源：http://qp.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zj.gzmigu.cn

[T59] Scala：循环
来源：http://rm.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://bv.huixiangedu.cn

[T60] Scala：折叠
来源：http://sg.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vi.szxytkj.cn

================================================================================
来源：http://mt.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iz.haigaiapp.cn

================================================================================
来源：http://le.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://ui.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ek.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://ih.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uz.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://aj.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ys.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://pp.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://na.nicolike.cn

[U05] Py：列表去重且保序
来源：http://pt.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://xz.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://zg.muxihuayi.cn

{**a, **b}
来源：http://ky.gzmigu.cn

[U07] Py：反转字典键值
来源：http://lg.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://kz.szsharing.cn

[U08] Py：展平二维列表
来源：http://us.bjjhwx.cn

[y for x in nested for y in x]
来源：http://fo.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://yq.huanxung.cn

max(d, key=d.get)
来源：http://gu.521024.cn

[U10] Py：按值排序字典
来源：http://bp.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ep.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://tv.521024.cn

(x * 2 for x in arr)
来源：http://wl.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tf.colortex.cn

Counter(arr).most_common(3)
来源：http://gd.521024.cn

[U13] Py：固定长度队列
来源：http://ts.hnjuh.cn

deque(maxlen=10)
来源：http://uj.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://av.shtwfgs.cn

defaultdict(list)
来源：http://zj.panjiajie.cn

[U15] Py：高精度计时
来源：http://pm.hnjuh.cn

t = time.perf_counter()
来源：http://co.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://ob.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sm.shxzukj.cn

[U17] Py：初始化日志
来源：http://zq.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://xh.colortex.cn

[U18] Py：预编译正则
来源：http://qk.huanxung.cn

pat = re.compile(r"\d+")
来源：http://tu.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://ld.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jt.szsharing.cn

[U20] Py：缓存函数结果
来源：http://uq.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://zd.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://ea.521024.cn

@contextlib.contextmanager
来源：http://mq.nicolike.cn

[U22] Py：矩阵转置
来源：http://xg.colortex.cn

list(zip(*m))
来源：http://ls.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://bk.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vb.colortex.cn

[U24] Py：路径操作
来源：http://de.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://re.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://hh.shtwfgs.cn

csv.DictReader(f)
来源：http://bs.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://fm.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lv.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://li.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://uh.nszjky.cn

[U28] Py：类型别名
来源：http://bv.521024.cn

UserId = int
来源：http://yl.shtwfgs.cn

[U29] Py：属性校验
来源：http://tn.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://gu.nszjky.cn

[U30] Py：数据类
来源：http://yd.bookmarksfly.cn

@dataclass(slots=True)
来源：http://cd.asd995.cn

[U31] Py：单测
来源：http://px.jctech888.com.cn

python -m pytest -q
来源：http://gc.bjjhwx.cn

[U32] Py：代码格式化
来源：http://jp.newstarts.cn

ruff format . && ruff check --fix .
来源：http://su.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://mo.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://zx.huanxung.cn

[U34] Py：判断编码
来源：http://kn.shxzukj.cn

chardet.detect(raw)
来源：http://un.shxzskj.cn

[U35] Py：发送邮件
来源：http://wd.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://no.521024.cn

[U36] Py：定时任务
来源：http://eh.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://xq.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://pr.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://md.521024.cn

[U38] Py：获取脚本所在目录
来源：http://ha.asd995.cn

Path(__file__).resolve().parent
来源：http://ek.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://yq.jctech888.com.cn

sys.stdout.isatty()
来源：http://ld.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ke.nicolike.cn

print("err", file=sys.stderr)
来源：http://ah.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://pt.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yd.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://jf.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nl.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://la.yuntaijiaju.cn

namespace App\Http;
来源：http://jh.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://md.nicolike.cn

declare(strict_types=1);
来源：http://qo.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://vc.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jk.9csxet.cn

[U46] PHP：可空类型
来源：http://ey.bjjhwx.cn

?string $name = null
来源：http://hk.gzmigu.cn

[U47] PHP：联合类型
来源：http://bb.newstarts.cn

int|string $id
来源：http://lt.huanxung.cn

[U48] PHP：纯枚举
来源：http://zy.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ck.newstarts.cn

[U49] PHP：只读属性
来源：http://ad.shtwfgs.cn

public readonly string $name
来源：http://sq.colortex.cn

[U50] PHP：构造器属性提升
来源：http://lw.nszjky.cn

public function __construct(private int $id) {}
来源：http://np.shtwfgs.cn

[U51] PHP：数组解构
来源：http://lw.huanxung.cn

[$a, $b] = $arr;
来源：http://wf.panjiajie.cn

[U52] PHP：箭头函数
来源：http://fy.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://zi.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://wo.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://go.panjiajie.cn

[U54] PHP：空安全调用
来源：http://oz.jianghongdianzi.cn

$obj?->method()
来源：http://lu.szsharing.cn

[U55] PHP：match 表达式
来源：http://mf.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ro.jctech888.com.cn

[U56] PHP：命名参数
来源：http://ar.colortex.cn

f(a: 1, b: 2)
来源：http://ds.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://tb.lnxyls.cn

"值: {$a}"
来源：http://bk.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://wh.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tx.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://dt.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vq.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://ve.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pk.gzmigu.cn

[U61] PHP：正则
来源：http://kb.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://as.szxytkj.cn

[U62] PHP：日期对象
来源：http://ce.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gk.haigaiapp.cn

[U63] PHP：文件读写
来源：http://xl.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tf.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://zs.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://ip.nszjky.cn

[U65] PHP：会话
来源：http://pd.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hl.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://za.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lx.colortex.cn

[U67] PHP：处理文件上传
来源：http://wt.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fs.huanxung.cn

[U68] PHP：PDO 连接
来源：http://nk.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yy.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://gs.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sy.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://em.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pd.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://px.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://br.nicolike.cn

[U72] PHP：写错误日志
来源：http://nj.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://sp.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://pt.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://hy.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://nk.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://ea.hnjuh.cn

[U75] PHP：依赖注入
来源：http://fv.panjiajie.cn

composer require psr/container
来源：http://mr.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://fs.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kn.lnxyls.cn

[U77] PHP：模板渲染
来源：http://fj.nicolike.cn

composer require twig/twig
来源：http://rg.chemitech.net.cn

[U78] PHP：单元测试
来源：http://mf.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://eu.521024.cn

[U79] PHP：静态分析
来源：http://sk.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://ym.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://kd.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jx.9csxet.cn

[U81] JS：初始化项目
来源：http://nj.bookmarksfly.cn

npm init -y;  npm i express
来源：http://hk.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://vz.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pf.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://ne.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cd.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://vo.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wi.bjjhwx.cn

[U85] JS：可选链
来源：http://lh.huixinmuqiang.cn

a?.b?.c
来源：http://hx.shxzskj.cn

[U86] JS：空值合并
来源：http://kt.jianghongdianzi.cn

a ?? b
来源：http://tn.521024.cn

[U87] JS：解构默认值
来源：http://uz.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://fv.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://kb.jianghongdianzi.cn

{ ...a, ...b }
来源：http://db.muxihuayi.cn

[U89] JS：数组去重
来源：http://cl.chemitech.net.cn

[...new Set(arr)]
来源：http://ug.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://zd.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://ve.asd995.cn

[U91] JS：对象键值遍历
来源：http://on.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.hahajie.cn

[U92] JS：深拷贝
来源：http://mo.shxzskj.cn

structuredClone(obj)
来源：http://zl.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://ba.jianghongdianzi.cn

`共 ${n} 条`
来源：http://jt.nszjky.cn

[U94] JS：箭头函数
来源：http://nv.panjiajie.cn

const double = x => x * 2;
来源：http://vq.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://ws.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://om.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://yl.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ia.wgjwhj.cn


<!-- 参考信息 -->