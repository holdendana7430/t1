代发 wailian999

[T49] Perl：函数
来源：http://vm.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ap.asd995.cn

[T50] Perl：逐行读文件
来源：http://ae.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yv.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://xv.shxzskj.cn

[T51] Scala：Hello World
来源：http://zs.chemitech.net.cn

println("Hello")
来源：http://zw.colortex.cn

[T52] Scala：变量
来源：http://df.521024.cn

val a = 1;  var b = 2
来源：http://xl.szxytkj.cn

[T53] Scala：字符串插值
来源：http://jf.shtwfgs.cn

s"值: $b"
来源：http://ir.szxytkj.cn

[T54] Scala：集合映射
来源：http://af.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://dh.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://fw.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ye.shxzskj.cn

[T56] Scala：样例类
来源：http://nf.lnxyls.cn

case class User(name: String, age: Int)
来源：http://bi.521024.cn

[T57] Scala：模式匹配
来源：http://ah.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fd.shxzskj.cn

[T58] Scala：函数定义
来源：http://vb.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dg.muxihuayi.cn

[T59] Scala：循环
来源：http://ph.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://bx.gzmigu.cn

[T60] Scala：折叠
来源：http://cr.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hj.shxzukj.cn

================================================================================
来源：http://gp.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ia.szsharing.cn

================================================================================
来源：http://jn.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://io.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vq.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://vw.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xy.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://fg.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cb.nszjky.cn

[U04] Py：变量调试打印
来源：http://xx.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xr.szsharing.cn

[U05] Py：列表去重且保序
来源：http://qc.szsharing.cn

list(dict.fromkeys(arr))
来源：http://pv.newstarts.cn

[U06] Py：合并两个字典
来源：http://fy.bookmarksfly.cn

{**a, **b}
来源：http://lf.gzmigu.cn

[U07] Py：反转字典键值
来源：http://mz.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://ae.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://ha.haigaiapp.cn

[y for x in nested for y in x]
来源：http://qu.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://cw.chemitech.net.cn

max(d, key=d.get)
来源：http://bn.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://cf.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xp.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://ws.521024.cn

(x * 2 for x in arr)
来源：http://at.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gj.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://zy.521024.cn

[U13] Py：固定长度队列
来源：http://px.szxytkj.cn

deque(maxlen=10)
来源：http://jp.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://cc.yuexingan06.cn

defaultdict(list)
来源：http://ci.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://uf.shxzukj.cn

t = time.perf_counter()
来源：http://gu.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://xe.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kl.panjiajie.cn

[U17] Py：初始化日志
来源：http://ht.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://bj.shtwfgs.cn

[U18] Py：预编译正则
来源：http://ge.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ax.asd995.cn

[U19] Py：正则替换带回调
来源：http://tg.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jg.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://nn.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://is.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ze.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ez.521024.cn

[U22] Py：矩阵转置
来源：http://mj.yuexingan06.cn

list(zip(*m))
来源：http://bg.9csxet.cn

[U23] Py：分块读取大文件
来源：http://tb.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nr.panjiajie.cn

[U24] Py：路径操作
来源：http://rf.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ab.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ke.yuntaijiaju.cn

csv.DictReader(f)
来源：http://jn.szxytkj.cn

[U26] Py：并发下载
来源：http://qo.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fk.colortex.cn

[U27] Py：异步 HTTP
来源：http://kl.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://xj.shxzukj.cn

[U28] Py：类型别名
来源：http://at.nicolike.cn

UserId = int
来源：http://uq.gzmigu.cn

[U29] Py：属性校验
来源：http://te.szxytkj.cn

@property 与 @x.setter 配合
来源：http://uv.nszjky.cn

[U30] Py：数据类
来源：http://ui.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://sm.hahajie.cn

[U31] Py：单测
来源：http://zh.jianghongdianzi.cn

python -m pytest -q
来源：http://an.szxytkj.cn

[U32] Py：代码格式化
来源：http://tg.asd995.cn

ruff format . && ruff check --fix .
来源：http://id.wgjwhj.cn

