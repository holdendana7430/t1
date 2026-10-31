代发 wailian999

[T39] Lua：模式匹配
来源：http://mo.hahajie.cn

string.find(s, "%d+")
来源：http://fh.colortex.cn

[T40] Lua：元表
来源：http://wm.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://bm.asd995.cn

[T41] Perl：Hello World
来源：http://al.newstarts.cn

print "Hello\n";
来源：http://id.hahajie.cn

[T42] Perl：变量类型
来源：http://gc.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fz.521024.cn

[T43] Perl：字符串插值
来源：http://sq.huanxung.cn

"值: $a"
来源：http://sk.shxzskj.cn

[T44] Perl：条件
来源：http://lt.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://bj.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://dq.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://uc.lnxyls.cn

[T46] Perl：哈希操作
来源：http://ca.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kf.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://hs.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ra.bjjhwx.cn

[T48] Perl：正则替换
来源：http://ap.lnxyls.cn

$s =~ s/old/new/g;
来源：http://eq.gzmigu.cn

[T49] Perl：函数
来源：http://nc.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gh.521024.cn

[T50] Perl：逐行读文件
来源：http://mp.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dv.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://yd.nicolike.cn

[T51] Scala：Hello World
来源：http://am.szsharing.cn

println("Hello")
来源：http://kc.lnxyls.cn

[T52] Scala：变量
来源：http://do.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://vz.shxzukj.cn

[T53] Scala：字符串插值
来源：http://qt.shxzskj.cn

s"值: $b"
来源：http://pu.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://fs.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://ya.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ro.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zl.huanxung.cn

[T56] Scala：样例类
来源：http://gd.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://cl.szsharing.cn

[T57] Scala：模式匹配
来源：http://wj.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vc.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://up.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cp.wgjwhj.cn

[T59] Scala：循环
来源：http://hb.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://gt.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://da.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tx.lnxyls.cn

================================================================================
来源：http://eg.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ko.shxzskj.cn

================================================================================
来源：http://go.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://jr.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vq.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://dz.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rh.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://hj.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uc.shxzukj.cn

[U04] Py：变量调试打印
来源：http://tw.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://og.hahajie.cn

[U05] Py：列表去重且保序
来源：http://wd.521024.cn

list(dict.fromkeys(arr))
来源：http://tz.9csxet.cn

[U06] Py：合并两个字典
来源：http://fe.szsharing.cn

{**a, **b}
来源：http://dg.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://dn.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://nx.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://rq.nszjky.cn

[y for x in nested for y in x]
来源：http://sl.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://zy.panjiajie.cn

max(d, key=d.get)
来源：http://np.9csxet.cn

[U10] Py：按值排序字典
来源：http://yk.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uf.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://rs.521024.cn

(x * 2 for x in arr)
来源：http://wx.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://co.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://so.9csxet.cn

[U13] Py：固定长度队列
来源：http://hw.521024.cn

deque(maxlen=10)
来源：http://by.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://qb.chemitech.net.cn

defaultdict(list)
来源：http://ee.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://ht.bookmarksfly.cn

t = time.perf_counter()
来源：http://gy.nszjky.cn

[U16] Py：命令行参数解析
来源：http://xf.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xm.bjjhwx.cn

[U17] Py：初始化日志
来源：http://st.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://zk.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://gj.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://kt.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://yn.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ze.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://mx.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://cf.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://aw.hnjuh.cn

@contextlib.contextmanager
来源：http://tz.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://nc.shtwfgs.cn

list(zip(*m))
来源：http://uz.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://vr.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gl.chemitech.net.cn

[U24] Py：路径操作
来源：http://pp.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vf.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://ej.szxytkj.cn

csv.DictReader(f)
来源：http://rb.nszjky.cn

[U26] Py：并发下载
来源：http://tb.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://as.nicolike.cn

[U27] Py：异步 HTTP
来源：http://vl.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://im.gzmigu.cn

[U28] Py：类型别名
来源：http://fw.521024.cn

UserId = int
来源：http://od.huanxung.cn

