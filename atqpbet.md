代发 wailian999

[T31] Lua：Hello World
来源：http://rk.panjiajie.cn

print("Hello")
来源：http://hj.jctech888.com.cn

[T32] Lua：局部变量
来源：http://bt.yuexingan06.cn

local a = 1
来源：http://kq.panjiajie.cn

[T33] Lua：表（数组）
来源：http://wn.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xq.9csxet.cn

[T34] Lua：遍历表
来源：http://wy.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hy.bookmarksfly.cn

[T35] Lua：字典表
来源：http://tc.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://nz.nszjky.cn

[T36] Lua：函数
来源：http://lg.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://ei.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://rm.chemitech.net.cn

"a" .. "b"
来源：http://md.wgjwhj.cn

[T38] Lua：条件
来源：http://oq.shtwfgs.cn

if x > 0 then print("正") end
来源：http://dp.szxytkj.cn

[T39] Lua：模式匹配
来源：http://fb.nicolike.cn

string.find(s, "%d+")
来源：http://lb.huixiangedu.cn

[T40] Lua：元表
来源：http://ro.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://hu.szsharing.cn

[T41] Perl：Hello World
来源：http://dy.szsharing.cn

print "Hello\n";
来源：http://qx.hnjuh.cn

[T42] Perl：变量类型
来源：http://jm.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vl.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://ec.lnxyls.cn

"值: $a"
来源：http://sx.bjjhwx.cn

[T44] Perl：条件
来源：http://nd.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ki.newstarts.cn

[T45] Perl：数组遍历
来源：http://fz.asd995.cn

for my $x (@arr) { print $x; }
来源：http://vu.newstarts.cn

[T46] Perl：哈希操作
来源：http://sd.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://id.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://ru.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ay.hahajie.cn

[T48] Perl：正则替换
来源：http://rv.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://xc.nicolike.cn

[T49] Perl：函数
来源：http://xr.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ep.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://cr.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lh.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://fv.newstarts.cn

[T51] Scala：Hello World
来源：http://sk.huanxung.cn

println("Hello")
来源：http://fw.jianghongdianzi.cn

[T52] Scala：变量
来源：http://cy.panjiajie.cn

val a = 1;  var b = 2
来源：http://nq.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://hv.gzmigu.cn

s"值: $b"
来源：http://tb.colortex.cn

[T54] Scala：集合映射
来源：http://ro.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://po.nicolike.cn

[T55] Scala：集合过滤
来源：http://du.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qe.hnjuh.cn

[T56] Scala：样例类
来源：http://qp.szsharing.cn

case class User(name: String, age: Int)
来源：http://ub.shxzskj.cn

[T57] Scala：模式匹配
来源：http://nm.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vu.bjjhwx.cn

[T58] Scala：函数定义
来源：http://cs.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hw.hnjuh.cn

[T59] Scala：循环
来源：http://jf.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://rk.bjjhwx.cn

[T60] Scala：折叠
来源：http://sk.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vd.shxzskj.cn

================================================================================
来源：http://yz.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mt.yuexingan06.cn

================================================================================
来源：http://je.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://uc.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yb.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://aj.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ec.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://ub.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vy.szsharing.cn

[U04] Py：变量调试打印
来源：http://fd.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uy.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://in.asd995.cn

list(dict.fromkeys(arr))
来源：http://an.huanxung.cn

[U06] Py：合并两个字典
来源：http://ub.newstarts.cn

{**a, **b}
来源：http://tw.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ot.newstarts.cn

{v: k for k, v in d.items()}
来源：http://vl.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://ev.colortex.cn

[y for x in nested for y in x]
来源：http://rz.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://zi.521024.cn

max(d, key=d.get)
来源：http://nw.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://wy.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ic.521024.cn

[U11] Py：生成器表达式
来源：http://pp.nszjky.cn

(x * 2 for x in arr)
来源：http://ln.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hj.gzmigu.cn

Counter(arr).most_common(3)
来源：http://ow.newstarts.cn

[U13] Py：固定长度队列
来源：http://tn.szsharing.cn

