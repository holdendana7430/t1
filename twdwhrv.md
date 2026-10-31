代发 wailian999

[T21] Swift：遍历
来源：http://zp.huixiangedu.cn

for x in a { print(x) }
来源：http://yx.bookmarksfly.cn

[T22] Swift：字典
来源：http://ub.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ab.hahajie.cn

[T23] Swift：函数
来源：http://tu.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://in.gzmigu.cn

[T24] Swift：闭包
来源：http://xd.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ee.hnjuh.cn

[T25] Swift：结构体
来源：http://kc.szsharing.cn

struct P { var x: Int }
来源：http://hl.colortex.cn

[T26] Swift：类与重写
来源：http://bo.asd995.cn

class A: Base { override func f() {} }
来源：http://pp.panjiajie.cn

[T27] Swift：错误处理
来源：http://bf.hahajie.cn

do { try f() } catch { print(error) }
来源：http://xe.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://lc.lnxyls.cn

enum Color { case red, green }
来源：http://bs.asd995.cn

[T29] Swift：guard 提前返回
来源：http://mb.huanxung.cn

guard let x = opt else { return }
来源：http://vu.huanxung.cn

[T30] Swift：协议
来源：http://qa.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://tf.shtwfgs.cn

[T31] Lua：Hello World
来源：http://gd.hnjuh.cn

print("Hello")
来源：http://bj.jctech888.com.cn

[T32] Lua：局部变量
来源：http://gl.panjiajie.cn

local a = 1
来源：http://ew.szsharing.cn

[T33] Lua：表（数组）
来源：http://aq.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gg.muxihuayi.cn

[T34] Lua：遍历表
来源：http://as.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qi.521024.cn

[T35] Lua：字典表
来源：http://mv.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://sw.gzmigu.cn

[T36] Lua：函数
来源：http://xk.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://tr.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://jv.shxzukj.cn

"a" .. "b"
来源：http://dk.shxzukj.cn

[T38] Lua：条件
来源：http://pi.muxihuayi.cn

if x > 0 then print("正") end
来源：http://lx.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://ff.colortex.cn

string.find(s, "%d+")
来源：http://ay.bjjhwx.cn

[T40] Lua：元表
来源：http://dk.9csxet.cn

setmetatable({}, { __index = base })
来源：http://qb.shxzukj.cn

[T41] Perl：Hello World
来源：http://zq.yuexingan06.cn

print "Hello\n";
来源：http://cr.szxytkj.cn

[T42] Perl：变量类型
来源：http://rr.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lr.nszjky.cn

[T43] Perl：字符串插值
来源：http://fn.shtwfgs.cn

"值: $a"
来源：http://fz.hnjuh.cn

[T44] Perl：条件
来源：http://hb.521024.cn

if ($a > 0) { print "正"; }
来源：http://ju.huanxung.cn

[T45] Perl：数组遍历
来源：http://jq.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://nq.9csxet.cn

[T46] Perl：哈希操作
来源：http://wi.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kc.shxzskj.cn

[T47] Perl：正则捕获
来源：http://hy.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fs.szsharing.cn

[T48] Perl：正则替换
来源：http://lf.panjiajie.cn

$s =~ s/old/new/g;
来源：http://ag.huanxung.cn

[T49] Perl：函数
来源：http://ql.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sa.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://sp.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rw.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://bh.hahajie.cn

[T51] Scala：Hello World
来源：http://ie.gzmigu.cn

println("Hello")
来源：http://ml.colortex.cn

[T52] Scala：变量
来源：http://tv.asd995.cn

val a = 1;  var b = 2
来源：http://gm.hnjuh.cn

[T53] Scala：字符串插值
来源：http://xr.jctech888.com.cn

s"值: $b"
来源：http://is.szxytkj.cn

[T54] Scala：集合映射
来源：http://fg.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://dq.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://fh.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wq.lnxyls.cn

[T56] Scala：样例类
来源：http://jz.szxytkj.cn

case class User(name: String, age: Int)
来源：http://kv.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://xp.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fg.huixiangedu.cn

[T58] Scala：函数定义
来源：http://xz.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wv.shxzukj.cn

[T59] Scala：循环
来源：http://ih.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://xa.haigaiapp.cn

[T60] Scala：折叠
来源：http://gf.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eh.huanxung.cn

