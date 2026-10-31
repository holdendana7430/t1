代发 wailian999

[T33] Lua：表（数组）
来源：http://kg.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ma.lnxyls.cn

[T34] Lua：遍历表
来源：http://rl.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fk.gzmigu.cn

[T35] Lua：字典表
来源：http://iw.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://yx.shtwfgs.cn

[T36] Lua：函数
来源：http://bl.wgjwhj.cn

function add(a, b) return a + b end
来源：http://kb.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://yk.lnxyls.cn

"a" .. "b"
来源：http://di.szxytkj.cn

[T38] Lua：条件
来源：http://fc.nszjky.cn

if x > 0 then print("正") end
来源：http://tp.shxzskj.cn

[T39] Lua：模式匹配
来源：http://xn.gzmigu.cn

string.find(s, "%d+")
来源：http://ry.yuexingan06.cn

[T40] Lua：元表
来源：http://qx.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://ov.chemitech.net.cn

[T41] Perl：Hello World
来源：http://cp.9csxet.cn

print "Hello\n";
来源：http://vd.jctech888.com.cn

[T42] Perl：变量类型
来源：http://mq.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ak.nszjky.cn

[T43] Perl：字符串插值
来源：http://eo.panjiajie.cn

"值: $a"
来源：http://gi.bookmarksfly.cn

[T44] Perl：条件
来源：http://nj.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://dj.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ih.colortex.cn

for my $x (@arr) { print $x; }
来源：http://bg.lnxyls.cn

[T46] Perl：哈希操作
来源：http://iw.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ph.521024.cn

[T47] Perl：正则捕获
来源：http://pi.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jn.nicolike.cn

[T48] Perl：正则替换
来源：http://wo.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://rm.yuntaijiaju.cn

[T49] Perl：函数
来源：http://gw.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://su.huanxung.cn

[T50] Perl：逐行读文件
来源：http://vl.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://du.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://df.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://cg.jianghongdianzi.cn

println("Hello")
来源：http://qs.gzmigu.cn

[T52] Scala：变量
来源：http://wx.szsharing.cn

val a = 1;  var b = 2
来源：http://aq.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://fa.shtwfgs.cn

s"值: $b"
来源：http://we.yuexingan06.cn

[T54] Scala：集合映射
来源：http://kz.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://fw.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://ic.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mz.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://lz.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://yo.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://az.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nj.haigaiapp.cn

[T58] Scala：函数定义
来源：http://yo.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ph.asd995.cn

[T59] Scala：循环
来源：http://jm.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://zr.shxzukj.cn

[T60] Scala：折叠
来源：http://uo.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://si.yuntaijiaju.cn

================================================================================
来源：http://ze.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dn.huixinmuqiang.cn

================================================================================
来源：http://qz.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ds.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mz.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://fa.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wr.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://vx.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fa.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://wf.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bw.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://ty.521024.cn

list(dict.fromkeys(arr))
来源：http://tv.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://th.asd995.cn

{**a, **b}
来源：http://hf.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://qa.huanxung.cn

{v: k for k, v in d.items()}
来源：http://jl.hahajie.cn

[U08] Py：展平二维列表
来源：http://gq.colortex.cn

[y for x in nested for y in x]
来源：http://gy.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://vr.shxzukj.cn

max(d, key=d.get)
来源：http://ei.newstarts.cn

[U10] Py：按值排序字典
来源：http://cf.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qn.hnjuh.cn

[U11] Py：生成器表达式
来源：http://vh.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://ht.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hz.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://ux.521024.cn

[U13] Py：固定长度队列
来源：http://ih.panjiajie.cn

deque(maxlen=10)
来源：http://ye.nszjky.cn

[U14] Py：分组收集到列表
来源：http://ov.bookmarksfly.cn

defaultdict(list)
来源：http://xy.yuexingan06.cn

[U15] Py：高精度计时
来源：http://nf.gzmigu.cn

t = time.perf_counter()
来源：http://pt.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://fa.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ff.hahajie.cn

[U17] Py：初始化日志
来源：http://jf.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://sl.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://ma.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://rl.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://mo.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wc.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://vn.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://vs.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://fs.asd995.cn

