代发 wailian999

[T23] Swift：函数
来源：http://pj.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wd.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://wy.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oz.nszjky.cn

[T25] Swift：结构体
来源：http://xl.asd995.cn

struct P { var x: Int }
来源：http://yk.nicolike.cn

[T26] Swift：类与重写
来源：http://xb.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://cd.hnjuh.cn

[T27] Swift：错误处理
来源：http://rc.asd995.cn

do { try f() } catch { print(error) }
来源：http://yj.muxihuayi.cn

[T28] Swift：枚举
来源：http://ta.gzmigu.cn

enum Color { case red, green }
来源：http://lo.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://vo.gzmigu.cn

guard let x = opt else { return }
来源：http://lc.yuntaijiaju.cn

[T30] Swift：协议
来源：http://lq.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://ya.shxzskj.cn

[T31] Lua：Hello World
来源：http://zy.szsharing.cn

print("Hello")
来源：http://jm.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://fd.bookmarksfly.cn

local a = 1
来源：http://md.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ur.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qn.nicolike.cn

[T34] Lua：遍历表
来源：http://jc.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ee.yuexingan06.cn

[T35] Lua：字典表
来源：http://wl.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://if.bookmarksfly.cn

[T36] Lua：函数
来源：http://mc.asd995.cn

function add(a, b) return a + b end
来源：http://uz.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://rj.colortex.cn

"a" .. "b"
来源：http://hh.szxytkj.cn

[T38] Lua：条件
来源：http://rc.9csxet.cn

if x > 0 then print("正") end
来源：http://tb.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://jh.jctech888.com.cn

string.find(s, "%d+")
来源：http://ms.bjjhwx.cn

[T40] Lua：元表
来源：http://ao.colortex.cn

setmetatable({}, { __index = base })
来源：http://zl.nicolike.cn

[T41] Perl：Hello World
来源：http://gd.gzmigu.cn

print "Hello\n";
来源：http://rf.haigaiapp.cn

[T42] Perl：变量类型
来源：http://th.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jp.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://lq.huanxung.cn

"值: $a"
来源：http://eg.huanxung.cn

[T44] Perl：条件
来源：http://qt.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://gr.szsharing.cn

[T45] Perl：数组遍历
来源：http://am.asd995.cn

for my $x (@arr) { print $x; }
来源：http://su.gzmigu.cn

[T46] Perl：哈希操作
来源：http://as.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hn.newstarts.cn

[T47] Perl：正则捕获
来源：http://xu.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ny.shxzskj.cn

[T48] Perl：正则替换
来源：http://ap.hnjuh.cn

$s =~ s/old/new/g;
来源：http://uu.asd995.cn

[T49] Perl：函数
来源：http://ea.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xr.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://rb.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ow.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://kw.521024.cn

[T51] Scala：Hello World
来源：http://pd.nszjky.cn

println("Hello")
来源：http://cm.szsharing.cn

[T52] Scala：变量
来源：http://yy.nicolike.cn

val a = 1;  var b = 2
来源：http://iy.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://et.szsharing.cn

s"值: $b"
来源：http://ll.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://dy.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://rx.asd995.cn

[T55] Scala：集合过滤
来源：http://zv.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ip.gzmigu.cn

[T56] Scala：样例类
来源：http://sl.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ve.colortex.cn

[T57] Scala：模式匹配
来源：http://tg.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zo.9csxet.cn

[T58] Scala：函数定义
来源：http://jt.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zr.huixinmuqiang.cn

[T59] Scala：循环
来源：http://eg.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ay.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://ry.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zd.newstarts.cn

================================================================================
来源：http://mv.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tl.huixiangedu.cn

================================================================================
来源：http://zu.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://km.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kh.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://xv.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sp.colortex.cn

[U03] Py：加载 .env 配置
来源：http://ta.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cs.newstarts.cn

[U04] Py：变量调试打印
来源：http://hd.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lj.nicolike.cn

[U05] Py：列表去重且保序
来源：http://bz.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://lo.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://vt.hnjuh.cn

