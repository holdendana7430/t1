代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://fb.colortex.cn

[T51] Scala：Hello World
来源：http://bk.yuntaijiaju.cn

println("Hello")
来源：http://yb.bjjhwx.cn

[T52] Scala：变量
来源：http://ed.panjiajie.cn

val a = 1;  var b = 2
来源：http://zz.panjiajie.cn

[T53] Scala：字符串插值
来源：http://li.newstarts.cn

s"值: $b"
来源：http://rc.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://vi.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ed.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://rv.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mp.521024.cn

[T56] Scala：样例类
来源：http://ga.panjiajie.cn

case class User(name: String, age: Int)
来源：http://cs.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://uv.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tr.muxihuayi.cn

[T58] Scala：函数定义
来源：http://pc.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iu.szsharing.cn

[T59] Scala：循环
来源：http://bf.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://ra.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://yu.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bu.panjiajie.cn

================================================================================
来源：http://jh.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nz.yuexingan06.cn

================================================================================
来源：http://tt.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://ti.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nb.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://zx.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://as.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://br.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pr.panjiajie.cn

[U04] Py：变量调试打印
来源：http://ru.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fm.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://gi.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://gd.lnxyls.cn

[U06] Py：合并两个字典
来源：http://iw.chemitech.net.cn

{**a, **b}
来源：http://zi.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://ke.9csxet.cn

{v: k for k, v in d.items()}
来源：http://ki.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://mv.huanxung.cn

[y for x in nested for y in x]
来源：http://vd.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://rr.9csxet.cn

max(d, key=d.get)
来源：http://fl.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://zk.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cg.gzmigu.cn

[U11] Py：生成器表达式
来源：http://gw.lnxyls.cn

(x * 2 for x in arr)
来源：http://ly.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mw.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://ep.newstarts.cn

[U13] Py：固定长度队列
来源：http://eb.hnjuh.cn

deque(maxlen=10)
来源：http://mn.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://zh.huanxung.cn

defaultdict(list)
来源：http://tw.newstarts.cn

[U15] Py：高精度计时
来源：http://iu.nszjky.cn

t = time.perf_counter()
来源：http://cg.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://mq.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yw.haigaiapp.cn

[U17] Py：初始化日志
来源：http://ce.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://mv.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ww.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://do.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://ha.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xs.asd995.cn

[U20] Py：缓存函数结果
来源：http://xm.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://za.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://ur.haigaiapp.cn

@contextlib.contextmanager
来源：http://bu.newstarts.cn

[U22] Py：矩阵转置
来源：http://tl.shxzskj.cn

list(zip(*m))
来源：http://fe.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://kx.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xe.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ve.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ct.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://lm.jctech888.com.cn

csv.DictReader(f)
来源：http://fj.szxytkj.cn

[U26] Py：并发下载
来源：http://jl.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://se.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://bj.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://jx.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://vb.huanxung.cn

UserId = int
来源：http://hi.nszjky.cn

[U29] Py：属性校验
来源：http://bq.nszjky.cn

@property 与 @x.setter 配合
来源：http://bb.haigaiapp.cn

[U30] Py：数据类
来源：http://yx.szxytkj.cn

@dataclass(slots=True)
来源：http://xp.yuexingan06.cn

[U31] Py：单测
来源：http://cr.szxytkj.cn

python -m pytest -q
来源：http://bl.colortex.cn

[U32] Py：代码格式化
来源：http://il.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://az.nicolike.cn

[U33] Py：打包发布
来源：http://xd.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://yb.hahajie.cn

[U34] Py：判断编码
来源：http://hs.yuntaijiaju.cn

chardet.detect(raw)
来源：http://zj.9csxet.cn

[U35] Py：发送邮件
来源：http://rn.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ai.521024.cn

[U36] Py：定时任务
来源：http://xw.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://cr.newstarts.cn

[U37] Py：读写 Excel
来源：http://zd.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sv.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://zv.gzmigu.cn

Path(__file__).resolve().parent
来源：http://em.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://cd.colortex.cn

