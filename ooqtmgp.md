代发 wailian999

val a = 1;  var b = 2
来源：http://gv.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://pl.bjjhwx.cn

s"值: $b"
来源：http://vy.shxzskj.cn

[T54] Scala：集合映射
来源：http://bb.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://xy.nicolike.cn

[T55] Scala：集合过滤
来源：http://jd.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cj.haigaiapp.cn

[T56] Scala：样例类
来源：http://lc.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://mf.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://zq.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hu.asd995.cn

[T58] Scala：函数定义
来源：http://tz.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oo.9csxet.cn

[T59] Scala：循环
来源：http://xi.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://mx.chemitech.net.cn

[T60] Scala：折叠
来源：http://db.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gc.newstarts.cn

================================================================================
来源：http://lg.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bf.nicolike.cn

================================================================================
来源：http://ja.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ha.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gc.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://xh.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mk.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://en.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://co.panjiajie.cn

[U04] Py：变量调试打印
来源：http://yb.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://to.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://qo.nszjky.cn

list(dict.fromkeys(arr))
来源：http://zz.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://ic.gzmigu.cn

{**a, **b}
来源：http://ze.nszjky.cn

[U07] Py：反转字典键值
来源：http://zm.nicolike.cn

{v: k for k, v in d.items()}
来源：http://sy.521024.cn

[U08] Py：展平二维列表
来源：http://jo.szxytkj.cn

[y for x in nested for y in x]
来源：http://wp.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://ur.szxytkj.cn

max(d, key=d.get)
来源：http://nx.hahajie.cn

[U10] Py：按值排序字典
来源：http://kq.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zs.hahajie.cn

[U11] Py：生成器表达式
来源：http://uq.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://lo.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eq.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://hl.asd995.cn

[U13] Py：固定长度队列
来源：http://of.nszjky.cn

deque(maxlen=10)
来源：http://me.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://wu.haigaiapp.cn

defaultdict(list)
来源：http://iu.huixiangedu.cn

[U15] Py：高精度计时
来源：http://hp.hahajie.cn

t = time.perf_counter()
来源：http://kp.szsharing.cn

[U16] Py：命令行参数解析
来源：http://ax.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zx.panjiajie.cn

[U17] Py：初始化日志
来源：http://un.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://yf.szsharing.cn

[U18] Py：预编译正则
来源：http://xv.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://gr.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://us.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fc.nicolike.cn

[U20] Py：缓存函数结果
来源：http://ml.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://jc.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://px.521024.cn

@contextlib.contextmanager
来源：http://za.colortex.cn

[U22] Py：矩阵转置
来源：http://zg.shtwfgs.cn

list(zip(*m))
来源：http://qt.newstarts.cn

[U23] Py：分块读取大文件
来源：http://wo.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pm.jctech888.com.cn

[U24] Py：路径操作
来源：http://pc.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ju.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://fl.nicolike.cn

csv.DictReader(f)
来源：http://qi.9csxet.cn

[U26] Py：并发下载
来源：http://ey.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ar.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://xu.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://rg.shtwfgs.cn

[U28] Py：类型别名
来源：http://yw.shxzskj.cn

UserId = int
来源：http://kh.hahajie.cn

[U29] Py：属性校验
来源：http://by.gzmigu.cn

@property 与 @x.setter 配合
来源：http://rl.lnxyls.cn

[U30] Py：数据类
来源：http://vx.szsharing.cn

@dataclass(slots=True)
来源：http://vh.yuexingan06.cn

[U31] Py：单测
来源：http://nx.szsharing.cn

python -m pytest -q
来源：http://da.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://rs.asd995.cn

ruff format . && ruff check --fix .
来源：http://em.bjjhwx.cn

[U33] Py：打包发布
来源：http://os.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ul.colortex.cn

[U34] Py：判断编码
来源：http://xl.huanxung.cn

chardet.detect(raw)
来源：http://po.nicolike.cn

[U35] Py：发送邮件
来源：http://cj.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://el.nszjky.cn

[U36] Py：定时任务
来源：http://ka.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://fv.521024.cn

[U37] Py：读写 Excel
来源：http://ot.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gq.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://ep.panjiajie.cn

