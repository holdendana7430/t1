代发 wailian999

[T31] Lua：Hello World
来源：http://tb.hnjuh.cn

print("Hello")
来源：http://ac.shxzukj.cn

[T32] Lua：局部变量
来源：http://vi.521024.cn

local a = 1
来源：http://cg.asd995.cn

[T33] Lua：表（数组）
来源：http://ws.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bc.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://jp.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nl.chemitech.net.cn

[T35] Lua：字典表
来源：http://el.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://jf.hnjuh.cn

[T36] Lua：函数
来源：http://eg.muxihuayi.cn

function add(a, b) return a + b end
来源：http://mz.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://sh.bookmarksfly.cn

"a" .. "b"
来源：http://ms.haigaiapp.cn

[T38] Lua：条件
来源：http://sa.muxihuayi.cn

if x > 0 then print("正") end
来源：http://zl.asd995.cn

[T39] Lua：模式匹配
来源：http://aq.newstarts.cn

string.find(s, "%d+")
来源：http://ri.asd995.cn

[T40] Lua：元表
来源：http://ko.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://zu.hnjuh.cn

[T41] Perl：Hello World
来源：http://oj.bookmarksfly.cn

print "Hello\n";
来源：http://zr.huanxung.cn

[T42] Perl：变量类型
来源：http://eg.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ot.9csxet.cn

[T43] Perl：字符串插值
来源：http://zu.bookmarksfly.cn

"值: $a"
来源：http://fq.nszjky.cn

[T44] Perl：条件
来源：http://db.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://sj.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://vg.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://uo.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://xe.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kt.lnxyls.cn

[T47] Perl：正则捕获
来源：http://mp.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jh.colortex.cn

[T48] Perl：正则替换
来源：http://ye.colortex.cn

$s =~ s/old/new/g;
来源：http://xi.yuntaijiaju.cn

[T49] Perl：函数
来源：http://mj.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mf.colortex.cn

[T50] Perl：逐行读文件
来源：http://pi.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jd.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://tv.haigaiapp.cn

[T51] Scala：Hello World
来源：http://rb.muxihuayi.cn

println("Hello")
来源：http://mt.gzmigu.cn

[T52] Scala：变量
来源：http://sf.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://ve.nszjky.cn

[T53] Scala：字符串插值
来源：http://mw.shxzukj.cn

s"值: $b"
来源：http://pt.shxzukj.cn

[T54] Scala：集合映射
来源：http://mg.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://nh.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://js.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yw.shxzukj.cn

[T56] Scala：样例类
来源：http://fs.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://tc.huanxung.cn

[T57] Scala：模式匹配
来源：http://ir.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lt.chemitech.net.cn

[T58] Scala：函数定义
来源：http://rq.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yc.szxytkj.cn

[T59] Scala：循环
来源：http://sv.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://pf.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://sj.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tl.newstarts.cn

================================================================================
来源：http://ku.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ni.bookmarksfly.cn

================================================================================
来源：http://qp.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://kh.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ul.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://eq.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ci.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ye.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pb.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://ia.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nw.newstarts.cn

[U05] Py：列表去重且保序
来源：http://ap.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://oa.shxzskj.cn

[U06] Py：合并两个字典
来源：http://ay.asd995.cn

{**a, **b}
来源：http://pw.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://sx.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://ki.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://ui.shxzskj.cn

[y for x in nested for y in x]
来源：http://yj.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ii.yuntaijiaju.cn

max(d, key=d.get)
来源：http://jh.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://nn.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mx.hnjuh.cn

[U11] Py：生成器表达式
来源：http://kt.hahajie.cn

(x * 2 for x in arr)
来源：http://wb.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kb.521024.cn

Counter(arr).most_common(3)
来源：http://ll.shxzskj.cn

[U13] Py：固定长度队列
来源：http://lo.lnxyls.cn

deque(maxlen=10)
来源：http://do.colortex.cn

[U14] Py：分组收集到列表
来源：http://mx.panjiajie.cn

defaultdict(list)
来源：http://ap.shxzukj.cn

[U15] Py：高精度计时
来源：http://ic.haigaiapp.cn

