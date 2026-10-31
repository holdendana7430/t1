代发 wailian999

[T35] Lua：字典表
来源：http://ph.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://wa.huanxung.cn

[T36] Lua：函数
来源：http://xf.jctech888.com.cn

function add(a, b) return a + b end
来源：http://wk.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://fk.szxytkj.cn

"a" .. "b"
来源：http://yd.shxzskj.cn

[T38] Lua：条件
来源：http://lm.shxzskj.cn

if x > 0 then print("正") end
来源：http://ck.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://on.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://dt.9csxet.cn

[T40] Lua：元表
来源：http://jp.hahajie.cn

setmetatable({}, { __index = base })
来源：http://so.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://gy.nicolike.cn

print "Hello\n";
来源：http://oe.shtwfgs.cn

[T42] Perl：变量类型
来源：http://wp.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nk.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://wi.gzmigu.cn

"值: $a"
来源：http://ul.huixiangedu.cn

[T44] Perl：条件
来源：http://da.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://dg.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://ve.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://ba.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://in.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://di.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://uq.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pm.wgjwhj.cn

[T48] Perl：正则替换
来源：http://eh.521024.cn

$s =~ s/old/new/g;
来源：http://bf.szsharing.cn

[T49] Perl：函数
来源：http://qf.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wq.nicolike.cn

[T50] Perl：逐行读文件
来源：http://st.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qo.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://nf.yuexingan06.cn

[T51] Scala：Hello World
来源：http://sm.muxihuayi.cn

println("Hello")
来源：http://xb.521024.cn

[T52] Scala：变量
来源：http://hh.huanxung.cn

val a = 1;  var b = 2
来源：http://kx.nszjky.cn

[T53] Scala：字符串插值
来源：http://ce.huixiangedu.cn

s"值: $b"
来源：http://vw.szxytkj.cn

[T54] Scala：集合映射
来源：http://az.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://mx.huanxung.cn

[T55] Scala：集合过滤
来源：http://do.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ap.shxzskj.cn

[T56] Scala：样例类
来源：http://oc.521024.cn

case class User(name: String, age: Int)
来源：http://eq.hnjuh.cn

[T57] Scala：模式匹配
来源：http://mk.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sp.shxzukj.cn

[T58] Scala：函数定义
来源：http://wo.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xk.huanxung.cn

[T59] Scala：循环
来源：http://uw.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://qu.521024.cn

[T60] Scala：折叠
来源：http://wr.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chemitech.net.cn

================================================================================
来源：http://vs.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fn.panjiajie.cn

================================================================================
来源：http://mf.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://si.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wd.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://gw.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yt.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://dw.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dr.shxzskj.cn

[U04] Py：变量调试打印
来源：http://kb.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ij.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://xi.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://qk.lnxyls.cn

[U06] Py：合并两个字典
来源：http://xt.haigaiapp.cn

{**a, **b}
来源：http://st.szxytkj.cn

[U07] Py：反转字典键值
来源：http://uu.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://nj.panjiajie.cn

[U08] Py：展平二维列表
来源：http://sr.huanxung.cn

[y for x in nested for y in x]
来源：http://iz.asd995.cn

[U09] Py：字典取最大值的键
来源：http://pg.szsharing.cn

max(d, key=d.get)
来源：http://ty.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://et.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gl.lnxyls.cn

[U11] Py：生成器表达式
来源：http://sd.yuexingan06.cn

(x * 2 for x in arr)
来源：http://ix.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sw.gzmigu.cn

Counter(arr).most_common(3)
来源：http://fb.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://fw.hnjuh.cn

deque(maxlen=10)
来源：http://bp.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://ny.newstarts.cn

defaultdict(list)
来源：http://cl.panjiajie.cn

[U15] Py：高精度计时
来源：http://xm.haigaiapp.cn

t = time.perf_counter()
来源：http://vw.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://nl.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ed.nszjky.cn

[U17] Py：初始化日志
来源：http://ws.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://wj.szsharing.cn

[U18] Py：预编译正则
来源：http://kf.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://vi.szsharing.cn

[U19] Py：正则替换带回调
来源：http://co.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gj.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://jh.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://yl.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://rh.nszjky.cn

