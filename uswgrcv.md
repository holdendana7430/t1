代发 wailian999

[T37] Lua：字符串拼接
来源：http://lq.yuexingan06.cn

"a" .. "b"
来源：http://ux.gzmigu.cn

[T38] Lua：条件
来源：http://ta.nszjky.cn

if x > 0 then print("正") end
来源：http://zu.521024.cn

[T39] Lua：模式匹配
来源：http://ej.nszjky.cn

string.find(s, "%d+")
来源：http://wv.szsharing.cn

[T40] Lua：元表
来源：http://xj.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://hx.muxihuayi.cn

[T41] Perl：Hello World
来源：http://er.chemitech.net.cn

print "Hello\n";
来源：http://nq.haigaiapp.cn

[T42] Perl：变量类型
来源：http://vl.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xc.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://wm.9csxet.cn

"值: $a"
来源：http://lk.panjiajie.cn

[T44] Perl：条件
来源：http://aa.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://ne.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://re.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://py.nszjky.cn

[T46] Perl：哈希操作
来源：http://lb.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cj.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://mi.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xd.colortex.cn

[T48] Perl：正则替换
来源：http://rs.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://qq.yuexingan06.cn

[T49] Perl：函数
来源：http://sd.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tb.521024.cn

[T50] Perl：逐行读文件
来源：http://mk.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bs.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://ja.chemitech.net.cn

[T51] Scala：Hello World
来源：http://ei.gzmigu.cn

println("Hello")
来源：http://be.nicolike.cn

[T52] Scala：变量
来源：http://hv.muxihuayi.cn

val a = 1;  var b = 2
来源：http://fx.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://ng.lnxyls.cn

s"值: $b"
来源：http://qa.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://mb.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sl.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://uk.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kx.szsharing.cn

[T56] Scala：样例类
来源：http://ru.szsharing.cn

case class User(name: String, age: Int)
来源：http://sq.nicolike.cn

[T57] Scala：模式匹配
来源：http://sd.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sp.9csxet.cn

[T58] Scala：函数定义
来源：http://gs.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nt.bookmarksfly.cn

[T59] Scala：循环
来源：http://qf.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ca.shxzukj.cn

[T60] Scala：折叠
来源：http://pw.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rh.huixinmuqiang.cn

================================================================================
来源：http://qm.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pn.huixiangedu.cn

================================================================================
来源：http://sm.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://pz.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bq.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://ji.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zs.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://fl.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eb.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://wh.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://os.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://gz.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://zh.nicolike.cn

[U06] Py：合并两个字典
来源：http://mw.nicolike.cn

{**a, **b}
来源：http://hu.szsharing.cn

[U07] Py：反转字典键值
来源：http://wv.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://pz.szxytkj.cn

[U08] Py：展平二维列表
来源：http://fs.szxytkj.cn

[y for x in nested for y in x]
来源：http://gh.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://jn.shxzukj.cn

max(d, key=d.get)
来源：http://af.hnjuh.cn

[U10] Py：按值排序字典
来源：http://wa.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ns.nszjky.cn

[U11] Py：生成器表达式
来源：http://fo.gzmigu.cn

(x * 2 for x in arr)
来源：http://wc.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uu.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ul.szxytkj.cn

[U13] Py：固定长度队列
来源：http://ux.nicolike.cn

deque(maxlen=10)
来源：http://bt.9csxet.cn

[U14] Py：分组收集到列表
来源：http://bj.shxzukj.cn

defaultdict(list)
来源：http://ay.haigaiapp.cn

[U15] Py：高精度计时
来源：http://vx.huixinmuqiang.cn

t = time.perf_counter()
来源：http://qt.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://yu.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ny.hnjuh.cn

[U17] Py：初始化日志
来源：http://ga.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://tv.gzmigu.cn

[U18] Py：预编译正则
来源：http://su.521024.cn

pat = re.compile(r"\d+")
来源：http://dc.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://yr.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sz.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://uy.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://nz.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://xd.wgjwhj.cn

@contextlib.contextmanager
来源：http://gf.nszjky.cn

[U22] Py：矩阵转置
来源：http://ci.bookmarksfly.cn

list(zip(*m))
来源：http://ec.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://mj.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://en.shtwfgs.cn

