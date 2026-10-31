代发 wailian999

[T33] Lua：表（数组）
来源：http://kp.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nd.lnxyls.cn

[T34] Lua：遍历表
来源：http://bc.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ju.shxzukj.cn

[T35] Lua：字典表
来源：http://hh.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://qp.hnjuh.cn

[T36] Lua：函数
来源：http://rn.nicolike.cn

function add(a, b) return a + b end
来源：http://uk.colortex.cn

[T37] Lua：字符串拼接
来源：http://pj.9csxet.cn

"a" .. "b"
来源：http://ib.9csxet.cn

[T38] Lua：条件
来源：http://wb.huanxung.cn

if x > 0 then print("正") end
来源：http://vt.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://vs.panjiajie.cn

string.find(s, "%d+")
来源：http://br.hnjuh.cn

[T40] Lua：元表
来源：http://gr.521024.cn

setmetatable({}, { __index = base })
来源：http://av.szsharing.cn

[T41] Perl：Hello World
来源：http://mv.haigaiapp.cn

print "Hello\n";
来源：http://np.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://za.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pk.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://rb.haigaiapp.cn

"值: $a"
来源：http://qw.jianghongdianzi.cn

[T44] Perl：条件
来源：http://jt.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ve.lnxyls.cn

[T45] Perl：数组遍历
来源：http://cg.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ss.nszjky.cn

[T46] Perl：哈希操作
来源：http://za.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fo.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://ht.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ch.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://sq.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://dg.huanxung.cn

[T49] Perl：函数
来源：http://ok.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yl.nicolike.cn

[T50] Perl：逐行读文件
来源：http://up.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bu.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://sd.jctech888.com.cn

[T51] Scala：Hello World
来源：http://tl.huixiangedu.cn

println("Hello")
来源：http://em.9csxet.cn

[T52] Scala：变量
来源：http://qa.newstarts.cn

val a = 1;  var b = 2
来源：http://fu.lnxyls.cn

[T53] Scala：字符串插值
来源：http://ka.hahajie.cn

s"值: $b"
来源：http://jw.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://en.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://rr.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ha.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ik.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://ob.colortex.cn

case class User(name: String, age: Int)
来源：http://qr.lnxyls.cn

[T57] Scala：模式匹配
来源：http://iv.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xc.shxzukj.cn

[T58] Scala：函数定义
来源：http://ww.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dx.yuntaijiaju.cn

[T59] Scala：循环
来源：http://oq.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://mo.panjiajie.cn

[T60] Scala：折叠
来源：http://rc.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gy.bjjhwx.cn

================================================================================
来源：http://bv.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tz.szsharing.cn

================================================================================
来源：http://xb.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://ef.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kz.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://jy.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zj.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://yu.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bg.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://ds.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yc.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://rc.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://as.9csxet.cn

[U06] Py：合并两个字典
来源：http://qv.newstarts.cn

{**a, **b}
来源：http://pd.nicolike.cn

[U07] Py：反转字典键值
来源：http://qr.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://vo.9csxet.cn

[U08] Py：展平二维列表
来源：http://sa.muxihuayi.cn

[y for x in nested for y in x]
来源：http://sn.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://bj.nszjky.cn

max(d, key=d.get)
来源：http://bd.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://mh.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eb.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://yh.huanxung.cn

(x * 2 for x in arr)
来源：http://gl.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rp.colortex.cn

Counter(arr).most_common(3)
来源：http://um.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://yj.shxzskj.cn

deque(maxlen=10)
来源：http://xt.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://bq.szxytkj.cn

defaultdict(list)
来源：http://yc.szsharing.cn

[U15] Py：高精度计时
来源：http://ud.hnjuh.cn

t = time.perf_counter()
来源：http://zn.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://do.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fa.szxytkj.cn

[U17] Py：初始化日志
来源：http://zc.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://qr.gzmigu.cn

[U18] Py：预编译正则
来源：http://ti.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://rz.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://is.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eg.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://jr.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://uf.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://ux.huanxung.cn