@contextlib.contextmanager
来源：http://oi.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://wy.chemitech.net.cn

list(zip(*m))
来源：http://ix.szsharing.cn

[U23] Py：分块读取大文件
来源：http://lj.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://an.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ez.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qa.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://az.9csxet.cn

csv.DictReader(f)
来源：http://ts.huanxung.cn

[U26] Py：并发下载
来源：http://pp.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ff.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ab.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://hm.panjiajie.cn

[U28] Py：类型别名
来源：http://yz.yuntaijiaju.cn

UserId = int
来源：http://lf.jctech888.com.cn

[U29] Py：属性校验
来源：http://lm.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://qo.shxzskj.cn

[U30] Py：数据类
来源：http://ed.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://aw.shxzukj.cn

[U31] Py：单测
来源：http://wd.nszjky.cn

python -m pytest -q
来源：http://pg.panjiajie.cn

[U32] Py：代码格式化
来源：http://wd.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://hq.shxzukj.cn

[U33] Py：打包发布
来源：http://bk.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://ef.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://lj.shxzskj.cn

chardet.detect(raw)
来源：http://ym.wgjwhj.cn

[U35] Py：发送邮件
来源：http://ej.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mj.bookmarksfly.cn

[U36] Py：定时任务
来源：http://wo.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://iz.hahajie.cn

[U37] Py：读写 Excel
来源：http://fa.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nw.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://wa.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://zc.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://rr.nszjky.cn

sys.stdout.isatty()
来源：http://ix.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://xj.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://wx.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://bm.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ox.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://uy.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ow.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://zz.newstarts.cn

namespace App\Http;
来源：http://eo.colortex.cn

[U44] PHP：开启严格类型
来源：http://ic.hahajie.cn

declare(strict_types=1);
来源：http://it.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://jd.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aa.bjjhwx.cn

[U46] PHP：可空类型
来源：http://ma.colortex.cn

?string $name = null
来源：http://xx.nicolike.cn

[U47] PHP：联合类型
来源：http://az.hahajie.cn

int|string $id
来源：http://kp.nszjky.cn

[U48] PHP：纯枚举
来源：http://yp.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mu.wgjwhj.cn

[U49] PHP：只读属性
来源：http://qw.521024.cn

public readonly string $name
来源：http://nh.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://hx.colortex.cn

public function __construct(private int $id) {}
来源：http://cu.yuexingan06.cn

[U51] PHP：数组解构
来源：http://mj.newstarts.cn

[$a, $b] = $arr;
来源：http://uw.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://iy.asd995.cn

$double = fn($x) => $x * 2;
来源：http://ep.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://jx.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://se.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://rj.9csxet.cn

$obj?->method()
来源：http://bd.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://lw.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://or.colortex.cn

[U56] PHP：命名参数
来源：http://uk.bjjhwx.cn

f(a: 1, b: 2)
来源：http://lo.gzmigu.cn

[U57] PHP：字符串插值
来源：http://gr.shxzskj.cn

"值: {$a}"
来源：http://zk.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://zi.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ef.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://ak.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tn.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://ke.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ii.haigaiapp.cn

[U61] PHP：正则
来源：http://vc.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uo.9csxet.cn

[U62] PHP：日期对象
来源：http://hs.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cn.asd995.cn

[U63] PHP：文件读写
来源：http://js.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nx.521024.cn

[U64] PHP：目录遍历
来源：http://ca.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://eg.shxzukj.cn

[U65] PHP：会话
来源：http://pb.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dj.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://sk.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rd.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://po.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://he.colortex.cn

[U68] PHP：PDO 连接
来源：http://zs.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fv.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://yz.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rk.asd995.cn

[U70] PHP：PDO 事务
来源：http://ip.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ht.521024.cn

[U71] PHP：抛出异常
来源：http://al.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://sj.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://th.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://lu.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://nf.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://oj.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://uw.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://le.asd995.cn

[U75] PHP：依赖注入
来源：http://js.muxihuayi.cn

composer require psr/container
来源：http://ah.newstarts.cn

[U76] PHP：简单路由
来源：http://bw.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rm.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ws.yuntaijiaju.cn

