代发 wailian999

[T39] Lua：模式匹配
来源：http://qv.jctech888.com.cn

string.find(s, "%d+")
来源：http://gm.muxihuayi.cn

[T40] Lua：元表
来源：http://au.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://ml.nicolike.cn

[T41] Perl：Hello World
来源：http://kc.hahajie.cn

print "Hello\n";
来源：http://kl.newstarts.cn

[T42] Perl：变量类型
来源：http://ql.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://du.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://ln.huixinmuqiang.cn

"值: $a"
来源：http://qa.szxytkj.cn

[T44] Perl：条件
来源：http://ni.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://bg.newstarts.cn

[T45] Perl：数组遍历
来源：http://du.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://zt.9csxet.cn

[T46] Perl：哈希操作
来源：http://hy.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aj.panjiajie.cn

[T47] Perl：正则捕获
来源：http://hx.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kt.shxzskj.cn

[T48] Perl：正则替换
来源：http://pf.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://vu.szxytkj.cn

[T49] Perl：函数
来源：http://of.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hs.colortex.cn

[T50] Perl：逐行读文件
来源：http://uv.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://td.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://cb.hnjuh.cn

[T51] Scala：Hello World
来源：http://nk.haigaiapp.cn

println("Hello")
来源：http://ij.bookmarksfly.cn

[T52] Scala：变量
来源：http://ar.shxzskj.cn

val a = 1;  var b = 2
来源：http://te.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://li.hahajie.cn

s"值: $b"
来源：http://ph.nszjky.cn

[T54] Scala：集合映射
来源：http://oe.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ze.panjiajie.cn

[T55] Scala：集合过滤
来源：http://xk.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qp.shxzukj.cn

[T56] Scala：样例类
来源：http://te.shxzukj.cn

case class User(name: String, age: Int)
来源：http://wd.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://ep.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rg.hahajie.cn

[T58] Scala：函数定义
来源：http://of.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ha.huixiangedu.cn

[T59] Scala：循环
来源：http://rg.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://kx.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://jm.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wn.hahajie.cn

================================================================================
来源：http://od.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oy.hnjuh.cn

================================================================================
来源：http://ov.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://hc.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bi.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://hk.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ja.colortex.cn

[U03] Py：加载 .env 配置
来源：http://xo.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eq.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://cw.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gi.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://mk.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://rn.nszjky.cn

[U06] Py：合并两个字典
来源：http://qm.yuexingan06.cn

{**a, **b}
来源：http://ns.newstarts.cn

[U07] Py：反转字典键值
来源：http://ik.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://qu.panjiajie.cn

[U08] Py：展平二维列表
来源：http://bu.colortex.cn

[y for x in nested for y in x]
来源：http://ta.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://bv.shxzukj.cn

max(d, key=d.get)
来源：http://ty.huanxung.cn

[U10] Py：按值排序字典
来源：http://hq.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qu.asd995.cn

[U11] Py：生成器表达式
来源：http://ts.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://dw.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dj.colortex.cn

Counter(arr).most_common(3)
来源：http://yy.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://xz.hnjuh.cn

deque(maxlen=10)
来源：http://qv.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://tc.newstarts.cn

defaultdict(list)
来源：http://da.szsharing.cn

[U15] Py：高精度计时
来源：http://ln.yuntaijiaju.cn

t = time.perf_counter()
来源：http://op.huanxung.cn

[U16] Py：命令行参数解析
来源：http://jf.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qh.bjjhwx.cn

[U17] Py：初始化日志
来源：http://lv.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://oq.bjjhwx.cn

[U18] Py：预编译正则
来源：http://yy.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://qi.521024.cn

[U19] Py：正则替换带回调
来源：http://yu.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qo.huanxung.cn

[U20] Py：缓存函数结果
来源：http://fp.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://sc.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://re.huanxung.cn

@contextlib.contextmanager
来源：http://es.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://nm.huixiangedu.cn

list(zip(*m))
来源：http://xk.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://lw.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ub.haigaiapp.cn

[U24] Py：路径操作
来源：http://of.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://it.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://gj.shxzskj.cn

csv.DictReader(f)
来源：http://qk.hnjuh.cn

[U26] Py：并发下载
来源：http://kl.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ip.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://pi.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://fi.gzmigu.cn