sys.stdout.isatty()
来源：http://ln.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://tx.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://xv.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://fz.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zw.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://xl.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://by.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://jy.yuntaijiaju.cn

namespace App\Http;
来源：http://tb.colortex.cn

[U44] PHP：开启严格类型
来源：http://ml.lnxyls.cn

declare(strict_types=1);
来源：http://gu.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://hz.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ra.521024.cn

[U46] PHP：可空类型
来源：http://oq.szxytkj.cn

?string $name = null
来源：http://ta.shtwfgs.cn

[U47] PHP：联合类型
来源：http://qj.jctech888.com.cn

int|string $id
来源：http://mq.asd995.cn

[U48] PHP：纯枚举
来源：http://up.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tq.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://hk.yuntaijiaju.cn

public readonly string $name
来源：http://tr.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://vl.huanxung.cn

public function __construct(private int $id) {}
来源：http://is.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ua.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://qx.9csxet.cn

[U52] PHP：箭头函数
来源：http://th.521024.cn

$double = fn($x) => $x * 2;
来源：http://jx.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://gu.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://in.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://vd.huixiangedu.cn

$obj?->method()
来源：http://hd.gzmigu.cn

[U55] PHP：match 表达式
来源：http://xr.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cj.wgjwhj.cn

[U56] PHP：命名参数
来源：http://rn.shxzskj.cn

f(a: 1, b: 2)
来源：http://bk.shxzukj.cn

[U57] PHP：字符串插值
来源：http://tv.bjjhwx.cn

"值: {$a}"
来源：http://pi.gzmigu.cn

[U58] PHP：数组三件套
来源：http://up.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jb.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://vh.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bk.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://kt.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bx.newstarts.cn

[U61] PHP：正则
来源：http://ff.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ep.hnjuh.cn

[U62] PHP：日期对象
来源：http://tw.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qb.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://wl.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zb.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://ol.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://sj.yuexingan06.cn

[U65] PHP：会话
来源：http://mj.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mb.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://mi.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dd.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://ev.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pk.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://gi.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://de.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://bb.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xl.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://jp.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gp.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://kt.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://mb.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://it.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://au.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://mp.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://an.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://bk.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://ge.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://cx.huixinmuqiang.cn

composer require psr/container
来源：http://kc.asd995.cn

[U76] PHP：简单路由
来源：http://fo.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iz.521024.cn

[U77] PHP：模板渲染
来源：http://hf.jctech888.com.cn

composer require twig/twig
来源：http://la.chemitech.net.cn

[U78] PHP：单元测试
来源：http://id.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://re.haigaiapp.cn

[U79] PHP：静态分析
来源：http://eb.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://hf.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://ok.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mi.chemitech.net.cn

[U81] JS：初始化项目
来源：http://ch.lnxyls.cn

npm init -y;  npm i express
来源：http://li.9csxet.cn

[U82] JS：package.json 脚本
来源：http://ib.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sh.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://bn.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nx.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://rz.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://de.hnjuh.cn

[U85] JS：可选链
来源：http://xv.haigaiapp.cn

a?.b?.c
来源：http://pv.hahajie.cn

[U86] JS：空值合并
来源：http://qe.szsharing.cn

a ?? b
来源：http://ee.521024.cn

[U87] JS：解构默认值
来源：http://sa.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://hj.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://ck.shtwfgs.cn

{ ...a, ...b }
来源：http://oa.hahajie.cn

[U89] JS：数组去重
来源：http://bu.nicolike.cn

[...new Set(arr)]
来源：http://io.nicolike.cn

[U90] JS：数字数组排序
来源：http://xb.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://jm.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://zr.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://az.jctech888.com.cn

[U92] JS：深拷贝
来源：http://dc.jctech888.com.cn

structuredClone(obj)
来源：http://bf.hnjuh.cn

[U93] JS：模板字符串
来源：http://gj.muxihuayi.cn

`共 ${n} 条`
来源：http://qn.wgjwhj.cn