composer require twig/twig
来源：http://nn.521024.cn

[U78] PHP：单元测试
来源：http://kc.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://co.asd995.cn

[U79] PHP：静态分析
来源：http://wz.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://jm.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://zx.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ga.asd995.cn

[U81] JS：初始化项目
来源：http://pq.szxytkj.cn

npm init -y;  npm i express
来源：http://qt.nicolike.cn

[U82] JS：package.json 脚本
来源：http://mk.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lm.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://zr.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://my.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://qz.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qx.wgjwhj.cn

[U85] JS：可选链
来源：http://fb.hahajie.cn

a?.b?.c
来源：http://hq.panjiajie.cn

[U86] JS：空值合并
来源：http://uc.chemitech.net.cn

a ?? b
来源：http://hv.shxzskj.cn

[U87] JS：解构默认值
来源：http://hc.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://tk.panjiajie.cn

[U88] JS：对象展开合并
来源：http://wx.jianghongdianzi.cn

{ ...a, ...b }
来源：http://na.asd995.cn

[U89] JS：数组去重
来源：http://gu.lnxyls.cn

[...new Set(arr)]
来源：http://yu.hahajie.cn

[U90] JS：数字数组排序
来源：http://nx.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://dw.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wz.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ku.yuexingan06.cn

[U92] JS：深拷贝
来源：http://uv.lnxyls.cn

structuredClone(obj)
来源：http://zc.lnxyls.cn

[U93] JS：模板字符串
来源：http://hd.asd995.cn

`共 ${n} 条`
来源：http://ay.jctech888.com.cn

[U94] JS：箭头函数
来源：http://fs.yuexingan06.cn

const double = x => x * 2;
来源：http://eg.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ea.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ez.hahajie.cn

[U96] JS：async/await 与异常
来源：http://za.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://is.yuexingan06.cn

[U97] JS：并发请求
来源：http://rs.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xt.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://wt.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://if.haigaiapp.cn

[U99] JS：事件监听
来源：http://dd.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://tv.nicolike.cn

[U100] JS：DOM 查询
来源：http://eb.huixiangedu.cn

document.querySelector(".item")
来源：http://is.521024.cn

[U101] JS：classList 操作
来源：http://hi.gzmigu.cn

el.classList.toggle("active")
来源：http://ie.nszjky.cn

[U102] JS：本地存储
来源：http://bh.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wa.muxihuayi.cn

[U103] JS：定时器
来源：http://tc.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vx.jianghongdianzi.cn

[U104] JS：防抖
来源：http://sw.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tl.521024.cn

[U105] JS：节流
来源：http://sg.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://th.gzmigu.cn

[U106] JS：日期格式化
来源：http://rc.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nw.9csxet.cn

[U107] JS：数字千分位
来源：http://us.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vr.yuexingan06.cn

[U108] JS：随机整数
来源：http://ma.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fx.huixiangedu.cn

[U109] JS：数组分组
来源：http://vu.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://ps.wgjwhj.cn

[U110] JS：数组分块
来源：http://kq.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fx.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://km.asd995.cn

new Map(Object.entries(obj))
来源：http://nn.shxzukj.cn

[U112] JS：字符串补位
来源：http://lf.521024.cn

"7".padStart(3, "0")
来源：http://ye.nszjky.cn

[U113] JS：正则替换全部
来源：http://xj.huanxung.cn

s.replaceAll("a", "b")
来源：http://ao.hahajie.cn

[U114] JS：JSON 深比较
来源：http://xu.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aw.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://gc.yuntaijiaju.cn

crypto.randomUUID()
来源：http://zi.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ku.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://wg.gzmigu.cn

[U117] JS：单元测试
来源：http://xj.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://uz.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://za.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://oj.szsharing.cn

[U119] JS：生产构建
来源：http://ma.shtwfgs.cn

npx vite build
来源：http://rw.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://ag.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://us.yuntaijiaju.cn

================================================================================
来源：http://fx.huixiangedu.cn

统计汇总
来源：http://dm.hahajie.cn

================================================================================
来源：http://dt.huanxung.cn

按语言统计（条）：
来源：http://od.szsharing.cn


<!-- 参考信息 -->