[U24] Py：路径操作
来源：http://mt.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xk.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://os.nicolike.cn

csv.DictReader(f)
来源：http://hx.bookmarksfly.cn

[U26] Py：并发下载
来源：http://sc.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://px.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://nz.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://zv.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://we.huixinmuqiang.cn

UserId = int
来源：http://hq.nszjky.cn

[U29] Py：属性校验
来源：http://wb.panjiajie.cn

@property 与 @x.setter 配合
来源：http://oe.bjjhwx.cn

[U30] Py：数据类
来源：http://nm.yuexingan06.cn

@dataclass(slots=True)
来源：http://gx.szsharing.cn

[U31] Py：单测
来源：http://fn.szxytkj.cn

python -m pytest -q
来源：http://mb.huanxung.cn

[U32] Py：代码格式化
来源：http://mf.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://sy.gzmigu.cn

[U33] Py：打包发布
来源：http://lp.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://np.szsharing.cn

[U34] Py：判断编码
来源：http://jt.huanxung.cn

chardet.detect(raw)
来源：http://ye.yuexingan06.cn

[U35] Py：发送邮件
来源：http://th.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ri.hahajie.cn

[U36] Py：定时任务
来源：http://pt.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://cp.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://wv.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xb.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://lz.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://fu.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://pb.hnjuh.cn

sys.stdout.isatty()
来源：http://it.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://qw.asd995.cn

print("err", file=sys.stderr)
来源：http://gy.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://rl.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wn.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://il.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pe.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://ej.lnxyls.cn

namespace App\Http;
来源：http://je.521024.cn

[U44] PHP：开启严格类型
来源：http://dr.nszjky.cn

declare(strict_types=1);
来源：http://uo.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://wu.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://le.huixiangedu.cn

[U46] PHP：可空类型
来源：http://le.gzmigu.cn

?string $name = null
来源：http://hc.shxzukj.cn

[U47] PHP：联合类型
来源：http://zt.muxihuayi.cn

int|string $id
来源：http://xx.panjiajie.cn

[U48] PHP：纯枚举
来源：http://xa.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ik.wgjwhj.cn

[U49] PHP：只读属性
来源：http://pq.shxzukj.cn

public readonly string $name
来源：http://tm.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://ev.lnxyls.cn

public function __construct(private int $id) {}
来源：http://rz.lnxyls.cn

[U51] PHP：数组解构
来源：http://oz.szsharing.cn

[$a, $b] = $arr;
来源：http://rn.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://lu.521024.cn

$double = fn($x) => $x * 2;
来源：http://pv.szsharing.cn

[U53] PHP：空合并运算符
来源：http://vq.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://vh.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://zp.huixinmuqiang.cn

$obj?->method()
来源：http://ka.shxzukj.cn

[U55] PHP：match 表达式
来源：http://jd.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yw.huixiangedu.cn

[U56] PHP：命名参数
来源：http://nz.nszjky.cn

f(a: 1, b: 2)
来源：http://fg.hnjuh.cn

[U57] PHP：字符串插值
来源：http://bx.yuntaijiaju.cn

"值: {$a}"
来源：http://bg.hnjuh.cn

[U58] PHP：数组三件套
来源：http://kt.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hl.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://jb.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pl.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://eo.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lt.huixiangedu.cn

[U61] PHP：正则
来源：http://ir.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qo.shxzukj.cn

[U62] PHP：日期对象
来源：http://ow.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ak.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ug.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kh.colortex.cn

[U64] PHP：目录遍历
来源：http://zw.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://nl.521024.cn

[U65] PHP：会话
来源：http://rc.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wg.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://dq.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bb.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://go.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xr.huanxung.cn

[U68] PHP：PDO 连接
来源：http://tj.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bg.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://ek.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pw.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://ao.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ji.lnxyls.cn

[U71] PHP：抛出异常
来源：http://nb.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://ky.521024.cn

[U72] PHP：写错误日志
来源：http://cx.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://ef.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://pn.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://es.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://pm.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://ci.huanxung.cn

[U75] PHP：依赖注入
来源：http://wg.lnxyls.cn

composer require psr/container
来源：http://su.haigaiapp.cn

