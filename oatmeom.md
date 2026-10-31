代发 wailian999

[T47] Perl：正则捕获
来源：http://fs.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jx.hnjuh.cn

[T48] Perl：正则替换
来源：http://cn.nszjky.cn

$s =~ s/old/new/g;
来源：http://ma.panjiajie.cn

[T49] Perl：函数
来源：http://uf.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hr.nicolike.cn

[T50] Perl：逐行读文件
来源：http://ga.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gg.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://yx.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://lq.haigaiapp.cn

println("Hello")
来源：http://dw.szxytkj.cn

[T52] Scala：变量
来源：http://uv.shxzukj.cn

val a = 1;  var b = 2
来源：http://pv.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://uo.gzmigu.cn

s"值: $b"
来源：http://sk.newstarts.cn

[T54] Scala：集合映射
来源：http://lq.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://js.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://sc.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oj.nicolike.cn

[T56] Scala：样例类
来源：http://qj.nszjky.cn

case class User(name: String, age: Int)
来源：http://bo.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://ya.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dr.asd995.cn

[T58] Scala：函数定义
来源：http://vg.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qd.newstarts.cn

[T59] Scala：循环
来源：http://qc.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://aa.nszjky.cn

[T60] Scala：折叠
来源：http://ro.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://px.yuexingan06.cn

================================================================================
来源：http://cq.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ym.hahajie.cn

================================================================================
来源：http://eq.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://mh.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vp.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://bk.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yw.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://dt.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lg.panjiajie.cn

[U04] Py：变量调试打印
来源：http://kt.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gl.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://pa.huanxung.cn

list(dict.fromkeys(arr))
来源：http://jh.9csxet.cn

[U06] Py：合并两个字典
来源：http://oe.wgjwhj.cn

{**a, **b}
来源：http://ru.szsharing.cn

[U07] Py：反转字典键值
来源：http://ye.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://mx.szxytkj.cn

[U08] Py：展平二维列表
来源：http://hz.hahajie.cn

[y for x in nested for y in x]
来源：http://wi.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://qi.nicolike.cn

max(d, key=d.get)
来源：http://fn.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://vo.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ia.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://iq.muxihuayi.cn

(x * 2 for x in arr)
来源：http://dp.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pq.9csxet.cn

Counter(arr).most_common(3)
来源：http://mx.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://xn.shxzukj.cn

deque(maxlen=10)
来源：http://du.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://in.hahajie.cn

defaultdict(list)
来源：http://fn.shxzskj.cn

[U15] Py：高精度计时
来源：http://li.nicolike.cn

t = time.perf_counter()
来源：http://kx.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://vv.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vj.yuexingan06.cn

[U17] Py：初始化日志
来源：http://os.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://kj.asd995.cn

[U18] Py：预编译正则
来源：http://ez.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://mn.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://ec.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wq.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://vp.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://mk.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://qv.gzmigu.cn

@contextlib.contextmanager
来源：http://os.nicolike.cn

[U22] Py：矩阵转置
来源：http://bu.huanxung.cn

list(zip(*m))
来源：http://hr.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://ba.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xc.hahajie.cn

[U24] Py：路径操作
来源：http://ng.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uw.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://dv.shxzskj.cn

csv.DictReader(f)
来源：http://ub.asd995.cn

[U26] Py：并发下载
来源：http://fo.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vd.521024.cn

[U27] Py：异步 HTTP
来源：http://tz.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://fg.shxzskj.cn

[U28] Py：类型别名
来源：http://pl.wgjwhj.cn

UserId = int
来源：http://ku.nszjky.cn

[U29] Py：属性校验
来源：http://ck.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://kf.huanxung.cn

[U30] Py：数据类
来源：http://bs.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://qm.hahajie.cn

[U31] Py：单测
来源：http://wx.jianghongdianzi.cn

python -m pytest -q
来源：http://ju.shxzukj.cn

[U32] Py：代码格式化
来源：http://fo.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://va.panjiajie.cn

[U33] Py：打包发布
来源：http://zg.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://bw.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://ga.jianghongdianzi.cn

