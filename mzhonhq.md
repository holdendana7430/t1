代发 wailian999

[T37] Lua：字符串拼接
来源：http://ao.bjjhwx.cn

"a" .. "b"
来源：http://md.bookmarksfly.cn

[T38] Lua：条件
来源：http://ya.gzmigu.cn

if x > 0 then print("正") end
来源：http://bv.panjiajie.cn

[T39] Lua：模式匹配
来源：http://jw.gzmigu.cn

string.find(s, "%d+")
来源：http://dm.huixiangedu.cn

[T40] Lua：元表
来源：http://lx.asd995.cn

setmetatable({}, { __index = base })
来源：http://gq.szsharing.cn

[T41] Perl：Hello World
来源：http://kq.muxihuayi.cn

print "Hello\n";
来源：http://lg.hnjuh.cn

[T42] Perl：变量类型
来源：http://cv.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://po.huanxung.cn

[T43] Perl：字符串插值
来源：http://dj.hnjuh.cn

"值: $a"
来源：http://if.lnxyls.cn

[T44] Perl：条件
来源：http://bx.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://ka.521024.cn

[T45] Perl：数组遍历
来源：http://yf.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://st.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://bc.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zt.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://rw.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bk.9csxet.cn

[T48] Perl：正则替换
来源：http://fx.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://kq.bjjhwx.cn

[T49] Perl：函数
来源：http://sl.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tt.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://du.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xg.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://qe.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://bc.newstarts.cn

println("Hello")
来源：http://gj.colortex.cn

[T52] Scala：变量
来源：http://ua.lnxyls.cn

val a = 1;  var b = 2
来源：http://ko.hahajie.cn

[T53] Scala：字符串插值
来源：http://ub.hnjuh.cn

s"值: $b"
来源：http://gj.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://fl.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://we.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://ze.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qv.huanxung.cn

[T56] Scala：样例类
来源：http://ra.szsharing.cn

case class User(name: String, age: Int)
来源：http://xk.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://yh.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ut.szxytkj.cn

[T58] Scala：函数定义
来源：http://cg.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lu.chemitech.net.cn

[T59] Scala：循环
来源：http://qb.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://dz.hnjuh.cn

[T60] Scala：折叠
来源：http://mx.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bx.wgjwhj.cn

================================================================================
来源：http://qd.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rz.newstarts.cn

================================================================================
来源：http://ty.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://na.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gx.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://va.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fs.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://oy.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uo.hahajie.cn

[U04] Py：变量调试打印
来源：http://ho.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://td.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://hg.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://ye.nszjky.cn

[U06] Py：合并两个字典
来源：http://es.bjjhwx.cn

{**a, **b}
来源：http://fn.shxzskj.cn

[U07] Py：反转字典键值
来源：http://ff.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://uv.lnxyls.cn

[U08] Py：展平二维列表
来源：http://tq.hahajie.cn

[y for x in nested for y in x]
来源：http://mg.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://ge.shxzskj.cn

max(d, key=d.get)
来源：http://hz.9csxet.cn

[U10] Py：按值排序字典
来源：http://py.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://is.panjiajie.cn

[U11] Py：生成器表达式
来源：http://oi.panjiajie.cn

(x * 2 for x in arr)
来源：http://ag.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iw.colortex.cn

Counter(arr).most_common(3)
来源：http://fp.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://zh.gzmigu.cn

deque(maxlen=10)
来源：http://wz.huanxung.cn

[U14] Py：分组收集到列表
来源：http://je.huanxung.cn

defaultdict(list)
来源：http://po.yuexingan06.cn

[U15] Py：高精度计时
来源：http://yj.9csxet.cn

t = time.perf_counter()
来源：http://dj.9csxet.cn

[U16] Py：命令行参数解析
来源：http://wt.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zm.521024.cn

[U17] Py：初始化日志
来源：http://ql.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ca.wgjwhj.cn

[U18] Py：预编译正则
来源：http://wx.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://vt.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://lx.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kk.asd995.cn

[U20] Py：缓存函数结果
来源：http://bg.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://pr.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://si.colortex.cn

@contextlib.contextmanager
来源：http://as.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://ta.muxihuayi.cn

list(zip(*m))
来源：http://ai.huanxung.cn

[U23] Py：分块读取大文件
来源：http://kr.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rs.shxzukj.cn

