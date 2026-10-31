代发 wailian999

[T33] Lua：表（数组）
来源：http://mb.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ws.lnxyls.cn

[T34] Lua：遍历表
来源：http://mu.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qs.jctech888.com.cn

[T35] Lua：字典表
来源：http://ng.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://xc.jctech888.com.cn

[T36] Lua：函数
来源：http://ur.newstarts.cn

function add(a, b) return a + b end
来源：http://iq.nszjky.cn

[T37] Lua：字符串拼接
来源：http://jm.lnxyls.cn

"a" .. "b"
来源：http://qv.hahajie.cn

[T38] Lua：条件
来源：http://es.shtwfgs.cn

if x > 0 then print("正") end
来源：http://wu.9csxet.cn

[T39] Lua：模式匹配
来源：http://dh.wgjwhj.cn

string.find(s, "%d+")
来源：http://sw.muxihuayi.cn

[T40] Lua：元表
来源：http://iw.nicolike.cn

setmetatable({}, { __index = base })
来源：http://ri.shxzukj.cn

[T41] Perl：Hello World
来源：http://ex.jctech888.com.cn

print "Hello\n";
来源：http://rm.szxytkj.cn

[T42] Perl：变量类型
来源：http://hg.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jh.newstarts.cn

[T43] Perl：字符串插值
来源：http://ih.bjjhwx.cn

"值: $a"
来源：http://xs.shxzukj.cn

[T44] Perl：条件
来源：http://fd.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://xc.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://hp.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://ob.asd995.cn

[T46] Perl：哈希操作
来源：http://qv.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ii.szxytkj.cn

[T47] Perl：正则捕获
来源：http://xd.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jb.szsharing.cn

[T48] Perl：正则替换
来源：http://uf.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://uq.huixinmuqiang.cn

[T49] Perl：函数
来源：http://xp.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gz.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://ic.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://el.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://fy.wgjwhj.cn

[T51] Scala：Hello World
来源：http://gi.szxytkj.cn

println("Hello")
来源：http://bh.shxzskj.cn

[T52] Scala：变量
来源：http://ta.jctech888.com.cn

val a = 1;  var b = 2
来源：http://xt.newstarts.cn

[T53] Scala：字符串插值
来源：http://lh.asd995.cn

s"值: $b"
来源：http://pm.hnjuh.cn

[T54] Scala：集合映射
来源：http://dt.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://ts.asd995.cn

[T55] Scala：集合过滤
来源：http://ht.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rq.gzmigu.cn

[T56] Scala：样例类
来源：http://ry.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://jr.nszjky.cn

[T57] Scala：模式匹配
来源：http://fl.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mz.haigaiapp.cn

[T58] Scala：函数定义
来源：http://da.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vh.asd995.cn

[T59] Scala：循环
来源：http://uw.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://mj.asd995.cn

[T60] Scala：折叠
来源：http://gl.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hf.shtwfgs.cn

================================================================================
来源：http://vf.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mc.bjjhwx.cn

================================================================================
来源：http://xi.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://ua.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cs.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://dt.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rn.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ba.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yj.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://au.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tk.asd995.cn

[U05] Py：列表去重且保序
来源：http://mt.newstarts.cn

list(dict.fromkeys(arr))
来源：http://sr.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://pr.huixinmuqiang.cn

{**a, **b}
来源：http://vq.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://np.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://bb.521024.cn

[U08] Py：展平二维列表
来源：http://ia.colortex.cn

[y for x in nested for y in x]
来源：http://gq.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://mp.bjjhwx.cn

max(d, key=d.get)
来源：http://gr.nszjky.cn

[U10] Py：按值排序字典
来源：http://tx.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ii.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://os.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ni.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fh.nszjky.cn

Counter(arr).most_common(3)
来源：http://tn.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://fb.bookmarksfly.cn

deque(maxlen=10)
来源：http://pe.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://jr.yuexingan06.cn

defaultdict(list)
来源：http://ml.9csxet.cn

[U15] Py：高精度计时
来源：http://jh.shtwfgs.cn

t = time.perf_counter()
来源：http://gg.521024.cn

