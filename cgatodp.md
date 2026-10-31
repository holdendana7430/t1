代发 wailian999

[T35] Lua：字典表
来源：http://jr.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://mz.asd995.cn

[T36] Lua：函数
来源：http://wf.hahajie.cn

function add(a, b) return a + b end
来源：http://ow.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://be.huanxung.cn

"a" .. "b"
来源：http://bn.newstarts.cn

[T38] Lua：条件
来源：http://uk.gzmigu.cn

if x > 0 then print("正") end
来源：http://hh.asd995.cn

[T39] Lua：模式匹配
来源：http://ls.gzmigu.cn

string.find(s, "%d+")
来源：http://nn.shxzskj.cn

[T40] Lua：元表
来源：http://lf.newstarts.cn

setmetatable({}, { __index = base })
来源：http://dl.szsharing.cn

[T41] Perl：Hello World
来源：http://af.bjjhwx.cn

print "Hello\n";
来源：http://fy.szsharing.cn

[T42] Perl：变量类型
来源：http://rg.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bc.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://nk.shxzukj.cn

"值: $a"
来源：http://qa.huanxung.cn

[T44] Perl：条件
来源：http://zo.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://iz.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://jf.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://oq.colortex.cn

[T46] Perl：哈希操作
来源：http://hx.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ln.huanxung.cn

[T47] Perl：正则捕获
来源：http://rs.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lm.szxytkj.cn

[T48] Perl：正则替换
来源：http://kt.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://sy.huanxung.cn

[T49] Perl：函数
来源：http://fi.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://be.nszjky.cn

[T50] Perl：逐行读文件
来源：http://fo.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wy.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://rm.panjiajie.cn

[T51] Scala：Hello World
来源：http://dt.asd995.cn

println("Hello")
来源：http://jo.chemitech.net.cn

[T52] Scala：变量
来源：http://gx.huixiangedu.cn

val a = 1;  var b = 2
来源：http://pd.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://jr.huixinmuqiang.cn

s"值: $b"
来源：http://wd.yuexingan06.cn

[T54] Scala：集合映射
来源：http://yo.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://uv.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://po.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oi.shxzskj.cn

[T56] Scala：样例类
来源：http://iz.hahajie.cn

case class User(name: String, age: Int)
来源：http://ki.hahajie.cn

[T57] Scala：模式匹配
来源：http://ck.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fa.nicolike.cn

[T58] Scala：函数定义
来源：http://xt.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://np.hnjuh.cn

[T59] Scala：循环
来源：http://oc.521024.cn

for (i <- 1 to 10) println(i)
来源：http://ol.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://nc.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ao.nicolike.cn

================================================================================
来源：http://kh.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dn.asd995.cn

================================================================================
来源：http://hp.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://jr.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ag.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://zq.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eq.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://ic.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://re.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://dl.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yk.asd995.cn

[U05] Py：列表去重且保序
来源：http://we.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://ye.hnjuh.cn

[U06] Py：合并两个字典
来源：http://lr.szsharing.cn

{**a, **b}
来源：http://iu.colortex.cn

[U07] Py：反转字典键值
来源：http://su.hahajie.cn

{v: k for k, v in d.items()}
来源：http://wi.szxytkj.cn

[U08] Py：展平二维列表
来源：http://ks.huanxung.cn

[y for x in nested for y in x]
来源：http://gd.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://ca.haigaiapp.cn

max(d, key=d.get)
来源：http://iu.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://rx.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dg.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://bh.szsharing.cn

(x * 2 for x in arr)
来源：http://pr.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mg.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://hl.hnjuh.cn

[U13] Py：固定长度队列
来源：http://zz.jianghongdianzi.cn

deque(maxlen=10)
来源：http://gq.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://hh.yuexingan06.cn

defaultdict(list)
来源：http://rq.newstarts.cn

[U15] Py：高精度计时
来源：http://qd.newstarts.cn

t = time.perf_counter()
来源：http://we.huanxung.cn

[U16] Py：命令行参数解析
来源：http://hg.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mu.521024.cn

[U17] Py：初始化日志
来源：http://ra.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://mq.bjjhwx.cn

[U18] Py：预编译正则
来源：http://wt.9csxet.cn

pat = re.compile(r"\d+")
来源：http://dj.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://pj.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iz.nszjky.cn