[U29] Py：属性校验
来源：http://aq.szsharing.cn

@property 与 @x.setter 配合
来源：http://qh.shtwfgs.cn

[U30] Py：数据类
来源：http://hy.szsharing.cn

@dataclass(slots=True)
来源：http://ql.szxytkj.cn

[U31] Py：单测
来源：http://fz.wgjwhj.cn

python -m pytest -q
来源：http://dx.muxihuayi.cn

[U32] Py：代码格式化
来源：http://mn.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://ul.lnxyls.cn

[U33] Py：打包发布
来源：http://bc.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://iq.wgjwhj.cn

[U34] Py：判断编码
来源：http://he.hahajie.cn

chardet.detect(raw)
来源：http://ji.521024.cn

[U35] Py：发送邮件
来源：http://jg.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ix.panjiajie.cn

[U36] Py：定时任务
来源：http://eo.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://sr.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://ta.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ma.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://rz.huanxung.cn

Path(__file__).resolve().parent
来源：http://il.521024.cn

[U39] Py：判断是否在交互环境
来源：http://pe.colortex.cn

sys.stdout.isatty()
来源：http://uy.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://ia.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://nd.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://wj.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://we.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://id.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wk.nszjky.cn

[U43] PHP：声明命名空间
来源：http://jx.wgjwhj.cn

namespace App\Http;
来源：http://xs.hahajie.cn

[U44] PHP：开启严格类型
来源：http://hb.huanxung.cn

declare(strict_types=1);
来源：http://vo.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://uk.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://uv.muxihuayi.cn

?string $name = null
来源：http://dp.huixiangedu.cn

[U47] PHP：联合类型
来源：http://wh.colortex.cn

int|string $id
来源：http://sl.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://br.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qw.panjiajie.cn

[U49] PHP：只读属性
来源：http://ed.chemitech.net.cn

public readonly string $name
来源：http://sf.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://cm.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://gu.asd995.cn

[U51] PHP：数组解构
来源：http://bw.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://wj.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://fg.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://fs.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://qr.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://bi.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://mw.jctech888.com.cn

$obj?->method()
来源：http://pr.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://vh.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gs.huixiangedu.cn

[U56] PHP：命名参数
来源：http://wy.chemitech.net.cn

f(a: 1, b: 2)
来源：http://eq.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://lr.asd995.cn

"值: {$a}"
来源：http://em.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://ao.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jm.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://kc.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mz.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://et.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ul.hahajie.cn

[U61] PHP：正则
来源：http://nz.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://an.shxzskj.cn

[U62] PHP：日期对象
来源：http://ki.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ju.bjjhwx.cn

[U63] PHP：文件读写
来源：http://hk.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xp.shxzskj.cn

[U64] PHP：目录遍历
来源：http://lc.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ji.colortex.cn

[U65] PHP：会话
来源：http://mn.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://no.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://ic.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jm.newstarts.cn

[U67] PHP：处理文件上传
来源：http://lm.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lz.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://ge.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pd.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://en.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dx.hahajie.cn

[U70] PHP：PDO 事务
来源：http://me.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pf.colortex.cn

[U71] PHP：抛出异常
来源：http://wv.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://qv.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://eq.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://rh.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://wa.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://uv.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://hz.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://hk.szsharing.cn

[U75] PHP：依赖注入
来源：http://fc.shtwfgs.cn

composer require psr/container
来源：http://ot.chemitech.net.cn

[U76] PHP：简单路由
来源：http://qr.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bo.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://yl.521024.cn

composer require twig/twig
来源：http://ht.wgjwhj.cn

[U78] PHP：单元测试
来源：http://bl.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://ir.panjiajie.cn

[U79] PHP：静态分析
来源：http://ek.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://sp.szsharing.cn

[U80] PHP：代码规范修复
来源：http://xw.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ib.lnxyls.cn

[U81] JS：初始化项目
来源：http://cp.wgjwhj.cn

npm init -y;  npm i express
来源：http://yg.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://in.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hw.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://iv.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://az.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://jh.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tw.szxytkj.cn