{**a, **b}
来源：http://wl.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://si.nicolike.cn

{v: k for k, v in d.items()}
来源：http://qe.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://oa.nszjky.cn

[y for x in nested for y in x]
来源：http://kf.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://kn.jctech888.com.cn

max(d, key=d.get)
来源：http://lt.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://pc.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://af.newstarts.cn

[U11] Py：生成器表达式
来源：http://tx.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://ge.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ei.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://bl.szxytkj.cn

[U13] Py：固定长度队列
来源：http://cv.wgjwhj.cn

deque(maxlen=10)
来源：http://ad.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://kx.huixiangedu.cn

defaultdict(list)
来源：http://ny.bjjhwx.cn

[U15] Py：高精度计时
来源：http://wg.chemitech.net.cn

t = time.perf_counter()
来源：http://di.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://eb.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vp.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ws.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://xl.panjiajie.cn

[U18] Py：预编译正则
来源：http://tc.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://fn.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://jw.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tv.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://wp.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://nz.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://tk.bjjhwx.cn

@contextlib.contextmanager
来源：http://nx.huanxung.cn

[U22] Py：矩阵转置
来源：http://xf.haigaiapp.cn

list(zip(*m))
来源：http://ob.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://in.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ql.muxihuayi.cn

[U24] Py：路径操作
来源：http://hw.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hn.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://my.szsharing.cn

csv.DictReader(f)
来源：http://zm.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://xn.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wj.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://vm.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://km.muxihuayi.cn

[U28] Py：类型别名
来源：http://di.shtwfgs.cn

UserId = int
来源：http://vb.muxihuayi.cn

[U29] Py：属性校验
来源：http://hh.521024.cn

@property 与 @x.setter 配合
来源：http://io.panjiajie.cn

[U30] Py：数据类
来源：http://em.shxzukj.cn

@dataclass(slots=True)
来源：http://af.asd995.cn

[U31] Py：单测
来源：http://zm.huixinmuqiang.cn

python -m pytest -q
来源：http://nh.colortex.cn

[U32] Py：代码格式化
来源：http://wp.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://xu.szsharing.cn

[U33] Py：打包发布
来源：http://lq.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://cm.szxytkj.cn

[U34] Py：判断编码
来源：http://ng.nicolike.cn

chardet.detect(raw)
来源：http://nz.shxzskj.cn

[U35] Py：发送邮件
来源：http://kx.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qd.hahajie.cn

[U36] Py：定时任务
来源：http://ic.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://aj.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://lw.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mr.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://nw.9csxet.cn

Path(__file__).resolve().parent
来源：http://dv.521024.cn

[U39] Py：判断是否在交互环境
来源：http://yw.9csxet.cn

sys.stdout.isatty()
来源：http://fe.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://ra.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://to.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://pw.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rj.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://mu.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dh.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://ef.muxihuayi.cn

namespace App\Http;
来源：http://rl.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://cg.szxytkj.cn

declare(strict_types=1);
来源：http://jm.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://es.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.huanxung.cn

[U46] PHP：可空类型
来源：http://lp.9csxet.cn

?string $name = null
来源：http://hi.521024.cn

[U47] PHP：联合类型
来源：http://nc.hnjuh.cn

int|string $id
来源：http://rl.9csxet.cn

[U48] PHP：纯枚举
来源：http://lf.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vu.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://hn.bjjhwx.cn

public readonly string $name
来源：http://yy.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://kr.asd995.cn

public function __construct(private int $id) {}
来源：http://wu.chemitech.net.cn

[U51] PHP：数组解构
来源：http://xw.szxytkj.cn

[$a, $b] = $arr;
来源：http://cf.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://qr.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://tz.nicolike.cn

[U53] PHP：空合并运算符
来源：http://qm.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://ee.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://gp.hahajie.cn

$obj?->method()
来源：http://ea.huanxung.cn

[U55] PHP：match 表达式
来源：http://rf.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wl.shtwfgs.cn

[U56] PHP：命名参数
来源：http://ed.lnxyls.cn