[U28] Py：类型别名
来源：http://ff.chemitech.net.cn

UserId = int
来源：http://jb.wgjwhj.cn

[U29] Py：属性校验
来源：http://sp.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://bg.shxzskj.cn

[U30] Py：数据类
来源：http://bb.shtwfgs.cn

@dataclass(slots=True)
来源：http://qc.szsharing.cn

[U31] Py：单测
来源：http://af.bjjhwx.cn

python -m pytest -q
来源：http://er.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://mu.szsharing.cn

ruff format . && ruff check --fix .
来源：http://tq.shxzukj.cn

[U33] Py：打包发布
来源：http://vr.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://ip.jctech888.com.cn

[U34] Py：判断编码
来源：http://ad.muxihuayi.cn

chardet.detect(raw)
来源：http://ky.wgjwhj.cn

[U35] Py：发送邮件
来源：http://vk.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rc.chemitech.net.cn

[U36] Py：定时任务
来源：http://wj.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://is.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ha.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zj.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://yv.nicolike.cn

Path(__file__).resolve().parent
来源：http://yi.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://hs.shxzukj.cn

sys.stdout.isatty()
来源：http://vv.newstarts.cn

[U40] Py：打印到标准错误
来源：http://yo.shxzukj.cn

print("err", file=sys.stderr)
来源：http://zk.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://hb.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zw.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://jo.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ds.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://dg.haigaiapp.cn

namespace App\Http;
来源：http://ko.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://pz.newstarts.cn

declare(strict_types=1);
来源：http://ns.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://qt.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xa.9csxet.cn

[U46] PHP：可空类型
来源：http://et.panjiajie.cn

?string $name = null
来源：http://sq.jctech888.com.cn

[U47] PHP：联合类型
来源：http://ml.521024.cn

int|string $id
来源：http://rj.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://pq.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ky.chemitech.net.cn

[U49] PHP：只读属性
来源：http://kd.hnjuh.cn

public readonly string $name
来源：http://wa.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://gq.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://jh.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://rd.newstarts.cn

[$a, $b] = $arr;
来源：http://uj.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ue.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://hj.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://dx.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://ns.szsharing.cn

[U54] PHP：空安全调用
来源：http://bv.chemitech.net.cn

$obj?->method()
来源：http://qs.shxzukj.cn

[U55] PHP：match 表达式
来源：http://wr.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zi.hnjuh.cn

[U56] PHP：命名参数
来源：http://ab.wgjwhj.cn

f(a: 1, b: 2)
来源：http://zz.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://fb.nszjky.cn

"值: {$a}"
来源：http://mm.nszjky.cn

[U58] PHP：数组三件套
来源：http://gr.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hs.panjiajie.cn

[U59] PHP：自定义排序
来源：http://ty.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://us.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://yd.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ri.panjiajie.cn

[U61] PHP：正则
来源：http://tk.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wm.szsharing.cn

[U62] PHP：日期对象
来源：http://tx.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zj.521024.cn

[U63] PHP：文件读写
来源：http://uz.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bu.lnxyls.cn

[U64] PHP：目录遍历
来源：http://xg.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://tx.yuntaijiaju.cn

[U65] PHP：会话
来源：http://ya.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sb.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://kh.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qf.nicolike.cn

[U67] PHP：处理文件上传
来源：http://ma.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wq.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://wk.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jz.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://tj.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zp.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://yt.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xf.szxytkj.cn

[U71] PHP：抛出异常
来源：http://ne.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://kd.521024.cn

[U72] PHP：写错误日志
来源：http://sm.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://wg.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://ll.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://jv.newstarts.cn

[U74] PHP：读取环境变量
来源：http://tg.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://nj.521024.cn

[U75] PHP：依赖注入
来源：http://bq.nicolike.cn

composer require psr/container
来源：http://uk.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://uq.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eu.hahajie.cn

[U77] PHP：模板渲染
来源：http://um.bookmarksfly.cn

composer require twig/twig
来源：http://wc.asd995.cn

[U78] PHP：单元测试
来源：http://xc.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://yw.gzmigu.cn

[U79] PHP：静态分析
来源：http://fg.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://jn.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://dc.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mb.panjiajie.cn

[U81] JS：初始化项目
来源：http://hq.hnjuh.cn