[U76] PHP：简单路由
来源：http://mr.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cu.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://rp.newstarts.cn

composer require twig/twig
来源：http://jp.wgjwhj.cn

[U78] PHP：单元测试
来源：http://bh.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ta.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://fk.asd995.cn

composer require --dev phpstan/phpstan
来源：http://nb.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://al.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yv.yuexingan06.cn

[U81] JS：初始化项目
来源：http://ii.chemitech.net.cn

npm init -y;  npm i express
来源：http://gf.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://ga.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vz.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://fa.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zn.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://zq.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ns.haigaiapp.cn

[U85] JS：可选链
来源：http://cn.szsharing.cn

a?.b?.c
来源：http://nk.colortex.cn

[U86] JS：空值合并
来源：http://ed.9csxet.cn

a ?? b
来源：http://kc.lnxyls.cn

[U87] JS：解构默认值
来源：http://yj.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://at.asd995.cn

[U88] JS：对象展开合并
来源：http://sw.muxihuayi.cn

{ ...a, ...b }
来源：http://ch.shtwfgs.cn

[U89] JS：数组去重
来源：http://hc.asd995.cn

[...new Set(arr)]
来源：http://tr.gzmigu.cn

[U90] JS：数字数组排序
来源：http://wh.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://tb.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://jr.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sa.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://jl.yuntaijiaju.cn

structuredClone(obj)
来源：http://dh.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://hg.szxytkj.cn

`共 ${n} 条`
来源：http://mo.yuexingan06.cn

[U94] JS：箭头函数
来源：http://zm.colortex.cn

const double = x => x * 2;
来源：http://jw.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://wg.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://qf.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://rj.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://su.jctech888.com.cn

[U97] JS：并发请求
来源：http://pd.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://se.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://qa.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ck.bjjhwx.cn

[U99] JS：事件监听
来源：http://fr.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://te.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://ow.hahajie.cn

document.querySelector(".item")
来源：http://jg.yuexingan06.cn

[U101] JS：classList 操作
来源：http://ct.521024.cn

el.classList.toggle("active")
来源：http://qm.szsharing.cn

[U102] JS：本地存储
来源：http://lx.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kr.wgjwhj.cn

[U103] JS：定时器
来源：http://lc.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kq.jianghongdianzi.cn

[U104] JS：防抖
来源：http://aq.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ed.chemitech.net.cn

[U105] JS：节流
来源：http://bq.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ef.huanxung.cn

[U106] JS：日期格式化
来源：http://vn.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xn.shtwfgs.cn

[U107] JS：数字千分位
来源：http://if.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ke.shxzukj.cn

[U108] JS：随机整数
来源：http://th.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qv.lnxyls.cn

[U109] JS：数组分组
来源：http://pe.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://es.9csxet.cn

[U110] JS：数组分块
来源：http://jd.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tj.521024.cn

[U111] JS：对象转 Map
来源：http://tp.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://ww.shxzukj.cn

[U112] JS：字符串补位
来源：http://uq.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://sp.521024.cn

[U113] JS：正则替换全部
来源：http://ee.huanxung.cn

s.replaceAll("a", "b")
来源：http://to.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://xa.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vg.panjiajie.cn

[U115] JS：生成 UUID
来源：http://yr.shtwfgs.cn

crypto.randomUUID()
来源：http://hw.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://mk.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://jo.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://gc.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://og.bjjhwx.cn

[U118] JS：开发服务器
来源：http://bz.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://as.huanxung.cn

[U119] JS：生产构建
来源：http://on.yuntaijiaju.cn

npx vite build
来源：http://bz.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ig.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://ba.hahajie.cn

================================================================================
来源：http://bk.asd995.cn

统计汇总
来源：http://jv.wgjwhj.cn

================================================================================
来源：http://ap.gzmigu.cn

按语言统计（条）：
来源：http://rm.shxzskj.cn

Python ......... 252
来源：http://ol.bjjhwx.cn

PHP ............ 252
来源：http://et.bookmarksfly.cn

JavaScript ..... 252
来源：http://oi.chemitech.net.cn

TypeScript ..... 212
来源：http://lv.szxytkj.cn


<!-- 参考信息 -->