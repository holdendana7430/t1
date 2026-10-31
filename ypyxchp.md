代发 wailian999

[T37] Lua：字符串拼接
来源：http://fa.hahajie.cn

"a" .. "b"
来源：http://eu.nicolike.cn

[T38] Lua：条件
来源：http://ks.nicolike.cn

if x > 0 then print("正") end
来源：http://ps.shxzskj.cn

[T39] Lua：模式匹配
来源：http://dx.shxzukj.cn

string.find(s, "%d+")
来源：http://gx.asd995.cn

[T40] Lua：元表
来源：http://va.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ss.9csxet.cn

[T41] Perl：Hello World
来源：http://ct.muxihuayi.cn

print "Hello\n";
来源：http://bc.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://qg.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pm.panjiajie.cn

[T43] Perl：字符串插值
来源：http://at.yuexingan06.cn

"值: $a"
来源：http://ke.huanxung.cn

[T44] Perl：条件
来源：http://rn.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://sp.hahajie.cn

[T45] Perl：数组遍历
来源：http://se.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://ki.asd995.cn

[T46] Perl：哈希操作
来源：http://qx.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qw.colortex.cn

[T47] Perl：正则捕获
来源：http://bk.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ml.shxzskj.cn

[T48] Perl：正则替换
来源：http://ou.shxzskj.cn

$s =~ s/old/new/g;
来源：http://oe.nszjky.cn

[T49] Perl：函数
来源：http://cb.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://np.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://js.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qw.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://iy.szsharing.cn

[T51] Scala：Hello World
来源：http://mk.chemitech.net.cn

println("Hello")
来源：http://ou.jctech888.com.cn

[T52] Scala：变量
来源：http://th.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://sg.huanxung.cn

[T53] Scala：字符串插值
来源：http://go.newstarts.cn

s"值: $b"
来源：http://zz.muxihuayi.cn

[T54] Scala：集合映射
来源：http://ju.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://jn.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://fq.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jz.yuexingan06.cn

[T56] Scala：样例类
来源：http://pr.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://le.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://np.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://td.hahajie.cn

[T58] Scala：函数定义
来源：http://zs.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uf.szxytkj.cn

[T59] Scala：循环
来源：http://um.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://so.wgjwhj.cn

[T60] Scala：折叠
来源：http://fj.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://il.hnjuh.cn

================================================================================
来源：http://ji.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zn.shtwfgs.cn

================================================================================
来源：http://bn.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://jo.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qn.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://sb.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hm.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://iv.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://al.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://qi.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://du.hahajie.cn

[U05] Py：列表去重且保序
来源：http://za.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://ud.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://ck.gzmigu.cn

{**a, **b}
来源：http://iw.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://jy.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://fq.colortex.cn

[U08] Py：展平二维列表
来源：http://jw.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://vo.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://xb.jianghongdianzi.cn

max(d, key=d.get)
来源：http://nj.9csxet.cn

[U10] Py：按值排序字典
来源：http://je.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wu.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ro.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://cb.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://it.newstarts.cn

Counter(arr).most_common(3)
来源：http://rt.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://mb.wgjwhj.cn

deque(maxlen=10)
来源：http://if.nszjky.cn

[U14] Py：分组收集到列表
来源：http://rz.chemitech.net.cn

defaultdict(list)
来源：http://ac.asd995.cn

[U15] Py：高精度计时
来源：http://ym.nszjky.cn

t = time.perf_counter()
来源：http://uf.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://bb.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cc.huanxung.cn

[U17] Py：初始化日志
来源：http://ql.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://td.hnjuh.cn

[U18] Py：预编译正则
来源：http://mh.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://cg.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://ok.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sj.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://dd.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://vh.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://ou.haigaiapp.cn

@contextlib.contextmanager
来源：http://ng.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://uc.nicolike.cn

list(zip(*m))
来源：http://uc.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://kb.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://in.9csxet.cn

[U24] Py：路径操作
来源：http://hx.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vt.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://uq.9csxet.cn