[U24] Py：路径操作
来源：http://bd.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dd.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://ul.nszjky.cn

csv.DictReader(f)
来源：http://dl.shxzskj.cn

[U26] Py：并发下载
来源：http://ld.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sq.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://qd.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://jw.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://hv.asd995.cn

UserId = int
来源：http://pf.521024.cn

[U29] Py：属性校验
来源：http://hz.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ja.muxihuayi.cn

[U30] Py：数据类
来源：http://rf.9csxet.cn

@dataclass(slots=True)
来源：http://hk.nszjky.cn

[U31] Py：单测
来源：http://be.newstarts.cn

python -m pytest -q
来源：http://si.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://ap.huanxung.cn

ruff format . && ruff check --fix .
来源：http://qi.huixiangedu.cn

[U33] Py：打包发布
来源：http://st.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://oc.panjiajie.cn

[U34] Py：判断编码
来源：http://ks.shxzskj.cn

chardet.detect(raw)
来源：http://ng.bjjhwx.cn

[U35] Py：发送邮件
来源：http://um.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uv.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://qa.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://ss.nszjky.cn

[U37] Py：读写 Excel
来源：http://xi.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cr.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://an.lnxyls.cn

Path(__file__).resolve().parent
来源：http://yg.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://oc.shxzukj.cn

sys.stdout.isatty()
来源：http://ss.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://dp.9csxet.cn

print("err", file=sys.stderr)
来源：http://aj.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://od.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bd.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://eo.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ke.huanxung.cn

[U43] PHP：声明命名空间
来源：http://od.lnxyls.cn

namespace App\Http;
来源：http://wb.szsharing.cn

[U44] PHP：开启严格类型
来源：http://af.hnjuh.cn

declare(strict_types=1);
来源：http://nb.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://tk.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tc.haigaiapp.cn

[U46] PHP：可空类型
来源：http://et.szxytkj.cn

?string $name = null
来源：http://pa.yuexingan06.cn

[U47] PHP：联合类型
来源：http://pi.nicolike.cn

int|string $id
来源：http://vt.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://vc.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rw.panjiajie.cn

[U49] PHP：只读属性
来源：http://ay.chemitech.net.cn

public readonly string $name
来源：http://xq.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://uo.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://lu.9csxet.cn

[U51] PHP：数组解构
来源：http://jk.newstarts.cn

[$a, $b] = $arr;
来源：http://ck.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://ib.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://rn.521024.cn

[U53] PHP：空合并运算符
来源：http://hr.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://hz.lnxyls.cn

[U54] PHP：空安全调用
来源：http://jr.jctech888.com.cn

$obj?->method()
来源：http://xr.newstarts.cn

[U55] PHP：match 表达式
来源：http://ka.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vv.wgjwhj.cn

[U56] PHP：命名参数
来源：http://zh.haigaiapp.cn

f(a: 1, b: 2)
来源：http://vt.nicolike.cn

[U57] PHP：字符串插值
来源：http://hn.shxzukj.cn

"值: {$a}"
来源：http://kr.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://uo.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pn.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://ji.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lg.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://cq.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mo.jctech888.com.cn

[U61] PHP：正则
来源：http://pj.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zc.lnxyls.cn

[U62] PHP：日期对象
来源：http://ys.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ds.lnxyls.cn

[U63] PHP：文件读写
来源：http://ri.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rx.shxzukj.cn

[U64] PHP：目录遍历
来源：http://as.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://oz.shtwfgs.cn

[U65] PHP：会话
来源：http://ud.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rm.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://ce.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jh.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://hc.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jc.huanxung.cn

[U68] PHP：PDO 连接
来源：http://fs.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nt.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://zq.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cc.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ae.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sf.nicolike.cn

[U71] PHP：抛出异常
来源：http://su.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://ec.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://pv.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://dg.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://xa.asd995.cn

parse_ini_file("config.ini", true)
来源：http://yi.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ys.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://df.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://kp.panjiajie.cn

composer require psr/container
来源：http://fg.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://zd.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mq.panjiajie.cn

[U77] PHP：模板渲染
来源：http://vp.panjiajie.cn

composer require twig/twig
来源：http://ux.szxytkj.cn

[U78] PHP：单元测试
来源：http://rl.521024.cn

composer require --dev phpunit/phpunit
来源：http://xf.szxytkj.cn

[U79] PHP：静态分析
来源：http://on.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://zy.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://df.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rd.colortex.cn

