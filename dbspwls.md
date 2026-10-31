代发 wailian999

[T47] Perl：正则捕获
来源：http://er.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zr.9csxet.cn

[T48] Perl：正则替换
来源：http://nw.szxytkj.cn

$s =~ s/old/new/g;
来源：http://zc.huixiangedu.cn

[T49] Perl：函数
来源：http://ke.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fd.nicolike.cn

[T50] Perl：逐行读文件
来源：http://fx.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mr.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://xv.asd995.cn

[T51] Scala：Hello World
来源：http://ui.chemitech.net.cn

println("Hello")
来源：http://wb.colortex.cn

[T52] Scala：变量
来源：http://fe.shxzskj.cn

val a = 1;  var b = 2
来源：http://er.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://wn.asd995.cn

s"值: $b"
来源：http://fk.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://xy.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://gy.szxytkj.cn

[T55] Scala：集合过滤
来源：http://nw.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ku.muxihuayi.cn

[T56] Scala：样例类
来源：http://co.gzmigu.cn

case class User(name: String, age: Int)
来源：http://zj.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://se.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mh.huanxung.cn

[T58] Scala：函数定义
来源：http://tc.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cp.jctech888.com.cn

[T59] Scala：循环
来源：http://zw.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://vr.szxytkj.cn

[T60] Scala：折叠
来源：http://hf.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ii.asd995.cn

================================================================================
来源：http://xm.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nf.nszjky.cn

================================================================================
来源：http://vq.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://wy.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jd.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://el.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xt.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://hv.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zf.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://cz.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jz.nicolike.cn

[U05] Py：列表去重且保序
来源：http://ik.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://lf.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://sc.nicolike.cn

{**a, **b}
来源：http://vq.szxytkj.cn

[U07] Py：反转字典键值
来源：http://bc.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://qb.asd995.cn

[U08] Py：展平二维列表
来源：http://au.haigaiapp.cn

[y for x in nested for y in x]
来源：http://hd.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://an.chemitech.net.cn

max(d, key=d.get)
来源：http://hs.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://qd.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sc.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://pf.haigaiapp.cn

(x * 2 for x in arr)
来源：http://fd.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oe.hnjuh.cn

Counter(arr).most_common(3)
来源：http://eg.asd995.cn

[U13] Py：固定长度队列
来源：http://of.newstarts.cn

deque(maxlen=10)
来源：http://eg.9csxet.cn

[U14] Py：分组收集到列表
来源：http://bl.hahajie.cn

defaultdict(list)
来源：http://fp.yuexingan06.cn

[U15] Py：高精度计时
来源：http://eb.nszjky.cn

t = time.perf_counter()
来源：http://uw.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://cs.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jh.asd995.cn

[U17] Py：初始化日志
来源：http://po.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://jt.9csxet.cn

[U18] Py：预编译正则
来源：http://cq.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://mu.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://ha.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://og.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://qc.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://kk.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://dv.521024.cn

@contextlib.contextmanager
来源：http://rm.hahajie.cn

[U22] Py：矩阵转置
来源：http://rd.bookmarksfly.cn

list(zip(*m))
来源：http://gx.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://pi.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mm.huixiangedu.cn

[U24] Py：路径操作
来源：http://qf.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ms.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://yg.shtwfgs.cn

csv.DictReader(f)
来源：http://sx.bookmarksfly.cn

[U26] Py：并发下载
来源：http://zy.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://re.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ym.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://oq.nicolike.cn

[U28] Py：类型别名
来源：http://tt.newstarts.cn

UserId = int
来源：http://at.muxihuayi.cn

[U29] Py：属性校验
来源：http://zq.521024.cn

@property 与 @x.setter 配合
来源：http://cv.nszjky.cn

[U30] Py：数据类
来源：http://sm.shtwfgs.cn

@dataclass(slots=True)
来源：http://vz.szsharing.cn

[U31] Py：单测
来源：http://tz.szsharing.cn

python -m pytest -q
来源：http://pn.lnxyls.cn

[U32] Py：代码格式化
来源：http://me.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://or.shxzskj.cn

[U33] Py：打包发布
来源：http://mt.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://qa.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://ev.newstarts.cn

