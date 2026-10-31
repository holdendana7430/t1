代发 wailian999

[T23] Swift：函数
来源：http://lz.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xr.jctech888.com.cn

[T24] Swift：闭包
来源：http://ac.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ud.nicolike.cn

[T25] Swift：结构体
来源：http://vw.huanxung.cn

struct P { var x: Int }
来源：http://eu.hnjuh.cn

[T26] Swift：类与重写
来源：http://cq.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://qj.521024.cn

[T27] Swift：错误处理
来源：http://rp.nicolike.cn

do { try f() } catch { print(error) }
来源：http://uz.shxzskj.cn

[T28] Swift：枚举
来源：http://aj.panjiajie.cn

enum Color { case red, green }
来源：http://ud.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://xj.szxytkj.cn

guard let x = opt else { return }
来源：http://dv.gzmigu.cn

[T30] Swift：协议
来源：http://aa.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://qe.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://us.lnxyls.cn

print("Hello")
来源：http://fp.shtwfgs.cn

[T32] Lua：局部变量
来源：http://hx.huixinmuqiang.cn

local a = 1
来源：http://zo.asd995.cn

[T33] Lua：表（数组）
来源：http://dg.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fn.haigaiapp.cn

[T34] Lua：遍历表
来源：http://xp.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kg.9csxet.cn

[T35] Lua：字典表
来源：http://tu.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://ph.nicolike.cn

[T36] Lua：函数
来源：http://un.shxzukj.cn

function add(a, b) return a + b end
来源：http://oe.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://xr.521024.cn

"a" .. "b"
来源：http://bz.wgjwhj.cn

[T38] Lua：条件
来源：http://hh.asd995.cn

if x > 0 then print("正") end
来源：http://gs.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://hu.asd995.cn

string.find(s, "%d+")
来源：http://ou.shxzskj.cn

[T40] Lua：元表
来源：http://wy.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://us.huanxung.cn

[T41] Perl：Hello World
来源：http://tf.shtwfgs.cn

print "Hello\n";
来源：http://al.yuexingan06.cn

[T42] Perl：变量类型
来源：http://yz.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qp.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://gr.lnxyls.cn

"值: $a"
来源：http://qb.huixiangedu.cn

[T44] Perl：条件
来源：http://cj.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://mh.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://ye.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://yi.9csxet.cn

[T46] Perl：哈希操作
来源：http://tx.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ax.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://sk.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rq.9csxet.cn

[T48] Perl：正则替换
来源：http://ji.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://xw.wgjwhj.cn

[T49] Perl：函数
来源：http://xh.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bt.nszjky.cn

[T50] Perl：逐行读文件
来源：http://xq.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bx.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://mi.hahajie.cn

[T51] Scala：Hello World
来源：http://ek.yuexingan06.cn

println("Hello")
来源：http://km.hnjuh.cn

[T52] Scala：变量
来源：http://rq.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://zy.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://ns.9csxet.cn

s"值: $b"
来源：http://ks.lnxyls.cn

[T54] Scala：集合映射
来源：http://ii.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://mp.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://yw.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://je.shtwfgs.cn

[T56] Scala：样例类
来源：http://gd.colortex.cn

case class User(name: String, age: Int)
来源：http://pb.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://uj.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fd.hahajie.cn

[T58] Scala：函数定义
来源：http://nb.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hl.newstarts.cn

[T59] Scala：循环
来源：http://hc.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://tr.colortex.cn

[T60] Scala：折叠
来源：http://ft.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mj.newstarts.cn

================================================================================
来源：http://en.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ip.panjiajie.cn

================================================================================
来源：http://tj.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://bh.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dc.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://wc.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mv.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://rh.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yp.szsharing.cn

[U04] Py：变量调试打印
来源：http://og.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://my.nicolike.cn

[U05] Py：列表去重且保序
来源：http://fn.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://ta.colortex.cn

[U06] Py：合并两个字典
来源：http://yf.nicolike.cn

{**a, **b}
来源：http://yl.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://xe.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://wr.asd995.cn

[U08] Py：展平二维列表
来源：http://hh.jctech888.com.cn

[y for x in nested for y in x]
来源：http://fn.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ot.huanxung.cn