Path(__file__).resolve().parent
来源：http://jd.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://ye.huixiangedu.cn

sys.stdout.isatty()
来源：http://oe.nicolike.cn

[U40] Py：打印到标准错误
来源：http://zx.huanxung.cn

print("err", file=sys.stderr)
来源：http://cj.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://ir.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rk.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://rt.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kw.521024.cn

[U43] PHP：声明命名空间
来源：http://nl.newstarts.cn

namespace App\Http;
来源：http://rh.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://ws.yuntaijiaju.cn

declare(strict_types=1);
来源：http://nh.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ln.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bb.shxzskj.cn

[U46] PHP：可空类型
来源：http://wu.hahajie.cn

?string $name = null
来源：http://ah.shxzukj.cn

[U47] PHP：联合类型
来源：http://cv.szsharing.cn

int|string $id
来源：http://bw.colortex.cn

[U48] PHP：纯枚举
来源：http://da.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mf.yuexingan06.cn

[U49] PHP：只读属性
来源：http://zd.hahajie.cn

public readonly string $name
来源：http://ga.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://ej.panjiajie.cn

public function __construct(private int $id) {}
来源：http://xy.jctech888.com.cn

[U51] PHP：数组解构
来源：http://bh.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://ww.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://fi.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://vc.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://op.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://yy.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://rb.gzmigu.cn

$obj?->method()
来源：http://yr.gzmigu.cn

[U55] PHP：match 表达式
来源：http://xx.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yd.shxzukj.cn

[U56] PHP：命名参数
来源：http://qv.wgjwhj.cn

f(a: 1, b: 2)
来源：http://tc.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://jq.shtwfgs.cn

"值: {$a}"
来源：http://kh.hnjuh.cn

[U58] PHP：数组三件套
来源：http://uc.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xx.9csxet.cn

[U59] PHP：自定义排序
来源：http://vu.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://id.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://fg.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bh.gzmigu.cn

[U61] PHP：正则
来源：http://dy.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ho.lnxyls.cn

[U62] PHP：日期对象
来源：http://xs.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://my.panjiajie.cn

[U63] PHP：文件读写
来源：http://ip.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ij.szxytkj.cn

[U64] PHP：目录遍历
来源：http://hw.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ua.gzmigu.cn

[U65] PHP：会话
来源：http://ft.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nh.521024.cn

[U66] PHP：设置 Cookie
来源：http://xy.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dx.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://ut.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mw.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://kd.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://af.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://kj.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zw.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://bd.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lt.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://xr.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://zf.panjiajie.cn

[U72] PHP：写错误日志
来源：http://aa.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ok.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://ms.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://fu.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://xz.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://jg.szxytkj.cn

[U75] PHP：依赖注入
来源：http://yr.huixiangedu.cn

composer require psr/container
来源：http://tp.shxzskj.cn

[U76] PHP：简单路由
来源：http://hn.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eo.9csxet.cn

[U77] PHP：模板渲染
来源：http://ok.shxzskj.cn

composer require twig/twig
来源：http://vw.nszjky.cn

[U78] PHP：单元测试
来源：http://li.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://va.haigaiapp.cn

[U79] PHP：静态分析
来源：http://wp.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://ab.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://bn.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lu.panjiajie.cn

[U81] JS：初始化项目
来源：http://ok.hnjuh.cn

npm init -y;  npm i express
来源：http://vz.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://ws.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xy.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://sj.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ww.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://en.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uh.nicolike.cn

[U85] JS：可选链
来源：http://lg.gzmigu.cn

a?.b?.c
来源：http://qm.szxytkj.cn

[U86] JS：空值合并
来源：http://ag.bookmarksfly.cn

a ?? b
来源：http://mz.jctech888.com.cn

[U87] JS：解构默认值
来源：http://wj.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://xn.hnjuh.cn

[U88] JS：对象展开合并
来源：http://nn.9csxet.cn

{ ...a, ...b }
来源：http://ce.newstarts.cn

[U89] JS：数组去重
来源：http://qw.szsharing.cn

[...new Set(arr)]
来源：http://hb.521024.cn

[U90] JS：数字数组排序
来源：http://dv.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://td.newstarts.cn