npm init -y;  npm i express
来源：http://qa.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://mw.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iw.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://zn.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xr.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://as.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dz.szxytkj.cn

[U85] JS：可选链
来源：http://sa.shxzukj.cn

a?.b?.c
来源：http://qd.huixiangedu.cn

[U86] JS：空值合并
来源：http://pi.shtwfgs.cn

a ?? b
来源：http://ra.bjjhwx.cn

[U87] JS：解构默认值
来源：http://kz.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://nr.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://bi.lnxyls.cn

{ ...a, ...b }
来源：http://pa.huanxung.cn

[U89] JS：数组去重
来源：http://zq.yuntaijiaju.cn

[...new Set(arr)]
来源：http://if.9csxet.cn

[U90] JS：数字数组排序
来源：http://th.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://kp.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://to.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uj.shxzukj.cn

[U92] JS：深拷贝
来源：http://bo.wgjwhj.cn

structuredClone(obj)
来源：http://la.wgjwhj.cn

[U93] JS：模板字符串
来源：http://zo.huanxung.cn

`共 ${n} 条`
来源：http://hv.szsharing.cn

[U94] JS：箭头函数
来源：http://lk.521024.cn

const double = x => x * 2;
来源：http://kr.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://zd.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://ki.huanxung.cn

[U96] JS：async/await 与异常
来源：http://bk.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lw.shxzukj.cn

[U97] JS：并发请求
来源：http://ga.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vr.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ev.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lp.hnjuh.cn

[U99] JS：事件监听
来源：http://sd.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://py.521024.cn

[U100] JS：DOM 查询
来源：http://dh.chemitech.net.cn

document.querySelector(".item")
来源：http://ed.panjiajie.cn

[U101] JS：classList 操作
来源：http://ky.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://ij.szxytkj.cn

[U102] JS：本地存储
来源：http://gp.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vi.colortex.cn

[U103] JS：定时器
来源：http://wg.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://et.szsharing.cn

[U104] JS：防抖
来源：http://wa.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rj.shxzukj.cn

[U105] JS：节流
来源：http://ys.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://np.colortex.cn

[U106] JS：日期格式化
来源：http://bk.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://if.hnjuh.cn

[U107] JS：数字千分位
来源：http://hc.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pf.bjjhwx.cn

[U108] JS：随机整数
来源：http://fy.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ln.asd995.cn

[U109] JS：数组分组
来源：http://wl.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://gb.huixiangedu.cn

[U110] JS：数组分块
来源：http://tm.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mr.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://lp.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ej.521024.cn

[U112] JS：字符串补位
来源：http://jj.szsharing.cn

"7".padStart(3, "0")
来源：http://ts.hahajie.cn

[U113] JS：正则替换全部
来源：http://yl.newstarts.cn

s.replaceAll("a", "b")
来源：http://rk.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://gm.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gw.521024.cn

[U115] JS：生成 UUID
来源：http://dg.newstarts.cn

crypto.randomUUID()
来源：http://ir.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://zj.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://wr.gzmigu.cn

[U117] JS：单元测试
来源：http://sz.colortex.cn

npm i -D vitest;  npx vitest
来源：http://jo.panjiajie.cn

[U118] JS：开发服务器
来源：http://cf.asd995.cn

npm i -D vite;  npx vite
来源：http://ra.huixiangedu.cn

[U119] JS：生产构建
来源：http://xk.nicolike.cn

npx vite build
来源：http://er.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://rs.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://ev.nszjky.cn

================================================================================
来源：http://ub.bjjhwx.cn

统计汇总
来源：http://yv.gzmigu.cn

================================================================================
来源：http://jo.shxzukj.cn

按语言统计（条）：
来源：http://lf.bjjhwx.cn

Python ......... 252
来源：http://md.hnjuh.cn

PHP ............ 252
来源：http://sn.shtwfgs.cn

JavaScript ..... 252
来源：http://vm.nicolike.cn

TypeScript ..... 212
来源：http://cx.muxihuayi.cn

Java ........... 212
来源：http://yf.shtwfgs.cn

Go ............. 212
来源：http://bg.jctech888.com.cn

Ruby ........... 212
来源：http://kx.colortex.cn

C# ............. 212
来源：http://bs.huanxung.cn


<!-- 参考信息 -->