@contextlib.contextmanager
来源：http://kh.nszjky.cn

[U22] Py：矩阵转置
来源：http://pn.yuexingan06.cn

list(zip(*m))
来源：http://gz.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://mg.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xh.hnjuh.cn

[U24] Py：路径操作
来源：http://wt.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ih.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://fp.nszjky.cn

csv.DictReader(f)
来源：http://jm.jctech888.com.cn

[U26] Py：并发下载
来源：http://de.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cc.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://uz.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://yp.wgjwhj.cn

[U28] Py：类型别名
来源：http://qw.hnjuh.cn

UserId = int
来源：http://hm.huixiangedu.cn

[U29] Py：属性校验
来源：http://we.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://ym.shtwfgs.cn

[U30] Py：数据类
来源：http://je.colortex.cn

@dataclass(slots=True)
来源：http://kt.jianghongdianzi.cn

[U31] Py：单测
来源：http://qf.colortex.cn

python -m pytest -q
来源：http://ih.shxzukj.cn

[U32] Py：代码格式化
来源：http://qo.hahajie.cn

ruff format . && ruff check --fix .
来源：http://wc.521024.cn

[U33] Py：打包发布
来源：http://hx.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://rm.9csxet.cn

[U34] Py：判断编码
来源：http://qk.hahajie.cn

chardet.detect(raw)
来源：http://dz.jctech888.com.cn

[U35] Py：发送邮件
来源：http://fn.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cp.shxzskj.cn

[U36] Py：定时任务
来源：http://as.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://dp.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://gd.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jz.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://up.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://sf.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://ff.jctech888.com.cn

sys.stdout.isatty()
来源：http://sm.huanxung.cn

[U40] Py：打印到标准错误
来源：http://ls.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://nr.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://gc.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yj.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://lk.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yb.hahajie.cn

[U43] PHP：声明命名空间
来源：http://ip.huixinmuqiang.cn

namespace App\Http;
来源：http://ea.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://mf.shtwfgs.cn

declare(strict_types=1);
来源：http://xk.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://ri.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ru.521024.cn

[U46] PHP：可空类型
来源：http://qm.bookmarksfly.cn

?string $name = null
来源：http://py.521024.cn

[U47] PHP：联合类型
来源：http://mj.haigaiapp.cn

int|string $id
来源：http://cd.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://ca.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sa.asd995.cn

[U49] PHP：只读属性
来源：http://ql.gzmigu.cn

public readonly string $name
来源：http://vt.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://yc.521024.cn

public function __construct(private int $id) {}
来源：http://to.nszjky.cn

[U51] PHP：数组解构
来源：http://tx.9csxet.cn

[$a, $b] = $arr;
来源：http://jr.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://yf.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://fw.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://ml.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://cd.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://pa.nszjky.cn

$obj?->method()
来源：http://rm.shxzskj.cn

[U55] PHP：match 表达式
来源：http://ur.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xc.nicolike.cn

[U56] PHP：命名参数
来源：http://hm.shtwfgs.cn

f(a: 1, b: 2)
来源：http://rc.colortex.cn

[U57] PHP：字符串插值
来源：http://na.hahajie.cn

"值: {$a}"
来源：http://aw.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://so.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vo.colortex.cn

[U59] PHP：自定义排序
来源：http://se.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vm.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://gu.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fy.nicolike.cn

[U61] PHP：正则
来源：http://kt.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yf.hnjuh.cn

[U62] PHP：日期对象
来源：http://vv.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wb.colortex.cn

[U63] PHP：文件读写
来源：http://ms.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vt.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://vx.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://oz.szxytkj.cn

[U65] PHP：会话
来源：http://vp.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dh.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://de.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://up.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://jf.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zg.9csxet.cn

[U68] PHP：PDO 连接
来源：http://sy.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qr.521024.cn

[U69] PHP：PDO 预处理
来源：http://vl.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hy.521024.cn

[U70] PHP：PDO 事务
来源：http://es.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ze.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://lk.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://gk.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://cv.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://jp.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://ap.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://tq.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://il.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ht.huanxung.cn

