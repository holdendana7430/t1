代发 wailian999

[T11] Kotlin：协程
来源：http://vn.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lg.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://do.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://nr.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://ly.asd995.cn

val m = mapOf("a" to 1)
来源：http://al.lnxyls.cn

[T14] Kotlin：循环
来源：http://xr.shxzukj.cn

for (i in 1..10) println(i)
来源：http://gv.panjiajie.cn

[T15] Kotlin：接口
来源：http://nf.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://do.shxzukj.cn

[T16] Swift：Hello World
来源：http://vo.shxzukj.cn

print("Hello")
来源：http://ju.nicolike.cn

[T17] Swift：变量与常量
来源：http://xr.szsharing.cn

var a = 1;  let b = 2
来源：http://hs.asd995.cn

[T18] Swift：字符串插值
来源：http://gp.asd995.cn

"值: \(b)"
来源：http://ad.hnjuh.cn

[T19] Swift：可选绑定
来源：http://hp.muxihuayi.cn

if let n = opt { print(n) }
来源：http://av.shtwfgs.cn

[T20] Swift：数组操作
来源：http://cd.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xt.shxzskj.cn

[T21] Swift：遍历
来源：http://px.bookmarksfly.cn

for x in a { print(x) }
来源：http://rk.lnxyls.cn

[T22] Swift：字典
来源：http://ac.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://it.asd995.cn

[T23] Swift：函数
来源：http://bo.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://la.shxzukj.cn

[T24] Swift：闭包
来源：http://ad.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pn.shxzskj.cn

[T25] Swift：结构体
来源：http://fd.haigaiapp.cn

struct P { var x: Int }
来源：http://jw.gzmigu.cn

[T26] Swift：类与重写
来源：http://an.shxzukj.cn

class A: Base { override func f() {} }
来源：http://uk.hnjuh.cn

[T27] Swift：错误处理
来源：http://ve.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://mz.lnxyls.cn

[T28] Swift：枚举
来源：http://du.szxytkj.cn

enum Color { case red, green }
来源：http://dp.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://me.shxzskj.cn

guard let x = opt else { return }
来源：http://ss.panjiajie.cn

[T30] Swift：协议
来源：http://bc.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://fz.lnxyls.cn

[T31] Lua：Hello World
来源：http://mw.bookmarksfly.cn

print("Hello")
来源：http://ux.shxzskj.cn

[T32] Lua：局部变量
来源：http://dn.521024.cn

local a = 1
来源：http://ti.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://ok.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sf.huixiangedu.cn

[T34] Lua：遍历表
来源：http://fo.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ln.colortex.cn

[T35] Lua：字典表
来源：http://fs.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://wj.gzmigu.cn

[T36] Lua：函数
来源：http://ar.hnjuh.cn

function add(a, b) return a + b end
来源：http://op.hahajie.cn

[T37] Lua：字符串拼接
来源：http://dj.jianghongdianzi.cn

"a" .. "b"
来源：http://nk.muxihuayi.cn

[T38] Lua：条件
来源：http://hv.nicolike.cn

if x > 0 then print("正") end
来源：http://zn.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://sr.szxytkj.cn

string.find(s, "%d+")
来源：http://cq.newstarts.cn

[T40] Lua：元表
来源：http://vw.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://ti.asd995.cn

[T41] Perl：Hello World
来源：http://ue.chemitech.net.cn

print "Hello\n";
来源：http://qw.9csxet.cn

[T42] Perl：变量类型
来源：http://gt.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fx.hnjuh.cn

[T43] Perl：字符串插值
来源：http://ix.muxihuayi.cn

"值: $a"
来源：http://rm.newstarts.cn

[T44] Perl：条件
来源：http://md.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ir.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://fe.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://qt.shxzskj.cn

[T46] Perl：哈希操作
来源：http://af.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uw.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://jz.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hp.shtwfgs.cn

[T48] Perl：正则替换
来源：http://ja.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://hi.huanxung.cn

[T49] Perl：函数
来源：http://yt.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://io.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://kp.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vn.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://sq.hnjuh.cn

[T51] Scala：Hello World
来源：http://sl.jctech888.com.cn

