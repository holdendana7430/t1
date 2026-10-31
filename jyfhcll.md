代发 wailian999

[T37] Lua：字符串拼接
来源：http://ni.muxihuayi.cn

"a" .. "b"
来源：http://aa.yuexingan06.cn

[T38] Lua：条件
来源：http://zd.wgjwhj.cn

if x > 0 then print("正") end
来源：http://sg.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://vz.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://tk.shtwfgs.cn

[T40] Lua：元表
来源：http://ql.9csxet.cn

setmetatable({}, { __index = base })
来源：http://nu.panjiajie.cn

[T41] Perl：Hello World
来源：http://bx.jianghongdianzi.cn

print "Hello\n";
来源：http://nw.gzmigu.cn

[T42] Perl：变量类型
来源：http://ix.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ay.hnjuh.cn

[T43] Perl：字符串插值
来源：http://aw.nicolike.cn

"值: $a"
来源：http://nb.colortex.cn

[T44] Perl：条件
来源：http://or.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://kq.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://nq.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://jf.521024.cn

[T46] Perl：哈希操作
来源：http://qx.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fe.huanxung.cn

[T47] Perl：正则捕获
来源：http://zw.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://to.lnxyls.cn

[T48] Perl：正则替换
来源：http://do.huanxung.cn

$s =~ s/old/new/g;
来源：http://gx.yuexingan06.cn

[T49] Perl：函数
来源：http://zo.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kw.521024.cn

[T50] Perl：逐行读文件
来源：http://we.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yd.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://wg.nicolike.cn

[T51] Scala：Hello World
来源：http://lm.panjiajie.cn

println("Hello")
来源：http://ce.lnxyls.cn

[T52] Scala：变量
来源：http://ot.gzmigu.cn

val a = 1;  var b = 2
来源：http://eg.521024.cn

[T53] Scala：字符串插值
来源：http://ad.lnxyls.cn

s"值: $b"
来源：http://mg.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://bi.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://kb.shxzukj.cn

[T55] Scala：集合过滤
来源：http://gu.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://du.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://ji.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://cz.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://qq.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aw.lnxyls.cn

[T58] Scala：函数定义
来源：http://ie.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iy.asd995.cn

[T59] Scala：循环
来源：http://ug.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://ov.huixiangedu.cn

[T60] Scala：折叠
来源：http://em.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ds.shxzskj.cn

================================================================================
来源：http://rh.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tt.chemitech.net.cn

================================================================================
来源：http://un.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://fh.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qy.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ne.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jm.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://mu.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gf.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://xa.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hf.colortex.cn

[U05] Py：列表去重且保序
来源：http://oq.asd995.cn

list(dict.fromkeys(arr))
来源：http://wm.szxytkj.cn

[U06] Py：合并两个字典
来源：http://oq.9csxet.cn

{**a, **b}
来源：http://jj.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://xs.521024.cn

{v: k for k, v in d.items()}
来源：http://sk.nicolike.cn

[U08] Py：展平二维列表
来源：http://el.szsharing.cn

[y for x in nested for y in x]
来源：http://px.asd995.cn

[U09] Py：字典取最大值的键
来源：http://vu.haigaiapp.cn

max(d, key=d.get)
来源：http://xe.nicolike.cn

[U10] Py：按值排序字典
来源：http://ff.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uk.asd995.cn

[U11] Py：生成器表达式
来源：http://iv.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://wy.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xs.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://ig.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://xv.bookmarksfly.cn

deque(maxlen=10)
来源：http://me.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ok.newstarts.cn

defaultdict(list)
来源：http://bl.gzmigu.cn

[U15] Py：高精度计时
来源：http://ii.shxzukj.cn

t = time.perf_counter()
来源：http://yl.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://vx.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://og.wgjwhj.cn

[U17] Py：初始化日志
来源：http://zr.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://zo.muxihuayi.cn

[U18] Py：预编译正则
来源：http://xf.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://uw.nszjky.cn

[U19] Py：正则替换带回调
来源：http://gj.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://no.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://cg.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://dp.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://vz.szxytkj.cn

@contextlib.contextmanager
来源：http://tx.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://lz.szsharing.cn

list(zip(*m))
来源：http://tb.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://uz.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fx.jctech888.com.cn