[U85] JS：可选链
来源：http://ex.nszjky.cn

a?.b?.c
来源：http://nz.bookmarksfly.cn

[U86] JS：空值合并
来源：http://be.nicolike.cn

a ?? b
来源：http://rw.shtwfgs.cn

[U87] JS：解构默认值
来源：http://yr.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://ft.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://bh.gzmigu.cn

{ ...a, ...b }
来源：http://ou.wgjwhj.cn

[U89] JS：数组去重
来源：http://fb.huanxung.cn

[...new Set(arr)]
来源：http://ba.nicolike.cn

[U90] JS：数字数组排序
来源：http://dr.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://mz.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://zi.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vl.bjjhwx.cn

[U92] JS：深拷贝
来源：http://og.gzmigu.cn

structuredClone(obj)
来源：http://uu.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://tz.haigaiapp.cn

`共 ${n} 条`
来源：http://uy.gzmigu.cn

[U94] JS：箭头函数
来源：http://qb.shxzukj.cn

const double = x => x * 2;
来源：http://rl.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://ry.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://cz.nszjky.cn

[U96] JS：async/await 与异常
来源：http://fm.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://db.521024.cn

[U97] JS：并发请求
来源：http://ox.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yi.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://mi.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zz.nszjky.cn

[U99] JS：事件监听
来源：http://tb.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://dt.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://hr.newstarts.cn

document.querySelector(".item")
来源：http://ze.szxytkj.cn

[U101] JS：classList 操作
来源：http://ko.szxytkj.cn

el.classList.toggle("active")
来源：http://no.szsharing.cn

[U102] JS：本地存储
来源：http://zy.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yv.muxihuayi.cn

[U103] JS：定时器
来源：http://yz.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fj.asd995.cn

[U104] JS：防抖
来源：http://fy.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ar.jianghongdianzi.cn

[U105] JS：节流
来源：http://py.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dq.hnjuh.cn

[U106] JS：日期格式化
来源：http://jh.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fx.chemitech.net.cn

[U107] JS：数字千分位
来源：http://nm.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hs.hnjuh.cn

[U108] JS：随机整数
来源：http://ax.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qy.521024.cn

[U109] JS：数组分组
来源：http://cg.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://wa.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://sa.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wp.shxzukj.cn

[U111] JS：对象转 Map
来源：http://iq.nszjky.cn

new Map(Object.entries(obj))
来源：http://is.hahajie.cn

[U112] JS：字符串补位
来源：http://aq.shxzukj.cn

"7".padStart(3, "0")
来源：http://mp.szxytkj.cn

[U113] JS：正则替换全部
来源：http://zm.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://nx.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://lg.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ho.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://es.shxzukj.cn

crypto.randomUUID()
来源：http://aq.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://dy.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://zi.colortex.cn

[U117] JS：单元测试
来源：http://is.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://dd.newstarts.cn

[U118] JS：开发服务器
来源：http://oy.shxzukj.cn

npm i -D vite;  npx vite
来源：http://my.szxytkj.cn

[U119] JS：生产构建
来源：http://pr.szxytkj.cn

npx vite build
来源：http://wy.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://bg.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://vx.shxzskj.cn

================================================================================
来源：http://xh.huixinmuqiang.cn

统计汇总
来源：http://os.521024.cn

================================================================================
来源：http://yq.bookmarksfly.cn

按语言统计（条）：
来源：http://it.asd995.cn

Python ......... 252
来源：http://np.jctech888.com.cn

PHP ............ 252
来源：http://vh.9csxet.cn

JavaScript ..... 252
来源：http://fr.szsharing.cn

TypeScript ..... 212
来源：http://dr.panjiajie.cn

Java ........... 212
来源：http://bw.shxzukj.cn

Go ............. 212
来源：http://cy.panjiajie.cn

Ruby ........... 212
来源：http://jp.panjiajie.cn

C# ............. 212
来源：http://hx.newstarts.cn


<!-- 参考信息 -->