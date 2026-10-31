代发 wailian999

[T37] Lua：字符串拼接
来源：http://sg.nicolike.cn

"a" .. "b"
来源：http://co.bjjhwx.cn

[T38] Lua：条件
来源：http://lf.muxihuayi.cn

if x > 0 then print("正") end
来源：http://nt.9csxet.cn

[T39] Lua：模式匹配
来源：http://ie.jctech888.com.cn

string.find(s, "%d+")
来源：http://nj.nszjky.cn

[T40] Lua：元表
来源：http://ji.colortex.cn

setmetatable({}, { __index = base })
来源：http://mo.panjiajie.cn

[T41] Perl：Hello World
来源：http://io.panjiajie.cn

print "Hello\n";
来源：http://rb.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://dt.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://la.newstarts.cn

[T43] Perl：字符串插值
来源：http://jd.bookmarksfly.cn

"值: $a"
来源：http://mn.yuntaijiaju.cn

[T44] Perl：条件
来源：http://nh.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ec.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://xa.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://sc.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://ri.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mp.szxytkj.cn

[T47] Perl：正则捕获
来源：http://db.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cl.shxzukj.cn

[T48] Perl：正则替换
来源：http://ux.huanxung.cn

$s =~ s/old/new/g;
来源：http://qd.wgjwhj.cn

[T49] Perl：函数
来源：http://uo.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cu.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://hu.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pw.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://lm.lnxyls.cn

[T51] Scala：Hello World
来源：http://ih.yuexingan06.cn

println("Hello")
来源：http://zq.shxzskj.cn

[T52] Scala：变量
来源：http://xm.shtwfgs.cn

val a = 1;  var b = 2
来源：http://ni.nicolike.cn

[T53] Scala：字符串插值
来源：http://hh.huanxung.cn

s"值: $b"
来源：http://cz.szsharing.cn

[T54] Scala：集合映射
来源：http://zs.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://bp.521024.cn

[T55] Scala：集合过滤
来源：http://kd.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zu.hahajie.cn

[T56] Scala：样例类
来源：http://av.szxytkj.cn

case class User(name: String, age: Int)
来源：http://xl.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://yr.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://el.huixiangedu.cn

[T58] Scala：函数定义
来源：http://bs.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oz.bjjhwx.cn

[T59] Scala：循环
来源：http://tq.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://cr.nszjky.cn

[T60] Scala：折叠
来源：http://jk.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ia.huanxung.cn

================================================================================
来源：http://ys.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://my.szsharing.cn

================================================================================
来源：http://se.asd995.cn

[U01] Py：创建虚拟环境
来源：http://yu.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nv.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://up.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://so.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://py.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jc.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://pm.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://so.9csxet.cn

[U05] Py：列表去重且保序
来源：http://dx.asd995.cn

list(dict.fromkeys(arr))
来源：http://gs.nszjky.cn

[U06] Py：合并两个字典
来源：http://od.shxzukj.cn

{**a, **b}
来源：http://gi.panjiajie.cn

[U07] Py：反转字典键值
来源：http://td.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://ul.asd995.cn

[U08] Py：展平二维列表
来源：http://zu.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://rv.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://rq.521024.cn

max(d, key=d.get)
来源：http://ox.shxzskj.cn

[U10] Py：按值排序字典
来源：http://cj.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://np.szsharing.cn

[U11] Py：生成器表达式
来源：http://hq.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://qp.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hw.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://vn.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://az.bjjhwx.cn

deque(maxlen=10)
来源：http://he.newstarts.cn

[U14] Py：分组收集到列表
来源：http://mq.szxytkj.cn

defaultdict(list)
来源：http://wh.colortex.cn

[U15] Py：高精度计时
来源：http://kf.huixiangedu.cn

t = time.perf_counter()
来源：http://sx.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://bw.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lr.panjiajie.cn

[U17] Py：初始化日志
来源：http://jj.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ea.asd995.cn

[U18] Py：预编译正则
来源：http://ra.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://nf.521024.cn

[U19] Py：正则替换带回调
来源：http://fs.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bp.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://sr.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://gy.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://ux.chemitech.net.cn

@contextlib.contextmanager
来源：http://ho.nszjky.cn

[U22] Py：矩阵转置
来源：http://mg.newstarts.cn

list(zip(*m))
来源：http://pi.521024.cn

