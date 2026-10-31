代发 wailian999

[T39] Lua：模式匹配
来源：http://wg.szsharing.cn

string.find(s, "%d+")
来源：http://pp.hnjuh.cn

[T40] Lua：元表
来源：http://eg.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://nd.shtwfgs.cn

[T41] Perl：Hello World
来源：http://ry.shxzukj.cn

print "Hello\n";
来源：http://up.panjiajie.cn

[T42] Perl：变量类型
来源：http://ah.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uh.asd995.cn

[T43] Perl：字符串插值
来源：http://iu.gzmigu.cn

"值: $a"
来源：http://lj.lnxyls.cn

[T44] Perl：条件
来源：http://ks.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://of.9csxet.cn

[T45] Perl：数组遍历
来源：http://jf.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://lq.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://rt.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zl.newstarts.cn

[T47] Perl：正则捕获
来源：http://yj.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gu.nicolike.cn

[T48] Perl：正则替换
来源：http://un.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://dk.bookmarksfly.cn

[T49] Perl：函数
来源：http://ex.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sx.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://xm.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xl.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ph.panjiajie.cn

[T51] Scala：Hello World
来源：http://xn.huixiangedu.cn

println("Hello")
来源：http://ws.nszjky.cn

[T52] Scala：变量
来源：http://yb.nicolike.cn

val a = 1;  var b = 2
来源：http://hb.hnjuh.cn

[T53] Scala：字符串插值
来源：http://dv.gzmigu.cn

s"值: $b"
来源：http://ja.lnxyls.cn

[T54] Scala：集合映射
来源：http://ot.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://ub.9csxet.cn

[T55] Scala：集合过滤
来源：http://dz.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xt.hahajie.cn

[T56] Scala：样例类
来源：http://pt.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://hs.shxzskj.cn

[T57] Scala：模式匹配
来源：http://mu.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://px.bjjhwx.cn

[T58] Scala：函数定义
来源：http://ny.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lj.hnjuh.cn

[T59] Scala：循环
来源：http://zm.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://ra.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://lf.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bx.nicolike.cn

================================================================================
来源：http://te.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ln.yuntaijiaju.cn

================================================================================
来源：http://lo.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://sz.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://es.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://hp.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ch.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://ox.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lj.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://in.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ox.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://yt.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://jf.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ny.huixinmuqiang.cn

{**a, **b}
来源：http://ca.panjiajie.cn

[U07] Py：反转字典键值
来源：http://rd.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://hb.nszjky.cn

[U08] Py：展平二维列表
来源：http://ji.hahajie.cn

[y for x in nested for y in x]
来源：http://eb.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://lp.jctech888.com.cn

max(d, key=d.get)
来源：http://vv.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://oe.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bb.lnxyls.cn

[U11] Py：生成器表达式
来源：http://cu.nicolike.cn

(x * 2 for x in arr)
来源：http://nx.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qc.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://qp.9csxet.cn

[U13] Py：固定长度队列
来源：http://no.shxzukj.cn

deque(maxlen=10)
来源：http://ac.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ku.hahajie.cn

defaultdict(list)
来源：http://oa.9csxet.cn

[U15] Py：高精度计时
来源：http://ec.jctech888.com.cn

t = time.perf_counter()
来源：http://vx.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://ug.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hl.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://hr.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://wc.lnxyls.cn

[U18] Py：预编译正则
来源：http://yb.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://jo.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://uq.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tm.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://fe.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://qi.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://xm.colortex.cn

@contextlib.contextmanager
来源：http://no.shxzukj.cn

[U22] Py：矩阵转置
来源：http://de.chemitech.net.cn

list(zip(*m))
来源：http://oe.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://qw.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://th.521024.cn

[U24] Py：路径操作
来源：http://fc.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yf.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ts.asd995.cn

csv.DictReader(f)
来源：http://qg.muxihuayi.cn

[U26] Py：并发下载
来源：http://xv.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oz.nicolike.cn

[U27] Py：异步 HTTP
来源：http://kc.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://zv.shtwfgs.cn

[U28] Py：类型别名
来源：http://ab.yuntaijiaju.cn

