代发 wailian999

[T35] Lua：字典表
来源：http://qp.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ed.huixiangedu.cn

[T36] Lua：函数
来源：http://yn.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://rg.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ko.colortex.cn

"a" .. "b"
来源：http://xl.haigaiapp.cn

[T38] Lua：条件
来源：http://jy.huixiangedu.cn

if x > 0 then print("正") end
来源：http://wh.9csxet.cn

[T39] Lua：模式匹配
来源：http://cs.bookmarksfly.cn

string.find(s, "%d+")
来源：http://tr.bookmarksfly.cn

[T40] Lua：元表
来源：http://fw.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://pk.nicolike.cn

[T41] Perl：Hello World
来源：http://ve.asd995.cn

print "Hello\n";
来源：http://zf.newstarts.cn

[T42] Perl：变量类型
来源：http://cp.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fu.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://wz.colortex.cn

"值: $a"
来源：http://tx.huanxung.cn

[T44] Perl：条件
来源：http://jx.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://rq.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://pl.asd995.cn

for my $x (@arr) { print $x; }
来源：http://jz.9csxet.cn

[T46] Perl：哈希操作
来源：http://ka.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gr.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://wl.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ms.shxzskj.cn

[T48] Perl：正则替换
来源：http://tv.hahajie.cn

$s =~ s/old/new/g;
来源：http://sl.bookmarksfly.cn

[T49] Perl：函数
来源：http://al.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nr.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ja.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gl.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://aw.nicolike.cn

[T51] Scala：Hello World
来源：http://mz.lnxyls.cn

println("Hello")
来源：http://fh.colortex.cn

[T52] Scala：变量
来源：http://fw.haigaiapp.cn

val a = 1;  var b = 2
来源：http://yu.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://rb.colortex.cn

s"值: $b"
来源：http://dl.szxytkj.cn

[T54] Scala：集合映射
来源：http://eo.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://tt.szsharing.cn

[T55] Scala：集合过滤
来源：http://py.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ms.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://be.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ro.huanxung.cn

[T57] Scala：模式匹配
来源：http://ob.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cc.panjiajie.cn

[T58] Scala：函数定义
来源：http://rs.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vl.shxzukj.cn

[T59] Scala：循环
来源：http://fj.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://iz.haigaiapp.cn

[T60] Scala：折叠
来源：http://zi.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ka.9csxet.cn

================================================================================
来源：http://oe.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jk.gzmigu.cn

================================================================================
来源：http://si.521024.cn

[U01] Py：创建虚拟环境
来源：http://gc.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ao.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ek.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gz.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://md.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sa.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://id.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://no.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://kx.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://iu.521024.cn

[U06] Py：合并两个字典
来源：http://ov.bookmarksfly.cn

{**a, **b}
来源：http://xi.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://vb.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://wf.szxytkj.cn

[U08] Py：展平二维列表
来源：http://yo.panjiajie.cn

[y for x in nested for y in x]
来源：http://jc.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://nu.huixinmuqiang.cn

max(d, key=d.get)
来源：http://zm.shxzskj.cn

[U10] Py：按值排序字典
来源：http://tw.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ep.colortex.cn

[U11] Py：生成器表达式
来源：http://fp.nszjky.cn

(x * 2 for x in arr)
来源：http://hl.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xa.gzmigu.cn

Counter(arr).most_common(3)
来源：http://hc.hnjuh.cn

[U13] Py：固定长度队列
来源：http://af.bookmarksfly.cn

deque(maxlen=10)
来源：http://ay.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://ug.wgjwhj.cn

defaultdict(list)
来源：http://an.muxihuayi.cn

[U15] Py：高精度计时
来源：http://sy.hahajie.cn

t = time.perf_counter()
来源：http://xz.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://tz.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xd.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://yn.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://su.nicolike.cn

[U18] Py：预编译正则
来源：http://fi.asd995.cn

pat = re.compile(r"\d+")
来源：http://sb.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://af.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qs.huanxung.cn

[U20] Py：缓存函数结果
来源：http://iv.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://sw.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://rj.colortex.cn

