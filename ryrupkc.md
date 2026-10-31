代发 wailian999

[T37] Lua：字符串拼接
来源：http://xk.asd995.cn

"a" .. "b"
来源：http://ji.gzmigu.cn

[T38] Lua：条件
来源：http://qh.nszjky.cn

if x > 0 then print("正") end
来源：http://mq.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://id.nszjky.cn

string.find(s, "%d+")
来源：http://ia.huanxung.cn

[T40] Lua：元表
来源：http://ek.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://or.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ux.huanxung.cn

print "Hello\n";
来源：http://cs.colortex.cn

[T42] Perl：变量类型
来源：http://sz.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oc.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://jk.wgjwhj.cn

"值: $a"
来源：http://fv.shxzukj.cn

[T44] Perl：条件
来源：http://vq.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://ou.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://ik.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://ms.9csxet.cn

[T46] Perl：哈希操作
来源：http://cj.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jk.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://ol.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rl.newstarts.cn

[T48] Perl：正则替换
来源：http://ep.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://ts.jianghongdianzi.cn

[T49] Perl：函数
来源：http://gi.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dn.nszjky.cn

[T50] Perl：逐行读文件
来源：http://am.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qz.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://xo.szsharing.cn

[T51] Scala：Hello World
来源：http://ib.jctech888.com.cn

println("Hello")
来源：http://gj.haigaiapp.cn

[T52] Scala：变量
来源：http://yv.lnxyls.cn

val a = 1;  var b = 2
来源：http://qb.shxzukj.cn

[T53] Scala：字符串插值
来源：http://vp.jianghongdianzi.cn

s"值: $b"
来源：http://hg.shxzskj.cn

[T54] Scala：集合映射
来源：http://iz.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://nb.colortex.cn

[T55] Scala：集合过滤
来源：http://rc.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mg.9csxet.cn

[T56] Scala：样例类
来源：http://sb.newstarts.cn

case class User(name: String, age: Int)
来源：http://dx.hahajie.cn

[T57] Scala：模式匹配
来源：http://px.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ez.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://tx.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ue.shtwfgs.cn

[T59] Scala：循环
来源：http://kd.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://cn.szxytkj.cn

[T60] Scala：折叠
来源：http://pw.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ya.jianghongdianzi.cn

================================================================================
来源：http://kt.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ve.jctech888.com.cn

================================================================================
来源：http://jh.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://rk.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sv.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://lo.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gn.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://ar.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rl.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ra.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xw.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://ed.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://ub.shxzskj.cn

[U06] Py：合并两个字典
来源：http://md.hahajie.cn

{**a, **b}
来源：http://iw.521024.cn

[U07] Py：反转字典键值
来源：http://ol.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://sl.szsharing.cn

[U08] Py：展平二维列表
来源：http://rp.nszjky.cn

[y for x in nested for y in x]
来源：http://ka.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://oa.asd995.cn

max(d, key=d.get)
来源：http://sw.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://sz.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ne.nszjky.cn

[U11] Py：生成器表达式
来源：http://we.chemitech.net.cn

(x * 2 for x in arr)
来源：http://pi.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pe.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://ml.521024.cn

[U13] Py：固定长度队列
来源：http://mt.chemitech.net.cn

deque(maxlen=10)
来源：http://cn.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://ol.hnjuh.cn

defaultdict(list)
来源：http://ud.shxzskj.cn

[U15] Py：高精度计时
来源：http://az.newstarts.cn

t = time.perf_counter()
来源：http://jz.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://js.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iu.9csxet.cn

[U17] Py：初始化日志
来源：http://fb.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://rf.muxihuayi.cn

[U18] Py：预编译正则
来源：http://nb.asd995.cn

pat = re.compile(r"\d+")
来源：http://qi.nicolike.cn

[U19] Py：正则替换带回调
来源：http://ds.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wl.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://tx.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://nc.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://vf.521024.cn

@contextlib.contextmanager
来源：http://cf.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://xh.huixinmuqiang.cn

list(zip(*m))
来源：http://fs.9csxet.cn

