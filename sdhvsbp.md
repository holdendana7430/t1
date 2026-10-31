代发 wailian999

[T21] Swift：遍历
来源：http://ud.szsharing.cn

for x in a { print(x) }
来源：http://aq.shxzskj.cn

[T22] Swift：字典
来源：http://mw.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sm.jianghongdianzi.cn

[T23] Swift：函数
来源：http://fz.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ak.wgjwhj.cn

[T24] Swift：闭包
来源：http://pq.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oi.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://rf.shtwfgs.cn

struct P { var x: Int }
来源：http://ct.muxihuayi.cn

[T26] Swift：类与重写
来源：http://xx.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://rz.gzmigu.cn

[T27] Swift：错误处理
来源：http://jq.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://fc.wgjwhj.cn

[T28] Swift：枚举
来源：http://mj.shtwfgs.cn

enum Color { case red, green }
来源：http://we.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://uy.bookmarksfly.cn

guard let x = opt else { return }
来源：http://nc.asd995.cn

[T30] Swift：协议
来源：http://px.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://vc.haigaiapp.cn

[T31] Lua：Hello World
来源：http://ou.haigaiapp.cn

print("Hello")
来源：http://ie.gzmigu.cn

[T32] Lua：局部变量
来源：http://nm.huixiangedu.cn

local a = 1
来源：http://nl.colortex.cn

[T33] Lua：表（数组）
来源：http://et.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xk.haigaiapp.cn

[T34] Lua：遍历表
来源：http://js.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mu.huanxung.cn

[T35] Lua：字典表
来源：http://hf.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://hw.panjiajie.cn

[T36] Lua：函数
来源：http://uw.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ud.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://uq.wgjwhj.cn

"a" .. "b"
来源：http://hc.shxzukj.cn

[T38] Lua：条件
来源：http://cx.muxihuayi.cn

if x > 0 then print("正") end
来源：http://yj.hnjuh.cn

[T39] Lua：模式匹配
来源：http://pq.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://zo.yuexingan06.cn

[T40] Lua：元表
来源：http://vt.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://rx.huanxung.cn

[T41] Perl：Hello World
来源：http://bv.shxzskj.cn

print "Hello\n";
来源：http://jh.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://cj.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bm.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://tz.newstarts.cn

"值: $a"
来源：http://io.shxzskj.cn

[T44] Perl：条件
来源：http://ke.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://vi.521024.cn

[T45] Perl：数组遍历
来源：http://tu.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://wf.panjiajie.cn

[T46] Perl：哈希操作
来源：http://bh.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tq.colortex.cn

[T47] Perl：正则捕获
来源：http://xp.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xo.shxzukj.cn

[T48] Perl：正则替换
来源：http://zp.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://zt.szsharing.cn

[T49] Perl：函数
来源：http://mv.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ss.szsharing.cn

[T50] Perl：逐行读文件
来源：http://ws.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://du.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://mw.nicolike.cn

[T51] Scala：Hello World
来源：http://bi.haigaiapp.cn

println("Hello")
来源：http://iz.jctech888.com.cn

[T52] Scala：变量
来源：http://kt.newstarts.cn

val a = 1;  var b = 2
来源：http://cd.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://eu.panjiajie.cn

s"值: $b"
来源：http://en.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://kh.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xu.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://gx.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://af.shxzukj.cn

[T56] Scala：样例类
来源：http://iw.lnxyls.cn

case class User(name: String, age: Int)
来源：http://tf.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://fm.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://td.jctech888.com.cn

[T58] Scala：函数定义
来源：http://xh.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zz.asd995.cn

[T59] Scala：循环
来源：http://aw.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://gy.gzmigu.cn

[T60] Scala：折叠
来源：http://cp.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tu.yuntaijiaju.cn

================================================================================
来源：http://wc.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hx.bookmarksfly.cn

================================================================================
来源：http://ej.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://up.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nj.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://jz.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ky.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://tn.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tk.9csxet.cn

[U04] Py：变量调试打印
来源：http://dh.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sk.asd995.cn

[U05] Py：列表去重且保序
来源：http://ld.521024.cn

list(dict.fromkeys(arr))
来源：http://ih.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://qn.haigaiapp.cn

{**a, **b}
来源：http://kc.hnjuh.cn