[U16] Py：命令行参数解析
来源：http://cj.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ms.521024.cn

[U17] Py：初始化日志
来源：http://ti.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://pl.hnjuh.cn

[U18] Py：预编译正则
来源：http://hu.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://ok.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://oe.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eh.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://cf.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://hi.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://ov.521024.cn

@contextlib.contextmanager
来源：http://zs.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://jj.huixinmuqiang.cn

list(zip(*m))
来源：http://gj.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://bc.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mc.shxzskj.cn

[U24] Py：路径操作
来源：http://na.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ew.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://pf.nicolike.cn

csv.DictReader(f)
来源：http://oo.colortex.cn

[U26] Py：并发下载
来源：http://hn.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wu.colortex.cn

[U27] Py：异步 HTTP
来源：http://zr.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://jj.muxihuayi.cn

[U28] Py：类型别名
来源：http://nw.colortex.cn

UserId = int
来源：http://bo.huanxung.cn

[U29] Py：属性校验
来源：http://rs.huanxung.cn

@property 与 @x.setter 配合
来源：http://ba.muxihuayi.cn

[U30] Py：数据类
来源：http://dz.shxzukj.cn

@dataclass(slots=True)
来源：http://fr.huixinmuqiang.cn

[U31] Py：单测
来源：http://vd.muxihuayi.cn

python -m pytest -q
来源：http://rd.colortex.cn

[U32] Py：代码格式化
来源：http://vr.asd995.cn

ruff format . && ruff check --fix .
来源：http://js.muxihuayi.cn

[U33] Py：打包发布
来源：http://qy.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://cq.haigaiapp.cn

[U34] Py：判断编码
来源：http://du.shxzukj.cn

chardet.detect(raw)
来源：http://jo.panjiajie.cn

[U35] Py：发送邮件
来源：http://na.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fb.yuexingan06.cn

[U36] Py：定时任务
来源：http://bo.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://vz.colortex.cn

[U37] Py：读写 Excel
来源：http://hv.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://or.521024.cn

[U38] Py：获取脚本所在目录
来源：http://nc.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://jw.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://ne.wgjwhj.cn

sys.stdout.isatty()
来源：http://am.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://qq.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://qu.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://vh.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ov.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://sc.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fm.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://fn.newstarts.cn

namespace App\Http;
来源：http://wq.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://mc.asd995.cn

declare(strict_types=1);
来源：http://sl.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://xe.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://je.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://zw.asd995.cn

?string $name = null
来源：http://tz.9csxet.cn

[U47] PHP：联合类型
来源：http://pk.lnxyls.cn

int|string $id
来源：http://ul.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://xz.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ad.hnjuh.cn

[U49] PHP：只读属性
来源：http://um.jctech888.com.cn

public readonly string $name
来源：http://jf.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://mp.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://vg.huixiangedu.cn

[U51] PHP：数组解构
来源：http://op.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://us.asd995.cn

[U52] PHP：箭头函数
来源：http://lu.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://kj.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://xz.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://wm.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://ry.haigaiapp.cn

$obj?->method()
来源：http://dc.shxzukj.cn

[U55] PHP：match 表达式
来源：http://yy.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ii.chemitech.net.cn

[U56] PHP：命名参数
来源：http://kz.newstarts.cn

f(a: 1, b: 2)
来源：http://kv.newstarts.cn

[U57] PHP：字符串插值
来源：http://cj.huixiangedu.cn

"值: {$a}"
来源：http://bg.shxzukj.cn

[U58] PHP：数组三件套
来源：http://et.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mo.shxzskj.cn

[U59] PHP：自定义排序
来源：http://ym.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ft.521024.cn

[U60] PHP：JSON 编解码
来源：http://gh.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cg.bjjhwx.cn

[U61] PHP：正则
来源：http://di.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qu.hahajie.cn

[U62] PHP：日期对象
来源：http://qx.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sj.huixiangedu.cn

[U63] PHP：文件读写
来源：http://xv.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yv.lnxyls.cn

[U64] PHP：目录遍历
来源：http://cj.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://aj.wgjwhj.cn