[U20] Py：缓存函数结果
来源：http://xq.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://oe.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://no.jctech888.com.cn

@contextlib.contextmanager
来源：http://qp.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://du.shxzukj.cn

list(zip(*m))
来源：http://wu.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://xp.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cs.shxzskj.cn

[U24] Py：路径操作
来源：http://yd.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yn.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://gx.colortex.cn

csv.DictReader(f)
来源：http://me.huanxung.cn

[U26] Py：并发下载
来源：http://dg.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cf.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://oa.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://ia.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://jf.yuntaijiaju.cn

UserId = int
来源：http://nu.chemitech.net.cn

[U29] Py：属性校验
来源：http://oe.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://vl.shxzskj.cn

[U30] Py：数据类
来源：http://rg.panjiajie.cn

@dataclass(slots=True)
来源：http://ja.gzmigu.cn

[U31] Py：单测
来源：http://tw.hnjuh.cn

python -m pytest -q
来源：http://jf.chemitech.net.cn

[U32] Py：代码格式化
来源：http://ke.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://as.yuexingan06.cn

[U33] Py：打包发布
来源：http://sr.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://vy.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://cq.colortex.cn

chardet.detect(raw)
来源：http://vr.hnjuh.cn

[U35] Py：发送邮件
来源：http://xn.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pq.nszjky.cn

[U36] Py：定时任务
来源：http://kr.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://gt.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://az.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ki.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://ni.shxzskj.cn

Path(__file__).resolve().parent
来源：http://mt.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://dq.bookmarksfly.cn

sys.stdout.isatty()
来源：http://eg.colortex.cn

[U40] Py：打印到标准错误
来源：http://zz.nicolike.cn

print("err", file=sys.stderr)
来源：http://zp.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://un.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cr.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://or.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hv.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://jn.szxytkj.cn

namespace App\Http;
来源：http://yl.newstarts.cn

[U44] PHP：开启严格类型
来源：http://cj.gzmigu.cn

declare(strict_types=1);
来源：http://fz.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://lb.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ec.shtwfgs.cn

[U46] PHP：可空类型
来源：http://bx.bjjhwx.cn

?string $name = null
来源：http://ns.shxzskj.cn

[U47] PHP：联合类型
来源：http://ft.shxzskj.cn

int|string $id
来源：http://jz.asd995.cn

[U48] PHP：纯枚举
来源：http://gb.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cs.nszjky.cn

[U49] PHP：只读属性
来源：http://ug.jianghongdianzi.cn

public readonly string $name
来源：http://xu.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://qw.nicolike.cn

public function __construct(private int $id) {}
来源：http://zo.szxytkj.cn

[U51] PHP：数组解构
来源：http://zr.chemitech.net.cn

[$a, $b] = $arr;
来源：http://kq.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ey.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://iq.asd995.cn

[U53] PHP：空合并运算符
来源：http://pg.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://fb.szsharing.cn

[U54] PHP：空安全调用
来源：http://xv.colortex.cn

$obj?->method()
来源：http://ny.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://iu.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xr.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://hg.panjiajie.cn

f(a: 1, b: 2)
来源：http://ve.colortex.cn

[U57] PHP：字符串插值
来源：http://hh.lnxyls.cn

"值: {$a}"
来源：http://ky.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://xv.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gv.hnjuh.cn

[U59] PHP：自定义排序
来源：http://lf.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gz.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://jb.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xd.wgjwhj.cn

[U61] PHP：正则
来源：http://mo.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uh.shxzukj.cn

[U62] PHP：日期对象
来源：http://kw.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yn.haigaiapp.cn

[U63] PHP：文件读写
来源：http://jl.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fn.shxzukj.cn

[U64] PHP：目录遍历
来源：http://yv.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://sg.muxihuayi.cn

[U65] PHP：会话
来源：http://by.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cr.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://kx.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fa.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://dz.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jq.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://fg.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xy.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://qo.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vk.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://zx.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qs.shxzukj.cn

[U71] PHP：抛出异常
来源：http://wg.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ga.nszjky.cn

[U72] PHP：写错误日志
来源：http://td.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://qi.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://rw.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://xc.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://ow.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://ib.szxytkj.cn

[U75] PHP：依赖注入
来源：http://st.bjjhwx.cn

