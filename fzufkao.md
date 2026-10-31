代发 wailian999

[T37] Lua：字符串拼接
来源：http://ck.hnjuh.cn

"a" .. "b"
来源：http://vv.haigaiapp.cn

[T38] Lua：条件
来源：http://wg.muxihuayi.cn

if x > 0 then print("正") end
来源：http://yg.hnjuh.cn

[T39] Lua：模式匹配
来源：http://pa.nszjky.cn

string.find(s, "%d+")
来源：http://lt.nszjky.cn

[T40] Lua：元表
来源：http://jz.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://cn.panjiajie.cn

[T41] Perl：Hello World
来源：http://vd.lnxyls.cn

print "Hello\n";
来源：http://pk.jctech888.com.cn

[T42] Perl：变量类型
来源：http://tb.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ml.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://jx.jianghongdianzi.cn

"值: $a"
来源：http://qf.hnjuh.cn

[T44] Perl：条件
来源：http://qh.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://bb.shxzskj.cn

[T45] Perl：数组遍历
来源：http://dt.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://mz.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://uo.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zz.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://fs.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xx.9csxet.cn

[T48] Perl：正则替换
来源：http://te.colortex.cn

$s =~ s/old/new/g;
来源：http://jb.newstarts.cn

[T49] Perl：函数
来源：http://ok.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ou.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://sr.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://si.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://xx.hnjuh.cn

[T51] Scala：Hello World
来源：http://ye.chemitech.net.cn

println("Hello")
来源：http://rz.lnxyls.cn

[T52] Scala：变量
来源：http://zp.yuexingan06.cn

val a = 1;  var b = 2
来源：http://eo.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://lg.shxzukj.cn

s"值: $b"
来源：http://fj.lnxyls.cn

[T54] Scala：集合映射
来源：http://wx.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://zx.shxzskj.cn

[T55] Scala：集合过滤
来源：http://zi.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ql.hahajie.cn

[T56] Scala：样例类
来源：http://lr.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://nb.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://zf.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gh.szxytkj.cn

[T58] Scala：函数定义
来源：http://kl.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wz.chemitech.net.cn

[T59] Scala：循环
来源：http://cq.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://bz.gzmigu.cn

[T60] Scala：折叠
来源：http://dh.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aa.hahajie.cn

================================================================================
来源：http://tt.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vv.szxytkj.cn

================================================================================
来源：http://uw.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://tq.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sg.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://po.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bx.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://rj.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gg.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://qb.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mu.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://rn.asd995.cn

list(dict.fromkeys(arr))
来源：http://kw.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ud.wgjwhj.cn

{**a, **b}
来源：http://mh.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://xl.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://mg.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://fo.nszjky.cn

[y for x in nested for y in x]
来源：http://nl.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://ba.bookmarksfly.cn

max(d, key=d.get)
来源：http://lg.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://wi.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dw.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://xg.huixiangedu.cn

(x * 2 for x in arr)
来源：http://vx.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zj.9csxet.cn

Counter(arr).most_common(3)
来源：http://ve.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ti.haigaiapp.cn

deque(maxlen=10)
来源：http://nb.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://fi.huixinmuqiang.cn

defaultdict(list)
来源：http://cn.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://ak.haigaiapp.cn

t = time.perf_counter()
来源：http://sx.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://ab.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://to.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://nr.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://le.chemitech.net.cn

[U18] Py：预编译正则
来源：http://iv.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://jv.newstarts.cn

[U19] Py：正则替换带回调
来源：http://ww.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fz.521024.cn

[U20] Py：缓存函数结果
来源：http://rn.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://ah.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://ja.shxzskj.cn

@contextlib.contextmanager
来源：http://ow.asd995.cn

[U22] Py：矩阵转置
来源：http://xk.szsharing.cn

list(zip(*m))
来源：http://bm.nszjky.cn

[U23] Py：分块读取大文件
来源：http://da.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ye.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://gw.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fi.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://ie.chemitech.net.cn