deque(maxlen=10)
来源：http://mq.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://ci.521024.cn

defaultdict(list)
来源：http://to.szsharing.cn

[U15] Py：高精度计时
来源：http://zn.szxytkj.cn

t = time.perf_counter()
来源：http://uz.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://ul.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yl.muxihuayi.cn

[U17] Py：初始化日志
来源：http://di.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://aq.huanxung.cn

[U18] Py：预编译正则
来源：http://up.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://id.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://sg.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bw.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://ig.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://fz.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://hc.jctech888.com.cn

@contextlib.contextmanager
来源：http://yr.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://ar.521024.cn

list(zip(*m))
来源：http://lw.szsharing.cn

[U23] Py：分块读取大文件
来源：http://uc.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pq.nicolike.cn

[U24] Py：路径操作
来源：http://lh.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tz.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://xk.521024.cn

csv.DictReader(f)
来源：http://dy.asd995.cn

[U26] Py：并发下载
来源：http://fo.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bm.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://uw.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://th.nszjky.cn

[U28] Py：类型别名
来源：http://eo.huixiangedu.cn

UserId = int
来源：http://nc.asd995.cn

[U29] Py：属性校验
来源：http://xf.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://sg.szsharing.cn

[U30] Py：数据类
来源：http://oz.huixiangedu.cn

@dataclass(slots=True)
来源：http://cu.jctech888.com.cn

[U31] Py：单测
来源：http://ip.lnxyls.cn

python -m pytest -q
来源：http://of.haigaiapp.cn

[U32] Py：代码格式化
来源：http://dp.hahajie.cn

ruff format . && ruff check --fix .
来源：http://wh.nicolike.cn

[U33] Py：打包发布
来源：http://jf.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://jb.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://hl.nszjky.cn

chardet.detect(raw)
来源：http://vp.szxytkj.cn

[U35] Py：发送邮件
来源：http://lk.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xr.hahajie.cn

[U36] Py：定时任务
来源：http://qw.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://ee.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://au.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ze.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ws.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://xa.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://gt.huixiangedu.cn

sys.stdout.isatty()
来源：http://ge.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://yz.colortex.cn

print("err", file=sys.stderr)
来源：http://ul.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://dq.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fh.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vp.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kk.nicolike.cn

[U43] PHP：声明命名空间
来源：http://ez.hahajie.cn

namespace App\Http;
来源：http://or.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://li.szxytkj.cn

declare(strict_types=1);
来源：http://dn.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://qa.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.nszjky.cn

[U46] PHP：可空类型
来源：http://hc.gzmigu.cn

?string $name = null
来源：http://ew.shxzskj.cn

[U47] PHP：联合类型
来源：http://uj.huixiangedu.cn

int|string $id
来源：http://ap.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://qe.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bv.bjjhwx.cn

[U49] PHP：只读属性
来源：http://og.gzmigu.cn

public readonly string $name
来源：http://we.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://fi.shxzskj.cn

public function __construct(private int $id) {}
来源：http://hi.hnjuh.cn

[U51] PHP：数组解构
来源：http://fy.muxihuayi.cn

[$a, $b] = $arr;
来源：http://jm.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://dh.asd995.cn

$double = fn($x) => $x * 2;
来源：http://an.newstarts.cn

[U53] PHP：空合并运算符
来源：http://fr.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://zr.colortex.cn

[U54] PHP：空安全调用
来源：http://ui.hahajie.cn

$obj?->method()
来源：http://oa.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://us.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fz.shxzukj.cn

[U56] PHP：命名参数
来源：http://mr.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ss.shxzskj.cn

[U57] PHP：字符串插值
来源：http://as.lnxyls.cn

"值: {$a}"
来源：http://vb.nszjky.cn

[U58] PHP：数组三件套
来源：http://ej.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gg.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://ac.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://he.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://rq.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kj.lnxyls.cn

[U61] PHP：正则
来源：http://gz.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qr.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://es.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kb.newstarts.cn

[U63] PHP：文件读写
来源：http://qv.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sx.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://uf.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://sb.szsharing.cn