composer require psr/container
来源：http://lp.szxytkj.cn

[U76] PHP：简单路由
来源：http://kt.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mz.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://hi.huixinmuqiang.cn

composer require twig/twig
来源：http://is.haigaiapp.cn

[U78] PHP：单元测试
来源：http://yi.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://sq.hahajie.cn

[U79] PHP：静态分析
来源：http://hg.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://mk.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://yq.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ml.muxihuayi.cn

[U81] JS：初始化项目
来源：http://jp.szsharing.cn

npm init -y;  npm i express
来源：http://ue.hahajie.cn

[U82] JS：package.json 脚本
来源：http://eq.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://it.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://yt.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rc.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://vv.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bg.jctech888.com.cn

[U85] JS：可选链
来源：http://zs.haigaiapp.cn

a?.b?.c
来源：http://dt.bjjhwx.cn

[U86] JS：空值合并
来源：http://sy.panjiajie.cn

a ?? b
来源：http://lw.jctech888.com.cn

[U87] JS：解构默认值
来源：http://zi.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://sw.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://aj.muxihuayi.cn

{ ...a, ...b }
来源：http://fq.nicolike.cn

[U89] JS：数组去重
来源：http://hu.yuntaijiaju.cn

[...new Set(arr)]
来源：http://vo.colortex.cn

[U90] JS：数字数组排序
来源：http://jc.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://sa.521024.cn

[U91] JS：对象键值遍历
来源：http://wr.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ko.jctech888.com.cn

[U92] JS：深拷贝
来源：http://ju.nicolike.cn

structuredClone(obj)
来源：http://ms.hahajie.cn

[U93] JS：模板字符串
来源：http://vc.shxzskj.cn

`共 ${n} 条`
来源：http://bf.lnxyls.cn

[U94] JS：箭头函数
来源：http://hm.jctech888.com.cn

const double = x => x * 2;
来源：http://qc.newstarts.cn

[U95] JS：Promise 包装
来源：http://jo.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://kf.huanxung.cn

[U96] JS：async/await 与异常
来源：http://is.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jy.asd995.cn

[U97] JS：并发请求
来源：http://ab.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://em.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://vf.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://el.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://as.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://wf.szxytkj.cn

[U100] JS：DOM 查询
来源：http://ev.wgjwhj.cn

document.querySelector(".item")
来源：http://yx.hnjuh.cn

[U101] JS：classList 操作
来源：http://pw.nicolike.cn

el.classList.toggle("active")
来源：http://kp.shtwfgs.cn

[U102] JS：本地存储
来源：http://tf.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zw.szsharing.cn

[U103] JS：定时器
来源：http://uy.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nh.muxihuayi.cn

[U104] JS：防抖
来源：http://ng.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jp.szsharing.cn

[U105] JS：节流
来源：http://wx.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wg.gzmigu.cn

[U106] JS：日期格式化
来源：http://vt.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uh.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://qm.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://do.hahajie.cn

[U108] JS：随机整数
来源：http://rq.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zi.jctech888.com.cn

[U109] JS：数组分组
来源：http://mn.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://ns.hahajie.cn

[U110] JS：数组分块
来源：http://uq.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mv.nicolike.cn

[U111] JS：对象转 Map
来源：http://ry.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://zj.hahajie.cn

[U112] JS：字符串补位
来源：http://cq.yuexingan06.cn

"7".padStart(3, "0")
来源：http://al.shxzskj.cn

[U113] JS：正则替换全部
来源：http://ag.shxzskj.cn

s.replaceAll("a", "b")
来源：http://sb.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://rx.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kt.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://db.shxzukj.cn

crypto.randomUUID()
来源：http://yt.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://wz.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://km.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://bj.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://rg.hahajie.cn

[U118] JS：开发服务器
来源：http://gq.nszjky.cn

npm i -D vite;  npx vite
来源：http://ak.nicolike.cn

[U119] JS：生产构建
来源：http://qt.shtwfgs.cn

npx vite build
来源：http://ht.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://fx.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://bb.nszjky.cn

================================================================================
来源：http://db.yuntaijiaju.cn

统计汇总
来源：http://nk.shxzukj.cn

================================================================================
来源：http://dk.huixiangedu.cn

按语言统计（条）：
来源：http://gj.asd995.cn


<!-- 参考信息 -->