[U23] Py：分块读取大文件
来源：http://aq.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eb.shxzskj.cn

[U24] Py：路径操作
来源：http://iq.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qy.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://rm.9csxet.cn

csv.DictReader(f)
来源：http://tx.bjjhwx.cn

[U26] Py：并发下载
来源：http://qa.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qa.newstarts.cn

[U27] Py：异步 HTTP
来源：http://oy.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://xg.lnxyls.cn

[U28] Py：类型别名
来源：http://fv.jianghongdianzi.cn

UserId = int
来源：http://bb.szsharing.cn

[U29] Py：属性校验
来源：http://ka.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://ro.jianghongdianzi.cn

[U30] Py：数据类
来源：http://ph.chemitech.net.cn

@dataclass(slots=True)
来源：http://mp.shxzukj.cn

[U31] Py：单测
来源：http://ot.bookmarksfly.cn

python -m pytest -q
来源：http://jn.bjjhwx.cn

[U32] Py：代码格式化
来源：http://ir.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://dy.lnxyls.cn

[U33] Py：打包发布
来源：http://cl.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://sk.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://yz.9csxet.cn

chardet.detect(raw)
来源：http://zg.nszjky.cn

[U35] Py：发送邮件
来源：http://me.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://el.nicolike.cn

[U36] Py：定时任务
来源：http://ya.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://vw.shxzukj.cn

[U37] Py：读写 Excel
来源：http://sr.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vf.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://en.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://rt.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://an.bjjhwx.cn

sys.stdout.isatty()
来源：http://mt.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://da.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://vl.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://zs.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ur.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://la.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ad.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://fa.bjjhwx.cn

namespace App\Http;
来源：http://wb.colortex.cn

[U44] PHP：开启严格类型
来源：http://em.panjiajie.cn

declare(strict_types=1);
来源：http://bh.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://hp.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fo.hnjuh.cn

[U46] PHP：可空类型
来源：http://lw.lnxyls.cn

?string $name = null
来源：http://yd.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://zu.shxzukj.cn

int|string $id
来源：http://pt.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://bp.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ht.shtwfgs.cn

[U49] PHP：只读属性
来源：http://bv.521024.cn

public readonly string $name
来源：http://mh.521024.cn

[U50] PHP：构造器属性提升
来源：http://pk.nszjky.cn

public function __construct(private int $id) {}
来源：http://so.haigaiapp.cn

[U51] PHP：数组解构
来源：http://ef.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://ax.nicolike.cn

[U52] PHP：箭头函数
来源：http://lp.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://rt.nszjky.cn

[U53] PHP：空合并运算符
来源：http://ah.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://ip.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://nu.bookmarksfly.cn

$obj?->method()
来源：http://de.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://xd.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ia.gzmigu.cn

[U56] PHP：命名参数
来源：http://jy.muxihuayi.cn

f(a: 1, b: 2)
来源：http://wc.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://pk.hnjuh.cn

"值: {$a}"
来源：http://ub.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://aj.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gl.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://ep.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ew.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://xt.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wh.shtwfgs.cn

[U61] PHP：正则
来源：http://tp.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wk.9csxet.cn

[U62] PHP：日期对象
来源：http://rg.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eh.wgjwhj.cn

[U63] PHP：文件读写
来源：http://no.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://io.newstarts.cn

[U64] PHP：目录遍历
来源：http://lp.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://co.gzmigu.cn

[U65] PHP：会话
来源：http://sg.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fp.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://kg.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zv.newstarts.cn

[U67] PHP：处理文件上传
来源：http://ka.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vx.nszjky.cn

[U68] PHP：PDO 连接
来源：http://ax.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lt.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://qi.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fp.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://th.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cb.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://tx.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://ux.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://qz.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://oa.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://qm.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://gg.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://gj.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://qj.shxzukj.cn

[U75] PHP：依赖注入
来源：http://tx.bookmarksfly.cn

composer require psr/container
来源：http://bs.szxytkj.cn

[U76] PHP：简单路由
来源：http://fh.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rc.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://il.nszjky.cn

