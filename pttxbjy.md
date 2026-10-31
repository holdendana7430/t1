代发 wailian999

[T11] Kotlin：协程
来源：http://ic.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://om.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://uv.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://mu.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://lo.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://wl.bjjhwx.cn

[T14] Kotlin：循环
来源：http://qd.szsharing.cn

for (i in 1..10) println(i)
来源：http://oz.panjiajie.cn

[T15] Kotlin：接口
来源：http://ye.huanxung.cn

interface Shape { fun area(): Double }
来源：http://iq.huanxung.cn

[T16] Swift：Hello World
来源：http://xw.9csxet.cn

print("Hello")
来源：http://fx.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ga.newstarts.cn

var a = 1;  let b = 2
来源：http://lr.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://yi.yuexingan06.cn

"值: \(b)"
来源：http://th.hnjuh.cn

[T19] Swift：可选绑定
来源：http://kt.szsharing.cn

if let n = opt { print(n) }
来源：http://me.jctech888.com.cn

[T20] Swift：数组操作
来源：http://xp.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ss.bookmarksfly.cn

[T21] Swift：遍历
来源：http://fa.bookmarksfly.cn

for x in a { print(x) }
来源：http://qi.bookmarksfly.cn

[T22] Swift：字典
来源：http://cy.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ua.521024.cn

[T23] Swift：函数
来源：http://ac.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gc.9csxet.cn

[T24] Swift：闭包
来源：http://mh.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ef.bookmarksfly.cn

[T25] Swift：结构体
来源：http://pv.szxytkj.cn

struct P { var x: Int }
来源：http://dm.huanxung.cn

[T26] Swift：类与重写
来源：http://kd.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://tc.hnjuh.cn

[T27] Swift：错误处理
来源：http://ah.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://kw.asd995.cn

[T28] Swift：枚举
来源：http://ei.szxytkj.cn

enum Color { case red, green }
来源：http://rs.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://ud.shxzukj.cn

guard let x = opt else { return }
来源：http://rh.shtwfgs.cn

[T30] Swift：协议
来源：http://nx.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://sp.wgjwhj.cn

[T31] Lua：Hello World
来源：http://oh.muxihuayi.cn

print("Hello")
来源：http://oo.9csxet.cn

[T32] Lua：局部变量
来源：http://xb.huixinmuqiang.cn

local a = 1
来源：http://oa.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://wt.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wj.jctech888.com.cn

[T34] Lua：遍历表
来源：http://fz.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zm.hahajie.cn

[T35] Lua：字典表
来源：http://re.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://hk.shxzukj.cn

[T36] Lua：函数
来源：http://zu.asd995.cn

function add(a, b) return a + b end
来源：http://wz.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://gx.521024.cn

"a" .. "b"
来源：http://ml.colortex.cn

[T38] Lua：条件
来源：http://nm.nszjky.cn

if x > 0 then print("正") end
来源：http://xo.lnxyls.cn

[T39] Lua：模式匹配
来源：http://lh.colortex.cn

string.find(s, "%d+")
来源：http://zr.haigaiapp.cn

[T40] Lua：元表
来源：http://hp.521024.cn

setmetatable({}, { __index = base })
来源：http://iq.521024.cn

[T41] Perl：Hello World
来源：http://uo.huixiangedu.cn

print "Hello\n";
来源：http://vq.9csxet.cn

[T42] Perl：变量类型
来源：http://iy.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ec.nszjky.cn

[T43] Perl：字符串插值
来源：http://rv.bookmarksfly.cn

"值: $a"
来源：http://lv.nszjky.cn

[T44] Perl：条件
来源：http://hg.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://vc.hnjuh.cn

[T45] Perl：数组遍历
来源：http://ck.asd995.cn

for my $x (@arr) { print $x; }
来源：http://dl.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://jr.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ni.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://lx.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kt.shtwfgs.cn

[T48] Perl：正则替换
来源：http://pf.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://hq.colortex.cn

[T49] Perl：函数
来源：http://jj.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qg.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://ff.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ol.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://da.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://gj.yuexingan06.cn

