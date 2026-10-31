代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://lq.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://tu.chemitech.net.cn

println("Hello")
来源：http://fe.gzmigu.cn

[T52] Scala：变量
来源：http://xv.gzmigu.cn

val a = 1;  var b = 2
来源：http://qs.gzmigu.cn

[T53] Scala：字符串插值
来源：http://um.chemitech.net.cn

s"值: $b"
来源：http://zu.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://lt.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ae.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://tm.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oq.bookmarksfly.cn

[T56] Scala：样例类
来源：http://nt.huanxung.cn

case class User(name: String, age: Int)
来源：http://zc.szsharing.cn

[T57] Scala：模式匹配
来源：http://ds.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cf.szsharing.cn

[T58] Scala：函数定义
来源：http://hf.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lh.muxihuayi.cn

[T59] Scala：循环
来源：http://px.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://gb.szsharing.cn

[T60] Scala：折叠
来源：http://yy.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lp.jctech888.com.cn

================================================================================
来源：http://hn.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iy.huanxung.cn

================================================================================
来源：http://uw.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://xz.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fp.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://yy.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vp.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://pm.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kj.hnjuh.cn

[U04] Py：变量调试打印
来源：http://se.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jg.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://ux.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://sy.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://or.haigaiapp.cn

{**a, **b}
来源：http://rx.shxzukj.cn

[U07] Py：反转字典键值
来源：http://bj.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://wi.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://zm.nszjky.cn

[y for x in nested for y in x]
来源：http://yd.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://ai.bjjhwx.cn

max(d, key=d.get)
来源：http://zw.asd995.cn

[U10] Py：按值排序字典
来源：http://gu.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sx.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://is.huanxung.cn

(x * 2 for x in arr)
来源：http://mn.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jn.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://rj.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://cm.muxihuayi.cn

deque(maxlen=10)
来源：http://wy.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://ht.colortex.cn

defaultdict(list)
来源：http://gy.hahajie.cn

[U15] Py：高精度计时
来源：http://gj.jianghongdianzi.cn

t = time.perf_counter()
来源：http://io.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://vv.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ep.shtwfgs.cn

[U17] Py：初始化日志
来源：http://jk.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://tc.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://rm.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://oy.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://ph.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bd.huanxung.cn

[U20] Py：缓存函数结果
来源：http://li.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://xi.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://cz.chemitech.net.cn

@contextlib.contextmanager
来源：http://oi.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://ri.szsharing.cn

list(zip(*m))
来源：http://ok.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://wg.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tm.nszjky.cn

[U24] Py：路径操作
来源：http://nb.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iy.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://sp.bookmarksfly.cn

csv.DictReader(f)
来源：http://og.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://ka.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mr.nszjky.cn

[U27] Py：异步 HTTP
来源：http://lc.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://mq.521024.cn

[U28] Py：类型别名
来源：http://if.nicolike.cn

UserId = int
来源：http://ic.shtwfgs.cn

[U29] Py：属性校验
来源：http://tg.shxzskj.cn

@property 与 @x.setter 配合
来源：http://cb.panjiajie.cn

[U30] Py：数据类
来源：http://bg.nszjky.cn

@dataclass(slots=True)
来源：http://ib.nicolike.cn

[U31] Py：单测
来源：http://uy.szxytkj.cn

python -m pytest -q
来源：http://hf.shtwfgs.cn

[U32] Py：代码格式化
来源：http://jb.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://kx.lnxyls.cn

[U33] Py：打包发布
来源：http://sj.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://kb.gzmigu.cn

[U34] Py：判断编码
来源：http://xo.huixiangedu.cn

chardet.detect(raw)
来源：http://on.szxytkj.cn

[U35] Py：发送邮件
来源：http://ub.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dm.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://fn.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://la.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://qr.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wf.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://so.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://as.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://hb.asd995.cn

sys.stdout.isatty()
来源：http://ya.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://gk.shxzskj.cn

print("err", file=sys.stderr)
来源：http://lo.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://ax.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pi.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://wn.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://su.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://av.yuntaijiaju.cn

