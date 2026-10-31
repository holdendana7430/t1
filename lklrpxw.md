代发 wailian999

[T49] Perl：函数
来源：http://ah.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ss.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://gc.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kb.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://qt.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://qr.jctech888.com.cn

println("Hello")
来源：http://fi.huixinmuqiang.cn

[T52] Scala：变量
来源：http://bu.huixiangedu.cn

val a = 1;  var b = 2
来源：http://by.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://yg.nszjky.cn

s"值: $b"
来源：http://ik.nicolike.cn

[T54] Scala：集合映射
来源：http://bw.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://tt.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://dn.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bb.jctech888.com.cn

[T56] Scala：样例类
来源：http://fs.asd995.cn

case class User(name: String, age: Int)
来源：http://gn.colortex.cn

[T57] Scala：模式匹配
来源：http://ay.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rv.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://pt.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oq.panjiajie.cn

[T59] Scala：循环
来源：http://qk.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://sw.haigaiapp.cn

[T60] Scala：折叠
来源：http://zp.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gv.huixinmuqiang.cn

================================================================================
来源：http://yn.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ol.gzmigu.cn

================================================================================
来源：http://jm.colortex.cn

[U01] Py：创建虚拟环境
来源：http://vc.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rt.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://md.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rv.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://yd.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kx.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://wx.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xw.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://ve.colortex.cn

list(dict.fromkeys(arr))
来源：http://wc.521024.cn

[U06] Py：合并两个字典
来源：http://tq.newstarts.cn

{**a, **b}
来源：http://yj.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://bm.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://tq.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://di.nicolike.cn

[y for x in nested for y in x]
来源：http://kw.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://il.gzmigu.cn

max(d, key=d.get)
来源：http://ji.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://yd.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cg.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://kz.nicolike.cn

(x * 2 for x in arr)
来源：http://ui.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zk.hahajie.cn

Counter(arr).most_common(3)
来源：http://bj.nicolike.cn

[U13] Py：固定长度队列
来源：http://eb.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ye.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://fj.yuexingan06.cn

defaultdict(list)
来源：http://pb.chemitech.net.cn

[U15] Py：高精度计时
来源：http://ie.hahajie.cn

t = time.perf_counter()
来源：http://qg.huanxung.cn

[U16] Py：命令行参数解析
来源：http://ed.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fa.shxzukj.cn

[U17] Py：初始化日志
来源：http://qe.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://xu.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://xq.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://lz.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://yt.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ci.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://oj.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://eo.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://yi.lnxyls.cn

@contextlib.contextmanager
来源：http://lx.colortex.cn

[U22] Py：矩阵转置
来源：http://nb.shxzukj.cn

list(zip(*m))
来源：http://fo.colortex.cn

[U23] Py：分块读取大文件
来源：http://sr.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uc.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://qt.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pg.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://ou.bookmarksfly.cn

csv.DictReader(f)
来源：http://sw.newstarts.cn

[U26] Py：并发下载
来源：http://bl.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pg.colortex.cn

[U27] Py：异步 HTTP
来源：http://wv.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://gw.huanxung.cn

[U28] Py：类型别名
来源：http://pm.szxytkj.cn

UserId = int
来源：http://jo.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://fz.shxzskj.cn

@property 与 @x.setter 配合
来源：http://ku.jctech888.com.cn

[U30] Py：数据类
来源：http://ce.asd995.cn

@dataclass(slots=True)
来源：http://ke.szxytkj.cn

[U31] Py：单测
来源：http://dm.shxzukj.cn

python -m pytest -q
来源：http://px.gzmigu.cn

[U32] Py：代码格式化
来源：http://fh.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://je.asd995.cn

[U33] Py：打包发布
来源：http://om.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://iz.huixiangedu.cn

[U34] Py：判断编码
来源：http://qu.jctech888.com.cn

chardet.detect(raw)
来源：http://xr.shtwfgs.cn

[U35] Py：发送邮件
来源：http://wk.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wt.9csxet.cn

[U36] Py：定时任务
来源：http://jy.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://us.panjiajie.cn

[U37] Py：读写 Excel
来源：http://vh.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zy.521024.cn