println("Hello")
来源：http://nh.asd995.cn

[T52] Scala：变量
来源：http://eo.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://pn.521024.cn

[T53] Scala：字符串插值
来源：http://ur.chemitech.net.cn

s"值: $b"
来源：http://yw.szxytkj.cn

[T54] Scala：集合映射
来源：http://hd.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://rc.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://cs.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qu.lnxyls.cn

[T56] Scala：样例类
来源：http://up.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://cz.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://me.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gf.szsharing.cn

[T58] Scala：函数定义
来源：http://vn.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ih.asd995.cn

[T59] Scala：循环
来源：http://oa.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://mn.shxzskj.cn

[T60] Scala：折叠
来源：http://bl.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ep.jctech888.com.cn

================================================================================
来源：http://ln.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pa.wgjwhj.cn

================================================================================
来源：http://fx.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://ea.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jx.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://tj.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fb.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://xu.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sk.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://au.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ro.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://tm.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://jg.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://ry.lnxyls.cn

{**a, **b}
来源：http://ik.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://lx.colortex.cn

{v: k for k, v in d.items()}
来源：http://bm.hahajie.cn

[U08] Py：展平二维列表
来源：http://ov.jctech888.com.cn

[y for x in nested for y in x]
来源：http://xt.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://qx.haigaiapp.cn

max(d, key=d.get)
来源：http://uj.szxytkj.cn

[U10] Py：按值排序字典
来源：http://ae.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://np.shxzukj.cn

[U11] Py：生成器表达式
来源：http://kr.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://wh.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ht.panjiajie.cn

Counter(arr).most_common(3)
来源：http://uq.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://hl.colortex.cn

deque(maxlen=10)
来源：http://pq.newstarts.cn

[U14] Py：分组收集到列表
来源：http://xy.yuexingan06.cn

defaultdict(list)
来源：http://ry.shtwfgs.cn

[U15] Py：高精度计时
来源：http://cg.nicolike.cn

t = time.perf_counter()
来源：http://ke.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://io.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://td.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://gc.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://gl.szxytkj.cn

[U18] Py：预编译正则
来源：http://bu.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://vb.521024.cn

[U19] Py：正则替换带回调
来源：http://aj.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ot.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://xr.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://uk.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ka.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://gc.hahajie.cn

[U22] Py：矩阵转置
来源：http://oc.hnjuh.cn

list(zip(*m))
来源：http://wv.9csxet.cn

[U23] Py：分块读取大文件
来源：http://yo.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ze.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://dc.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pq.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://pz.521024.cn

csv.DictReader(f)
来源：http://ny.jctech888.com.cn

[U26] Py：并发下载
来源：http://gd.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sl.hahajie.cn

[U27] Py：异步 HTTP
来源：http://yl.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ci.muxihuayi.cn

[U28] Py：类型别名
来源：http://xv.yuntaijiaju.cn

UserId = int
来源：http://gw.haigaiapp.cn

[U29] Py：属性校验
来源：http://re.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://dw.nszjky.cn

[U30] Py：数据类
来源：http://ig.shtwfgs.cn

@dataclass(slots=True)
来源：http://px.huanxung.cn

[U31] Py：单测
来源：http://iz.jianghongdianzi.cn

python -m pytest -q
来源：http://iy.chemitech.net.cn

[U32] Py：代码格式化
来源：http://sq.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://cv.shxzukj.cn

[U33] Py：打包发布
来源：http://cq.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://ls.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://zd.wgjwhj.cn

chardet.detect(raw)
来源：http://ie.nszjky.cn

[U35] Py：发送邮件
来源：http://sn.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hq.shxzukj.cn

[U36] Py：定时任务
来源：http://ju.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://yh.newstarts.cn

[U37] Py：读写 Excel
来源：http://bx.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mb.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://gx.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://wf.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://in.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://vz.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://wh.huanxung.cn

print("err", file=sys.stderr)
来源：http://qz.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ix.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yr.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://en.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pe.newstarts.cn

[U43] PHP：声明命名空间
来源：http://in.shtwfgs.cn

namespace App\Http;
来源：http://br.huanxung.cn