[U65] PHP：会话
来源：http://yp.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ja.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://vz.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bt.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://vu.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ev.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://mn.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mv.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://ld.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ii.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://pl.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lh.nicolike.cn

[U71] PHP：抛出异常
来源：http://bq.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://iq.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://he.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://yj.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://mj.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://qj.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ii.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://gz.lnxyls.cn

[U75] PHP：依赖注入
来源：http://mf.shxzskj.cn

composer require psr/container
来源：http://ty.haigaiapp.cn

[U76] PHP：简单路由
来源：http://hr.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rs.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://fm.panjiajie.cn

composer require twig/twig
来源：http://gi.panjiajie.cn

[U78] PHP：单元测试
来源：http://dz.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://xm.521024.cn

[U79] PHP：静态分析
来源：http://sn.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://hv.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://hc.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ie.newstarts.cn

[U81] JS：初始化项目
来源：http://ri.gzmigu.cn

npm init -y;  npm i express
来源：http://ry.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://uc.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dz.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://ml.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wq.521024.cn

[U84] JS：CommonJS 写法
来源：http://md.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uz.521024.cn

[U85] JS：可选链
来源：http://as.nszjky.cn

a?.b?.c
来源：http://eb.nicolike.cn

[U86] JS：空值合并
来源：http://wp.nicolike.cn

a ?? b
来源：http://pg.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ek.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://gk.shxzskj.cn

[U88] JS：对象展开合并
来源：http://wa.newstarts.cn

{ ...a, ...b }
来源：http://uq.9csxet.cn

[U89] JS：数组去重
来源：http://ku.yuexingan06.cn

[...new Set(arr)]
来源：http://bh.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://dv.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://og.hahajie.cn

[U91] JS：对象键值遍历
来源：http://ei.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gz.chemitech.net.cn

[U92] JS：深拷贝
来源：http://ef.colortex.cn

structuredClone(obj)
来源：http://jm.newstarts.cn

[U93] JS：模板字符串
来源：http://nf.shtwfgs.cn

`共 ${n} 条`
来源：http://zt.haigaiapp.cn

[U94] JS：箭头函数
来源：http://sc.huanxung.cn

const double = x => x * 2;
来源：http://du.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://mr.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://jv.newstarts.cn

[U96] JS：async/await 与异常
来源：http://xm.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xm.huanxung.cn

[U97] JS：并发请求
来源：http://li.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ir.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://cg.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://em.shtwfgs.cn

[U99] JS：事件监听
来源：http://vn.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://xp.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://dd.bookmarksfly.cn

document.querySelector(".item")
来源：http://fy.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://uc.szsharing.cn

el.classList.toggle("active")
来源：http://lc.wgjwhj.cn

[U102] JS：本地存储
来源：http://mx.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zu.nicolike.cn

[U103] JS：定时器
来源：http://wo.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wy.bookmarksfly.cn

[U104] JS：防抖
来源：http://sl.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://er.shxzukj.cn

[U105] JS：节流
来源：http://su.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sx.hahajie.cn

[U106] JS：日期格式化
来源：http://he.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nr.lnxyls.cn

[U107] JS：数字千分位
来源：http://lz.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kc.jctech888.com.cn

[U108] JS：随机整数
来源：http://fy.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ge.szxytkj.cn

[U109] JS：数组分组
来源：http://ti.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://bq.shtwfgs.cn

[U110] JS：数组分块
来源：http://do.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sk.huanxung.cn

[U111] JS：对象转 Map
来源：http://dg.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ql.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://wa.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://wt.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://oc.hnjuh.cn

s.replaceAll("a", "b")
来源：http://ei.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://cm.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pc.panjiajie.cn

[U115] JS：生成 UUID
来源：http://np.colortex.cn

crypto.randomUUID()
来源：http://bu.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://tv.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://yn.jctech888.com.cn

[U117] JS：单元测试
来源：http://hl.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://ir.szsharing.cn

[U118] JS：开发服务器
来源：http://oh.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://gr.shtwfgs.cn

[U119] JS：生产构建
来源：http://kf.jianghongdianzi.cn

npx vite build
来源：http://ol.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://qe.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://td.hnjuh.cn


<!-- 参考信息 -->