[U38] Py：获取脚本所在目录
来源：http://se.huanxung.cn

Path(__file__).resolve().parent
来源：http://gk.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://xi.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://yw.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://ri.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://ge.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://pf.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xj.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://cg.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vi.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://dc.hahajie.cn

namespace App\Http;
来源：http://tf.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://lc.muxihuayi.cn

declare(strict_types=1);
来源：http://yy.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://gu.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.lnxyls.cn

[U46] PHP：可空类型
来源：http://kz.nszjky.cn

?string $name = null
来源：http://pg.newstarts.cn

[U47] PHP：联合类型
来源：http://wy.huanxung.cn

int|string $id
来源：http://ct.huanxung.cn

[U48] PHP：纯枚举
来源：http://mb.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ra.panjiajie.cn

[U49] PHP：只读属性
来源：http://vv.haigaiapp.cn

public readonly string $name
来源：http://ev.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://lz.nicolike.cn

public function __construct(private int $id) {}
来源：http://wc.panjiajie.cn

[U51] PHP：数组解构
来源：http://ud.panjiajie.cn

[$a, $b] = $arr;
来源：http://pl.lnxyls.cn

[U52] PHP：箭头函数
来源：http://xr.521024.cn

$double = fn($x) => $x * 2;
来源：http://gp.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://cy.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://pw.nszjky.cn

[U54] PHP：空安全调用
来源：http://tv.panjiajie.cn

$obj?->method()
来源：http://zv.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://dq.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mb.panjiajie.cn

[U56] PHP：命名参数
来源：http://xe.9csxet.cn

f(a: 1, b: 2)
来源：http://tl.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://sn.jianghongdianzi.cn

"值: {$a}"
来源：http://uk.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://mg.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://am.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://nf.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nl.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://kb.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sc.bookmarksfly.cn

[U61] PHP：正则
来源：http://lc.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ru.huanxung.cn

[U62] PHP：日期对象
来源：http://rb.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ha.shtwfgs.cn

[U63] PHP：文件读写
来源：http://mm.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xu.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://ad.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://yo.chemitech.net.cn

[U65] PHP：会话
来源：http://xv.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gh.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ki.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gi.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://wk.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rz.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://oj.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jz.521024.cn

[U69] PHP：PDO 预处理
来源：http://ts.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mj.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://ji.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yg.hnjuh.cn

[U71] PHP：抛出异常
来源：http://qb.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://st.newstarts.cn

[U72] PHP：写错误日志
来源：http://cu.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://qh.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://da.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://rr.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://gx.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://tc.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://rh.muxihuayi.cn

composer require psr/container
来源：http://ev.9csxet.cn

[U76] PHP：简单路由
来源：http://qq.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xg.panjiajie.cn

[U77] PHP：模板渲染
来源：http://tm.nicolike.cn

composer require twig/twig
来源：http://zc.9csxet.cn

[U78] PHP：单元测试
来源：http://kl.asd995.cn

composer require --dev phpunit/phpunit
来源：http://mr.shxzukj.cn

[U79] PHP：静态分析
来源：http://ad.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://eq.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://hd.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sl.yuexingan06.cn

[U81] JS：初始化项目
来源：http://cu.haigaiapp.cn

npm init -y;  npm i express
来源：http://qd.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://nn.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dl.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://pw.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sc.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://kc.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iy.wgjwhj.cn

[U85] JS：可选链
来源：http://hx.jctech888.com.cn

a?.b?.c
来源：http://sc.shxzukj.cn

[U86] JS：空值合并
来源：http://bt.huixiangedu.cn

a ?? b
来源：http://qo.nszjky.cn

[U87] JS：解构默认值
来源：http://nt.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://ot.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://de.asd995.cn

{ ...a, ...b }
来源：http://ch.bjjhwx.cn

[U89] JS：数组去重
来源：http://zv.szxytkj.cn

[...new Set(arr)]
来源：http://rg.nszjky.cn

[U90] JS：数字数组排序
来源：http://xy.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://ip.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wj.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mo.huanxung.cn