[U81] JS：初始化项目
来源：http://qz.chemitech.net.cn

npm init -y;  npm i express
来源：http://uw.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://zv.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ia.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://rp.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sz.colortex.cn

[U84] JS：CommonJS 写法
来源：http://yq.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://je.bookmarksfly.cn

[U85] JS：可选链
来源：http://sb.yuntaijiaju.cn

a?.b?.c
来源：http://wi.colortex.cn

[U86] JS：空值合并
来源：http://nr.shxzskj.cn

a ?? b
来源：http://ls.huanxung.cn

[U87] JS：解构默认值
来源：http://th.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://cz.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://nn.newstarts.cn

{ ...a, ...b }
来源：http://fr.chemitech.net.cn

[U89] JS：数组去重
来源：http://kj.jianghongdianzi.cn

[...new Set(arr)]
来源：http://dk.9csxet.cn

[U90] JS：数字数组排序
来源：http://ge.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://tw.nszjky.cn

[U91] JS：对象键值遍历
来源：http://hx.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lo.shtwfgs.cn

[U92] JS：深拷贝
来源：http://vt.chemitech.net.cn

structuredClone(obj)
来源：http://le.shtwfgs.cn

[U93] JS：模板字符串
来源：http://wk.huanxung.cn

`共 ${n} 条`
来源：http://at.bjjhwx.cn

[U94] JS：箭头函数
来源：http://xg.colortex.cn

const double = x => x * 2;
来源：http://zv.szsharing.cn

[U95] JS：Promise 包装
来源：http://ny.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://zw.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://wz.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kx.nicolike.cn

[U97] JS：并发请求
来源：http://sb.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bh.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://wc.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rr.gzmigu.cn

[U99] JS：事件监听
来源：http://lm.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://zj.szsharing.cn

[U100] JS：DOM 查询
来源：http://sc.jianghongdianzi.cn

document.querySelector(".item")
来源：http://ow.nszjky.cn

[U101] JS：classList 操作
来源：http://xd.huixiangedu.cn

el.classList.toggle("active")
来源：http://gu.muxihuayi.cn

[U102] JS：本地存储
来源：http://lf.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zy.newstarts.cn

[U103] JS：定时器
来源：http://kp.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pk.colortex.cn

[U104] JS：防抖
来源：http://xe.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vy.bjjhwx.cn

[U105] JS：节流
来源：http://xg.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gj.huixiangedu.cn

[U106] JS：日期格式化
来源：http://xn.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gs.9csxet.cn

[U107] JS：数字千分位
来源：http://ri.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sy.shtwfgs.cn

[U108] JS：随机整数
来源：http://wh.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xp.muxihuayi.cn

[U109] JS：数组分组
来源：http://ml.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://ey.hnjuh.cn

[U110] JS：数组分块
来源：http://sh.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ta.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://as.521024.cn

new Map(Object.entries(obj))
来源：http://qs.521024.cn

[U112] JS：字符串补位
来源：http://nd.521024.cn

"7".padStart(3, "0")
来源：http://nj.szsharing.cn

[U113] JS：正则替换全部
来源：http://jv.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://rk.9csxet.cn

[U114] JS：JSON 深比较
来源：http://za.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ca.521024.cn

[U115] JS：生成 UUID
来源：http://ki.yuntaijiaju.cn

crypto.randomUUID()
来源：http://no.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://mi.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://bg.shxzukj.cn

[U117] JS：单元测试
来源：http://ud.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://og.huixiangedu.cn

[U118] JS：开发服务器
来源：http://lx.hahajie.cn

npm i -D vite;  npx vite
来源：http://pz.muxihuayi.cn

[U119] JS：生产构建
来源：http://xe.huixinmuqiang.cn

npx vite build
来源：http://nx.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://ra.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://pp.yuntaijiaju.cn

================================================================================
来源：http://lu.hahajie.cn

统计汇总
来源：http://ad.jctech888.com.cn

================================================================================
来源：http://rc.nicolike.cn

按语言统计（条）：
来源：http://hi.521024.cn

Python ......... 252
来源：http://gg.hahajie.cn

PHP ............ 252
来源：http://cc.huixiangedu.cn

JavaScript ..... 252
来源：http://up.wgjwhj.cn

TypeScript ..... 212
来源：http://li.newstarts.cn


<!-- 参考信息 -->