t = time.perf_counter()
来源：http://cp.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://jj.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eb.panjiajie.cn

[U17] Py：初始化日志
来源：http://nq.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://mt.shtwfgs.cn

[U18] Py：预编译正则
来源：http://uo.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://pj.colortex.cn

[U19] Py：正则替换带回调
来源：http://qa.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hl.colortex.cn

[U20] Py：缓存函数结果
来源：http://jy.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://bg.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://hf.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://bx.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://bk.chemitech.net.cn

list(zip(*m))
来源：http://vu.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://wl.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ci.nszjky.cn

[U24] Py：路径操作
来源：http://ay.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fr.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://tc.muxihuayi.cn

csv.DictReader(f)
来源：http://gk.shxzukj.cn

[U26] Py：并发下载
来源：http://zi.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rg.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://ko.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://sp.newstarts.cn

[U28] Py：类型别名
来源：http://on.shxzskj.cn

UserId = int
来源：http://qu.gzmigu.cn

[U29] Py：属性校验
来源：http://zr.lnxyls.cn

@property 与 @x.setter 配合
来源：http://jh.shxzukj.cn

[U30] Py：数据类
来源：http://gg.shxzskj.cn

@dataclass(slots=True)
来源：http://ij.jctech888.com.cn

[U31] Py：单测
来源：http://vn.hahajie.cn

python -m pytest -q
来源：http://tj.nszjky.cn

[U32] Py：代码格式化
来源：http://cg.szsharing.cn

ruff format . && ruff check --fix .
来源：http://jg.bookmarksfly.cn

[U33] Py：打包发布
来源：http://ae.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://jy.hnjuh.cn

[U34] Py：判断编码
来源：http://wa.yuntaijiaju.cn

chardet.detect(raw)
来源：http://rz.asd995.cn

[U35] Py：发送邮件
来源：http://nf.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ed.hnjuh.cn

[U36] Py：定时任务
来源：http://az.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://fp.huanxung.cn

[U37] Py：读写 Excel
来源：http://qm.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vh.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://qk.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://jf.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://hl.huixiangedu.cn

sys.stdout.isatty()
来源：http://fe.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://vf.panjiajie.cn

print("err", file=sys.stderr)
来源：http://rp.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ol.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xb.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://xj.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nm.asd995.cn

[U43] PHP：声明命名空间
来源：http://rz.colortex.cn

namespace App\Http;
来源：http://pk.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://rp.colortex.cn

declare(strict_types=1);
来源：http://mt.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://ds.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lc.9csxet.cn

[U46] PHP：可空类型
来源：http://hz.yuexingan06.cn

?string $name = null
来源：http://tf.bjjhwx.cn

[U47] PHP：联合类型
来源：http://bq.shtwfgs.cn

int|string $id
来源：http://hk.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://nj.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qu.szxytkj.cn

[U49] PHP：只读属性
来源：http://pz.asd995.cn

public readonly string $name
来源：http://hp.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://sk.szxytkj.cn

public function __construct(private int $id) {}
来源：http://jx.chemitech.net.cn

[U51] PHP：数组解构
来源：http://fx.nszjky.cn

[$a, $b] = $arr;
来源：http://bk.nicolike.cn

[U52] PHP：箭头函数
来源：http://tv.colortex.cn

$double = fn($x) => $x * 2;
来源：http://fj.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://rd.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://np.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://yz.huixiangedu.cn

$obj?->method()
来源：http://km.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://wo.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kd.hahajie.cn

[U56] PHP：命名参数
来源：http://jn.asd995.cn

f(a: 1, b: 2)
来源：http://oy.asd995.cn

[U57] PHP：字符串插值
来源：http://mp.shxzskj.cn

"值: {$a}"
来源：http://am.szxytkj.cn

[U58] PHP：数组三件套
来源：http://pd.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zo.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://cn.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jf.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://lg.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xs.jianghongdianzi.cn

[U61] PHP：正则
来源：http://kp.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qx.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://vt.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nt.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://yf.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ju.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://xd.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://oa.muxihuayi.cn

[U65] PHP：会话
来源：http://gp.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cd.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://tv.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ij.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://db.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://co.newstarts.cn