================================================================================
来源：http://ez.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wh.521024.cn

================================================================================
来源：http://mi.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://lh.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mq.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://rd.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ew.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://hs.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://er.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://ef.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mc.newstarts.cn

[U05] Py：列表去重且保序
来源：http://ea.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://rw.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://eb.bookmarksfly.cn

{**a, **b}
来源：http://ye.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://mu.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://fb.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://pw.wgjwhj.cn

[y for x in nested for y in x]
来源：http://tc.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://vm.shxzukj.cn

max(d, key=d.get)
来源：http://ds.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://iy.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cr.panjiajie.cn

[U11] Py：生成器表达式
来源：http://sh.haigaiapp.cn

(x * 2 for x in arr)
来源：http://zs.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ww.shxzskj.cn

Counter(arr).most_common(3)
来源：http://co.gzmigu.cn

[U13] Py：固定长度队列
来源：http://qs.jianghongdianzi.cn

deque(maxlen=10)
来源：http://fb.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://dv.huixinmuqiang.cn

defaultdict(list)
来源：http://ai.huanxung.cn

[U15] Py：高精度计时
来源：http://pz.panjiajie.cn

t = time.perf_counter()
来源：http://kx.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://nt.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fs.haigaiapp.cn

[U17] Py：初始化日志
来源：http://cy.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://iw.nicolike.cn

[U18] Py：预编译正则
来源：http://ho.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://bg.hahajie.cn

[U19] Py：正则替换带回调
来源：http://wn.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ie.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://nd.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://mp.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://yv.haigaiapp.cn

@contextlib.contextmanager
来源：http://ie.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://em.chemitech.net.cn

list(zip(*m))
来源：http://ze.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://kk.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qe.muxihuayi.cn

[U24] Py：路径操作
来源：http://dm.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ga.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://qn.panjiajie.cn

csv.DictReader(f)
来源：http://if.huixiangedu.cn

[U26] Py：并发下载
来源：http://on.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xx.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://cj.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://vc.9csxet.cn

[U28] Py：类型别名
来源：http://wl.panjiajie.cn

UserId = int
来源：http://ei.muxihuayi.cn

[U29] Py：属性校验
来源：http://rb.nszjky.cn

@property 与 @x.setter 配合
来源：http://vi.szxytkj.cn

[U30] Py：数据类
来源：http://pq.huanxung.cn

@dataclass(slots=True)
来源：http://zt.bjjhwx.cn

[U31] Py：单测
来源：http://or.newstarts.cn

python -m pytest -q
来源：http://cm.szsharing.cn

[U32] Py：代码格式化
来源：http://ix.521024.cn

ruff format . && ruff check --fix .
来源：http://pv.asd995.cn

[U33] Py：打包发布
来源：http://hs.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://nr.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://uu.huixinmuqiang.cn

chardet.detect(raw)
来源：http://zq.nszjky.cn

[U35] Py：发送邮件
来源：http://oj.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ft.bjjhwx.cn

[U36] Py：定时任务
来源：http://hv.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://gi.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://ii.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dc.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://ga.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://tz.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://zb.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://xq.9csxet.cn

[U40] Py：打印到标准错误
来源：http://nk.gzmigu.cn

print("err", file=sys.stderr)
来源：http://yx.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://vs.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cv.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://fj.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lg.newstarts.cn

[U43] PHP：声明命名空间
来源：http://xo.panjiajie.cn

namespace App\Http;
来源：http://ew.asd995.cn

[U44] PHP：开启严格类型
来源：http://pr.hahajie.cn

declare(strict_types=1);
来源：http://oq.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://jq.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.shtwfgs.cn

[U46] PHP：可空类型
来源：http://ku.panjiajie.cn

?string $name = null
来源：http://hw.huixiangedu.cn

[U47] PHP：联合类型
来源：http://zq.nszjky.cn

int|string $id
来源：http://qp.szsharing.cn

[U48] PHP：纯枚举
来源：http://ab.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wl.shxzskj.cn

[U49] PHP：只读属性
来源：http://rk.colortex.cn

public readonly string $name
来源：http://fg.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://lg.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://iz.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://tc.bjjhwx.cn

[$a, $b] = $arr;
来源：http://sf.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://zx.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://lj.hahajie.cn