csv.DictReader(f)
来源：http://bs.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://iu.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zy.colortex.cn

[U27] Py：异步 HTTP
来源：http://bg.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://wg.nszjky.cn

[U28] Py：类型别名
来源：http://ft.521024.cn

UserId = int
来源：http://qn.haigaiapp.cn

[U29] Py：属性校验
来源：http://oc.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://rx.bookmarksfly.cn

[U30] Py：数据类
来源：http://xj.bookmarksfly.cn

@dataclass(slots=True)
来源：http://bq.wgjwhj.cn

[U31] Py：单测
来源：http://dx.huixinmuqiang.cn

python -m pytest -q
来源：http://sy.nicolike.cn

[U32] Py：代码格式化
来源：http://ra.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://dw.lnxyls.cn

[U33] Py：打包发布
来源：http://cr.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://uu.jctech888.com.cn

[U34] Py：判断编码
来源：http://zu.bjjhwx.cn

chardet.detect(raw)
来源：http://mx.jctech888.com.cn

[U35] Py：发送邮件
来源：http://ce.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bg.shxzskj.cn

[U36] Py：定时任务
来源：http://gx.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://sz.9csxet.cn

[U37] Py：读写 Excel
来源：http://pi.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jy.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://qt.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://wh.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://dr.haigaiapp.cn

sys.stdout.isatty()
来源：http://dt.nicolike.cn

[U40] Py：打印到标准错误
来源：http://np.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://dd.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://ux.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ej.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://qn.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qd.asd995.cn

[U43] PHP：声明命名空间
来源：http://gz.bjjhwx.cn

namespace App\Http;
来源：http://og.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://ew.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ka.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://jk.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ut.wgjwhj.cn

[U46] PHP：可空类型
来源：http://es.yuntaijiaju.cn

?string $name = null
来源：http://bz.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://ho.huixinmuqiang.cn

int|string $id
来源：http://aa.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://ju.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://td.wgjwhj.cn

[U49] PHP：只读属性
来源：http://lj.haigaiapp.cn

public readonly string $name
来源：http://fv.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://hn.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://cx.muxihuayi.cn

[U51] PHP：数组解构
来源：http://hw.panjiajie.cn

[$a, $b] = $arr;
来源：http://no.asd995.cn

[U52] PHP：箭头函数
来源：http://sb.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://ms.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://vt.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://qu.huanxung.cn

[U54] PHP：空安全调用
来源：http://uq.chemitech.net.cn

$obj?->method()
来源：http://eb.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://ep.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uv.huanxung.cn

[U56] PHP：命名参数
来源：http://nl.chemitech.net.cn

f(a: 1, b: 2)
来源：http://wl.hahajie.cn

[U57] PHP：字符串插值
来源：http://oc.lnxyls.cn

"值: {$a}"
来源：http://hh.shxzskj.cn

[U58] PHP：数组三件套
来源：http://nz.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ht.szsharing.cn

[U59] PHP：自定义排序
来源：http://fg.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hw.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://dt.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sd.chemitech.net.cn

[U61] PHP：正则
来源：http://rg.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jr.szsharing.cn

[U62] PHP：日期对象
来源：http://kk.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://en.huanxung.cn

[U63] PHP：文件读写
来源：http://gf.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fz.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://jr.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://zk.szxytkj.cn

[U65] PHP：会话
来源：http://rs.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dh.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://sj.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ex.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://yk.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vv.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://bu.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ui.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://be.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wu.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://lq.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://em.hnjuh.cn

[U71] PHP：抛出异常
来源：http://vs.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://md.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://lv.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://sc.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://yi.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ce.colortex.cn

[U74] PHP：读取环境变量
来源：http://nw.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://el.521024.cn

[U75] PHP：依赖注入
来源：http://xv.huixiangedu.cn

composer require psr/container
来源：http://cv.gzmigu.cn

[U76] PHP：简单路由
来源：http://kk.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lt.lnxyls.cn

[U77] PHP：模板渲染
来源：http://xp.shxzskj.cn

composer require twig/twig
来源：http://ez.hnjuh.cn

