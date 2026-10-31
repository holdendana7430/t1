代发 wailian999

[T29] Swift：guard 提前返回
来源：http://ek.wgjwhj.cn

guard let x = opt else { return }
来源：http://jb.colortex.cn

[T30] Swift：协议
来源：http://hk.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://uc.gzmigu.cn

[T31] Lua：Hello World
来源：http://uu.bjjhwx.cn

print("Hello")
来源：http://on.nicolike.cn

[T32] Lua：局部变量
来源：http://qw.huixiangedu.cn

local a = 1
来源：http://bq.521024.cn

[T33] Lua：表（数组）
来源：http://gx.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vd.yuexingan06.cn

[T34] Lua：遍历表
来源：http://wq.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vr.yuexingan06.cn

[T35] Lua：字典表
来源：http://xz.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://tz.gzmigu.cn

[T36] Lua：函数
来源：http://qy.yuexingan06.cn

function add(a, b) return a + b end
来源：http://sz.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://sh.nszjky.cn

"a" .. "b"
来源：http://ny.asd995.cn

[T38] Lua：条件
来源：http://vy.shxzukj.cn

if x > 0 then print("正") end
来源：http://ps.asd995.cn

[T39] Lua：模式匹配
来源：http://qt.huanxung.cn

string.find(s, "%d+")
来源：http://pq.chemitech.net.cn

[T40] Lua：元表
来源：http://ea.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://ji.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://lc.jctech888.com.cn

print "Hello\n";
来源：http://fo.hnjuh.cn

[T42] Perl：变量类型
来源：http://ev.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://on.shxzukj.cn

[T43] Perl：字符串插值
来源：http://ps.shxzukj.cn

"值: $a"
来源：http://hy.hnjuh.cn

[T44] Perl：条件
来源：http://ph.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://nx.newstarts.cn

[T45] Perl：数组遍历
来源：http://bf.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://xs.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://cj.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://el.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://rx.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bs.hnjuh.cn

[T48] Perl：正则替换
来源：http://et.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://et.bjjhwx.cn

[T49] Perl：函数
来源：http://xm.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nu.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://wb.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ch.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://xd.nicolike.cn

[T51] Scala：Hello World
来源：http://bp.shtwfgs.cn

println("Hello")
来源：http://li.521024.cn

[T52] Scala：变量
来源：http://bh.muxihuayi.cn

val a = 1;  var b = 2
来源：http://gc.szxytkj.cn

[T53] Scala：字符串插值
来源：http://ej.szsharing.cn

s"值: $b"
来源：http://yq.bjjhwx.cn

[T54] Scala：集合映射
来源：http://xm.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://ay.huanxung.cn

[T55] Scala：集合过滤
来源：http://fk.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ln.shxzukj.cn

[T56] Scala：样例类
来源：http://hr.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://mw.panjiajie.cn

[T57] Scala：模式匹配
来源：http://zz.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qd.haigaiapp.cn

[T58] Scala：函数定义
来源：http://ag.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ps.szsharing.cn

[T59] Scala：循环
来源：http://qe.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://qw.hahajie.cn

[T60] Scala：折叠
来源：http://oq.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jm.521024.cn

================================================================================
来源：http://hf.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iv.yuexingan06.cn

================================================================================
来源：http://ck.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://jk.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nk.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://ng.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lm.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://yc.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uu.szxytkj.cn

[U04] Py：变量调试打印
来源：http://ck.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ka.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://te.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://tx.colortex.cn

[U06] Py：合并两个字典
来源：http://uw.jctech888.com.cn

{**a, **b}
来源：http://zx.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://pu.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ay.nicolike.cn

[U08] Py：展平二维列表
来源：http://bj.muxihuayi.cn

[y for x in nested for y in x]
来源：http://ok.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://gi.shtwfgs.cn

max(d, key=d.get)
来源：http://vb.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://px.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vm.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://bj.nicolike.cn

(x * 2 for x in arr)
来源：http://rh.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rp.szsharing.cn

Counter(arr).most_common(3)
来源：http://pm.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://xr.hahajie.cn