[U24] Py：路径操作
来源：http://cj.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uj.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://gv.colortex.cn

csv.DictReader(f)
来源：http://rx.yuexingan06.cn

[U26] Py：并发下载
来源：http://oy.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bx.asd995.cn

[U27] Py：异步 HTTP
来源：http://jt.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://ok.9csxet.cn

[U28] Py：类型别名
来源：http://gu.nszjky.cn

UserId = int
来源：http://se.bjjhwx.cn

[U29] Py：属性校验
来源：http://jc.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://mz.haigaiapp.cn

[U30] Py：数据类
来源：http://db.hahajie.cn

@dataclass(slots=True)
来源：http://wp.hahajie.cn

[U31] Py：单测
来源：http://kc.huanxung.cn

python -m pytest -q
来源：http://lc.jctech888.com.cn

[U32] Py：代码格式化
来源：http://ez.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://vt.nicolike.cn

[U33] Py：打包发布
来源：http://te.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://by.nicolike.cn

[U34] Py：判断编码
来源：http://qb.huixinmuqiang.cn

chardet.detect(raw)
来源：http://ff.colortex.cn

[U35] Py：发送邮件
来源：http://tk.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iq.chemitech.net.cn

[U36] Py：定时任务
来源：http://mf.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://uz.asd995.cn

[U37] Py：读写 Excel
来源：http://ko.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://am.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://vv.szxytkj.cn

Path(__file__).resolve().parent
来源：http://tq.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://yk.muxihuayi.cn

sys.stdout.isatty()
来源：http://ng.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://wc.shxzukj.cn

print("err", file=sys.stderr)
来源：http://bv.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ac.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zv.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://zg.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lo.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://lm.gzmigu.cn

namespace App\Http;
来源：http://bh.szsharing.cn

[U44] PHP：开启严格类型
来源：http://zt.lnxyls.cn

declare(strict_types=1);
来源：http://rn.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://nq.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mq.bjjhwx.cn

[U46] PHP：可空类型
来源：http://xd.jctech888.com.cn

?string $name = null
来源：http://tl.shxzukj.cn

[U47] PHP：联合类型
来源：http://ga.hnjuh.cn

int|string $id
来源：http://xq.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://jh.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://es.shxzukj.cn

[U49] PHP：只读属性
来源：http://cv.huanxung.cn

public readonly string $name
来源：http://px.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://rp.newstarts.cn

public function __construct(private int $id) {}
来源：http://qe.huixiangedu.cn

[U51] PHP：数组解构
来源：http://oo.nszjky.cn

[$a, $b] = $arr;
来源：http://hh.newstarts.cn

[U52] PHP：箭头函数
来源：http://kk.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ls.nszjky.cn

[U53] PHP：空合并运算符
来源：http://cv.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://ac.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://ch.huixinmuqiang.cn

$obj?->method()
来源：http://fg.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://mz.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yl.colortex.cn

[U56] PHP：命名参数
来源：http://hz.shxzukj.cn

f(a: 1, b: 2)
来源：http://gp.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://mp.yuntaijiaju.cn

"值: {$a}"
来源：http://zt.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ee.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ef.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://vf.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ls.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://oq.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qi.bjjhwx.cn

[U61] PHP：正则
来源：http://xb.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vk.9csxet.cn

[U62] PHP：日期对象
来源：http://qw.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ya.asd995.cn

[U63] PHP：文件读写
来源：http://xx.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hu.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://ir.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://zd.bjjhwx.cn

[U65] PHP：会话
来源：http://yd.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ln.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://kk.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zj.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://wy.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yc.asd995.cn

[U68] PHP：PDO 连接
来源：http://vy.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sd.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://rq.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bm.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ka.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xn.newstarts.cn

[U71] PHP：抛出异常
来源：http://nn.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://gf.huanxung.cn

[U72] PHP：写错误日志
来源：http://vr.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://il.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://ei.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://ry.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://im.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://uk.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://of.jctech888.com.cn

composer require psr/container
来源：http://jg.asd995.cn

[U76] PHP：简单路由
来源：http://si.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tb.hnjuh.cn

[U77] PHP：模板渲染
来源：http://mb.nszjky.cn