csv.DictReader(f)
来源：http://fv.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://ua.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ym.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://ct.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://cc.gzmigu.cn

[U28] Py：类型别名
来源：http://sq.panjiajie.cn

UserId = int
来源：http://gl.hahajie.cn

[U29] Py：属性校验
来源：http://jx.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://cp.shxzukj.cn

[U30] Py：数据类
来源：http://ml.bookmarksfly.cn

@dataclass(slots=True)
来源：http://fs.hnjuh.cn

[U31] Py：单测
来源：http://fx.nicolike.cn

python -m pytest -q
来源：http://vt.chemitech.net.cn

[U32] Py：代码格式化
来源：http://sl.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://nn.yuexingan06.cn

[U33] Py：打包发布
来源：http://yo.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ti.hnjuh.cn

[U34] Py：判断编码
来源：http://hf.szxytkj.cn

chardet.detect(raw)
来源：http://jh.haigaiapp.cn

[U35] Py：发送邮件
来源：http://bb.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kx.nicolike.cn

[U36] Py：定时任务
来源：http://ts.521024.cn

schedule.every(10).minutes.do(job)
来源：http://or.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://sm.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yv.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://dt.panjiajie.cn

Path(__file__).resolve().parent
来源：http://eb.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://kr.chemitech.net.cn

sys.stdout.isatty()
来源：http://ys.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://ig.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://rz.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://gr.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mf.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://kd.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hu.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://xn.nszjky.cn

namespace App\Http;
来源：http://ec.newstarts.cn

[U44] PHP：开启严格类型
来源：http://ns.huixiangedu.cn

declare(strict_types=1);
来源：http://lm.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://gz.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.huixiangedu.cn

[U46] PHP：可空类型
来源：http://rk.9csxet.cn

?string $name = null
来源：http://xv.newstarts.cn

[U47] PHP：联合类型
来源：http://ns.shxzukj.cn

int|string $id
来源：http://dr.asd995.cn

[U48] PHP：纯枚举
来源：http://ok.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pz.wgjwhj.cn

[U49] PHP：只读属性
来源：http://ac.9csxet.cn

public readonly string $name
来源：http://rb.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://aw.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://nt.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ns.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://yt.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://va.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://jz.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://qp.521024.cn

$v = $a ?? $b ?? "default";
来源：http://ve.panjiajie.cn

[U54] PHP：空安全调用
来源：http://bh.lnxyls.cn

$obj?->method()
来源：http://jg.9csxet.cn

[U55] PHP：match 表达式
来源：http://po.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bi.9csxet.cn

[U56] PHP：命名参数
来源：http://hv.huanxung.cn

f(a: 1, b: 2)
来源：http://ri.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://kr.shxzskj.cn

"值: {$a}"
来源：http://rl.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://yi.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vg.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://ho.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zf.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://qe.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://se.lnxyls.cn

[U61] PHP：正则
来源：http://rh.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fc.shxzskj.cn

[U62] PHP：日期对象
来源：http://fr.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nu.colortex.cn

[U63] PHP：文件读写
来源：http://ii.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eo.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://up.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://hg.bookmarksfly.cn

[U65] PHP：会话
来源：http://yg.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uy.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://xx.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wr.9csxet.cn

[U67] PHP：处理文件上传
来源：http://lr.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://we.521024.cn

[U68] PHP：PDO 连接
来源：http://se.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eu.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://rr.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eq.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://cz.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rj.gzmigu.cn

[U71] PHP：抛出异常
来源：http://ox.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://dd.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://cg.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://zp.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://gf.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://eg.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://qz.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://ln.521024.cn

[U75] PHP：依赖注入
来源：http://hq.huixinmuqiang.cn

composer require psr/container
来源：http://cy.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ol.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://en.521024.cn

[U77] PHP：模板渲染
来源：http://vn.9csxet.cn

composer require twig/twig
来源：http://lx.lnxyls.cn

[U78] PHP：单元测试
来源：http://tk.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://ty.huixiangedu.cn

[U79] PHP：静态分析
来源：http://mj.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://tz.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://kq.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nf.szsharing.cn