[U68] PHP：PDO 连接
来源：http://lz.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lc.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://th.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://va.szsharing.cn

[U70] PHP：PDO 事务
来源：http://xe.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sh.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://dd.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://xf.asd995.cn

[U72] PHP：写错误日志
来源：http://by.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://mj.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://dm.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://eb.asd995.cn

[U74] PHP：读取环境变量
来源：http://nt.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://vy.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://wc.gzmigu.cn

composer require psr/container
来源：http://yq.huixiangedu.cn

[U76] PHP：简单路由
来源：http://dn.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dd.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://gw.colortex.cn

composer require twig/twig
来源：http://ic.shtwfgs.cn

[U78] PHP：单元测试
来源：http://zh.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://qo.chemitech.net.cn

[U79] PHP：静态分析
来源：http://rv.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://kn.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://xw.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ve.szxytkj.cn

[U81] JS：初始化项目
来源：http://gs.shtwfgs.cn

npm init -y;  npm i express
来源：http://lp.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://jp.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://de.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://ow.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ej.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://op.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vu.lnxyls.cn

[U85] JS：可选链
来源：http://zd.hnjuh.cn

a?.b?.c
来源：http://ha.lnxyls.cn

[U86] JS：空值合并
来源：http://qx.yuntaijiaju.cn

a ?? b
来源：http://wq.newstarts.cn

[U87] JS：解构默认值
来源：http://op.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://aj.colortex.cn

[U88] JS：对象展开合并
来源：http://hn.huixinmuqiang.cn

{ ...a, ...b }
来源：http://ev.szsharing.cn

[U89] JS：数组去重
来源：http://iq.bookmarksfly.cn

[...new Set(arr)]
来源：http://ti.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://di.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://mm.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://td.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hp.colortex.cn

[U92] JS：深拷贝
来源：http://fg.yuntaijiaju.cn

structuredClone(obj)
来源：http://xd.521024.cn

[U93] JS：模板字符串
来源：http://si.panjiajie.cn

`共 ${n} 条`
来源：http://mt.shxzskj.cn

[U94] JS：箭头函数
来源：http://sg.shxzukj.cn

const double = x => x * 2;
来源：http://tl.panjiajie.cn

[U95] JS：Promise 包装
来源：http://or.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://ke.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://pp.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://me.muxihuayi.cn

[U97] JS：并发请求
来源：http://bf.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ka.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://hn.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tr.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://na.szsharing.cn

el.addEventListener("click", e => {})
来源：http://bg.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://wm.newstarts.cn

document.querySelector(".item")
来源：http://nt.gzmigu.cn

[U101] JS：classList 操作
来源：http://mq.nicolike.cn

el.classList.toggle("active")
来源：http://md.nszjky.cn

[U102] JS：本地存储
来源：http://ep.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ty.gzmigu.cn

[U103] JS：定时器
来源：http://xt.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nn.jctech888.com.cn

[U104] JS：防抖
来源：http://uj.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.colortex.cn

[U105] JS：节流
来源：http://fk.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://du.shtwfgs.cn

[U106] JS：日期格式化
来源：http://tr.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://un.hahajie.cn

[U107] JS：数字千分位
来源：http://wp.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://to.yuexingan06.cn

[U108] JS：随机整数
来源：http://os.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hj.szxytkj.cn

[U109] JS：数组分组
来源：http://nc.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://yy.lnxyls.cn

[U110] JS：数组分块
来源：http://yp.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uk.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://cm.9csxet.cn

new Map(Object.entries(obj))
来源：http://ww.jctech888.com.cn

[U112] JS：字符串补位
来源：http://fj.nicolike.cn

"7".padStart(3, "0")
来源：http://cu.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://px.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://zr.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://vl.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hv.shxzskj.cn

[U115] JS：生成 UUID
来源：http://kf.colortex.cn

crypto.randomUUID()
来源：http://aq.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://gi.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://ut.9csxet.cn

[U117] JS：单元测试
来源：http://iu.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://ps.huanxung.cn

[U118] JS：开发服务器
来源：http://jf.521024.cn

npm i -D vite;  npx vite
来源：http://sz.asd995.cn


<!-- 参考信息 -->