代发 wailian999

[T35] Lua：字典表
来源：http://uy.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://qy.huanxung.cn

[T36] Lua：函数
来源：http://lk.szsharing.cn

function add(a, b) return a + b end
来源：http://jy.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://pk.gzmigu.cn

"a" .. "b"
来源：http://ij.szxytkj.cn

[T38] Lua：条件
来源：http://yo.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://mu.szsharing.cn

[T39] Lua：模式匹配
来源：http://yv.hnjuh.cn

string.find(s, "%d+")
来源：http://ha.huanxung.cn

[T40] Lua：元表
来源：http://pu.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://zy.chemitech.net.cn

[T41] Perl：Hello World
来源：http://ga.szxytkj.cn

print "Hello\n";
来源：http://xt.521024.cn

[T42] Perl：变量类型
来源：http://qt.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kj.hahajie.cn

[T43] Perl：字符串插值
来源：http://kl.szxytkj.cn

"值: $a"
来源：http://gp.hnjuh.cn

[T44] Perl：条件
来源：http://si.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ng.shxzskj.cn

[T45] Perl：数组遍历
来源：http://be.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://hz.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://hz.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ev.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://aj.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qs.haigaiapp.cn

[T48] Perl：正则替换
来源：http://zz.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://qr.panjiajie.cn

[T49] Perl：函数
来源：http://lb.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://az.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://fu.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cg.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://uc.nszjky.cn

[T51] Scala：Hello World
来源：http://lr.huixiangedu.cn

println("Hello")
来源：http://qw.jctech888.com.cn

[T52] Scala：变量
来源：http://by.hahajie.cn

val a = 1;  var b = 2
来源：http://ha.gzmigu.cn

[T53] Scala：字符串插值
来源：http://gf.szsharing.cn

s"值: $b"
来源：http://uc.szsharing.cn

[T54] Scala：集合映射
来源：http://ya.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://gs.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://lw.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fl.yuexingan06.cn

[T56] Scala：样例类
来源：http://gh.szsharing.cn

case class User(name: String, age: Int)
来源：http://ml.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://ab.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mu.szsharing.cn

[T58] Scala：函数定义
来源：http://di.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tv.jctech888.com.cn

[T59] Scala：循环
来源：http://ui.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://of.huixiangedu.cn

[T60] Scala：折叠
来源：http://kx.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mj.yuexingan06.cn

================================================================================
来源：http://tg.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qx.huixiangedu.cn

================================================================================
来源：http://rj.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://bk.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://um.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://oo.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iz.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://oz.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://st.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://cd.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mc.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://kc.huanxung.cn

list(dict.fromkeys(arr))
来源：http://xs.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://qn.jianghongdianzi.cn

{**a, **b}
来源：http://kj.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://ej.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://cx.gzmigu.cn

[U08] Py：展平二维列表
来源：http://av.hahajie.cn

[y for x in nested for y in x]
来源：http://ly.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://gk.wgjwhj.cn

max(d, key=d.get)
来源：http://pj.521024.cn

[U10] Py：按值排序字典
来源：http://em.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jg.gzmigu.cn

[U11] Py：生成器表达式
来源：http://po.newstarts.cn

(x * 2 for x in arr)
来源：http://bt.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sg.shxzukj.cn

Counter(arr).most_common(3)
来源：http://pr.nszjky.cn

[U13] Py：固定长度队列
来源：http://ev.wgjwhj.cn

deque(maxlen=10)
来源：http://da.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://fp.muxihuayi.cn

defaultdict(list)
来源：http://du.jctech888.com.cn

[U15] Py：高精度计时
来源：http://hc.bjjhwx.cn

t = time.perf_counter()
来源：http://tg.colortex.cn

[U16] Py：命令行参数解析
来源：http://ih.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yg.szsharing.cn

[U17] Py：初始化日志
来源：http://nt.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://zz.szsharing.cn

[U18] Py：预编译正则
来源：http://xr.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://lh.szsharing.cn

[U19] Py：正则替换带回调
来源：http://do.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dl.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://my.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://bo.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://ug.nszjky.cn

@contextlib.contextmanager
来源：http://qb.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://oe.yuntaijiaju.cn

list(zip(*m))
来源：http://jn.hahajie.cn

[U23] Py：分块读取大文件
来源：http://ga.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zh.yuexingan06.cn