[U07] Py：反转字典键值
来源：http://vb.asd995.cn

{v: k for k, v in d.items()}
来源：http://jw.lnxyls.cn

[U08] Py：展平二维列表
来源：http://nn.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://ga.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://fl.szsharing.cn

max(d, key=d.get)
来源：http://aa.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://sl.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zz.nicolike.cn

[U11] Py：生成器表达式
来源：http://dn.asd995.cn

(x * 2 for x in arr)
来源：http://hi.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xv.lnxyls.cn

Counter(arr).most_common(3)
来源：http://qg.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ww.shxzskj.cn

deque(maxlen=10)
来源：http://li.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://lc.yuntaijiaju.cn

defaultdict(list)
来源：http://mz.shxzskj.cn

[U15] Py：高精度计时
来源：http://cy.chemitech.net.cn

t = time.perf_counter()
来源：http://qv.521024.cn

[U16] Py：命令行参数解析
来源：http://ls.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dg.muxihuayi.cn

[U17] Py：初始化日志
来源：http://fy.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://mi.asd995.cn

[U18] Py：预编译正则
来源：http://cm.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://hj.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://fj.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jo.asd995.cn

[U20] Py：缓存函数结果
来源：http://hn.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://wh.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://bq.gzmigu.cn

@contextlib.contextmanager
来源：http://lm.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://wj.jianghongdianzi.cn

list(zip(*m))
来源：http://xv.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://mw.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xd.yuexingan06.cn

[U24] Py：路径操作
来源：http://bh.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ng.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://qk.wgjwhj.cn

csv.DictReader(f)
来源：http://wy.hahajie.cn

[U26] Py：并发下载
来源：http://yg.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ic.huanxung.cn

[U27] Py：异步 HTTP
来源：http://fo.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://kc.shtwfgs.cn

[U28] Py：类型别名
来源：http://of.bookmarksfly.cn

UserId = int
来源：http://dk.shxzukj.cn

[U29] Py：属性校验
来源：http://bf.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://gf.shxzskj.cn

[U30] Py：数据类
来源：http://kn.haigaiapp.cn

@dataclass(slots=True)
来源：http://ii.gzmigu.cn

[U31] Py：单测
来源：http://uu.shxzukj.cn

python -m pytest -q
来源：http://iv.nszjky.cn

[U32] Py：代码格式化
来源：http://jr.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://gs.shxzukj.cn

[U33] Py：打包发布
来源：http://qk.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://cn.panjiajie.cn

[U34] Py：判断编码
来源：http://xa.huixiangedu.cn

chardet.detect(raw)
来源：http://wr.nicolike.cn

[U35] Py：发送邮件
来源：http://px.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jp.bookmarksfly.cn

[U36] Py：定时任务
来源：http://kw.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://cs.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://sx.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yh.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://yp.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://zl.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://qn.panjiajie.cn

sys.stdout.isatty()
来源：http://ue.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://rh.lnxyls.cn

print("err", file=sys.stderr)
来源：http://im.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://qm.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mj.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://qh.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fz.huanxung.cn

[U43] PHP：声明命名空间
来源：http://el.panjiajie.cn

namespace App\Http;
来源：http://pf.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://hx.gzmigu.cn

declare(strict_types=1);
来源：http://rb.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://qy.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xt.huanxung.cn

[U46] PHP：可空类型
来源：http://vv.huixinmuqiang.cn

?string $name = null
来源：http://wi.lnxyls.cn

[U47] PHP：联合类型
来源：http://lg.bjjhwx.cn

int|string $id
来源：http://ln.nicolike.cn

[U48] PHP：纯枚举
来源：http://jd.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ey.gzmigu.cn

[U49] PHP：只读属性
来源：http://nd.asd995.cn

public readonly string $name
来源：http://sg.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://qm.huanxung.cn

public function __construct(private int $id) {}
来源：http://wk.haigaiapp.cn

[U51] PHP：数组解构
来源：http://yo.szxytkj.cn

[$a, $b] = $arr;
来源：http://td.hnjuh.cn

[U52] PHP：箭头函数
来源：http://su.colortex.cn

$double = fn($x) => $x * 2;
来源：http://ir.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://ak.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://qt.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://gq.gzmigu.cn

$obj?->method()
来源：http://jj.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://mp.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mu.szsharing.cn