@contextlib.contextmanager
来源：http://pt.szsharing.cn

[U22] Py：矩阵转置
来源：http://mb.wgjwhj.cn

list(zip(*m))
来源：http://kk.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://mc.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hg.shxzskj.cn

[U24] Py：路径操作
来源：http://us.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nu.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://mt.szsharing.cn

csv.DictReader(f)
来源：http://et.wgjwhj.cn

[U26] Py：并发下载
来源：http://ll.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ys.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://gn.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://xb.szxytkj.cn

[U28] Py：类型别名
来源：http://yn.huixinmuqiang.cn

UserId = int
来源：http://fy.nszjky.cn

[U29] Py：属性校验
来源：http://dp.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://il.wgjwhj.cn

[U30] Py：数据类
来源：http://ik.panjiajie.cn

@dataclass(slots=True)
来源：http://uw.chemitech.net.cn

[U31] Py：单测
来源：http://ja.lnxyls.cn

python -m pytest -q
来源：http://ot.hnjuh.cn

[U32] Py：代码格式化
来源：http://ca.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://ka.newstarts.cn

[U33] Py：打包发布
来源：http://wv.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://cw.newstarts.cn

[U34] Py：判断编码
来源：http://zw.szxytkj.cn

chardet.detect(raw)
来源：http://qc.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://cd.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xs.szsharing.cn

[U36] Py：定时任务
来源：http://ww.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://dv.hahajie.cn

[U37] Py：读写 Excel
来源：http://qm.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xx.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://qr.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://cl.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://am.hnjuh.cn

sys.stdout.isatty()
来源：http://fk.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://fz.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://eh.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://sz.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vx.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://xx.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lw.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ph.haigaiapp.cn

namespace App\Http;
来源：http://nt.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://ae.yuexingan06.cn

declare(strict_types=1);
来源：http://sn.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://qm.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wn.newstarts.cn

[U46] PHP：可空类型
来源：http://zk.panjiajie.cn

?string $name = null
来源：http://mr.shxzukj.cn

[U47] PHP：联合类型
来源：http://al.szsharing.cn

int|string $id
来源：http://jq.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://no.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wb.colortex.cn

[U49] PHP：只读属性
来源：http://jv.nszjky.cn

public readonly string $name
来源：http://gz.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://xr.shxzskj.cn

public function __construct(private int $id) {}
来源：http://vb.chemitech.net.cn

[U51] PHP：数组解构
来源：http://wb.newstarts.cn

[$a, $b] = $arr;
来源：http://ur.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://la.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://nd.asd995.cn

[U53] PHP：空合并运算符
来源：http://lj.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://ao.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://it.shtwfgs.cn

$obj?->method()
来源：http://gc.nszjky.cn

[U55] PHP：match 表达式
来源：http://ja.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oz.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://bg.lnxyls.cn

f(a: 1, b: 2)
来源：http://bp.szxytkj.cn

[U57] PHP：字符串插值
来源：http://al.shxzukj.cn

"值: {$a}"
来源：http://lu.521024.cn

[U58] PHP：数组三件套
来源：http://tz.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nk.nszjky.cn

[U59] PHP：自定义排序
来源：http://sv.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lj.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://dm.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iu.shxzskj.cn

[U61] PHP：正则
来源：http://va.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://so.jctech888.com.cn

[U62] PHP：日期对象
来源：http://nr.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kt.yuexingan06.cn

[U63] PHP：文件读写
来源：http://vm.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fz.asd995.cn

[U64] PHP：目录遍历
来源：http://vl.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://nw.huanxung.cn

[U65] PHP：会话
来源：http://dm.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://no.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://fd.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rq.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://lt.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dq.huanxung.cn

[U68] PHP：PDO 连接
来源：http://px.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lm.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://tb.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://it.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://of.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zi.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ui.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://tu.panjiajie.cn

[U72] PHP：写错误日志
来源：http://ih.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://km.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://hp.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://ag.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://do.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://ln.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://oa.yuntaijiaju.cn