max(d, key=d.get)
来源：http://xv.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://cq.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mx.shxzskj.cn

[U11] Py：生成器表达式
来源：http://wq.nszjky.cn

(x * 2 for x in arr)
来源：http://ww.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nf.hnjuh.cn

Counter(arr).most_common(3)
来源：http://na.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://ly.huanxung.cn

deque(maxlen=10)
来源：http://yi.huanxung.cn

[U14] Py：分组收集到列表
来源：http://kc.jctech888.com.cn

defaultdict(list)
来源：http://jp.bjjhwx.cn

[U15] Py：高精度计时
来源：http://ow.colortex.cn

t = time.perf_counter()
来源：http://sp.hahajie.cn

[U16] Py：命令行参数解析
来源：http://rw.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://me.newstarts.cn

[U17] Py：初始化日志
来源：http://zr.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ct.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://qt.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://xo.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://az.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xt.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://oq.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://jg.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ao.9csxet.cn

@contextlib.contextmanager
来源：http://qj.hahajie.cn

[U22] Py：矩阵转置
来源：http://so.yuexingan06.cn

list(zip(*m))
来源：http://gy.9csxet.cn

[U23] Py：分块读取大文件
来源：http://ob.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hh.9csxet.cn

[U24] Py：路径操作
来源：http://uj.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gc.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://sg.hnjuh.cn

csv.DictReader(f)
来源：http://lz.szxytkj.cn

[U26] Py：并发下载
来源：http://ja.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xw.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://ec.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://og.yuexingan06.cn

[U28] Py：类型别名
来源：http://ok.hahajie.cn

UserId = int
来源：http://zr.panjiajie.cn

[U29] Py：属性校验
来源：http://ry.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://rh.nszjky.cn

[U30] Py：数据类
来源：http://tt.panjiajie.cn

@dataclass(slots=True)
来源：http://hg.asd995.cn

[U31] Py：单测
来源：http://kt.szsharing.cn

python -m pytest -q
来源：http://di.yuexingan06.cn

[U32] Py：代码格式化
来源：http://rt.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://wr.shtwfgs.cn

[U33] Py：打包发布
来源：http://dx.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://sh.shxzukj.cn

[U34] Py：判断编码
来源：http://my.hnjuh.cn

chardet.detect(raw)
来源：http://xi.shxzskj.cn

[U35] Py：发送邮件
来源：http://mk.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qn.muxihuayi.cn

[U36] Py：定时任务
来源：http://gf.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://xo.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://rf.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pa.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://qy.huanxung.cn

Path(__file__).resolve().parent
来源：http://rs.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ii.newstarts.cn

sys.stdout.isatty()
来源：http://fi.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://rv.szxytkj.cn

print("err", file=sys.stderr)
来源：http://hi.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://zw.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pm.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://ov.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vs.nszjky.cn

[U43] PHP：声明命名空间
来源：http://ws.yuntaijiaju.cn

namespace App\Http;
来源：http://iy.colortex.cn

[U44] PHP：开启严格类型
来源：http://af.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ew.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://hc.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bf.chemitech.net.cn

[U46] PHP：可空类型
来源：http://sy.9csxet.cn

?string $name = null
来源：http://oe.muxihuayi.cn

[U47] PHP：联合类型
来源：http://vt.muxihuayi.cn

int|string $id
来源：http://rr.9csxet.cn

[U48] PHP：纯枚举
来源：http://ay.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wo.huixiangedu.cn

[U49] PHP：只读属性
来源：http://xt.muxihuayi.cn

public readonly string $name
来源：http://df.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://oy.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://bu.huixiangedu.cn

[U51] PHP：数组解构
来源：http://eb.asd995.cn

[$a, $b] = $arr;
来源：http://nt.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://uz.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://hl.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://ok.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://vt.nszjky.cn

[U54] PHP：空安全调用
来源：http://fv.yuexingan06.cn

$obj?->method()
来源：http://tm.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://zq.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kr.nicolike.cn

[U56] PHP：命名参数
来源：http://sk.haigaiapp.cn

f(a: 1, b: 2)
来源：http://bz.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://rl.huixiangedu.cn

"值: {$a}"
来源：http://go.asd995.cn

[U58] PHP：数组三件套
来源：http://bb.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cb.asd995.cn