[U56] PHP：命名参数
来源：http://sw.chemitech.net.cn

f(a: 1, b: 2)
来源：http://rn.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://fk.muxihuayi.cn

"值: {$a}"
来源：http://df.nszjky.cn

[U58] PHP：数组三件套
来源：http://yb.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nr.szsharing.cn

[U59] PHP：自定义排序
来源：http://ju.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ro.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://ly.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hm.jianghongdianzi.cn

[U61] PHP：正则
来源：http://fn.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gf.huixiangedu.cn

[U62] PHP：日期对象
来源：http://by.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vm.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://iq.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ck.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://qi.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://yc.lnxyls.cn

[U65] PHP：会话
来源：http://mg.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tr.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://qx.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://od.asd995.cn

[U67] PHP：处理文件上传
来源：http://cr.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tn.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://kw.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oz.colortex.cn

[U69] PHP：PDO 预处理
来源：http://kz.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ed.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://eb.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://md.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://lk.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://ql.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ji.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://sv.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://qj.521024.cn

parse_ini_file("config.ini", true)
来源：http://bl.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://un.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://me.colortex.cn

[U75] PHP：依赖注入
来源：http://er.jctech888.com.cn

composer require psr/container
来源：http://fx.huixiangedu.cn

[U76] PHP：简单路由
来源：http://rx.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://be.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://px.jianghongdianzi.cn

composer require twig/twig
来源：http://qt.asd995.cn

[U78] PHP：单元测试
来源：http://ai.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://aq.huanxung.cn

[U79] PHP：静态分析
来源：http://fs.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://at.9csxet.cn

[U80] PHP：代码规范修复
来源：http://tq.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kn.yuexingan06.cn

[U81] JS：初始化项目
来源：http://aa.szsharing.cn

npm init -y;  npm i express
来源：http://ks.szsharing.cn

[U82] JS：package.json 脚本
来源：http://qc.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ag.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://ir.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://go.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ad.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://an.nicolike.cn

[U85] JS：可选链
来源：http://wg.bjjhwx.cn

a?.b?.c
来源：http://ba.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ow.lnxyls.cn

a ?? b
来源：http://ua.chemitech.net.cn

[U87] JS：解构默认值
来源：http://nz.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://pi.newstarts.cn

[U88] JS：对象展开合并
来源：http://tg.hnjuh.cn

{ ...a, ...b }
来源：http://dq.lnxyls.cn

[U89] JS：数组去重
来源：http://ya.nicolike.cn

[...new Set(arr)]
来源：http://zl.521024.cn

[U90] JS：数字数组排序
来源：http://wy.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://pm.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://tj.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jc.haigaiapp.cn

[U92] JS：深拷贝
来源：http://if.bjjhwx.cn

structuredClone(obj)
来源：http://ng.szsharing.cn

[U93] JS：模板字符串
来源：http://gc.yuntaijiaju.cn

`共 ${n} 条`
来源：http://ck.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://rb.shtwfgs.cn

const double = x => x * 2;
来源：http://mb.colortex.cn

[U95] JS：Promise 包装
来源：http://pk.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://eg.newstarts.cn

[U96] JS：async/await 与异常
来源：http://ob.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bm.panjiajie.cn

[U97] JS：并发请求
来源：http://lw.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bf.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://nq.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ki.yuexingan06.cn

[U99] JS：事件监听
来源：http://nl.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://sb.shxzskj.cn

[U100] JS：DOM 查询
来源：http://vu.shxzukj.cn

document.querySelector(".item")
来源：http://nu.hahajie.cn

[U101] JS：classList 操作
来源：http://jq.panjiajie.cn

el.classList.toggle("active")
来源：http://di.bjjhwx.cn

[U102] JS：本地存储
来源：http://an.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ye.huanxung.cn

[U103] JS：定时器
来源：http://kn.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zt.gzmigu.cn

[U104] JS：防抖
来源：http://jg.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gy.szsharing.cn

[U105] JS：节流
来源：http://ve.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ok.huixiangedu.cn

[U106] JS：日期格式化
来源：http://wx.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ii.yuexingan06.cn

[U107] JS：数字千分位
来源：http://ir.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yb.shxzukj.cn

[U108] JS：随机整数
来源：http://ih.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vq.nicolike.cn


<!-- 参考信息 -->