[U33] Py：打包发布
来源：http://it.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://xa.muxihuayi.cn

[U34] Py：判断编码
来源：http://bk.bjjhwx.cn

chardet.detect(raw)
来源：http://se.asd995.cn

[U35] Py：发送邮件
来源：http://kd.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fo.nszjky.cn

[U36] Py：定时任务
来源：http://qq.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://yr.nszjky.cn

[U37] Py：读写 Excel
来源：http://pc.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cm.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://hh.hahajie.cn

Path(__file__).resolve().parent
来源：http://xk.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://bb.hahajie.cn

sys.stdout.isatty()
来源：http://uw.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://il.asd995.cn

print("err", file=sys.stderr)
来源：http://ag.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://un.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vr.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://dc.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fu.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://yy.wgjwhj.cn

namespace App\Http;
来源：http://ny.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ol.bookmarksfly.cn

declare(strict_types=1);
来源：http://gb.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ql.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lb.huanxung.cn

[U46] PHP：可空类型
来源：http://fv.lnxyls.cn

?string $name = null
来源：http://oh.muxihuayi.cn

[U47] PHP：联合类型
来源：http://ox.hahajie.cn

int|string $id
来源：http://ox.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://uj.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pz.huanxung.cn

[U49] PHP：只读属性
来源：http://rl.muxihuayi.cn

public readonly string $name
来源：http://oy.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ci.panjiajie.cn

public function __construct(private int $id) {}
来源：http://rw.wgjwhj.cn

[U51] PHP：数组解构
来源：http://ww.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://ly.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ai.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://xr.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://qm.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://sq.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://qj.panjiajie.cn

$obj?->method()
来源：http://xg.gzmigu.cn

[U55] PHP：match 表达式
来源：http://jh.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dv.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://mm.haigaiapp.cn

f(a: 1, b: 2)
来源：http://qm.shxzukj.cn

[U57] PHP：字符串插值
来源：http://xi.jctech888.com.cn

"值: {$a}"
来源：http://sd.asd995.cn

[U58] PHP：数组三件套
来源：http://fc.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qf.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://kz.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gt.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://ak.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dy.hahajie.cn

[U61] PHP：正则
来源：http://iw.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xf.jctech888.com.cn

[U62] PHP：日期对象
来源：http://gq.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zn.lnxyls.cn

[U63] PHP：文件读写
来源：http://bo.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://db.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://kx.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://kd.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ka.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://og.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://vy.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gp.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://kl.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://el.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://zb.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lc.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://cx.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fa.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://pv.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ao.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://uv.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://bm.colortex.cn

[U72] PHP：写错误日志
来源：http://lm.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://rb.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://oa.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://bk.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://in.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://ib.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://rz.newstarts.cn

composer require psr/container
来源：http://xq.colortex.cn

[U76] PHP：简单路由
来源：http://so.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jr.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ui.nszjky.cn

composer require twig/twig
来源：http://vs.jctech888.com.cn

[U78] PHP：单元测试
来源：http://ru.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://pt.muxihuayi.cn

[U79] PHP：静态分析
来源：http://ke.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://yy.nicolike.cn

[U80] PHP：代码规范修复
来源：http://ad.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vv.9csxet.cn

[U81] JS：初始化项目
来源：http://uj.gzmigu.cn

npm init -y;  npm i express
来源：http://dw.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://pd.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vi.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://qs.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ns.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://xu.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ja.colortex.cn

[U85] JS：可选链
来源：http://ef.newstarts.cn

a?.b?.c
来源：http://bk.hahajie.cn

[U86] JS：空值合并
来源：http://ad.huixinmuqiang.cn

a ?? b
来源：http://cx.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://ha.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://bf.shxzukj.cn

[U88] JS：对象展开合并
来源：http://dw.nszjky.cn

{ ...a, ...b }
来源：http://xo.yuexingan06.cn

[U89] JS：数组去重
来源：http://on.shxzukj.cn

[...new Set(arr)]
来源：http://ol.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://aw.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://es.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://rn.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zk.jctech888.com.cn