composer require twig/twig
来源：http://tx.haigaiapp.cn

[U78] PHP：单元测试
来源：http://uf.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://gt.szsharing.cn

[U79] PHP：静态分析
来源：http://vj.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://ij.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://uc.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sl.nszjky.cn

[U81] JS：初始化项目
来源：http://wj.colortex.cn

npm init -y;  npm i express
来源：http://tu.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://ns.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xe.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://ax.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cu.asd995.cn

[U84] JS：CommonJS 写法
来源：http://vw.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qr.nicolike.cn

[U85] JS：可选链
来源：http://wo.szxytkj.cn

a?.b?.c
来源：http://qg.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://nk.yuexingan06.cn

a ?? b
来源：http://sv.9csxet.cn

[U87] JS：解构默认值
来源：http://vt.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://wy.szsharing.cn

[U88] JS：对象展开合并
来源：http://mf.muxihuayi.cn

{ ...a, ...b }
来源：http://mu.jctech888.com.cn

[U89] JS：数组去重
来源：http://mi.yuntaijiaju.cn

[...new Set(arr)]
来源：http://kt.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://rb.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://hf.hahajie.cn

[U91] JS：对象键值遍历
来源：http://fe.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cv.9csxet.cn

[U92] JS：深拷贝
来源：http://no.hnjuh.cn

structuredClone(obj)
来源：http://jp.nicolike.cn

[U93] JS：模板字符串
来源：http://ii.huixinmuqiang.cn

`共 ${n} 条`
来源：http://ac.haigaiapp.cn

[U94] JS：箭头函数
来源：http://ze.nszjky.cn

const double = x => x * 2;
来源：http://jp.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://dh.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://wv.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://uo.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://up.colortex.cn

[U97] JS：并发请求
来源：http://ve.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qf.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://ut.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uw.wgjwhj.cn

[U99] JS：事件监听
来源：http://qw.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://si.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://rh.chemitech.net.cn

document.querySelector(".item")
来源：http://ja.panjiajie.cn

[U101] JS：classList 操作
来源：http://au.szsharing.cn

el.classList.toggle("active")
来源：http://tu.yuexingan06.cn

[U102] JS：本地存储
来源：http://yc.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xm.asd995.cn

[U103] JS：定时器
来源：http://do.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vc.521024.cn

[U104] JS：防抖
来源：http://sw.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uf.haigaiapp.cn

[U105] JS：节流
来源：http://zv.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qj.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://bp.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bl.jctech888.com.cn

[U107] JS：数字千分位
来源：http://bj.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xw.panjiajie.cn

[U108] JS：随机整数
来源：http://qx.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sc.hahajie.cn

[U109] JS：数组分组
来源：http://qj.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://ml.hnjuh.cn

[U110] JS：数组分块
来源：http://cy.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://of.hnjuh.cn

[U111] JS：对象转 Map
来源：http://io.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://cb.bjjhwx.cn

[U112] JS：字符串补位
来源：http://tm.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://ph.szsharing.cn

[U113] JS：正则替换全部
来源：http://ep.hnjuh.cn

s.replaceAll("a", "b")
来源：http://dc.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://pl.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ki.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://vz.shxzukj.cn

crypto.randomUUID()
来源：http://tt.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://ix.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://yt.haigaiapp.cn

[U117] JS：单元测试
来源：http://ri.colortex.cn

npm i -D vitest;  npx vitest
来源：http://vw.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://yq.lnxyls.cn

npm i -D vite;  npx vite
来源：http://dq.521024.cn

[U119] JS：生产构建
来源：http://ge.shxzukj.cn

npx vite build
来源：http://bc.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://ds.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://mq.shtwfgs.cn

================================================================================
来源：http://hi.muxihuayi.cn

统计汇总
来源：http://nr.muxihuayi.cn

================================================================================
来源：http://dr.szsharing.cn

按语言统计（条）：
来源：http://kh.lnxyls.cn

Python ......... 252
来源：http://ld.521024.cn

PHP ............ 252
来源：http://pt.yuntaijiaju.cn

JavaScript ..... 252
来源：http://js.shtwfgs.cn

TypeScript ..... 212
来源：http://fp.newstarts.cn


<!-- 参考信息 -->