[U91] JS：对象键值遍历
来源：http://ry.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yq.gzmigu.cn

[U92] JS：深拷贝
来源：http://uh.9csxet.cn

structuredClone(obj)
来源：http://oj.panjiajie.cn

[U93] JS：模板字符串
来源：http://kp.wgjwhj.cn

`共 ${n} 条`
来源：http://al.shtwfgs.cn

[U94] JS：箭头函数
来源：http://yh.szsharing.cn

const double = x => x * 2;
来源：http://aw.9csxet.cn

[U95] JS：Promise 包装
来源：http://th.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://le.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://zk.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://op.shxzukj.cn

[U97] JS：并发请求
来源：http://wk.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nm.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://zr.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ah.nszjky.cn

[U99] JS：事件监听
来源：http://tz.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://zo.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://dx.asd995.cn

document.querySelector(".item")
来源：http://tl.lnxyls.cn

[U101] JS：classList 操作
来源：http://zu.bookmarksfly.cn

el.classList.toggle("active")
来源：http://ju.wgjwhj.cn

[U102] JS：本地存储
来源：http://dm.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nd.huixiangedu.cn

[U103] JS：定时器
来源：http://jy.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zk.nszjky.cn

[U104] JS：防抖
来源：http://jw.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jp.shxzukj.cn

[U105] JS：节流
来源：http://mu.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fv.asd995.cn

[U106] JS：日期格式化
来源：http://mk.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mt.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://mv.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mo.shxzskj.cn

[U108] JS：随机整数
来源：http://kv.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ut.lnxyls.cn

[U109] JS：数组分组
来源：http://rt.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://yp.nicolike.cn

[U110] JS：数组分块
来源：http://hc.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ww.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ee.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://mc.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://zj.haigaiapp.cn

"7".padStart(3, "0")
来源：http://wl.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://kk.colortex.cn

s.replaceAll("a", "b")
来源：http://fm.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://bv.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kw.lnxyls.cn

[U115] JS：生成 UUID
来源：http://my.yuntaijiaju.cn

crypto.randomUUID()
来源：http://wb.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://hq.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://im.asd995.cn

[U117] JS：单元测试
来源：http://le.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://dr.huixiangedu.cn

[U118] JS：开发服务器
来源：http://ib.hahajie.cn

npm i -D vite;  npx vite
来源：http://ci.bookmarksfly.cn

[U119] JS：生产构建
来源：http://vf.shxzskj.cn

npx vite build
来源：http://gf.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://gi.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://uo.haigaiapp.cn

================================================================================
来源：http://ai.huanxung.cn

统计汇总
来源：http://vr.jctech888.com.cn

================================================================================
来源：http://dx.hnjuh.cn

按语言统计（条）：
来源：http://pv.521024.cn

Python ......... 252
来源：http://wg.nszjky.cn

PHP ............ 252
来源：http://zn.gzmigu.cn

JavaScript ..... 252
来源：http://hx.lnxyls.cn

TypeScript ..... 212
来源：http://yf.szxytkj.cn

Java ........... 212
来源：http://ke.shxzskj.cn

Go ............. 212
来源：http://gi.521024.cn

Ruby ........... 212
来源：http://dx.shxzukj.cn

C# ............. 212
来源：http://ax.jianghongdianzi.cn

C .............. 30
来源：http://dh.nszjky.cn

C++ ............ 30
来源：http://xw.huanxung.cn

SQL ............ 90
来源：http://hj.shxzukj.cn

Bash ........... 80
来源：http://jj.wgjwhj.cn

Kotlin ......... 15
来源：http://xd.lnxyls.cn

Swift .......... 15
来源：http://xm.huanxung.cn

Lua ............ 10
来源：http://ox.haigaiapp.cn

Perl ........... 10
来源：http://ju.asd995.cn

Scala .......... 10
来源：http://sf.521024.cn

------------------------------------
来源：http://rr.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://fj.panjiajie.cn

按章节统计：
来源：http://pg.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cz.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oc.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uv.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kf.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ts.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gy.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fn.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sz.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://op.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pk.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hv.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jd.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ka.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zo.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dy.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bj.muxihuayi.cn


<!-- 参考信息 -->