namespace App\Http;
来源：http://yb.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://rx.9csxet.cn

declare(strict_types=1);
来源：http://jc.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://mp.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lv.hahajie.cn

[U46] PHP：可空类型
来源：http://sm.hahajie.cn

?string $name = null
来源：http://nc.bjjhwx.cn

[U47] PHP：联合类型
来源：http://xa.shtwfgs.cn

int|string $id
来源：http://nn.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://he.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rv.huanxung.cn

[U49] PHP：只读属性
来源：http://en.szxytkj.cn

public readonly string $name
来源：http://on.colortex.cn

[U50] PHP：构造器属性提升
来源：http://hm.shxzukj.cn

public function __construct(private int $id) {}
来源：http://un.szxytkj.cn

[U51] PHP：数组解构
来源：http://yk.panjiajie.cn

[$a, $b] = $arr;
来源：http://oc.nszjky.cn

[U52] PHP：箭头函数
来源：http://vf.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://to.9csxet.cn

[U53] PHP：空合并运算符
来源：http://at.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://nl.shxzukj.cn

[U54] PHP：空安全调用
来源：http://pv.yuntaijiaju.cn

$obj?->method()
来源：http://yk.szxytkj.cn

[U55] PHP：match 表达式
来源：http://wv.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yc.shtwfgs.cn

[U56] PHP：命名参数
来源：http://zz.asd995.cn

f(a: 1, b: 2)
来源：http://ur.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ln.newstarts.cn

"值: {$a}"
来源：http://df.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://jh.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cz.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://tr.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zl.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://ar.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xy.yuntaijiaju.cn

[U61] PHP：正则
来源：http://nk.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gr.hahajie.cn

[U62] PHP：日期对象
来源：http://jm.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cm.nicolike.cn

[U63] PHP：文件读写
来源：http://qy.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iy.521024.cn

[U64] PHP：目录遍历
来源：http://lm.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://nu.newstarts.cn

[U65] PHP：会话
来源：http://mt.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rk.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://mi.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dn.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://nr.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bx.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://qc.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lv.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://zz.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vs.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://xy.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dg.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://fq.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://pa.colortex.cn

[U72] PHP：写错误日志
来源：http://ez.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://px.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://zf.asd995.cn

parse_ini_file("config.ini", true)
来源：http://sz.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://wd.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://oc.shxzskj.cn

[U75] PHP：依赖注入
来源：http://gc.asd995.cn

composer require psr/container
来源：http://jz.panjiajie.cn

[U76] PHP：简单路由
来源：http://rq.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zz.shxzukj.cn

[U77] PHP：模板渲染
来源：http://zp.yuexingan06.cn

composer require twig/twig
来源：http://zb.muxihuayi.cn

[U78] PHP：单元测试
来源：http://lz.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://im.haigaiapp.cn

[U79] PHP：静态分析
来源：http://au.colortex.cn

composer require --dev phpstan/phpstan
来源：http://jq.hahajie.cn

[U80] PHP：代码规范修复
来源：http://fy.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://me.colortex.cn

[U81] JS：初始化项目
来源：http://ha.chemitech.net.cn

npm init -y;  npm i express
来源：http://ko.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://kd.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uq.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://fo.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sj.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://vk.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ko.asd995.cn

[U85] JS：可选链
来源：http://so.newstarts.cn

a?.b?.c
来源：http://si.szsharing.cn

[U86] JS：空值合并
来源：http://dr.asd995.cn

a ?? b
来源：http://cd.lnxyls.cn

[U87] JS：解构默认值
来源：http://id.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://si.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://pe.yuntaijiaju.cn

{ ...a, ...b }
来源：http://zw.shxzskj.cn

[U89] JS：数组去重
来源：http://gd.9csxet.cn

[...new Set(arr)]
来源：http://vc.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://fk.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://oi.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://qq.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bk.521024.cn

[U92] JS：深拷贝
来源：http://lu.chemitech.net.cn

structuredClone(obj)
来源：http://oe.huixiangedu.cn