[U75] PHP：依赖注入
来源：http://du.huixiangedu.cn

composer require psr/container
来源：http://zl.shxzskj.cn

[U76] PHP：简单路由
来源：http://sa.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pz.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://wl.muxihuayi.cn

composer require twig/twig
来源：http://wx.shxzskj.cn

[U78] PHP：单元测试
来源：http://oj.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://wx.gzmigu.cn

[U79] PHP：静态分析
来源：http://np.asd995.cn

composer require --dev phpstan/phpstan
来源：http://ys.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://ka.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fo.colortex.cn

[U81] JS：初始化项目
来源：http://sd.nicolike.cn

npm init -y;  npm i express
来源：http://kj.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://bx.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kd.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://pi.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://on.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://gy.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eq.newstarts.cn

[U85] JS：可选链
来源：http://yf.yuexingan06.cn

a?.b?.c
来源：http://nh.hnjuh.cn

[U86] JS：空值合并
来源：http://na.haigaiapp.cn

a ?? b
来源：http://zh.shxzukj.cn

[U87] JS：解构默认值
来源：http://bj.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://bt.shxzukj.cn

[U88] JS：对象展开合并
来源：http://qb.9csxet.cn

{ ...a, ...b }
来源：http://xm.shtwfgs.cn

[U89] JS：数组去重
来源：http://yw.newstarts.cn

[...new Set(arr)]
来源：http://qv.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://sr.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://zv.9csxet.cn

[U91] JS：对象键值遍历
来源：http://cr.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jm.shxzukj.cn

[U92] JS：深拷贝
来源：http://pt.lnxyls.cn

structuredClone(obj)
来源：http://iw.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ks.nszjky.cn

`共 ${n} 条`
来源：http://ye.szxytkj.cn

[U94] JS：箭头函数
来源：http://ae.shxzskj.cn

const double = x => x * 2;
来源：http://fh.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://ve.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://oj.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://il.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xf.521024.cn

[U97] JS：并发请求
来源：http://ua.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dy.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://ri.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://th.shtwfgs.cn

[U99] JS：事件监听
来源：http://vt.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://eu.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://dv.szsharing.cn

document.querySelector(".item")
来源：http://ti.hnjuh.cn

[U101] JS：classList 操作
来源：http://yb.haigaiapp.cn

el.classList.toggle("active")
来源：http://xp.jctech888.com.cn

[U102] JS：本地存储
来源：http://oo.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gq.wgjwhj.cn

[U103] JS：定时器
来源：http://gf.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rw.bookmarksfly.cn

[U104] JS：防抖
来源：http://cd.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://af.gzmigu.cn

[U105] JS：节流
来源：http://kw.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mw.shxzskj.cn

[U106] JS：日期格式化
来源：http://ig.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://or.szsharing.cn

[U107] JS：数字千分位
来源：http://sv.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ni.nszjky.cn

[U108] JS：随机整数
来源：http://dk.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tl.szsharing.cn

[U109] JS：数组分组
来源：http://of.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://nf.shxzukj.cn

[U110] JS：数组分块
来源：http://ui.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ik.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ee.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://sb.panjiajie.cn

[U112] JS：字符串补位
来源：http://ab.9csxet.cn

"7".padStart(3, "0")
来源：http://ac.hnjuh.cn

[U113] JS：正则替换全部
来源：http://zd.szxytkj.cn

s.replaceAll("a", "b")
来源：http://dg.nicolike.cn

[U114] JS：JSON 深比较
来源：http://wc.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zp.lnxyls.cn

[U115] JS：生成 UUID
来源：http://wd.nszjky.cn

crypto.randomUUID()
来源：http://kc.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://po.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://gg.jctech888.com.cn

[U117] JS：单元测试
来源：http://ab.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://ps.huixiangedu.cn

[U118] JS：开发服务器
来源：http://ag.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://qy.bookmarksfly.cn

[U119] JS：生产构建
来源：http://wx.shtwfgs.cn

npx vite build
来源：http://lp.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://wi.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://uj.yuntaijiaju.cn


<!-- 参考信息 -->