deque(maxlen=10)
来源：http://pe.hahajie.cn

[U14] Py：分组收集到列表
来源：http://dm.huixinmuqiang.cn

defaultdict(list)
来源：http://th.wgjwhj.cn

[U15] Py：高精度计时
来源：http://ld.colortex.cn

t = time.perf_counter()
来源：http://ey.asd995.cn

[U16] Py：命令行参数解析
来源：http://ms.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://is.nicolike.cn

[U17] Py：初始化日志
来源：http://su.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://tx.9csxet.cn

[U18] Py：预编译正则
来源：http://bk.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://nd.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://qs.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ia.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://lw.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://ge.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://pl.haigaiapp.cn

@contextlib.contextmanager
来源：http://rn.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://oa.yuexingan06.cn

list(zip(*m))
来源：http://gg.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://pt.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vt.jctech888.com.cn

[U24] Py：路径操作
来源：http://fd.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://je.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://zt.huanxung.cn

csv.DictReader(f)
来源：http://el.shxzskj.cn

[U26] Py：并发下载
来源：http://nu.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vb.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://gw.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://gy.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://wm.colortex.cn

UserId = int
来源：http://wo.yuexingan06.cn

[U29] Py：属性校验
来源：http://gh.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://rq.bjjhwx.cn

[U30] Py：数据类
来源：http://zy.hnjuh.cn

@dataclass(slots=True)
来源：http://xi.9csxet.cn

[U31] Py：单测
来源：http://ev.hahajie.cn

python -m pytest -q
来源：http://sd.9csxet.cn

[U32] Py：代码格式化
来源：http://ea.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://di.9csxet.cn

[U33] Py：打包发布
来源：http://px.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://ff.shxzskj.cn

[U34] Py：判断编码
来源：http://xz.jianghongdianzi.cn

chardet.detect(raw)
来源：http://ln.gzmigu.cn

[U35] Py：发送邮件
来源：http://ek.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vd.panjiajie.cn

[U36] Py：定时任务
来源：http://kf.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://yg.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://ib.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://br.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ix.szsharing.cn

Path(__file__).resolve().parent
来源：http://bk.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://wj.nszjky.cn

sys.stdout.isatty()
来源：http://ib.521024.cn

[U40] Py：打印到标准错误
来源：http://oa.szxytkj.cn

print("err", file=sys.stderr)
来源：http://tw.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xi.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nr.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://qq.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zm.colortex.cn

[U43] PHP：声明命名空间
来源：http://qn.nicolike.cn

namespace App\Http;
来源：http://qu.colortex.cn

[U44] PHP：开启严格类型
来源：http://jj.newstarts.cn

declare(strict_types=1);
来源：http://yc.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://by.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fn.shxzukj.cn

[U46] PHP：可空类型
来源：http://bd.gzmigu.cn

?string $name = null
来源：http://oc.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://qp.huixinmuqiang.cn

int|string $id
来源：http://qq.panjiajie.cn

[U48] PHP：纯枚举
来源：http://zd.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mw.lnxyls.cn

[U49] PHP：只读属性
来源：http://ah.colortex.cn

public readonly string $name
来源：http://ny.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://vx.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://pi.bjjhwx.cn

[U51] PHP：数组解构
来源：http://dp.nicolike.cn

[$a, $b] = $arr;
来源：http://qt.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://yt.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://ew.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://yv.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://ms.szxytkj.cn

[U54] PHP：空安全调用
来源：http://sn.bjjhwx.cn

$obj?->method()
来源：http://tx.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://gh.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ic.nszjky.cn

[U56] PHP：命名参数
来源：http://an.yuexingan06.cn

f(a: 1, b: 2)
来源：http://ig.shxzukj.cn

[U57] PHP：字符串插值
来源：http://cu.yuntaijiaju.cn

"值: {$a}"
来源：http://ol.9csxet.cn

[U58] PHP：数组三件套
来源：http://rk.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zo.newstarts.cn

[U59] PHP：自定义排序
来源：http://ti.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gd.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://zw.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dv.yuntaijiaju.cn

[U61] PHP：正则
来源：http://rm.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qo.bjjhwx.cn