[U93] JS：模板字符串
来源：http://im.szsharing.cn

`共 ${n} 条`
来源：http://rv.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://nd.9csxet.cn

const double = x => x * 2;
来源：http://ol.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ff.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://vf.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://kk.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bj.nszjky.cn

[U97] JS：并发请求
来源：http://mx.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pc.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://hh.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vz.nszjky.cn

[U99] JS：事件监听
来源：http://vt.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://vd.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://do.newstarts.cn

document.querySelector(".item")
来源：http://mf.shtwfgs.cn

[U101] JS：classList 操作
来源：http://xc.huixiangedu.cn

el.classList.toggle("active")
来源：http://uw.hahajie.cn

[U102] JS：本地存储
来源：http://gx.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hm.yuexingan06.cn

[U103] JS：定时器
来源：http://xn.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wf.yuexingan06.cn

[U104] JS：防抖
来源：http://je.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bx.nicolike.cn

[U105] JS：节流
来源：http://at.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aj.gzmigu.cn

[U106] JS：日期格式化
来源：http://wt.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gf.wgjwhj.cn

[U107] JS：数字千分位
来源：http://hi.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xg.panjiajie.cn

[U108] JS：随机整数
来源：http://vo.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jv.szxytkj.cn

[U109] JS：数组分组
来源：http://ke.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://es.haigaiapp.cn

[U110] JS：数组分块
来源：http://ic.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fl.nszjky.cn

[U111] JS：对象转 Map
来源：http://tw.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://fc.yuexingan06.cn

[U112] JS：字符串补位
来源：http://ty.chemitech.net.cn

"7".padStart(3, "0")
来源：http://qd.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://cm.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://hx.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://um.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dz.hahajie.cn

[U115] JS：生成 UUID
来源：http://lm.szxytkj.cn

crypto.randomUUID()
来源：http://ht.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://oe.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://wu.hnjuh.cn

[U117] JS：单元测试
来源：http://dx.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://di.nszjky.cn

[U118] JS：开发服务器
来源：http://bo.hahajie.cn

npm i -D vite;  npx vite
来源：http://lk.szsharing.cn

[U119] JS：生产构建
来源：http://ux.nszjky.cn

npx vite build
来源：http://jl.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://tr.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://ok.szsharing.cn

================================================================================
来源：http://qr.haigaiapp.cn

统计汇总
来源：http://wg.lnxyls.cn

================================================================================
来源：http://qc.huanxung.cn

按语言统计（条）：
来源：http://jk.panjiajie.cn

Python ......... 252
来源：http://ki.wgjwhj.cn

PHP ............ 252
来源：http://iq.jctech888.com.cn

JavaScript ..... 252
来源：http://iy.hnjuh.cn

TypeScript ..... 212
来源：http://qo.jianghongdianzi.cn

Java ........... 212
来源：http://gr.521024.cn

Go ............. 212
来源：http://io.nicolike.cn

Ruby ........... 212
来源：http://gw.bookmarksfly.cn

C# ............. 212
来源：http://ju.jctech888.com.cn

C .............. 30
来源：http://ot.haigaiapp.cn

C++ ............ 30
来源：http://fl.jctech888.com.cn

SQL ............ 90
来源：http://ls.jctech888.com.cn

Bash ........... 80
来源：http://dv.jctech888.com.cn

Kotlin ......... 15
来源：http://mm.9csxet.cn

Swift .......... 15
来源：http://ug.9csxet.cn

Lua ............ 10
来源：http://yh.shxzukj.cn

Perl ........... 10
来源：http://yg.huanxung.cn

Scala .......... 10
来源：http://rf.haigaiapp.cn

------------------------------------
来源：http://ib.yuexingan06.cn

合计 ........... 2106 条
来源：http://nw.chemitech.net.cn

按章节统计：
来源：http://ye.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tq.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://av.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ld.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uo.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vy.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://re.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ji.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vc.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oz.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cq.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://db.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sf.haigaiapp.cn


<!-- 参考信息 -->