composer require psr/container
来源：http://te.yuexingan06.cn

[U76] PHP：简单路由
来源：http://yk.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ru.szsharing.cn

[U77] PHP：模板渲染
来源：http://qn.hnjuh.cn

composer require twig/twig
来源：http://jm.shxzukj.cn

[U78] PHP：单元测试
来源：http://ym.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://tw.szxytkj.cn

[U79] PHP：静态分析
来源：http://fx.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://el.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://wo.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ll.wgjwhj.cn

[U81] JS：初始化项目
来源：http://em.chemitech.net.cn

npm init -y;  npm i express
来源：http://xl.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://wq.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ub.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://rh.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lx.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://wb.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rt.521024.cn

[U85] JS：可选链
来源：http://if.haigaiapp.cn

a?.b?.c
来源：http://dj.panjiajie.cn

[U86] JS：空值合并
来源：http://zu.521024.cn

a ?? b
来源：http://wr.bjjhwx.cn

[U87] JS：解构默认值
来源：http://oh.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://ik.asd995.cn

[U88] JS：对象展开合并
来源：http://ck.panjiajie.cn

{ ...a, ...b }
来源：http://fi.jctech888.com.cn

[U89] JS：数组去重
来源：http://hb.gzmigu.cn

[...new Set(arr)]
来源：http://bn.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://vl.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://ms.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://rs.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fq.szxytkj.cn

[U92] JS：深拷贝
来源：http://uf.hnjuh.cn

structuredClone(obj)
来源：http://yw.9csxet.cn

[U93] JS：模板字符串
来源：http://uu.lnxyls.cn

`共 ${n} 条`
来源：http://qw.shxzskj.cn

[U94] JS：箭头函数
来源：http://hg.nicolike.cn

const double = x => x * 2;
来源：http://br.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://ku.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://py.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://xd.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yu.9csxet.cn

[U97] JS：并发请求
来源：http://an.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://or.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://kr.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yr.lnxyls.cn

[U99] JS：事件监听
来源：http://mb.szsharing.cn

el.addEventListener("click", e => {})
来源：http://fx.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://eg.hnjuh.cn

document.querySelector(".item")
来源：http://ea.nszjky.cn

[U101] JS：classList 操作
来源：http://ek.muxihuayi.cn

el.classList.toggle("active")
来源：http://hb.panjiajie.cn

[U102] JS：本地存储
来源：http://yx.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ac.gzmigu.cn

[U103] JS：定时器
来源：http://tb.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lu.gzmigu.cn

[U104] JS：防抖
来源：http://jp.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kh.panjiajie.cn

[U105] JS：节流
来源：http://nv.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gl.nszjky.cn

[U106] JS：日期格式化
来源：http://rr.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lf.szxytkj.cn

[U107] JS：数字千分位
来源：http://zr.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qe.shxzukj.cn

[U108] JS：随机整数
来源：http://pf.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qr.lnxyls.cn

[U109] JS：数组分组
来源：http://rp.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://gb.panjiajie.cn

[U110] JS：数组分块
来源：http://iz.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nd.hahajie.cn

[U111] JS：对象转 Map
来源：http://ux.colortex.cn

new Map(Object.entries(obj))
来源：http://xx.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://mx.szxytkj.cn

"7".padStart(3, "0")
来源：http://kj.9csxet.cn

[U113] JS：正则替换全部
来源：http://eu.shxzukj.cn

s.replaceAll("a", "b")
来源：http://rk.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://cs.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://et.hahajie.cn

[U115] JS：生成 UUID
来源：http://ss.lnxyls.cn

crypto.randomUUID()
来源：http://sa.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://wk.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://ps.hahajie.cn

[U117] JS：单元测试
来源：http://sp.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://yj.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://en.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://aq.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://bk.asd995.cn

npx vite build
来源：http://or.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://rq.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://ek.yuntaijiaju.cn


<!-- 参考信息 -->