f(a: 1, b: 2)
来源：http://ml.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://ge.lnxyls.cn

"值: {$a}"
来源：http://pv.nicolike.cn

[U58] PHP：数组三件套
来源：http://vj.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oa.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://dn.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lz.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://od.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://of.bookmarksfly.cn

[U61] PHP：正则
来源：http://mx.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://it.gzmigu.cn

[U62] PHP：日期对象
来源：http://di.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hg.hahajie.cn

[U63] PHP：文件读写
来源：http://kw.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yi.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://mq.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://lv.huixinmuqiang.cn

[U65] PHP：会话
来源：http://nh.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xz.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://oz.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dh.huanxung.cn

[U67] PHP：处理文件上传
来源：http://gx.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ox.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://ig.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fk.colortex.cn

[U69] PHP：PDO 预处理
来源：http://re.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vq.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://xd.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vh.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://fc.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://yb.hnjuh.cn

[U72] PHP：写错误日志
来源：http://jc.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://gf.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://ii.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://hz.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://zq.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://te.huanxung.cn

[U75] PHP：依赖注入
来源：http://jr.huixiangedu.cn

composer require psr/container
来源：http://tr.9csxet.cn

[U76] PHP：简单路由
来源：http://gt.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ou.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://gi.shtwfgs.cn

composer require twig/twig
来源：http://xr.muxihuayi.cn

[U78] PHP：单元测试
来源：http://yk.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://ts.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://yq.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://hw.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://xe.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cx.muxihuayi.cn

[U81] JS：初始化项目
来源：http://ln.jctech888.com.cn

npm init -y;  npm i express
来源：http://yv.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://bq.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yg.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://nu.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zf.521024.cn

[U84] JS：CommonJS 写法
来源：http://nt.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bu.szsharing.cn

[U85] JS：可选链
来源：http://go.yuexingan06.cn

a?.b?.c
来源：http://xp.hahajie.cn

[U86] JS：空值合并
来源：http://se.bookmarksfly.cn

a ?? b
来源：http://ou.jctech888.com.cn

[U87] JS：解构默认值
来源：http://pc.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://pt.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://up.panjiajie.cn

{ ...a, ...b }
来源：http://gn.shxzukj.cn

[U89] JS：数组去重
来源：http://mr.huixinmuqiang.cn

[...new Set(arr)]
来源：http://rr.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://ng.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://ry.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://iq.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.newstarts.cn

[U92] JS：深拷贝
来源：http://vs.hahajie.cn

structuredClone(obj)
来源：http://vy.hnjuh.cn

[U93] JS：模板字符串
来源：http://nn.asd995.cn

`共 ${n} 条`
来源：http://ke.shxzskj.cn

[U94] JS：箭头函数
来源：http://rb.shxzukj.cn

const double = x => x * 2;
来源：http://ip.hnjuh.cn

[U95] JS：Promise 包装
来源：http://zp.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://wk.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://yc.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ul.wgjwhj.cn

[U97] JS：并发请求
来源：http://hn.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://qd.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sy.panjiajie.cn

[U99] JS：事件监听
来源：http://cy.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://as.huanxung.cn

[U100] JS：DOM 查询
来源：http://ds.colortex.cn

document.querySelector(".item")
来源：http://hc.chemitech.net.cn

[U101] JS：classList 操作
来源：http://tm.9csxet.cn

el.classList.toggle("active")
来源：http://du.bjjhwx.cn

[U102] JS：本地存储
来源：http://dz.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qn.nicolike.cn

[U103] JS：定时器
来源：http://ws.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ok.szxytkj.cn

[U104] JS：防抖
来源：http://we.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ym.haigaiapp.cn

[U105] JS：节流
来源：http://kn.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ig.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://cz.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ik.muxihuayi.cn

[U107] JS：数字千分位
来源：http://so.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xw.hahajie.cn

[U108] JS：随机整数
来源：http://ja.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qc.szsharing.cn

[U109] JS：数组分组
来源：http://gd.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://lo.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ne.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sd.yuntaijiaju.cn


<!-- 参考信息 -->