@contextlib.contextmanager
来源：http://vu.hahajie.cn

[U22] Py：矩阵转置
来源：http://og.gzmigu.cn

list(zip(*m))
来源：http://tx.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://kg.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pz.panjiajie.cn

[U24] Py：路径操作
来源：http://so.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ur.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://na.newstarts.cn

csv.DictReader(f)
来源：http://dl.huixiangedu.cn

[U26] Py：并发下载
来源：http://nk.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yq.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://rn.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://ei.shxzukj.cn

[U28] Py：类型别名
来源：http://ii.haigaiapp.cn

UserId = int
来源：http://ab.szsharing.cn

[U29] Py：属性校验
来源：http://wt.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://fp.muxihuayi.cn

[U30] Py：数据类
来源：http://yc.colortex.cn

@dataclass(slots=True)
来源：http://bi.nicolike.cn

[U31] Py：单测
来源：http://na.colortex.cn

python -m pytest -q
来源：http://ar.asd995.cn

[U32] Py：代码格式化
来源：http://ky.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://xm.muxihuayi.cn

[U33] Py：打包发布
来源：http://dh.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ia.nicolike.cn

[U34] Py：判断编码
来源：http://vo.szxytkj.cn

chardet.detect(raw)
来源：http://kg.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://ch.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fo.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://oc.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://xs.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://bq.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mf.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://ul.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://ft.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://gd.nicolike.cn

sys.stdout.isatty()
来源：http://to.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://uk.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://lg.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://gw.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ip.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://ci.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://za.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://fc.muxihuayi.cn

namespace App\Http;
来源：http://ko.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://tu.muxihuayi.cn

declare(strict_types=1);
来源：http://fo.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://kb.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ob.hahajie.cn

[U46] PHP：可空类型
来源：http://zo.haigaiapp.cn

?string $name = null
来源：http://oh.bjjhwx.cn

[U47] PHP：联合类型
来源：http://aa.hahajie.cn

int|string $id
来源：http://ro.hnjuh.cn

[U48] PHP：纯枚举
来源：http://xn.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lr.muxihuayi.cn

[U49] PHP：只读属性
来源：http://oh.9csxet.cn

public readonly string $name
来源：http://wr.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://ys.nicolike.cn

public function __construct(private int $id) {}
来源：http://au.jctech888.com.cn

[U51] PHP：数组解构
来源：http://fg.wgjwhj.cn

[$a, $b] = $arr;
来源：http://wc.nicolike.cn

[U52] PHP：箭头函数
来源：http://mc.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://we.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://jz.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://ck.panjiajie.cn

[U54] PHP：空安全调用
来源：http://ec.lnxyls.cn

$obj?->method()
来源：http://ob.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://oh.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gd.yuexingan06.cn

[U56] PHP：命名参数
来源：http://cg.lnxyls.cn

f(a: 1, b: 2)
来源：http://jo.nicolike.cn

[U57] PHP：字符串插值
来源：http://oj.panjiajie.cn

"值: {$a}"
来源：http://wf.panjiajie.cn

[U58] PHP：数组三件套
来源：http://ih.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nw.asd995.cn

[U59] PHP：自定义排序
来源：http://zk.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pz.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://qs.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vp.colortex.cn

[U61] PHP：正则
来源：http://wx.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zb.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://fe.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cj.nszjky.cn

[U63] PHP：文件读写
来源：http://wk.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ht.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://pw.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://jc.chemitech.net.cn

[U65] PHP：会话
来源：http://xs.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cl.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://iv.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://am.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://gy.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fc.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://gv.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fk.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://xb.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vl.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://ii.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cc.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ei.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ay.9csxet.cn

[U72] PHP：写错误日志
来源：http://be.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://ld.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://mz.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://ge.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://dk.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://wd.huanxung.cn

[U75] PHP：依赖注入
来源：http://bw.colortex.cn

composer require psr/container
来源：http://yw.9csxet.cn

[U76] PHP：简单路由
来源：http://js.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zz.newstarts.cn

[U77] PHP：模板渲染
来源：http://jn.hahajie.cn