[U44] PHP：开启严格类型
来源：http://eh.gzmigu.cn

declare(strict_types=1);
来源：http://nl.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://ut.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yb.gzmigu.cn

[U46] PHP：可空类型
来源：http://rr.huixiangedu.cn

?string $name = null
来源：http://qy.muxihuayi.cn

[U47] PHP：联合类型
来源：http://ww.haigaiapp.cn

int|string $id
来源：http://qu.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://wg.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bi.521024.cn

[U49] PHP：只读属性
来源：http://yu.shtwfgs.cn

public readonly string $name
来源：http://cy.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://qs.521024.cn

public function __construct(private int $id) {}
来源：http://vb.panjiajie.cn

[U51] PHP：数组解构
来源：http://zd.wgjwhj.cn

[$a, $b] = $arr;
来源：http://rm.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://xi.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://mv.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://pt.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://vc.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://bi.chemitech.net.cn

$obj?->method()
来源：http://hi.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://ee.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ah.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://wy.hnjuh.cn

f(a: 1, b: 2)
来源：http://qa.colortex.cn

[U57] PHP：字符串插值
来源：http://de.shtwfgs.cn

"值: {$a}"
来源：http://od.colortex.cn

[U58] PHP：数组三件套
来源：http://uv.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sk.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://ft.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hk.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://sx.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ui.huixinmuqiang.cn

[U61] PHP：正则
来源：http://rd.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sc.bjjhwx.cn

[U62] PHP：日期对象
来源：http://wu.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jl.szxytkj.cn

[U63] PHP：文件读写
来源：http://ej.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fj.newstarts.cn

[U64] PHP：目录遍历
来源：http://dx.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://li.muxihuayi.cn

[U65] PHP：会话
来源：http://mb.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vb.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://zw.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ul.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://an.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ns.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://ep.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rc.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://gv.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lo.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://aw.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rh.newstarts.cn

[U71] PHP：抛出异常
来源：http://vx.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://ll.newstarts.cn

[U72] PHP：写错误日志
来源：http://sd.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://wz.521024.cn

[U73] PHP：读取 ini 配置
来源：http://lm.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://jn.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://pz.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://cg.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://jb.huixiangedu.cn

composer require psr/container
来源：http://og.muxihuayi.cn

[U76] PHP：简单路由
来源：http://we.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qi.nicolike.cn

[U77] PHP：模板渲染
来源：http://sg.jianghongdianzi.cn

composer require twig/twig
来源：http://ol.szxytkj.cn

[U78] PHP：单元测试
来源：http://bi.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://ei.chemitech.net.cn

[U79] PHP：静态分析
来源：http://ch.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://tj.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://tz.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uf.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://ze.huixiangedu.cn

npm init -y;  npm i express
来源：http://so.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://kh.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://za.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://mb.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cm.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://et.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mz.muxihuayi.cn

[U85] JS：可选链
来源：http://vm.lnxyls.cn

a?.b?.c
来源：http://fg.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://oq.chemitech.net.cn

a ?? b
来源：http://fa.shxzukj.cn

[U87] JS：解构默认值
来源：http://hh.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ya.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://ue.hnjuh.cn

{ ...a, ...b }
来源：http://wg.nicolike.cn

[U89] JS：数组去重
来源：http://mf.521024.cn

[...new Set(arr)]
来源：http://ke.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://lh.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://cu.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://jv.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ug.huanxung.cn

[U92] JS：深拷贝
来源：http://br.bjjhwx.cn

structuredClone(obj)
来源：http://je.lnxyls.cn

[U93] JS：模板字符串
来源：http://hm.gzmigu.cn

`共 ${n} 条`
来源：http://bi.nszjky.cn

[U94] JS：箭头函数
来源：http://gu.huixiangedu.cn

const double = x => x * 2;
来源：http://dt.9csxet.cn

[U95] JS：Promise 包装
来源：http://vk.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://so.hahajie.cn

[U96] JS：async/await 与异常
来源：http://ii.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sz.newstarts.cn

[U97] JS：并发请求
来源：http://ie.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://qv.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ii.bookmarksfly.cn


<!-- 参考信息 -->