[U92] JS：深拷贝
来源：http://ms.szxytkj.cn

structuredClone(obj)
来源：http://pd.szsharing.cn

[U93] JS：模板字符串
来源：http://ea.hnjuh.cn

`共 ${n} 条`
来源：http://lz.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://ah.szxytkj.cn

const double = x => x * 2;
来源：http://ny.gzmigu.cn

[U95] JS：Promise 包装
来源：http://wy.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://xp.newstarts.cn

[U96] JS：async/await 与异常
来源：http://kc.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tv.bjjhwx.cn

[U97] JS：并发请求
来源：http://py.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rg.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ol.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ku.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://yy.521024.cn

el.addEventListener("click", e => {})
来源：http://zk.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://nb.9csxet.cn

document.querySelector(".item")
来源：http://pu.chemitech.net.cn

[U101] JS：classList 操作
来源：http://qz.asd995.cn

el.classList.toggle("active")
来源：http://tz.muxihuayi.cn

[U102] JS：本地存储
来源：http://pc.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rj.huixinmuqiang.cn

[U103] JS：定时器
来源：http://xs.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ks.9csxet.cn

[U104] JS：防抖
来源：http://ty.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ln.9csxet.cn

[U105] JS：节流
来源：http://ma.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jj.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://yz.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ok.521024.cn

[U107] JS：数字千分位
来源：http://wx.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pb.521024.cn

[U108] JS：随机整数
来源：http://qs.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fr.521024.cn

[U109] JS：数组分组
来源：http://di.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://lx.shtwfgs.cn

[U110] JS：数组分块
来源：http://gr.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kg.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://wp.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://sn.nszjky.cn

[U112] JS：字符串补位
来源：http://nw.huixiangedu.cn

"7".padStart(3, "0")
来源：http://jz.shxzskj.cn

[U113] JS：正则替换全部
来源：http://ri.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://vf.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://of.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fp.shxzskj.cn

[U115] JS：生成 UUID
来源：http://sx.nicolike.cn

crypto.randomUUID()
来源：http://iy.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://kn.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://ih.szsharing.cn

[U117] JS：单元测试
来源：http://ea.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://an.shxzukj.cn

[U118] JS：开发服务器
来源：http://hh.gzmigu.cn

npm i -D vite;  npx vite
来源：http://wp.asd995.cn

[U119] JS：生产构建
来源：http://zj.haigaiapp.cn

npx vite build
来源：http://wp.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://zz.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://dk.nszjky.cn

================================================================================
来源：http://st.huanxung.cn

统计汇总
来源：http://le.bookmarksfly.cn

================================================================================
来源：http://qf.nszjky.cn

按语言统计（条）：
来源：http://pa.colortex.cn

Python ......... 252
来源：http://pw.gzmigu.cn

PHP ............ 252
来源：http://pi.chemitech.net.cn

JavaScript ..... 252
来源：http://vi.colortex.cn

TypeScript ..... 212
来源：http://nu.szsharing.cn

Java ........... 212
来源：http://nb.huixiangedu.cn

Go ............. 212
来源：http://qu.wgjwhj.cn

Ruby ........... 212
来源：http://fe.bookmarksfly.cn

C# ............. 212
来源：http://qh.huixinmuqiang.cn

C .............. 30
来源：http://ww.lnxyls.cn

C++ ............ 30
来源：http://bq.hahajie.cn

SQL ............ 90
来源：http://on.yuexingan06.cn

Bash ........... 80
来源：http://df.muxihuayi.cn

Kotlin ......... 15
来源：http://bj.huanxung.cn

Swift .......... 15
来源：http://gh.muxihuayi.cn

Lua ............ 10
来源：http://vu.bookmarksfly.cn

Perl ........... 10
来源：http://fl.huixinmuqiang.cn

Scala .......... 10
来源：http://sr.huanxung.cn

------------------------------------
来源：http://ix.lnxyls.cn

合计 ........... 2106 条
来源：http://ve.huanxung.cn

按章节统计：
来源：http://fw.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yb.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eu.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wu.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hx.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xm.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://do.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cg.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://in.shxzukj.cn


<!-- 参考信息 -->