UserId = int
来源：http://xx.hahajie.cn

[U29] Py：属性校验
来源：http://bj.nicolike.cn

@property 与 @x.setter 配合
来源：http://fk.yuexingan06.cn

[U30] Py：数据类
来源：http://lt.gzmigu.cn

@dataclass(slots=True)
来源：http://um.nicolike.cn

[U31] Py：单测
来源：http://bo.shxzukj.cn

python -m pytest -q
来源：http://mu.szxytkj.cn

[U32] Py：代码格式化
来源：http://hm.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://es.jctech888.com.cn

[U33] Py：打包发布
来源：http://bv.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://pc.nicolike.cn

[U34] Py：判断编码
来源：http://vo.jctech888.com.cn

chardet.detect(raw)
来源：http://tk.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ao.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kk.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://oj.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://fe.asd995.cn

[U37] Py：读写 Excel
来源：http://ce.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vf.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://yb.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://hn.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://hb.panjiajie.cn

sys.stdout.isatty()
来源：http://nx.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://wd.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://we.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://zc.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pj.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://mx.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ko.asd995.cn

[U43] PHP：声明命名空间
来源：http://tn.bookmarksfly.cn

namespace App\Http;
来源：http://fx.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ys.gzmigu.cn

declare(strict_types=1);
来源：http://pf.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://vr.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bv.yuexingan06.cn

[U46] PHP：可空类型
来源：http://pd.haigaiapp.cn

?string $name = null
来源：http://gk.huanxung.cn

[U47] PHP：联合类型
来源：http://gt.huixiangedu.cn

int|string $id
来源：http://st.newstarts.cn

[U48] PHP：纯枚举
来源：http://fk.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bs.panjiajie.cn

[U49] PHP：只读属性
来源：http://su.jctech888.com.cn

public readonly string $name
来源：http://zm.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://zd.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://fu.jctech888.com.cn

[U51] PHP：数组解构
来源：http://bz.shtwfgs.cn

[$a, $b] = $arr;
来源：http://yc.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://uz.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://tz.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://bg.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://vu.hahajie.cn

[U54] PHP：空安全调用
来源：http://fe.shxzukj.cn

$obj?->method()
来源：http://zl.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://to.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gt.shxzukj.cn

[U56] PHP：命名参数
来源：http://yd.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://jj.nicolike.cn

[U57] PHP：字符串插值
来源：http://io.shxzukj.cn

"值: {$a}"
来源：http://up.shxzskj.cn

[U58] PHP：数组三件套
来源：http://di.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zu.newstarts.cn

[U59] PHP：自定义排序
来源：http://hd.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vl.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://xh.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zp.huixinmuqiang.cn

[U61] PHP：正则
来源：http://hd.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rf.colortex.cn

[U62] PHP：日期对象
来源：http://fw.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cj.huixiangedu.cn

[U63] PHP：文件读写
来源：http://ud.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gk.lnxyls.cn

[U64] PHP：目录遍历
来源：http://qv.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://dz.muxihuayi.cn

[U65] PHP：会话
来源：http://re.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ul.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://xe.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pm.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://ca.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://va.szsharing.cn

[U68] PHP：PDO 连接
来源：http://bb.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pv.asd995.cn

[U69] PHP：PDO 预处理
来源：http://lt.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yu.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://oy.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pt.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://az.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://ye.huanxung.cn

[U72] PHP：写错误日志
来源：http://gw.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://mj.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://gh.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://mr.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://fc.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://vj.newstarts.cn

[U75] PHP：依赖注入
来源：http://ia.shtwfgs.cn

composer require psr/container
来源：http://jo.shxzskj.cn

[U76] PHP：简单路由
来源：http://pp.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xy.gzmigu.cn

[U77] PHP：模板渲染
来源：http://hb.huixiangedu.cn

composer require twig/twig
来源：http://sb.9csxet.cn

[U78] PHP：单元测试
来源：http://ez.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://qs.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://ck.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://gu.newstarts.cn

[U80] PHP：代码规范修复
来源：http://hf.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nt.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://vt.521024.cn