[U94] JS：箭头函数
来源：http://zc.bookmarksfly.cn

const double = x => x * 2;
来源：http://ft.colortex.cn

[U95] JS：Promise 包装
来源：http://io.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://ea.asd995.cn

[U96] JS：async/await 与异常
来源：http://kj.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qa.wgjwhj.cn

[U97] JS：并发请求
来源：http://ru.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://by.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://fa.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cf.haigaiapp.cn

[U99] JS：事件监听
来源：http://it.hahajie.cn

el.addEventListener("click", e => {})
来源：http://nh.shxzskj.cn

[U100] JS：DOM 查询
来源：http://hf.szxytkj.cn

document.querySelector(".item")
来源：http://oz.gzmigu.cn

[U101] JS：classList 操作
来源：http://wu.hnjuh.cn

el.classList.toggle("active")
来源：http://sf.muxihuayi.cn

[U102] JS：本地存储
来源：http://wv.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qh.bjjhwx.cn

[U103] JS：定时器
来源：http://uv.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zc.9csxet.cn

[U104] JS：防抖
来源：http://ju.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.huixiangedu.cn

[U105] JS：节流
来源：http://vn.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hl.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://ba.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gq.gzmigu.cn

[U107] JS：数字千分位
来源：http://ii.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xt.wgjwhj.cn

[U108] JS：随机整数
来源：http://hn.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ca.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://rb.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://vu.hahajie.cn

[U110] JS：数组分块
来源：http://bg.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bn.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://rg.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://od.nszjky.cn

[U112] JS：字符串补位
来源：http://ci.nicolike.cn

"7".padStart(3, "0")
来源：http://fu.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ai.shxzukj.cn

s.replaceAll("a", "b")
来源：http://ne.huanxung.cn

[U114] JS：JSON 深比较
来源：http://ot.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ve.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://es.huanxung.cn

crypto.randomUUID()
来源：http://fw.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://vy.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://eh.huanxung.cn

[U117] JS：单元测试
来源：http://zq.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://sq.yuexingan06.cn

[U118] JS：开发服务器
来源：http://dn.gzmigu.cn

npm i -D vite;  npx vite
来源：http://gj.colortex.cn

[U119] JS：生产构建
来源：http://xu.muxihuayi.cn

npx vite build
来源：http://ii.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://qi.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://kh.hnjuh.cn

================================================================================
来源：http://pz.521024.cn

统计汇总
来源：http://tf.bjjhwx.cn

================================================================================
来源：http://hg.yuntaijiaju.cn

按语言统计（条）：
来源：http://nq.nicolike.cn

Python ......... 252
来源：http://rn.huixinmuqiang.cn

PHP ............ 252
来源：http://uq.shxzukj.cn

JavaScript ..... 252
来源：http://nl.jctech888.com.cn

TypeScript ..... 212
来源：http://da.shxzskj.cn

Java ........... 212
来源：http://vz.shxzukj.cn

Go ............. 212
来源：http://ot.haigaiapp.cn

Ruby ........... 212
来源：http://ok.jctech888.com.cn

C# ............. 212
来源：http://oc.521024.cn

C .............. 30
来源：http://ty.nicolike.cn

C++ ............ 30
来源：http://lh.shxzskj.cn

SQL ............ 90
来源：http://xe.lnxyls.cn

Bash ........... 80
来源：http://fx.newstarts.cn

Kotlin ......... 15
来源：http://pd.9csxet.cn

Swift .......... 15
来源：http://ch.huanxung.cn

Lua ............ 10
来源：http://vq.jctech888.com.cn

Perl ........... 10
来源：http://te.haigaiapp.cn

Scala .......... 10
来源：http://pa.lnxyls.cn

------------------------------------
来源：http://ab.szxytkj.cn

合计 ........... 2106 条
来源：http://xf.panjiajie.cn

按章节统计：
来源：http://ui.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ih.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bk.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wh.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zm.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ky.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ts.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fm.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jc.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sx.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xl.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gd.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nm.szxytkj.cn


<!-- 参考信息 -->