println("Hello")
来源：http://rj.bjjhwx.cn

[T52] Scala：变量
来源：http://tx.asd995.cn

val a = 1;  var b = 2
来源：http://db.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ol.jctech888.com.cn

s"值: $b"
来源：http://sz.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://bx.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ln.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ik.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hs.wgjwhj.cn

[T56] Scala：样例类
来源：http://os.colortex.cn

case class User(name: String, age: Int)
来源：http://ra.asd995.cn

[T57] Scala：模式匹配
来源：http://hh.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mb.nszjky.cn

[T58] Scala：函数定义
来源：http://da.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://la.521024.cn

[T59] Scala：循环
来源：http://sv.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://fh.nicolike.cn

[T60] Scala：折叠
来源：http://ax.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://il.9csxet.cn

================================================================================
来源：http://ly.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://of.gzmigu.cn

================================================================================
来源：http://fw.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://jd.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tp.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://ky.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mv.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://dn.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vo.hahajie.cn

[U04] Py：变量调试打印
来源：http://jt.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wj.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://xs.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://qj.9csxet.cn

[U06] Py：合并两个字典
来源：http://pz.hnjuh.cn

{**a, **b}
来源：http://rd.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://iq.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://ei.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://fj.shxzukj.cn

[y for x in nested for y in x]
来源：http://uz.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://mk.shxzukj.cn

max(d, key=d.get)
来源：http://da.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://mq.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yp.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://gh.shxzukj.cn

(x * 2 for x in arr)
来源：http://ad.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gi.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://yh.newstarts.cn

[U13] Py：固定长度队列
来源：http://dd.shxzskj.cn

deque(maxlen=10)
来源：http://zh.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ab.wgjwhj.cn

defaultdict(list)
来源：http://tz.hahajie.cn

[U15] Py：高精度计时
来源：http://ne.shxzskj.cn

t = time.perf_counter()
来源：http://mv.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://eq.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bm.huanxung.cn

[U17] Py：初始化日志
来源：http://la.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://wj.shxzukj.cn

[U18] Py：预编译正则
来源：http://xx.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://xh.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://ll.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kt.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://zz.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://eh.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://mo.bjjhwx.cn

@contextlib.contextmanager
来源：http://lh.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://av.hnjuh.cn

list(zip(*m))
来源：http://cm.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://ng.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://us.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ag.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ow.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://rk.panjiajie.cn

csv.DictReader(f)
来源：http://by.huanxung.cn

[U26] Py：并发下载
来源：http://gw.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yb.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://ki.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://yc.shxzukj.cn

[U28] Py：类型别名
来源：http://nh.gzmigu.cn

UserId = int
来源：http://ah.bookmarksfly.cn

[U29] Py：属性校验
来源：http://ib.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://ck.haigaiapp.cn

[U30] Py：数据类
来源：http://yz.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://ak.nicolike.cn

[U31] Py：单测
来源：http://zk.yuexingan06.cn

python -m pytest -q
来源：http://cn.gzmigu.cn

[U32] Py：代码格式化
来源：http://ht.521024.cn

ruff format . && ruff check --fix .
来源：http://fa.huanxung.cn

[U33] Py：打包发布
来源：http://az.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ba.gzmigu.cn

[U34] Py：判断编码
来源：http://he.bookmarksfly.cn

chardet.detect(raw)
来源：http://gu.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://au.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mn.wgjwhj.cn

[U36] Py：定时任务
来源：http://kz.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://xe.huanxung.cn

[U37] Py：读写 Excel
来源：http://et.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wx.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://xs.9csxet.cn

Path(__file__).resolve().parent
来源：http://nx.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://mq.chemitech.net.cn

sys.stdout.isatty()
来源：http://yy.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://qm.521024.cn

print("err", file=sys.stderr)
来源：http://di.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://ed.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iu.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://rh.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zb.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://hq.haigaiapp.cn

namespace App\Http;
来源：http://ej.colortex.cn

[U44] PHP：开启严格类型
来源：http://ny.huixiangedu.cn

declare(strict_types=1);
来源：http://on.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://cz.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tb.shxzskj.cn