[U65] PHP：会话
来源：http://ox.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dg.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://cr.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://um.colortex.cn

[U67] PHP：处理文件上传
来源：http://ap.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hr.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://xi.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cj.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://dp.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oe.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://rd.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://to.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ti.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://dd.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://xz.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://vm.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://jo.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://sv.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://hv.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://uu.huanxung.cn

[U75] PHP：依赖注入
来源：http://md.jianghongdianzi.cn

composer require psr/container
来源：http://hl.hnjuh.cn

[U76] PHP：简单路由
来源：http://gb.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dc.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://ed.bjjhwx.cn

composer require twig/twig
来源：http://ae.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://mh.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://kd.nicolike.cn

[U79] PHP：静态分析
来源：http://ox.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://mg.newstarts.cn

[U80] PHP：代码规范修复
来源：http://np.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bo.newstarts.cn

[U81] JS：初始化项目
来源：http://zv.shxzskj.cn

npm init -y;  npm i express
来源：http://kc.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://up.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dx.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://gl.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zu.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://xl.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mf.shxzukj.cn

[U85] JS：可选链
来源：http://ki.shtwfgs.cn

a?.b?.c
来源：http://ww.shxzukj.cn

[U86] JS：空值合并
来源：http://ne.haigaiapp.cn

a ?? b
来源：http://wi.521024.cn

[U87] JS：解构默认值
来源：http://wg.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://so.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://zh.bjjhwx.cn

{ ...a, ...b }
来源：http://fq.bookmarksfly.cn

[U89] JS：数组去重
来源：http://ve.huixinmuqiang.cn

[...new Set(arr)]
来源：http://ul.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://wq.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://cg.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://pi.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nc.muxihuayi.cn

[U92] JS：深拷贝
来源：http://ra.bjjhwx.cn

structuredClone(obj)
来源：http://wf.shxzukj.cn

[U93] JS：模板字符串
来源：http://nb.szxytkj.cn

`共 ${n} 条`
来源：http://ma.muxihuayi.cn

[U94] JS：箭头函数
来源：http://lh.huanxung.cn

const double = x => x * 2;
来源：http://kp.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://sb.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://jm.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://hh.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aa.521024.cn

[U97] JS：并发请求
来源：http://ji.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zu.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://vw.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pg.szxytkj.cn

[U99] JS：事件监听
来源：http://br.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://ld.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://pc.wgjwhj.cn

document.querySelector(".item")
来源：http://fc.gzmigu.cn

[U101] JS：classList 操作
来源：http://iw.hahajie.cn

el.classList.toggle("active")
来源：http://da.jctech888.com.cn

[U102] JS：本地存储
来源：http://vy.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xq.shxzukj.cn

[U103] JS：定时器
来源：http://yb.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bi.nszjky.cn

[U104] JS：防抖
来源：http://wy.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fg.bjjhwx.cn

[U105] JS：节流
来源：http://ov.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ve.9csxet.cn

[U106] JS：日期格式化
来源：http://ch.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gs.hahajie.cn

[U107] JS：数字千分位
来源：http://ck.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jt.haigaiapp.cn

[U108] JS：随机整数
来源：http://zm.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://al.asd995.cn

[U109] JS：数组分组
来源：http://ke.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://tz.shxzukj.cn

[U110] JS：数组分块
来源：http://se.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vr.gzmigu.cn

[U111] JS：对象转 Map
来源：http://ro.hahajie.cn

new Map(Object.entries(obj))
来源：http://bg.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://qh.nicolike.cn

"7".padStart(3, "0")
来源：http://fm.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://jk.shxzskj.cn

s.replaceAll("a", "b")
来源：http://uj.newstarts.cn

[U114] JS：JSON 深比较
来源：http://he.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://if.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://qi.nszjky.cn

crypto.randomUUID()
来源：http://yn.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ow.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://my.shxzukj.cn

[U117] JS：单元测试
来源：http://ry.asd995.cn

npm i -D vitest;  npx vitest
来源：http://bg.colortex.cn

[U118] JS：开发服务器
来源：http://bb.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://qa.hahajie.cn


<!-- 参考信息 -->