[U59] PHP：自定义排序
来源：http://jm.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gd.colortex.cn

[U60] PHP：JSON 编解码
来源：http://mc.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iq.hnjuh.cn

[U61] PHP：正则
来源：http://kp.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fs.muxihuayi.cn

[U62] PHP：日期对象
来源：http://jx.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ic.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://sf.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bn.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://vc.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://kd.huixinmuqiang.cn

[U65] PHP：会话
来源：http://pi.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tp.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://oy.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fd.nszjky.cn

[U67] PHP：处理文件上传
来源：http://ns.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vu.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://ay.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sq.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://zp.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vd.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://jf.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oh.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ge.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://nz.nszjky.cn

[U72] PHP：写错误日志
来源：http://fd.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://oc.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://ov.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://rd.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://kq.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://dc.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://qp.9csxet.cn

composer require psr/container
来源：http://rt.yuexingan06.cn

[U76] PHP：简单路由
来源：http://ow.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jm.panjiajie.cn

[U77] PHP：模板渲染
来源：http://no.521024.cn

composer require twig/twig
来源：http://tb.bjjhwx.cn

[U78] PHP：单元测试
来源：http://vg.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://vp.shxzukj.cn

[U79] PHP：静态分析
来源：http://hy.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://kp.colortex.cn

[U80] PHP：代码规范修复
来源：http://gb.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mf.huixiangedu.cn

[U81] JS：初始化项目
来源：http://jd.szxytkj.cn

npm init -y;  npm i express
来源：http://ch.nszjky.cn

[U82] JS：package.json 脚本
来源：http://yw.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zo.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://is.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lw.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://ey.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yd.hnjuh.cn

[U85] JS：可选链
来源：http://km.jianghongdianzi.cn

a?.b?.c
来源：http://rp.bookmarksfly.cn

[U86] JS：空值合并
来源：http://di.jianghongdianzi.cn

a ?? b
来源：http://pc.huanxung.cn

[U87] JS：解构默认值
来源：http://lj.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://oz.hnjuh.cn

[U88] JS：对象展开合并
来源：http://sd.asd995.cn

{ ...a, ...b }
来源：http://ix.bjjhwx.cn

[U89] JS：数组去重
来源：http://ig.huixinmuqiang.cn

[...new Set(arr)]
来源：http://hz.9csxet.cn

[U90] JS：数字数组排序
来源：http://zp.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://cw.hahajie.cn

[U91] JS：对象键值遍历
来源：http://vu.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fv.bjjhwx.cn

[U92] JS：深拷贝
来源：http://pk.huanxung.cn

structuredClone(obj)
来源：http://dk.yuexingan06.cn

[U93] JS：模板字符串
来源：http://hm.bookmarksfly.cn

`共 ${n} 条`
来源：http://lm.szsharing.cn

[U94] JS：箭头函数
来源：http://tw.huanxung.cn

const double = x => x * 2;
来源：http://zm.huanxung.cn

[U95] JS：Promise 包装
来源：http://gb.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://me.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://rq.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rb.hahajie.cn

[U97] JS：并发请求
来源：http://qp.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pi.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://cw.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sh.szsharing.cn

[U99] JS：事件监听
来源：http://qp.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://wa.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://oo.bookmarksfly.cn

document.querySelector(".item")
来源：http://sh.huanxung.cn

[U101] JS：classList 操作
来源：http://ts.wgjwhj.cn

el.classList.toggle("active")
来源：http://qe.panjiajie.cn

[U102] JS：本地存储
来源：http://us.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rp.yuexingan06.cn

[U103] JS：定时器
来源：http://zd.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tm.jctech888.com.cn

[U104] JS：防抖
来源：http://vg.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qo.hahajie.cn

[U105] JS：节流
来源：http://ov.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sa.9csxet.cn

[U106] JS：日期格式化
来源：http://et.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yb.wgjwhj.cn

[U107] JS：数字千分位
来源：http://ai.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kg.hahajie.cn

[U108] JS：随机整数
来源：http://vt.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xk.bookmarksfly.cn

[U109] JS：数组分组
来源：http://yi.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://nc.521024.cn

[U110] JS：数组分块
来源：http://pj.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://px.bjjhwx.cn


<!-- 参考信息 -->