[U62] PHP：日期对象
来源：http://cp.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qn.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://vb.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qy.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://sz.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://xq.shxzukj.cn

[U65] PHP：会话
来源：http://hb.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lc.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://gy.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zr.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://dn.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://er.521024.cn

[U68] PHP：PDO 连接
来源：http://mz.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bb.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://lp.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iq.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://ns.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ze.lnxyls.cn

[U71] PHP：抛出异常
来源：http://mn.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://pg.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://zo.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://sl.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://wk.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://no.asd995.cn

[U74] PHP：读取环境变量
来源：http://cb.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://gt.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://yv.shxzukj.cn

composer require psr/container
来源：http://hm.chemitech.net.cn

[U76] PHP：简单路由
来源：http://vm.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ss.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://bl.muxihuayi.cn

composer require twig/twig
来源：http://ev.muxihuayi.cn

[U78] PHP：单元测试
来源：http://ax.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://hf.wgjwhj.cn

[U79] PHP：静态分析
来源：http://uh.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://yy.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://hx.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gj.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ss.yuexingan06.cn

npm init -y;  npm i express
来源：http://so.9csxet.cn

[U82] JS：package.json 脚本
来源：http://dw.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ei.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://yu.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xy.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://hm.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yl.9csxet.cn

[U85] JS：可选链
来源：http://sf.hnjuh.cn

a?.b?.c
来源：http://xf.hnjuh.cn

[U86] JS：空值合并
来源：http://sy.shxzukj.cn

a ?? b
来源：http://fk.yuexingan06.cn

[U87] JS：解构默认值
来源：http://vn.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://uq.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://lu.shxzukj.cn

{ ...a, ...b }
来源：http://at.yuexingan06.cn

[U89] JS：数组去重
来源：http://qc.nicolike.cn

[...new Set(arr)]
来源：http://dw.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://zm.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://mk.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://tg.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qv.nszjky.cn

[U92] JS：深拷贝
来源：http://rq.colortex.cn

structuredClone(obj)
来源：http://xj.bjjhwx.cn

[U93] JS：模板字符串
来源：http://uf.newstarts.cn

`共 ${n} 条`
来源：http://jv.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://wx.asd995.cn

const double = x => x * 2;
来源：http://cn.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://pt.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ez.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://ka.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gt.newstarts.cn

[U97] JS：并发请求
来源：http://qa.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mk.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://yg.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jx.wgjwhj.cn

[U99] JS：事件监听
来源：http://qh.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://kb.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://ut.bjjhwx.cn

document.querySelector(".item")
来源：http://yb.hnjuh.cn

[U101] JS：classList 操作
来源：http://ol.huanxung.cn

el.classList.toggle("active")
来源：http://md.newstarts.cn

[U102] JS：本地存储
来源：http://bw.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fa.muxihuayi.cn

[U103] JS：定时器
来源：http://on.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bq.hnjuh.cn

[U104] JS：防抖
来源：http://gu.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fq.9csxet.cn

[U105] JS：节流
来源：http://cq.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rm.szxytkj.cn

[U106] JS：日期格式化
来源：http://vp.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zg.chemitech.net.cn

[U107] JS：数字千分位
来源：http://bx.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eq.huixiangedu.cn

[U108] JS：随机整数
来源：http://jh.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xf.wgjwhj.cn

[U109] JS：数组分组
来源：http://zv.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://vc.bjjhwx.cn

[U110] JS：数组分块
来源：http://zc.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zt.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://ii.asd995.cn

new Map(Object.entries(obj))
来源：http://ch.shtwfgs.cn

[U112] JS：字符串补位
来源：http://fa.hahajie.cn

"7".padStart(3, "0")
来源：http://vm.lnxyls.cn

[U113] JS：正则替换全部
来源：http://ib.huanxung.cn

s.replaceAll("a", "b")
来源：http://oc.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://qm.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mv.lnxyls.cn

[U115] JS：生成 UUID
来源：http://eh.nicolike.cn

crypto.randomUUID()
来源：http://pg.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://le.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://dw.yuexingan06.cn


<!-- 参考信息 -->