[U53] PHP：空合并运算符
来源：http://hp.521024.cn

$v = $a ?? $b ?? "default";
来源：http://vg.newstarts.cn

[U54] PHP：空安全调用
来源：http://fl.bookmarksfly.cn

$obj?->method()
来源：http://kx.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://zk.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ni.wgjwhj.cn

[U56] PHP：命名参数
来源：http://aj.521024.cn

f(a: 1, b: 2)
来源：http://ey.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://hc.gzmigu.cn

"值: {$a}"
来源：http://qz.colortex.cn

[U58] PHP：数组三件套
来源：http://wq.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vy.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://wf.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pm.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://jk.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bf.muxihuayi.cn

[U61] PHP：正则
来源：http://sl.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rr.bjjhwx.cn

[U62] PHP：日期对象
来源：http://gv.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://js.newstarts.cn

[U63] PHP：文件读写
来源：http://hb.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hp.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://wv.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://zg.9csxet.cn

[U65] PHP：会话
来源：http://by.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fw.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://os.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://te.huanxung.cn

[U67] PHP：处理文件上传
来源：http://be.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fx.colortex.cn

[U68] PHP：PDO 连接
来源：http://dz.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wa.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://lr.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nl.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://qi.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nj.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://iz.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://qw.lnxyls.cn

[U72] PHP：写错误日志
来源：http://ln.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://lx.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://mj.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ie.newstarts.cn

[U74] PHP：读取环境变量
来源：http://jn.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://hw.521024.cn

[U75] PHP：依赖注入
来源：http://mw.asd995.cn

composer require psr/container
来源：http://uy.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://ji.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ms.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://or.colortex.cn

composer require twig/twig
来源：http://ul.gzmigu.cn

[U78] PHP：单元测试
来源：http://hc.colortex.cn

composer require --dev phpunit/phpunit
来源：http://cf.asd995.cn

[U79] PHP：静态分析
来源：http://qa.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://qb.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ny.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yb.panjiajie.cn

[U81] JS：初始化项目
来源：http://bt.panjiajie.cn

npm init -y;  npm i express
来源：http://rg.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://bj.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oo.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://cl.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ch.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://im.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://he.hahajie.cn

[U85] JS：可选链
来源：http://wz.jianghongdianzi.cn

a?.b?.c
来源：http://ys.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ig.shxzskj.cn

a ?? b
来源：http://av.shtwfgs.cn

[U87] JS：解构默认值
来源：http://qb.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://kk.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://wy.huanxung.cn

{ ...a, ...b }
来源：http://kl.521024.cn

[U89] JS：数组去重
来源：http://ku.nszjky.cn

[...new Set(arr)]
来源：http://qr.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://sa.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://qn.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://nv.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ga.panjiajie.cn

[U92] JS：深拷贝
来源：http://ox.hahajie.cn

structuredClone(obj)
来源：http://vp.colortex.cn

[U93] JS：模板字符串
来源：http://ai.szsharing.cn

`共 ${n} 条`
来源：http://wj.9csxet.cn

[U94] JS：箭头函数
来源：http://ek.huixinmuqiang.cn

const double = x => x * 2;
来源：http://on.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://jc.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://lk.szsharing.cn

[U96] JS：async/await 与异常
来源：http://gx.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yd.nszjky.cn

[U97] JS：并发请求
来源：http://wh.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ez.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://er.panjiajie.cn

[U99] JS：事件监听
来源：http://io.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://jb.asd995.cn

[U100] JS：DOM 查询
来源：http://qn.nicolike.cn

document.querySelector(".item")
来源：http://rf.9csxet.cn

[U101] JS：classList 操作
来源：http://zs.nicolike.cn

el.classList.toggle("active")
来源：http://hi.shxzukj.cn

[U102] JS：本地存储
来源：http://oo.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nr.jctech888.com.cn

[U103] JS：定时器
来源：http://nb.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dc.521024.cn

[U104] JS：防抖
来源：http://tp.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lv.chemitech.net.cn

[U105] JS：节流
来源：http://rm.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://da.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://qt.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://op.panjiajie.cn

[U107] JS：数字千分位
来源：http://ps.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vx.szxytkj.cn

[U108] JS：随机整数
来源：http://yq.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lp.muxihuayi.cn


<!-- 参考信息 -->