[U81] JS：初始化项目
来源：http://qi.wgjwhj.cn

npm init -y;  npm i express
来源：http://dc.9csxet.cn

[U82] JS：package.json 脚本
来源：http://nr.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gf.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://dr.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://if.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://tk.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xh.yuexingan06.cn

[U85] JS：可选链
来源：http://mn.huixiangedu.cn

a?.b?.c
来源：http://io.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://zg.jianghongdianzi.cn

a ?? b
来源：http://vg.szxytkj.cn

[U87] JS：解构默认值
来源：http://fd.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://qb.521024.cn

[U88] JS：对象展开合并
来源：http://xq.haigaiapp.cn

{ ...a, ...b }
来源：http://rc.yuexingan06.cn

[U89] JS：数组去重
来源：http://qz.huixinmuqiang.cn

[...new Set(arr)]
来源：http://ys.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://nm.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://kb.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://nu.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yc.nicolike.cn

[U92] JS：深拷贝
来源：http://im.hahajie.cn

structuredClone(obj)
来源：http://jx.szxytkj.cn

[U93] JS：模板字符串
来源：http://ev.shxzukj.cn

`共 ${n} 条`
来源：http://ef.shtwfgs.cn

[U94] JS：箭头函数
来源：http://qj.newstarts.cn

const double = x => x * 2;
来源：http://sq.nicolike.cn

[U95] JS：Promise 包装
来源：http://gd.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://ap.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://de.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yk.chemitech.net.cn

[U97] JS：并发请求
来源：http://lo.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yl.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://uz.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bp.lnxyls.cn

[U99] JS：事件监听
来源：http://le.nszjky.cn

el.addEventListener("click", e => {})
来源：http://sh.newstarts.cn

[U100] JS：DOM 查询
来源：http://jn.huixinmuqiang.cn

document.querySelector(".item")
来源：http://fi.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://uh.hahajie.cn

el.classList.toggle("active")
来源：http://aw.9csxet.cn

[U102] JS：本地存储
来源：http://in.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zt.haigaiapp.cn

[U103] JS：定时器
来源：http://dv.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ah.hnjuh.cn

[U104] JS：防抖
来源：http://sf.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://so.asd995.cn

[U105] JS：节流
来源：http://xs.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://of.szxytkj.cn

[U106] JS：日期格式化
来源：http://dx.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ge.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://vu.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yu.huanxung.cn

[U108] JS：随机整数
来源：http://db.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cl.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://wk.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://hv.panjiajie.cn

[U110] JS：数组分块
来源：http://gu.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ad.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://kv.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://rt.colortex.cn

[U112] JS：字符串补位
来源：http://gw.shxzukj.cn

"7".padStart(3, "0")
来源：http://tf.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://tx.hahajie.cn

s.replaceAll("a", "b")
来源：http://tv.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://vb.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vs.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://dr.gzmigu.cn

crypto.randomUUID()
来源：http://vq.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://uk.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://pl.newstarts.cn

[U117] JS：单元测试
来源：http://wo.colortex.cn

npm i -D vitest;  npx vitest
来源：http://pg.huixiangedu.cn

[U118] JS：开发服务器
来源：http://zh.9csxet.cn

npm i -D vite;  npx vite
来源：http://mn.shxzukj.cn

[U119] JS：生产构建
来源：http://bf.szxytkj.cn

npx vite build
来源：http://ce.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://aa.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://uc.shtwfgs.cn

================================================================================
来源：http://wj.shxzukj.cn

统计汇总
来源：http://nw.colortex.cn

================================================================================
来源：http://sg.shtwfgs.cn

按语言统计（条）：
来源：http://vd.yuntaijiaju.cn

Python ......... 252
来源：http://oy.hahajie.cn

PHP ............ 252
来源：http://bs.chemitech.net.cn

JavaScript ..... 252
来源：http://bu.gzmigu.cn

TypeScript ..... 212
来源：http://hc.nszjky.cn


<!-- 参考信息 -->