npm init -y;  npm i express
来源：http://ul.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://ei.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yu.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://nq.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qj.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://sa.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mv.nszjky.cn

[U85] JS：可选链
来源：http://ln.gzmigu.cn

a?.b?.c
来源：http://ju.haigaiapp.cn

[U86] JS：空值合并
来源：http://sw.huixiangedu.cn

a ?? b
来源：http://ke.shxzskj.cn

[U87] JS：解构默认值
来源：http://nv.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://tg.hnjuh.cn

[U88] JS：对象展开合并
来源：http://zw.9csxet.cn

{ ...a, ...b }
来源：http://sq.muxihuayi.cn

[U89] JS：数组去重
来源：http://vw.yuntaijiaju.cn

[...new Set(arr)]
来源：http://uy.shxzukj.cn

[U90] JS：数字数组排序
来源：http://hf.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://fh.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://yh.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://st.huixiangedu.cn

[U92] JS：深拷贝
来源：http://gk.521024.cn

structuredClone(obj)
来源：http://eb.521024.cn

[U93] JS：模板字符串
来源：http://tq.panjiajie.cn

`共 ${n} 条`
来源：http://js.shxzskj.cn

[U94] JS：箭头函数
来源：http://sf.huixinmuqiang.cn

const double = x => x * 2;
来源：http://bl.szsharing.cn

[U95] JS：Promise 包装
来源：http://ae.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://we.szsharing.cn

[U96] JS：async/await 与异常
来源：http://rk.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qo.hahajie.cn

[U97] JS：并发请求
来源：http://lm.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pl.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://lw.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cr.shxzukj.cn

[U99] JS：事件监听
来源：http://ex.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://vt.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://px.nicolike.cn

document.querySelector(".item")
来源：http://at.huanxung.cn

[U101] JS：classList 操作
来源：http://ro.jctech888.com.cn

el.classList.toggle("active")
来源：http://jm.shxzukj.cn

[U102] JS：本地存储
来源：http://dv.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lq.haigaiapp.cn

[U103] JS：定时器
来源：http://ov.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iv.jianghongdianzi.cn

[U104] JS：防抖
来源：http://fw.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xf.jianghongdianzi.cn

[U105] JS：节流
来源：http://yx.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hi.panjiajie.cn

[U106] JS：日期格式化
来源：http://vg.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://un.huixiangedu.cn

[U107] JS：数字千分位
来源：http://cn.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lk.huanxung.cn

[U108] JS：随机整数
来源：http://yx.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zx.shxzukj.cn

[U109] JS：数组分组
来源：http://xh.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://rz.chemitech.net.cn

[U110] JS：数组分块
来源：http://ju.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xw.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://gj.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://yz.shxzskj.cn

[U112] JS：字符串补位
来源：http://uf.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://po.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://rz.newstarts.cn

s.replaceAll("a", "b")
来源：http://ao.hahajie.cn

[U114] JS：JSON 深比较
来源：http://tx.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yo.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://ws.shxzukj.cn

crypto.randomUUID()
来源：http://il.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://qy.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://ko.lnxyls.cn

[U117] JS：单元测试
来源：http://xp.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://hl.yuexingan06.cn

[U118] JS：开发服务器
来源：http://yc.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://lf.colortex.cn

[U119] JS：生产构建
来源：http://hu.huixiangedu.cn

npx vite build
来源：http://ek.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://di.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://mt.huanxung.cn

================================================================================
来源：http://ht.lnxyls.cn

统计汇总
来源：http://vo.szxytkj.cn

================================================================================
来源：http://ht.gzmigu.cn

按语言统计（条）：
来源：http://ca.9csxet.cn

Python ......... 252
来源：http://we.colortex.cn

PHP ............ 252
来源：http://wp.huanxung.cn

JavaScript ..... 252
来源：http://jq.chemitech.net.cn

TypeScript ..... 212
来源：http://ja.gzmigu.cn

Java ........... 212
来源：http://sb.szsharing.cn

Go ............. 212
来源：http://pp.huixinmuqiang.cn

Ruby ........... 212
来源：http://zs.huanxung.cn

C# ............. 212
来源：http://az.huanxung.cn


<!-- 参考信息 -->