chardet.detect(raw)
来源：http://lc.nicolike.cn

[U35] Py：发送邮件
来源：http://pq.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ec.huanxung.cn

[U36] Py：定时任务
来源：http://uc.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://gb.gzmigu.cn

[U37] Py：读写 Excel
来源：http://py.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pb.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://fq.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://uq.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://re.chemitech.net.cn

sys.stdout.isatty()
来源：http://ju.nicolike.cn

[U40] Py：打印到标准错误
来源：http://cl.hahajie.cn

print("err", file=sys.stderr)
来源：http://ri.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://iv.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zp.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://jr.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ze.nszjky.cn

[U43] PHP：声明命名空间
来源：http://zj.shxzukj.cn

namespace App\Http;
来源：http://kp.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://no.gzmigu.cn

declare(strict_types=1);
来源：http://ru.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://lg.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rh.shxzskj.cn

[U46] PHP：可空类型
来源：http://zb.nicolike.cn

?string $name = null
来源：http://jk.yuexingan06.cn

[U47] PHP：联合类型
来源：http://vz.colortex.cn

int|string $id
来源：http://bi.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://ar.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xp.nszjky.cn

[U49] PHP：只读属性
来源：http://dk.gzmigu.cn

public readonly string $name
来源：http://vp.asd995.cn

[U50] PHP：构造器属性提升
来源：http://rg.lnxyls.cn

public function __construct(private int $id) {}
来源：http://yo.521024.cn

[U51] PHP：数组解构
来源：http://fp.newstarts.cn

[$a, $b] = $arr;
来源：http://ys.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://gh.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://et.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://na.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://xb.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ou.nicolike.cn

$obj?->method()
来源：http://er.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://pj.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gc.hahajie.cn

[U56] PHP：命名参数
来源：http://ui.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://eu.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://yf.newstarts.cn

"值: {$a}"
来源：http://qi.shxzukj.cn

[U58] PHP：数组三件套
来源：http://zw.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://me.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://yt.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yf.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://fa.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jd.bookmarksfly.cn

[U61] PHP：正则
来源：http://rh.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zu.newstarts.cn

[U62] PHP：日期对象
来源：http://ev.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cy.9csxet.cn

[U63] PHP：文件读写
来源：http://jy.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ga.asd995.cn

[U64] PHP：目录遍历
来源：http://rq.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://bd.yuntaijiaju.cn

[U65] PHP：会话
来源：http://hk.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xv.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://ov.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pq.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://qo.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uf.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://wl.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fw.colortex.cn

[U69] PHP：PDO 预处理
来源：http://cb.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sr.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://gy.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vq.shxzukj.cn

[U71] PHP：抛出异常
来源：http://re.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://pr.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://ve.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://qg.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://fs.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://ml.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://dc.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://jw.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://sp.yuexingan06.cn

composer require psr/container
来源：http://hf.huixiangedu.cn

[U76] PHP：简单路由
来源：http://hs.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ik.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://nr.muxihuayi.cn

composer require twig/twig
来源：http://kj.huixiangedu.cn

[U78] PHP：单元测试
来源：http://vv.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://cs.bjjhwx.cn

[U79] PHP：静态分析
来源：http://hh.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://qk.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://lw.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tq.jctech888.com.cn

[U81] JS：初始化项目
来源：http://lg.jctech888.com.cn

npm init -y;  npm i express
来源：http://pv.huanxung.cn

[U82] JS：package.json 脚本
来源：http://iz.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zm.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://rt.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://im.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://me.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ae.9csxet.cn

[U85] JS：可选链
来源：http://rs.newstarts.cn

a?.b?.c
来源：http://bp.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://zf.jctech888.com.cn

a ?? b
来源：http://wn.wgjwhj.cn

[U87] JS：解构默认值
来源：http://uo.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://yp.asd995.cn

[U88] JS：对象展开合并
来源：http://nt.bookmarksfly.cn

{ ...a, ...b }
来源：http://la.colortex.cn

[U89] JS：数组去重
来源：http://yq.9csxet.cn

[...new Set(arr)]
来源：http://fq.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://hr.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://np.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://kq.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dm.bjjhwx.cn

[U92] JS：深拷贝
来源：http://uy.gzmigu.cn