composer require twig/twig
来源：http://ft.newstarts.cn

[U78] PHP：单元测试
来源：http://vn.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://hf.9csxet.cn

[U79] PHP：静态分析
来源：http://aj.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://dk.521024.cn

[U80] PHP：代码规范修复
来源：http://zg.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vk.521024.cn

[U81] JS：初始化项目
来源：http://jl.lnxyls.cn

npm init -y;  npm i express
来源：http://tv.9csxet.cn

[U82] JS：package.json 脚本
来源：http://wp.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ot.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://mt.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://go.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://ry.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://so.nszjky.cn

[U85] JS：可选链
来源：http://xv.szxytkj.cn

a?.b?.c
来源：http://su.muxihuayi.cn

[U86] JS：空值合并
来源：http://an.szxytkj.cn

a ?? b
来源：http://vp.chemitech.net.cn

[U87] JS：解构默认值
来源：http://bx.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://es.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://at.shxzukj.cn

{ ...a, ...b }
来源：http://tp.wgjwhj.cn

[U89] JS：数组去重
来源：http://ml.hahajie.cn

[...new Set(arr)]
来源：http://by.hnjuh.cn

[U90] JS：数字数组排序
来源：http://xi.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://yx.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ro.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fc.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://cy.asd995.cn

structuredClone(obj)
来源：http://bk.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://rb.bookmarksfly.cn

`共 ${n} 条`
来源：http://sk.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://xt.muxihuayi.cn

const double = x => x * 2;
来源：http://sd.shxzukj.cn

[U95] JS：Promise 包装
来源：http://fo.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://vp.huanxung.cn

[U96] JS：async/await 与异常
来源：http://mk.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ry.huixiangedu.cn

[U97] JS：并发请求
来源：http://ph.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bg.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ui.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ac.hahajie.cn

[U99] JS：事件监听
来源：http://aw.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://ti.nszjky.cn

[U100] JS：DOM 查询
来源：http://ia.521024.cn

document.querySelector(".item")
来源：http://ai.hnjuh.cn

[U101] JS：classList 操作
来源：http://db.huixiangedu.cn

el.classList.toggle("active")
来源：http://zw.huanxung.cn

[U102] JS：本地存储
来源：http://qq.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xd.hahajie.cn

[U103] JS：定时器
来源：http://ua.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ny.szsharing.cn

[U104] JS：防抖
来源：http://pu.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ux.colortex.cn

[U105] JS：节流
来源：http://bv.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pg.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://tt.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lz.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://xg.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iq.muxihuayi.cn

[U108] JS：随机整数
来源：http://bp.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ko.asd995.cn

[U109] JS：数组分组
来源：http://by.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://ei.nicolike.cn

[U110] JS：数组分块
来源：http://nz.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ce.huanxung.cn

[U111] JS：对象转 Map
来源：http://id.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://sm.huanxung.cn

[U112] JS：字符串补位
来源：http://ql.hnjuh.cn

"7".padStart(3, "0")
来源：http://ol.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://oy.521024.cn

s.replaceAll("a", "b")
来源：http://fm.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://qr.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ff.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://tx.huixiangedu.cn

crypto.randomUUID()
来源：http://ib.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://ff.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://hk.gzmigu.cn

[U117] JS：单元测试
来源：http://ii.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://kd.colortex.cn

[U118] JS：开发服务器
来源：http://ha.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://di.szxytkj.cn

[U119] JS：生产构建
来源：http://ml.shxzskj.cn

npx vite build
来源：http://kx.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://wd.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://pj.hahajie.cn

================================================================================
来源：http://am.panjiajie.cn

统计汇总
来源：http://lq.shxzukj.cn

================================================================================
来源：http://yw.shxzukj.cn

按语言统计（条）：
来源：http://bs.hnjuh.cn

Python ......... 252
来源：http://ax.szsharing.cn

PHP ............ 252
来源：http://vq.shtwfgs.cn

JavaScript ..... 252
来源：http://vq.jianghongdianzi.cn

TypeScript ..... 212
来源：http://dn.chemitech.net.cn


<!-- 参考信息 -->