[U23] Py：分块读取大文件
来源：http://dw.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lp.9csxet.cn

[U24] Py：路径操作
来源：http://be.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tb.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://ja.huanxung.cn

csv.DictReader(f)
来源：http://yr.9csxet.cn

[U26] Py：并发下载
来源：http://ce.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://je.newstarts.cn

[U27] Py：异步 HTTP
来源：http://ah.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://mz.bjjhwx.cn

[U28] Py：类型别名
来源：http://ru.jctech888.com.cn

UserId = int
来源：http://ya.colortex.cn

[U29] Py：属性校验
来源：http://wg.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://ju.9csxet.cn

[U30] Py：数据类
来源：http://xz.colortex.cn

@dataclass(slots=True)
来源：http://if.lnxyls.cn

[U31] Py：单测
来源：http://rt.shxzskj.cn

python -m pytest -q
来源：http://bi.bjjhwx.cn

[U32] Py：代码格式化
来源：http://rt.nicolike.cn

ruff format . && ruff check --fix .
来源：http://bf.szxytkj.cn

[U33] Py：打包发布
来源：http://lu.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://mm.hahajie.cn

[U34] Py：判断编码
来源：http://tg.asd995.cn

chardet.detect(raw)
来源：http://hs.wgjwhj.cn

[U35] Py：发送邮件
来源：http://ij.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xy.muxihuayi.cn

[U36] Py：定时任务
来源：http://dl.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://gh.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://st.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qc.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ky.521024.cn

Path(__file__).resolve().parent
来源：http://zf.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://ws.bookmarksfly.cn

sys.stdout.isatty()
来源：http://uh.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://zj.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://te.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://at.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rq.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://xp.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ll.nszjky.cn

[U43] PHP：声明命名空间
来源：http://sr.haigaiapp.cn

namespace App\Http;
来源：http://jl.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://xe.9csxet.cn

declare(strict_types=1);
来源：http://gy.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://qk.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wr.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://il.9csxet.cn

?string $name = null
来源：http://dr.wgjwhj.cn

[U47] PHP：联合类型
来源：http://tm.chemitech.net.cn

int|string $id
来源：http://hb.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://hm.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pa.bjjhwx.cn

[U49] PHP：只读属性
来源：http://gf.asd995.cn

public readonly string $name
来源：http://ab.colortex.cn

[U50] PHP：构造器属性提升
来源：http://zt.panjiajie.cn

public function __construct(private int $id) {}
来源：http://zc.nicolike.cn

[U51] PHP：数组解构
来源：http://td.521024.cn

[$a, $b] = $arr;
来源：http://aw.nicolike.cn

[U52] PHP：箭头函数
来源：http://oh.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://hl.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ca.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://vq.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://sp.shxzskj.cn

$obj?->method()
来源：http://oh.shxzukj.cn

[U55] PHP：match 表达式
来源：http://ix.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qe.jctech888.com.cn

[U56] PHP：命名参数
来源：http://ig.jctech888.com.cn

f(a: 1, b: 2)
来源：http://uu.hnjuh.cn

[U57] PHP：字符串插值
来源：http://lk.shxzskj.cn

"值: {$a}"
来源：http://dw.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ye.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cc.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://kw.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ld.asd995.cn

[U60] PHP：JSON 编解码
来源：http://nl.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ql.haigaiapp.cn

[U61] PHP：正则
来源：http://xq.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dv.newstarts.cn

[U62] PHP：日期对象
来源：http://aq.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://my.huanxung.cn

[U63] PHP：文件读写
来源：http://ar.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://is.hahajie.cn

[U64] PHP：目录遍历
来源：http://xo.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://zi.panjiajie.cn

[U65] PHP：会话
来源：http://hw.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mi.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://gj.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vg.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://lb.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mn.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://jl.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hb.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://xw.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pq.szsharing.cn

[U70] PHP：PDO 事务
来源：http://kh.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aq.9csxet.cn

[U71] PHP：抛出异常
来源：http://dy.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://gs.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://zk.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://ht.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://nh.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://tz.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://ty.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ry.hahajie.cn

[U75] PHP：依赖注入
来源：http://zk.jianghongdianzi.cn

composer require psr/container
来源：http://xf.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://wo.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dp.szxytkj.cn

[U77] PHP：模板渲染
来源：http://bs.jctech888.com.cn

composer require twig/twig
来源：http://bp.haigaiapp.cn