structuredClone(obj)
来源：http://zs.nicolike.cn

[U93] JS：模板字符串
来源：http://fo.panjiajie.cn

`共 ${n} 条`
来源：http://jl.hahajie.cn

[U94] JS：箭头函数
来源：http://wj.asd995.cn

const double = x => x * 2;
来源：http://jx.shxzukj.cn

[U95] JS：Promise 包装
来源：http://kf.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://ta.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://gq.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://il.nicolike.cn

[U97] JS：并发请求
来源：http://jn.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://un.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://sw.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kl.huixiangedu.cn

[U99] JS：事件监听
来源：http://vl.nszjky.cn

el.addEventListener("click", e => {})
来源：http://sj.newstarts.cn

[U100] JS：DOM 查询
来源：http://mu.yuexingan06.cn

document.querySelector(".item")
来源：http://su.huanxung.cn

[U101] JS：classList 操作
来源：http://ds.shxzskj.cn

el.classList.toggle("active")
来源：http://vm.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://le.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gt.hnjuh.cn

[U103] JS：定时器
来源：http://pq.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aq.nicolike.cn

[U104] JS：防抖
来源：http://si.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://js.nicolike.cn

[U105] JS：节流
来源：http://bn.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fa.9csxet.cn

[U106] JS：日期格式化
来源：http://eu.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ci.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://rf.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zz.yuexingan06.cn

[U108] JS：随机整数
来源：http://gj.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://up.bookmarksfly.cn

[U109] JS：数组分组
来源：http://wy.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://nc.hahajie.cn

[U110] JS：数组分块
来源：http://ds.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jj.shxzskj.cn

[U111] JS：对象转 Map
来源：http://oo.gzmigu.cn

new Map(Object.entries(obj))
来源：http://oy.lnxyls.cn

[U112] JS：字符串补位
来源：http://sc.521024.cn

"7".padStart(3, "0")
来源：http://ke.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://fl.huanxung.cn

s.replaceAll("a", "b")
来源：http://gc.nicolike.cn

[U114] JS：JSON 深比较
来源：http://lf.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nz.nicolike.cn

[U115] JS：生成 UUID
来源：http://vl.521024.cn

crypto.randomUUID()
来源：http://kx.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://ce.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://hd.bjjhwx.cn

[U117] JS：单元测试
来源：http://lb.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://ee.521024.cn

[U118] JS：开发服务器
来源：http://en.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://xq.haigaiapp.cn

[U119] JS：生产构建
来源：http://gz.bookmarksfly.cn

npx vite build
来源：http://sz.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://jn.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://cy.hahajie.cn

================================================================================
来源：http://sm.9csxet.cn

统计汇总
来源：http://wl.bjjhwx.cn

================================================================================
来源：http://kb.hahajie.cn

按语言统计（条）：
来源：http://no.bjjhwx.cn

Python ......... 252
来源：http://vm.huixinmuqiang.cn

PHP ............ 252
来源：http://al.muxihuayi.cn

JavaScript ..... 252
来源：http://uj.shxzskj.cn

TypeScript ..... 212
来源：http://qg.szsharing.cn

Java ........... 212
来源：http://ud.szxytkj.cn

Go ............. 212
来源：http://qd.szsharing.cn

Ruby ........... 212
来源：http://tn.shxzukj.cn

C# ............. 212
来源：http://rd.jianghongdianzi.cn

C .............. 30
来源：http://cf.chemitech.net.cn

C++ ............ 30
来源：http://hx.lnxyls.cn

SQL ............ 90
来源：http://li.hahajie.cn

Bash ........... 80
来源：http://oz.nicolike.cn

Kotlin ......... 15
来源：http://fu.huanxung.cn

Swift .......... 15
来源：http://pt.colortex.cn

Lua ............ 10
来源：http://iv.hahajie.cn

Perl ........... 10
来源：http://eu.wgjwhj.cn

Scala .......... 10
来源：http://cc.gzmigu.cn

------------------------------------
来源：http://hg.521024.cn

合计 ........... 2106 条
来源：http://oe.haigaiapp.cn

按章节统计：
来源：http://rj.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oe.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ki.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ln.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yt.shxzukj.cn


<!-- 参考信息 -->