[U92] JS：深拷贝
来源：http://xg.gzmigu.cn

structuredClone(obj)
来源：http://la.asd995.cn

[U93] JS：模板字符串
来源：http://zy.hahajie.cn

`共 ${n} 条`
来源：http://ny.hahajie.cn

[U94] JS：箭头函数
来源：http://sw.gzmigu.cn

const double = x => x * 2;
来源：http://de.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://hj.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://cu.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://lw.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://em.chemitech.net.cn

[U97] JS：并发请求
来源：http://rw.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hg.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://zt.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hi.shxzskj.cn

[U99] JS：事件监听
来源：http://hm.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://sl.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://ob.jianghongdianzi.cn

document.querySelector(".item")
来源：http://zo.jctech888.com.cn

[U101] JS：classList 操作
来源：http://ap.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://jt.hahajie.cn

[U102] JS：本地存储
来源：http://mk.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sx.jctech888.com.cn

[U103] JS：定时器
来源：http://sc.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ox.jianghongdianzi.cn

[U104] JS：防抖
来源：http://jh.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rh.huanxung.cn

[U105] JS：节流
来源：http://mi.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://af.szsharing.cn

[U106] JS：日期格式化
来源：http://ve.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jl.gzmigu.cn

[U107] JS：数字千分位
来源：http://ft.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fg.9csxet.cn

[U108] JS：随机整数
来源：http://lq.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://os.bookmarksfly.cn

[U109] JS：数组分组
来源：http://cs.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://kf.bookmarksfly.cn

[U110] JS：数组分块
来源：http://oz.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fn.szxytkj.cn

[U111] JS：对象转 Map
来源：http://cf.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://ll.nicolike.cn

[U112] JS：字符串补位
来源：http://oa.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://eh.huanxung.cn

[U113] JS：正则替换全部
来源：http://id.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://mo.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://jg.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ll.newstarts.cn

[U115] JS：生成 UUID
来源：http://sd.haigaiapp.cn

crypto.randomUUID()
来源：http://bg.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://hg.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://wy.gzmigu.cn

[U117] JS：单元测试
来源：http://ft.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://tg.hahajie.cn

[U118] JS：开发服务器
来源：http://nl.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://xn.asd995.cn

[U119] JS：生产构建
来源：http://hx.gzmigu.cn

npx vite build
来源：http://pm.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://lx.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://vb.bjjhwx.cn

================================================================================
来源：http://mv.colortex.cn

统计汇总
来源：http://tt.lnxyls.cn

================================================================================
来源：http://bj.nszjky.cn

按语言统计（条）：
来源：http://qi.panjiajie.cn

Python ......... 252
来源：http://yd.nszjky.cn

PHP ............ 252
来源：http://zk.shtwfgs.cn

JavaScript ..... 252
来源：http://qg.huanxung.cn

TypeScript ..... 212
来源：http://bp.jctech888.com.cn

Java ........... 212
来源：http://tr.nszjky.cn

Go ............. 212
来源：http://gi.hnjuh.cn

Ruby ........... 212
来源：http://vh.huixinmuqiang.cn

C# ............. 212
来源：http://bk.szsharing.cn

C .............. 30
来源：http://dt.panjiajie.cn

C++ ............ 30
来源：http://sv.chemitech.net.cn

SQL ............ 90
来源：http://pp.shxzukj.cn

Bash ........... 80
来源：http://wt.lnxyls.cn

Kotlin ......... 15
来源：http://sf.521024.cn

Swift .......... 15
来源：http://wa.9csxet.cn

Lua ............ 10
来源：http://eb.jctech888.com.cn

Perl ........... 10
来源：http://pq.wgjwhj.cn

Scala .......... 10
来源：http://qg.muxihuayi.cn

------------------------------------
来源：http://am.shxzskj.cn

合计 ........... 2106 条
来源：http://lo.colortex.cn

按章节统计：
来源：http://dt.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mm.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tr.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zw.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lj.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gd.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mn.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ou.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tq.szsharing.cn


<!-- 参考信息 -->