chardet.detect(raw)
来源：http://xm.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://bs.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gn.asd995.cn

[U36] Py：定时任务
来源：http://ln.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://ze.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://un.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ve.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://gn.panjiajie.cn

Path(__file__).resolve().parent
来源：http://yd.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://qx.muxihuayi.cn

sys.stdout.isatty()
来源：http://zt.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://cd.nszjky.cn

print("err", file=sys.stderr)
来源：http://ns.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://gs.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nb.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://oq.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jf.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://dr.521024.cn

namespace App\Http;
来源：http://un.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://bv.chemitech.net.cn

declare(strict_types=1);
来源：http://zm.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://lo.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zo.shxzukj.cn

[U46] PHP：可空类型
来源：http://vx.nszjky.cn

?string $name = null
来源：http://nx.9csxet.cn

[U47] PHP：联合类型
来源：http://ia.haigaiapp.cn

int|string $id
来源：http://zv.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://zg.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dn.9csxet.cn

[U49] PHP：只读属性
来源：http://dz.huixiangedu.cn

public readonly string $name
来源：http://dt.asd995.cn

[U50] PHP：构造器属性提升
来源：http://og.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://my.chemitech.net.cn

[U51] PHP：数组解构
来源：http://uc.521024.cn

[$a, $b] = $arr;
来源：http://zt.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://lj.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://tn.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://or.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://dn.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://pr.521024.cn

$obj?->method()
来源：http://ck.9csxet.cn

[U55] PHP：match 表达式
来源：http://og.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jk.colortex.cn

[U56] PHP：命名参数
来源：http://yd.shxzskj.cn

f(a: 1, b: 2)
来源：http://ws.asd995.cn

[U57] PHP：字符串插值
来源：http://ds.9csxet.cn

"值: {$a}"
来源：http://pp.lnxyls.cn

[U58] PHP：数组三件套
来源：http://ac.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://de.shxzskj.cn

[U59] PHP：自定义排序
来源：http://ex.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sy.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://xk.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dn.jctech888.com.cn

[U61] PHP：正则
来源：http://sy.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wd.shxzskj.cn

[U62] PHP：日期对象
来源：http://ev.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wm.hnjuh.cn

[U63] PHP：文件读写
来源：http://yu.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vx.gzmigu.cn

[U64] PHP：目录遍历
来源：http://hx.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://oh.nszjky.cn

[U65] PHP：会话
来源：http://ah.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ss.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://rk.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kk.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://gv.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tt.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://we.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zf.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://fs.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ka.nicolike.cn

[U70] PHP：PDO 事务
来源：http://jt.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://da.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://aw.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://zf.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://pv.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://mm.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://zz.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://rt.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://kj.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://fo.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://wq.lnxyls.cn

composer require psr/container
来源：http://dy.huixiangedu.cn

[U76] PHP：简单路由
来源：http://ax.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rh.hahajie.cn

[U77] PHP：模板渲染
来源：http://sy.szxytkj.cn

composer require twig/twig
来源：http://iq.shtwfgs.cn

[U78] PHP：单元测试
来源：http://xp.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://wg.chemitech.net.cn

[U79] PHP：静态分析
来源：http://ie.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://jt.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://fj.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kz.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://nh.huanxung.cn

npm init -y;  npm i express
来源：http://ft.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://oo.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gd.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://fy.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hp.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://he.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nt.shxzukj.cn

[U85] JS：可选链
来源：http://aj.szsharing.cn

a?.b?.c
来源：http://da.huixiangedu.cn

[U86] JS：空值合并
来源：http://ya.jianghongdianzi.cn

a ?? b
来源：http://oi.yuexingan06.cn

[U87] JS：解构默认值
来源：http://ov.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://aq.huanxung.cn

[U88] JS：对象展开合并
来源：http://dg.chemitech.net.cn

{ ...a, ...b }
来源：http://gx.jctech888.com.cn

[U89] JS：数组去重
来源：http://bb.shxzukj.cn

[...new Set(arr)]
来源：http://zv.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://us.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://jh.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://se.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xk.haigaiapp.cn