[U24] Py：路径操作
来源：http://kn.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ga.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://xq.521024.cn

csv.DictReader(f)
来源：http://qa.yuexingan06.cn

[U26] Py：并发下载
来源：http://uk.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jt.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://bc.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://cf.hahajie.cn

[U28] Py：类型别名
来源：http://zp.bjjhwx.cn

UserId = int
来源：http://fx.nicolike.cn

[U29] Py：属性校验
来源：http://qp.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://ww.bookmarksfly.cn

[U30] Py：数据类
来源：http://eb.asd995.cn

@dataclass(slots=True)
来源：http://lz.jctech888.com.cn

[U31] Py：单测
来源：http://kf.9csxet.cn

python -m pytest -q
来源：http://ul.wgjwhj.cn

[U32] Py：代码格式化
来源：http://ek.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://gt.yuexingan06.cn

[U33] Py：打包发布
来源：http://bn.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ca.lnxyls.cn

[U34] Py：判断编码
来源：http://wo.huixinmuqiang.cn

chardet.detect(raw)
来源：http://dp.haigaiapp.cn

[U35] Py：发送邮件
来源：http://fn.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tr.szxytkj.cn

[U36] Py：定时任务
来源：http://zl.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://li.szxytkj.cn

[U37] Py：读写 Excel
来源：http://pk.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ye.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://gr.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://qh.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://jm.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://oa.szsharing.cn

[U40] Py：打印到标准错误
来源：http://pp.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://md.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://nk.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://fv.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fd.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://wl.521024.cn

namespace App\Http;
来源：http://xn.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://xe.yuexingan06.cn

declare(strict_types=1);
来源：http://lt.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://dp.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.nszjky.cn

[U46] PHP：可空类型
来源：http://zr.yuntaijiaju.cn

?string $name = null
来源：http://ad.lnxyls.cn

[U47] PHP：联合类型
来源：http://mm.nszjky.cn

int|string $id
来源：http://fe.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://bk.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kk.shxzukj.cn

[U49] PHP：只读属性
来源：http://kk.szsharing.cn

public readonly string $name
来源：http://rh.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://uh.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://wa.shtwfgs.cn

[U51] PHP：数组解构
来源：http://os.hahajie.cn

[$a, $b] = $arr;
来源：http://wg.szsharing.cn

[U52] PHP：箭头函数
来源：http://ps.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://sp.szsharing.cn

[U53] PHP：空合并运算符
来源：http://vv.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ho.hahajie.cn

[U54] PHP：空安全调用
来源：http://mb.bjjhwx.cn

$obj?->method()
来源：http://od.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://nq.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bf.huanxung.cn

[U56] PHP：命名参数
来源：http://xz.panjiajie.cn

f(a: 1, b: 2)
来源：http://mu.szxytkj.cn

[U57] PHP：字符串插值
来源：http://iq.chemitech.net.cn

"值: {$a}"
来源：http://vs.lnxyls.cn

[U58] PHP：数组三件套
来源：http://jo.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lv.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://bm.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tz.asd995.cn

[U60] PHP：JSON 编解码
来源：http://hg.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zg.yuntaijiaju.cn

[U61] PHP：正则
来源：http://tv.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://px.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://hh.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oy.lnxyls.cn

[U63] PHP：文件读写
来源：http://dj.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xj.nicolike.cn

[U64] PHP：目录遍历
来源：http://ql.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://bw.shtwfgs.cn

[U65] PHP：会话
来源：http://wb.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jn.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://eu.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gi.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://hn.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eb.nicolike.cn

[U68] PHP：PDO 连接
来源：http://uj.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mt.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://yz.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lp.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://jd.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bk.panjiajie.cn

[U71] PHP：抛出异常
来源：http://oc.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://lp.nicolike.cn

[U72] PHP：写错误日志
来源：http://ag.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://ai.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://ei.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://fv.9csxet.cn

[U74] PHP：读取环境变量
来源：http://aj.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://vg.lnxyls.cn

[U75] PHP：依赖注入
来源：http://fk.wgjwhj.cn

composer require psr/container
来源：http://ba.huixiangedu.cn

[U76] PHP：简单路由
来源：http://dn.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cg.shxzskj.cn

[U77] PHP：模板渲染
来源：http://bc.hahajie.cn

