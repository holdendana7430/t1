代发 wailian999

[T39] Lua：模式匹配
来源：http://ng.szsharing.cn

string.find(s, "%d+")
来源：http://br.521024.cn

[T40] Lua：元表
来源：http://nj.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://lr.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://pu.newstarts.cn

print "Hello\n";
来源：http://bm.jctech888.com.cn

[T42] Perl：变量类型
来源：http://ds.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qp.lnxyls.cn

[T43] Perl：字符串插值
来源：http://fj.szsharing.cn

"值: $a"
来源：http://yo.szxytkj.cn

[T44] Perl：条件
来源：http://ed.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ey.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://ta.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://ka.shxzskj.cn

[T46] Perl：哈希操作
来源：http://td.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rg.colortex.cn

[T47] Perl：正则捕获
来源：http://ix.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fv.gzmigu.cn

[T48] Perl：正则替换
来源：http://ge.panjiajie.cn

$s =~ s/old/new/g;
来源：http://ci.shxzskj.cn

[T49] Perl：函数
来源：http://bt.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rb.szsharing.cn

[T50] Perl：逐行读文件
来源：http://fq.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rw.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://cb.muxihuayi.cn

[T51] Scala：Hello World
来源：http://lm.bookmarksfly.cn

println("Hello")
来源：http://cg.jianghongdianzi.cn

[T52] Scala：变量
来源：http://xz.lnxyls.cn

val a = 1;  var b = 2
来源：http://cw.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://mm.muxihuayi.cn

s"值: $b"
来源：http://sx.huanxung.cn

[T54] Scala：集合映射
来源：http://on.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://rj.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://qg.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://of.jctech888.com.cn

[T56] Scala：样例类
来源：http://iv.hahajie.cn

case class User(name: String, age: Int)
来源：http://vo.huanxung.cn

[T57] Scala：模式匹配
来源：http://bv.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gj.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://ii.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ba.hnjuh.cn

[T59] Scala：循环
来源：http://dy.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://zy.panjiajie.cn

[T60] Scala：折叠
来源：http://xd.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://km.shxzskj.cn

================================================================================
来源：http://id.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ld.huanxung.cn

================================================================================
来源：http://zz.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://oj.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oa.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://wv.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pa.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://ax.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zr.szxytkj.cn

[U04] Py：变量调试打印
来源：http://rm.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ey.nszjky.cn

[U05] Py：列表去重且保序
来源：http://tw.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://vj.colortex.cn

[U06] Py：合并两个字典
来源：http://pa.hahajie.cn

{**a, **b}
来源：http://df.huanxung.cn

[U07] Py：反转字典键值
来源：http://yu.huanxung.cn

{v: k for k, v in d.items()}
来源：http://xn.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://fk.shxzskj.cn

[y for x in nested for y in x]
来源：http://bs.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://rr.9csxet.cn

max(d, key=d.get)
来源：http://pb.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://xk.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vn.9csxet.cn

[U11] Py：生成器表达式
来源：http://jg.shxzukj.cn

(x * 2 for x in arr)
来源：http://gz.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tw.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://fi.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://bf.yuexingan06.cn

deque(maxlen=10)
来源：http://zi.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ki.jianghongdianzi.cn

defaultdict(list)
来源：http://gh.asd995.cn

[U15] Py：高精度计时
来源：http://ku.huixiangedu.cn

t = time.perf_counter()
来源：http://bh.521024.cn

[U16] Py：命令行参数解析
来源：http://xc.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ig.nicolike.cn

[U17] Py：初始化日志
来源：http://fu.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://yu.yuexingan06.cn

[U18] Py：预编译正则
来源：http://hz.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://ft.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://pe.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fd.asd995.cn

[U20] Py：缓存函数结果
来源：http://ze.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://cg.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://nk.bjjhwx.cn

@contextlib.contextmanager
来源：http://jy.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://js.szsharing.cn

list(zip(*m))
来源：http://mi.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://ia.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zm.jctech888.com.cn

[U24] Py：路径操作
来源：http://uo.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fx.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://dh.bookmarksfly.cn

csv.DictReader(f)
来源：http://mb.szsharing.cn

[U26] Py：并发下载
来源：http://ri.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tt.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://bo.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://kq.huixiangedu.cn

[U28] Py：类型别名
来源：http://is.newstarts.cn