[U78] PHP：单元测试
来源：http://vs.521024.cn

composer require --dev phpunit/phpunit
来源：http://kz.hnjuh.cn

[U79] PHP：静态分析
来源：http://ok.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://lc.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://hp.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mn.szsharing.cn

[U81] JS：初始化项目
来源：http://ly.wgjwhj.cn

npm init -y;  npm i express
来源：http://kd.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://jf.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yg.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://pw.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ec.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://cf.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cx.szsharing.cn

[U85] JS：可选链
来源：http://hw.shxzukj.cn

a?.b?.c
来源：http://nd.yuexingan06.cn

[U86] JS：空值合并
来源：http://lb.huixinmuqiang.cn

a ?? b
来源：http://hz.nszjky.cn

[U87] JS：解构默认值
来源：http://qk.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://yr.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://qw.jianghongdianzi.cn

{ ...a, ...b }
来源：http://ab.521024.cn

[U89] JS：数组去重
来源：http://ye.nicolike.cn

[...new Set(arr)]
来源：http://sp.521024.cn

[U90] JS：数字数组排序
来源：http://qw.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://se.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://vz.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jp.yuexingan06.cn

[U92] JS：深拷贝
来源：http://sl.huixinmuqiang.cn

structuredClone(obj)
来源：http://gq.muxihuayi.cn

[U93] JS：模板字符串
来源：http://tn.wgjwhj.cn

`共 ${n} 条`
来源：http://sg.jctech888.com.cn

[U94] JS：箭头函数
来源：http://qz.shxzukj.cn

const double = x => x * 2;
来源：http://zf.hahajie.cn

[U95] JS：Promise 包装
来源：http://nz.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://tk.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://xa.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ex.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://nk.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://pm.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zx.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://ab.nicolike.cn

el.addEventListener("click", e => {})
来源：http://tq.shxzukj.cn

[U100] JS：DOM 查询
来源：http://xc.colortex.cn

document.querySelector(".item")
来源：http://pk.asd995.cn

[U101] JS：classList 操作
来源：http://hh.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://dk.lnxyls.cn

[U102] JS：本地存储
来源：http://up.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pt.gzmigu.cn

[U103] JS：定时器
来源：http://rb.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zg.colortex.cn

[U104] JS：防抖
来源：http://mh.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uv.huixiangedu.cn

[U105] JS：节流
来源：http://pw.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fw.lnxyls.cn

[U106] JS：日期格式化
来源：http://yr.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ju.yuexingan06.cn

[U107] JS：数字千分位
来源：http://ac.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rr.szsharing.cn

[U108] JS：随机整数
来源：http://yd.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yy.newstarts.cn

[U109] JS：数组分组
来源：http://xp.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://pc.colortex.cn

[U110] JS：数组分块
来源：http://vz.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ci.newstarts.cn

[U111] JS：对象转 Map
来源：http://jv.huanxung.cn

new Map(Object.entries(obj))
来源：http://co.nszjky.cn

[U112] JS：字符串补位
来源：http://eo.huixiangedu.cn

"7".padStart(3, "0")
来源：http://bt.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://kd.hnjuh.cn

s.replaceAll("a", "b")
来源：http://vi.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://rh.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ad.huanxung.cn

[U115] JS：生成 UUID
来源：http://vf.shxzskj.cn

crypto.randomUUID()
来源：http://gv.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://gj.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://bq.shxzukj.cn

[U117] JS：单元测试
来源：http://ig.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://kw.asd995.cn

[U118] JS：开发服务器
来源：http://gv.shxzskj.cn

npm i -D vite;  npx vite
来源：http://aq.szxytkj.cn

[U119] JS：生产构建
来源：http://rx.huixinmuqiang.cn

npx vite build
来源：http://gx.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://xa.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://fy.bookmarksfly.cn

================================================================================
来源：http://rk.521024.cn

统计汇总
来源：http://oi.panjiajie.cn

================================================================================
来源：http://se.jctech888.com.cn

按语言统计（条）：
来源：http://th.gzmigu.cn

Python ......... 252
来源：http://kn.panjiajie.cn

PHP ............ 252
来源：http://vm.shxzskj.cn

JavaScript ..... 252
来源：http://hm.haigaiapp.cn

TypeScript ..... 212
来源：http://sw.jianghongdianzi.cn


<!-- 参考信息 -->