composer require twig/twig
来源：http://hi.newstarts.cn

[U78] PHP：单元测试
来源：http://gu.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://oi.shtwfgs.cn

[U79] PHP：静态分析
来源：http://xv.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://ws.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://nc.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wv.521024.cn

[U81] JS：初始化项目
来源：http://nx.newstarts.cn

npm init -y;  npm i express
来源：http://dz.newstarts.cn

[U82] JS：package.json 脚本
来源：http://wf.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yd.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://iz.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kr.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://gh.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dm.9csxet.cn

[U85] JS：可选链
来源：http://vx.huixinmuqiang.cn

a?.b?.c
来源：http://rg.nszjky.cn

[U86] JS：空值合并
来源：http://ys.nicolike.cn

a ?? b
来源：http://zg.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://xy.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://ap.huanxung.cn

[U88] JS：对象展开合并
来源：http://oz.jctech888.com.cn

{ ...a, ...b }
来源：http://fo.521024.cn

[U89] JS：数组去重
来源：http://my.shxzukj.cn

[...new Set(arr)]
来源：http://oy.panjiajie.cn

[U90] JS：数字数组排序
来源：http://dz.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://di.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://rz.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://me.hnjuh.cn

[U92] JS：深拷贝
来源：http://xn.lnxyls.cn

structuredClone(obj)
来源：http://dy.jctech888.com.cn

[U93] JS：模板字符串
来源：http://ed.lnxyls.cn

`共 ${n} 条`
来源：http://wu.shxzukj.cn

[U94] JS：箭头函数
来源：http://gb.9csxet.cn

const double = x => x * 2;
来源：http://qk.szxytkj.cn

[U95] JS：Promise 包装
来源：http://rg.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://uy.colortex.cn

[U96] JS：async/await 与异常
来源：http://ev.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gv.huixiangedu.cn

[U97] JS：并发请求
来源：http://rt.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ha.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://wr.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pv.chemitech.net.cn

[U99] JS：事件监听
来源：http://uj.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://pf.asd995.cn

[U100] JS：DOM 查询
来源：http://eg.muxihuayi.cn

document.querySelector(".item")
来源：http://mt.9csxet.cn

[U101] JS：classList 操作
来源：http://nt.9csxet.cn

el.classList.toggle("active")
来源：http://zf.haigaiapp.cn

[U102] JS：本地存储
来源：http://ur.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gd.nicolike.cn

[U103] JS：定时器
来源：http://tr.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nd.bookmarksfly.cn

[U104] JS：防抖
来源：http://tk.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vh.yuexingan06.cn

[U105] JS：节流
来源：http://nr.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://du.asd995.cn

[U106] JS：日期格式化
来源：http://oe.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zr.szsharing.cn

[U107] JS：数字千分位
来源：http://bw.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qo.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://lf.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mk.bjjhwx.cn

[U109] JS：数组分组
来源：http://bv.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://nj.colortex.cn

[U110] JS：数组分块
来源：http://bj.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yu.huanxung.cn

[U111] JS：对象转 Map
来源：http://yp.panjiajie.cn

new Map(Object.entries(obj))
来源：http://bi.shxzukj.cn

[U112] JS：字符串补位
来源：http://dz.hnjuh.cn

"7".padStart(3, "0")
来源：http://yt.colortex.cn

[U113] JS：正则替换全部
来源：http://hk.521024.cn

s.replaceAll("a", "b")
来源：http://lc.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://la.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://po.szsharing.cn

[U115] JS：生成 UUID
来源：http://me.521024.cn

crypto.randomUUID()
来源：http://jn.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://yd.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://dn.muxihuayi.cn

[U117] JS：单元测试
来源：http://oq.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://gv.muxihuayi.cn

[U118] JS：开发服务器
来源：http://um.hnjuh.cn

npm i -D vite;  npx vite
来源：http://tv.muxihuayi.cn

[U119] JS：生产构建
来源：http://gh.szxytkj.cn

npx vite build
来源：http://pn.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://up.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://wl.jianghongdianzi.cn

================================================================================
来源：http://nj.hahajie.cn

统计汇总
来源：http://sm.jianghongdianzi.cn

================================================================================
来源：http://zn.haigaiapp.cn

按语言统计（条）：
来源：http://cz.jianghongdianzi.cn


<!-- 参考信息 -->