composer require twig/twig
来源：http://ym.szxytkj.cn

[U78] PHP：单元测试
来源：http://ns.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://bb.shxzskj.cn

[U79] PHP：静态分析
来源：http://wk.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://jh.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://nj.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uh.bjjhwx.cn

[U81] JS：初始化项目
来源：http://ta.nszjky.cn

npm init -y;  npm i express
来源：http://um.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://xv.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ir.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://qg.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dq.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://qw.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rm.asd995.cn

[U85] JS：可选链
来源：http://rv.lnxyls.cn

a?.b?.c
来源：http://qd.bjjhwx.cn

[U86] JS：空值合并
来源：http://xd.nszjky.cn

a ?? b
来源：http://pr.shtwfgs.cn

[U87] JS：解构默认值
来源：http://fn.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://mh.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://ad.huixiangedu.cn

{ ...a, ...b }
来源：http://az.nszjky.cn

[U89] JS：数组去重
来源：http://ep.shtwfgs.cn

[...new Set(arr)]
来源：http://iz.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://hh.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://dj.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://rq.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ep.shtwfgs.cn

[U92] JS：深拷贝
来源：http://fk.nszjky.cn

structuredClone(obj)
来源：http://gb.9csxet.cn

[U93] JS：模板字符串
来源：http://ef.chemitech.net.cn

`共 ${n} 条`
来源：http://ze.9csxet.cn

[U94] JS：箭头函数
来源：http://uy.jctech888.com.cn

const double = x => x * 2;
来源：http://uc.newstarts.cn

[U95] JS：Promise 包装
来源：http://mn.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://fc.9csxet.cn

[U96] JS：async/await 与异常
来源：http://ru.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sr.yuexingan06.cn

[U97] JS：并发请求
来源：http://nv.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ru.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://vf.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qg.newstarts.cn

[U99] JS：事件监听
来源：http://tz.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://zc.nszjky.cn

[U100] JS：DOM 查询
来源：http://wv.newstarts.cn

document.querySelector(".item")
来源：http://de.bjjhwx.cn

[U101] JS：classList 操作
来源：http://gt.wgjwhj.cn

el.classList.toggle("active")
来源：http://mf.521024.cn

[U102] JS：本地存储
来源：http://fd.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xd.yuntaijiaju.cn

[U103] JS：定时器
来源：http://my.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zo.colortex.cn

[U104] JS：防抖
来源：http://ds.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.hnjuh.cn

[U105] JS：节流
来源：http://py.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://al.huanxung.cn

[U106] JS：日期格式化
来源：http://ov.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yw.panjiajie.cn

[U107] JS：数字千分位
来源：http://rr.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://au.hahajie.cn

[U108] JS：随机整数
来源：http://zu.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cd.newstarts.cn

[U109] JS：数组分组
来源：http://ou.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://nu.haigaiapp.cn

[U110] JS：数组分块
来源：http://ah.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tb.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://ra.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ds.shxzskj.cn

[U112] JS：字符串补位
来源：http://vj.jctech888.com.cn

"7".padStart(3, "0")
来源：http://jg.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://qh.521024.cn

s.replaceAll("a", "b")
来源：http://eb.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://io.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gs.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://cn.asd995.cn

crypto.randomUUID()
来源：http://gi.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://pn.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://py.nszjky.cn

[U117] JS：单元测试
来源：http://yd.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://jg.szxytkj.cn

[U118] JS：开发服务器
来源：http://rz.panjiajie.cn

npm i -D vite;  npx vite
来源：http://df.bjjhwx.cn

[U119] JS：生产构建
来源：http://la.jianghongdianzi.cn

npx vite build
来源：http://om.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://nj.asd995.cn

import.meta.env.VITE_API_URL
来源：http://og.9csxet.cn

================================================================================
来源：http://rv.jctech888.com.cn

统计汇总
来源：http://zm.haigaiapp.cn

================================================================================
来源：http://vu.gzmigu.cn

按语言统计（条）：
来源：http://fi.huixinmuqiang.cn


<!-- 参考信息 -->