[U92] JS：深拷贝
来源：http://uj.colortex.cn

structuredClone(obj)
来源：http://qj.newstarts.cn

[U93] JS：模板字符串
来源：http://ft.chemitech.net.cn

`共 ${n} 条`
来源：http://lq.asd995.cn

[U94] JS：箭头函数
来源：http://jn.szsharing.cn

const double = x => x * 2;
来源：http://fw.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://fz.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://qw.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://dl.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ob.colortex.cn

[U97] JS：并发请求
来源：http://ih.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uh.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://oh.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rl.asd995.cn

[U99] JS：事件监听
来源：http://nr.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://gk.newstarts.cn

[U100] JS：DOM 查询
来源：http://ix.jianghongdianzi.cn

document.querySelector(".item")
来源：http://qq.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://sx.nszjky.cn

el.classList.toggle("active")
来源：http://wi.shxzukj.cn

[U102] JS：本地存储
来源：http://ad.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ei.newstarts.cn

[U103] JS：定时器
来源：http://ho.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sk.shtwfgs.cn

[U104] JS：防抖
来源：http://tq.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zl.yuexingan06.cn

[U105] JS：节流
来源：http://vc.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ri.yuexingan06.cn

[U106] JS：日期格式化
来源：http://ms.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xs.hahajie.cn

[U107] JS：数字千分位
来源：http://ta.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ug.nszjky.cn

[U108] JS：随机整数
来源：http://cf.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bk.jctech888.com.cn

[U109] JS：数组分组
来源：http://go.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://hf.newstarts.cn

[U110] JS：数组分块
来源：http://gl.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lk.hahajie.cn

[U111] JS：对象转 Map
来源：http://re.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://re.9csxet.cn

[U112] JS：字符串补位
来源：http://pa.gzmigu.cn

"7".padStart(3, "0")
来源：http://ul.szsharing.cn

[U113] JS：正则替换全部
来源：http://hj.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://re.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://cz.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ri.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://hc.yuexingan06.cn

crypto.randomUUID()
来源：http://ma.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://xi.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://ar.hahajie.cn

[U117] JS：单元测试
来源：http://xd.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://zy.bjjhwx.cn

[U118] JS：开发服务器
来源：http://xz.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://gz.chemitech.net.cn

[U119] JS：生产构建
来源：http://kk.gzmigu.cn

npx vite build
来源：http://mu.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://wv.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://ak.szxytkj.cn

================================================================================
来源：http://xp.nszjky.cn

统计汇总
来源：http://hc.muxihuayi.cn

================================================================================
来源：http://vu.bjjhwx.cn

按语言统计（条）：
来源：http://xv.nszjky.cn

Python ......... 252
来源：http://ki.huixiangedu.cn

PHP ............ 252
来源：http://aa.lnxyls.cn

JavaScript ..... 252
来源：http://rx.hahajie.cn

TypeScript ..... 212
来源：http://yy.jianghongdianzi.cn

Java ........... 212
来源：http://hr.muxihuayi.cn

Go ............. 212
来源：http://hf.nicolike.cn

Ruby ........... 212
来源：http://qn.yuexingan06.cn

C# ............. 212
来源：http://rt.bookmarksfly.cn

C .............. 30
来源：http://wt.haigaiapp.cn

C++ ............ 30
来源：http://jf.huixinmuqiang.cn

SQL ............ 90
来源：http://ir.521024.cn

Bash ........... 80
来源：http://jh.nszjky.cn

Kotlin ......... 15
来源：http://ty.jctech888.com.cn

Swift .......... 15
来源：http://oy.haigaiapp.cn

Lua ............ 10
来源：http://ei.shxzukj.cn

Perl ........... 10
来源：http://wd.huanxung.cn

Scala .......... 10
来源：http://sa.huixinmuqiang.cn

------------------------------------
来源：http://ti.colortex.cn

合计 ........... 2106 条
来源：http://ev.yuexingan06.cn

按章节统计：
来源：http://wo.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ey.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tq.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://of.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ki.lnxyls.cn


<!-- 参考信息 -->