UserId = int
来源：http://ph.nszjky.cn

[U29] Py：属性校验
来源：http://za.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://uz.haigaiapp.cn

[U30] Py：数据类
来源：http://ga.huixiangedu.cn

@dataclass(slots=True)
来源：http://pv.huanxung.cn

[U31] Py：单测
来源：http://jx.hahajie.cn

python -m pytest -q
来源：http://mr.hahajie.cn

[U32] Py：代码格式化
来源：http://zp.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://ev.haigaiapp.cn

[U33] Py：打包发布
来源：http://un.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://lw.nszjky.cn

[U34] Py：判断编码
来源：http://us.asd995.cn

chardet.detect(raw)
来源：http://jd.szxytkj.cn

[U35] Py：发送邮件
来源：http://rw.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://id.shxzukj.cn

[U36] Py：定时任务
来源：http://mk.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://vg.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://oj.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eu.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://ed.asd995.cn

Path(__file__).resolve().parent
来源：http://sa.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://zv.gzmigu.cn

sys.stdout.isatty()
来源：http://ez.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://ek.hnjuh.cn

print("err", file=sys.stderr)
来源：http://jq.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ta.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kz.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://lj.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mk.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://td.colortex.cn

namespace App\Http;
来源：http://se.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://ww.lnxyls.cn

declare(strict_types=1);
来源：http://lu.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ar.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cy.huanxung.cn

[U46] PHP：可空类型
来源：http://bx.huixinmuqiang.cn

?string $name = null
来源：http://kx.hahajie.cn

[U47] PHP：联合类型
来源：http://ky.newstarts.cn

int|string $id
来源：http://zp.newstarts.cn

[U48] PHP：纯枚举
来源：http://td.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qm.yuexingan06.cn

[U49] PHP：只读属性
来源：http://gb.szxytkj.cn

public readonly string $name
来源：http://bz.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://km.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ka.wgjwhj.cn

[U51] PHP：数组解构
来源：http://xs.shxzukj.cn

[$a, $b] = $arr;
来源：http://au.hahajie.cn

[U52] PHP：箭头函数
来源：http://ha.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://uw.huanxung.cn

[U53] PHP：空合并运算符
来源：http://vs.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://qj.asd995.cn

[U54] PHP：空安全调用
来源：http://mf.shxzskj.cn

$obj?->method()
来源：http://le.lnxyls.cn

[U55] PHP：match 表达式
来源：http://dp.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rj.521024.cn

[U56] PHP：命名参数
来源：http://xm.shtwfgs.cn

f(a: 1, b: 2)
来源：http://md.nicolike.cn

[U57] PHP：字符串插值
来源：http://ro.szsharing.cn

"值: {$a}"
来源：http://ix.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://lk.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rc.asd995.cn

[U59] PHP：自定义排序
来源：http://kw.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ow.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://la.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jz.nicolike.cn

[U61] PHP：正则
来源：http://tf.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qr.muxihuayi.cn

[U62] PHP：日期对象
来源：http://bp.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rs.newstarts.cn

[U63] PHP：文件读写
来源：http://nj.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://go.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://op.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://je.nicolike.cn

[U65] PHP：会话
来源：http://kg.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wm.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://ps.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tm.nicolike.cn

[U67] PHP：处理文件上传
来源：http://jn.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ku.newstarts.cn

[U68] PHP：PDO 连接
来源：http://ka.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yi.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://ur.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jo.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://kc.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nv.szxytkj.cn

[U71] PHP：抛出异常
来源：http://tl.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://zo.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://vm.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://kg.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://dp.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://pv.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://hd.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://sn.lnxyls.cn

[U75] PHP：依赖注入
来源：http://es.wgjwhj.cn

composer require psr/container
来源：http://tf.szxytkj.cn

[U76] PHP：简单路由
来源：http://dg.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ay.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://kg.nszjky.cn

composer require twig/twig
来源：http://uk.yuexingan06.cn

[U78] PHP：单元测试
来源：http://rs.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://aj.muxihuayi.cn

[U79] PHP：静态分析
来源：http://dx.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://er.nszjky.cn

[U80] PHP：代码规范修复
来源：http://wi.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bj.haigaiapp.cn

[U81] JS：初始化项目
来源：http://lt.colortex.cn

npm init -y;  npm i express
来源：http://kq.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://db.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://al.521024.cn