[U78] PHP：单元测试
来源：http://yd.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://vp.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://rx.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://zk.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://zd.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xd.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://vl.shtwfgs.cn

npm init -y;  npm i express
来源：http://qi.9csxet.cn

[U82] JS：package.json 脚本
来源：http://dj.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://si.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://kb.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vx.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://cs.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ur.asd995.cn

[U85] JS：可选链
来源：http://uz.muxihuayi.cn

a?.b?.c
来源：http://ea.huixiangedu.cn

[U86] JS：空值合并
来源：http://lr.muxihuayi.cn

a ?? b
来源：http://zm.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://av.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://yl.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://lb.huixiangedu.cn

{ ...a, ...b }
来源：http://vf.huanxung.cn

[U89] JS：数组去重
来源：http://mx.nicolike.cn

[...new Set(arr)]
来源：http://fq.colortex.cn

[U90] JS：数字数组排序
来源：http://su.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://ih.hahajie.cn

[U91] JS：对象键值遍历
来源：http://qf.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cu.muxihuayi.cn

[U92] JS：深拷贝
来源：http://ej.szxytkj.cn

structuredClone(obj)
来源：http://wy.nicolike.cn

[U93] JS：模板字符串
来源：http://aa.gzmigu.cn

`共 ${n} 条`
来源：http://kw.nszjky.cn

[U94] JS：箭头函数
来源：http://mu.bookmarksfly.cn

const double = x => x * 2;
来源：http://es.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ej.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://aw.huanxung.cn

[U96] JS：async/await 与异常
来源：http://yl.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gi.wgjwhj.cn

[U97] JS：并发请求
来源：http://pc.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nf.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://uw.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gn.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://xn.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://pw.hahajie.cn

[U100] JS：DOM 查询
来源：http://cc.szxytkj.cn

document.querySelector(".item")
来源：http://lf.jctech888.com.cn

[U101] JS：classList 操作
来源：http://uq.panjiajie.cn

el.classList.toggle("active")
来源：http://hu.yuexingan06.cn

[U102] JS：本地存储
来源：http://de.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ee.nicolike.cn

[U103] JS：定时器
来源：http://is.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mu.lnxyls.cn

[U104] JS：防抖
来源：http://mz.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dt.szsharing.cn

[U105] JS：节流
来源：http://ji.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yh.szxytkj.cn

[U106] JS：日期格式化
来源：http://iu.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bx.lnxyls.cn

[U107] JS：数字千分位
来源：http://uw.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ac.newstarts.cn

[U108] JS：随机整数
来源：http://ky.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qb.bjjhwx.cn

[U109] JS：数组分组
来源：http://vb.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://hp.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://id.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eg.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://aa.lnxyls.cn

new Map(Object.entries(obj))
来源：http://vw.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://pc.panjiajie.cn

"7".padStart(3, "0")
来源：http://oh.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://yz.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://df.szsharing.cn

[U114] JS：JSON 深比较
来源：http://bn.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gq.shxzskj.cn

[U115] JS：生成 UUID
来源：http://zd.panjiajie.cn

crypto.randomUUID()
来源：http://tp.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://ks.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://je.521024.cn

[U117] JS：单元测试
来源：http://in.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://np.9csxet.cn

[U118] JS：开发服务器
来源：http://ag.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ww.9csxet.cn

[U119] JS：生产构建
来源：http://vq.huanxung.cn

npx vite build
来源：http://bb.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://xm.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://nd.nszjky.cn

================================================================================
来源：http://qa.wgjwhj.cn

统计汇总
来源：http://eu.bookmarksfly.cn

================================================================================
来源：http://ar.huanxung.cn

按语言统计（条）：
来源：http://wc.haigaiapp.cn

Python ......... 252
来源：http://yp.gzmigu.cn

PHP ............ 252
来源：http://ah.jianghongdianzi.cn

JavaScript ..... 252
来源：http://cx.gzmigu.cn

TypeScript ..... 212
来源：http://nz.newstarts.cn


<!-- 参考信息 -->