[U46] PHP：可空类型
来源：http://gv.wgjwhj.cn

?string $name = null
来源：http://il.bjjhwx.cn

[U47] PHP：联合类型
来源：http://kn.szsharing.cn

int|string $id
来源：http://ax.gzmigu.cn

[U48] PHP：纯枚举
来源：http://ns.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qj.shxzukj.cn

[U49] PHP：只读属性
来源：http://pm.colortex.cn

public readonly string $name
来源：http://dg.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://bh.newstarts.cn

public function __construct(private int $id) {}
来源：http://vz.newstarts.cn

[U51] PHP：数组解构
来源：http://qk.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://me.shxzukj.cn

[U52] PHP：箭头函数
来源：http://pv.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://vx.colortex.cn

[U53] PHP：空合并运算符
来源：http://rv.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://kd.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://qq.bookmarksfly.cn

$obj?->method()
来源：http://rv.szxytkj.cn

[U55] PHP：match 表达式
来源：http://so.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gd.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://zt.shxzskj.cn

f(a: 1, b: 2)
来源：http://ec.asd995.cn

[U57] PHP：字符串插值
来源：http://fk.yuntaijiaju.cn

"值: {$a}"
来源：http://lb.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ml.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zd.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://og.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ug.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://mp.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yv.jctech888.com.cn

[U61] PHP：正则
来源：http://ca.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hk.bjjhwx.cn

[U62] PHP：日期对象
来源：http://it.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sz.yuexingan06.cn

[U63] PHP：文件读写
来源：http://pt.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qk.hahajie.cn

[U64] PHP：目录遍历
来源：http://ux.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://wo.panjiajie.cn

[U65] PHP：会话
来源：http://el.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aj.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://fc.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://te.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://zh.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vb.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://ap.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zr.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://nf.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://om.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://sh.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tb.nszjky.cn

[U71] PHP：抛出异常
来源：http://hj.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://wv.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ym.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://to.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://yc.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://hg.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://dd.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://hw.shxzskj.cn

[U75] PHP：依赖注入
来源：http://vp.yuntaijiaju.cn

composer require psr/container
来源：http://bv.huixiangedu.cn

[U76] PHP：简单路由
来源：http://fg.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ju.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://hl.huixinmuqiang.cn

composer require twig/twig
来源：http://zp.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ek.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://ym.bjjhwx.cn

[U79] PHP：静态分析
来源：http://nz.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://zr.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://jr.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vs.muxihuayi.cn

[U81] JS：初始化项目
来源：http://br.yuexingan06.cn

npm init -y;  npm i express
来源：http://ba.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://mc.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sf.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://tm.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://za.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://zi.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ed.asd995.cn

[U85] JS：可选链
来源：http://jz.wgjwhj.cn

a?.b?.c
来源：http://tb.shxzskj.cn

[U86] JS：空值合并
来源：http://sp.bookmarksfly.cn

a ?? b
来源：http://uu.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://zr.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://ct.nicolike.cn

[U88] JS：对象展开合并
来源：http://hn.nszjky.cn

{ ...a, ...b }
来源：http://kl.shtwfgs.cn

[U89] JS：数组去重
来源：http://ng.lnxyls.cn

[...new Set(arr)]
来源：http://ko.shxzskj.cn

[U90] JS：数字数组排序
来源：http://ra.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://yw.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://xs.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mh.asd995.cn

[U92] JS：深拷贝
来源：http://xl.lnxyls.cn

structuredClone(obj)
来源：http://eb.szsharing.cn

[U93] JS：模板字符串
来源：http://mt.panjiajie.cn

`共 ${n} 条`
来源：http://mf.nszjky.cn

[U94] JS：箭头函数
来源：http://wq.colortex.cn

const double = x => x * 2;
来源：http://yf.colortex.cn

[U95] JS：Promise 包装
来源：http://gi.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://at.hahajie.cn

[U96] JS：async/await 与异常
来源：http://xi.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ve.szxytkj.cn

[U97] JS：并发请求
来源：http://yt.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ba.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://tz.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gx.huixinmuqiang.cn


<!-- 参考信息 -->