[U83] JS：ES Module 导入导出
来源：http://kq.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ci.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://ba.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ax.hnjuh.cn

[U85] JS：可选链
来源：http://ht.muxihuayi.cn

a?.b?.c
来源：http://uq.hnjuh.cn

[U86] JS：空值合并
来源：http://cx.huixinmuqiang.cn

a ?? b
来源：http://bm.szsharing.cn

[U87] JS：解构默认值
来源：http://qt.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://ak.nszjky.cn

[U88] JS：对象展开合并
来源：http://pn.lnxyls.cn

{ ...a, ...b }
来源：http://dk.szxytkj.cn

[U89] JS：数组去重
来源：http://hx.bookmarksfly.cn

[...new Set(arr)]
来源：http://rw.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ij.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://rg.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://dt.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aw.shxzukj.cn

[U92] JS：深拷贝
来源：http://td.gzmigu.cn

structuredClone(obj)
来源：http://ti.nicolike.cn

[U93] JS：模板字符串
来源：http://tt.bjjhwx.cn

`共 ${n} 条`
来源：http://iv.hahajie.cn

[U94] JS：箭头函数
来源：http://ez.chemitech.net.cn

const double = x => x * 2;
来源：http://al.hnjuh.cn

[U95] JS：Promise 包装
来源：http://yx.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://cr.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://zt.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sh.hahajie.cn

[U97] JS：并发请求
来源：http://wp.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jn.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://or.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://me.chemitech.net.cn

[U99] JS：事件监听
来源：http://hd.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://sm.shxzukj.cn

[U100] JS：DOM 查询
来源：http://qb.huixiangedu.cn

document.querySelector(".item")
来源：http://zw.colortex.cn

[U101] JS：classList 操作
来源：http://wu.panjiajie.cn

el.classList.toggle("active")
来源：http://ig.nszjky.cn

[U102] JS：本地存储
来源：http://md.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jw.panjiajie.cn

[U103] JS：定时器
来源：http://zw.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eg.hnjuh.cn

[U104] JS：防抖
来源：http://xt.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oj.huixiangedu.cn

[U105] JS：节流
来源：http://ff.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://su.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://nf.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://va.huixiangedu.cn

[U107] JS：数字千分位
来源：http://gy.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ny.muxihuayi.cn

[U108] JS：随机整数
来源：http://ht.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pz.nszjky.cn

[U109] JS：数组分组
来源：http://ol.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://op.chemitech.net.cn

[U110] JS：数组分块
来源：http://ij.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cr.szxytkj.cn

[U111] JS：对象转 Map
来源：http://gz.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://jp.huixiangedu.cn

[U112] JS：字符串补位
来源：http://uo.szsharing.cn

"7".padStart(3, "0")
来源：http://tk.521024.cn

[U113] JS：正则替换全部
来源：http://bl.asd995.cn

s.replaceAll("a", "b")
来源：http://rp.huanxung.cn

[U114] JS：JSON 深比较
来源：http://op.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ji.shxzskj.cn

[U115] JS：生成 UUID
来源：http://xd.nszjky.cn

crypto.randomUUID()
来源：http://ji.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://cu.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://fm.bjjhwx.cn

[U117] JS：单元测试
来源：http://jg.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://fm.hnjuh.cn

[U118] JS：开发服务器
来源：http://um.newstarts.cn

npm i -D vite;  npx vite
来源：http://ce.hahajie.cn

[U119] JS：生产构建
来源：http://le.521024.cn

npx vite build
来源：http://qz.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://su.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://bm.bookmarksfly.cn

================================================================================
来源：http://kf.bjjhwx.cn

统计汇总
来源：http://zz.bookmarksfly.cn

================================================================================
来源：http://ss.bookmarksfly.cn

按语言统计（条）：
来源：http://gk.szsharing.cn

Python ......... 252
来源：http://du.huixinmuqiang.cn

PHP ............ 252
来源：http://dg.newstarts.cn

JavaScript ..... 252
来源：http://kv.jianghongdianzi.cn

TypeScript ..... 212
来源：http://kk.hahajie.cn

Java ........... 212
来源：http://ln.shxzukj.cn

Go ............. 212
来源：http://hz.shtwfgs.cn

Ruby ........... 212
来源：http://ka.panjiajie.cn

C# ............. 212
来源：http://ym.shxzukj.cn


<!-- 参考信息 -->