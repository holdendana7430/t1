代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://pz.chemitech.net.cn

[T51] Scala：Hello World
来源：http://gk.huixinmuqiang.cn

println("Hello")
来源：http://cx.newstarts.cn

[T52] Scala：变量
来源：http://ev.chemitech.net.cn

val a = 1;  var b = 2
来源：http://mf.szxytkj.cn

[T53] Scala：字符串插值
来源：http://bw.shxzukj.cn

s"值: $b"
来源：http://ol.asd995.cn

[T54] Scala：集合映射
来源：http://on.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://wv.colortex.cn

[T55] Scala：集合过滤
来源：http://ni.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wx.huanxung.cn

[T56] Scala：样例类
来源：http://fe.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://sx.newstarts.cn

[T57] Scala：模式匹配
来源：http://yb.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qw.chemitech.net.cn

[T58] Scala：函数定义
来源：http://oq.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://if.shxzukj.cn

[T59] Scala：循环
来源：http://ji.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://zh.asd995.cn

[T60] Scala：折叠
来源：http://cw.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ot.shtwfgs.cn

================================================================================
来源：http://qt.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qi.colortex.cn

================================================================================
来源：http://zo.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://kn.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ae.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://dk.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qn.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://gw.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pw.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://ms.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iq.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://fz.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://bh.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://fe.huanxung.cn

{**a, **b}
来源：http://rz.szxytkj.cn

[U07] Py：反转字典键值
来源：http://dn.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://dr.shxzukj.cn

[U08] Py：展平二维列表
来源：http://sl.newstarts.cn

[y for x in nested for y in x]
来源：http://se.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://bj.colortex.cn

max(d, key=d.get)
来源：http://lm.9csxet.cn

[U10] Py：按值排序字典
来源：http://nb.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cg.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://jt.9csxet.cn

(x * 2 for x in arr)
来源：http://it.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wi.shxzskj.cn

Counter(arr).most_common(3)
来源：http://mi.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ej.shtwfgs.cn

deque(maxlen=10)
来源：http://vn.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://pv.huixinmuqiang.cn

defaultdict(list)
来源：http://ny.szxytkj.cn

[U15] Py：高精度计时
来源：http://ry.haigaiapp.cn

t = time.perf_counter()
来源：http://gt.colortex.cn

[U16] Py：命令行参数解析
来源：http://yd.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ad.jctech888.com.cn

[U17] Py：初始化日志
来源：http://bq.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://on.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://hl.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://ja.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://jb.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hc.nicolike.cn

[U20] Py：缓存函数结果
来源：http://vb.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://ec.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://bj.bookmarksfly.cn

@contextlib.contextmanager
来源：http://cg.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://zt.hnjuh.cn

list(zip(*m))
来源：http://it.9csxet.cn

[U23] Py：分块读取大文件
来源：http://oj.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bu.chemitech.net.cn

[U24] Py：路径操作
来源：http://ul.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lo.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://lf.yuexingan06.cn

csv.DictReader(f)
来源：http://el.chemitech.net.cn

[U26] Py：并发下载
来源：http://hx.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jv.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://tj.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://uq.521024.cn

[U28] Py：类型别名
来源：http://fh.hnjuh.cn

UserId = int
来源：http://cy.bjjhwx.cn

[U29] Py：属性校验
来源：http://ai.colortex.cn

@property 与 @x.setter 配合
来源：http://qh.hahajie.cn

[U30] Py：数据类
来源：http://pw.shxzukj.cn

@dataclass(slots=True)
来源：http://fb.haigaiapp.cn

[U31] Py：单测
来源：http://pd.newstarts.cn

python -m pytest -q
来源：http://ws.muxihuayi.cn

[U32] Py：代码格式化
来源：http://jq.szsharing.cn

ruff format . && ruff check --fix .
来源：http://yk.521024.cn

[U33] Py：打包发布
来源：http://pd.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://dp.szxytkj.cn

[U34] Py：判断编码
来源：http://vq.haigaiapp.cn

chardet.detect(raw)
来源：http://ua.nszjky.cn

[U35] Py：发送邮件
来源：http://ob.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://in.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://af.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://tk.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://nx.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tc.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://eq.newstarts.cn

Path(__file__).resolve().parent
来源：http://nj.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://hi.nszjky.cn

sys.stdout.isatty()
来源：http://dh.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://zx.asd995.cn

print("err", file=sys.stderr)
来源：http://co.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://zs.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ax.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://jo.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dh.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://dh.yuntaijiaju.cn

namespace App\Http;
来源：http://ng.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://an.yuntaijiaju.cn

declare(strict_types=1);
来源：http://ks.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://ci.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ai.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://lj.shxzskj.cn

?string $name = null
来源：http://zm.nszjky.cn

[U47] PHP：联合类型
来源：http://vf.colortex.cn

int|string $id
来源：http://if.newstarts.cn

[U48] PHP：纯枚举
来源：http://sb.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qn.nszjky.cn

[U49] PHP：只读属性
来源：http://ao.szxytkj.cn

public readonly string $name
来源：http://rw.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://qh.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ji.shxzskj.cn

[U51] PHP：数组解构
来源：http://es.521024.cn

[$a, $b] = $arr;
来源：http://pt.hahajie.cn

[U52] PHP：箭头函数
来源：http://ox.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://uo.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://ii.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://uo.szsharing.cn

[U54] PHP：空安全调用
来源：http://cq.haigaiapp.cn

$obj?->method()
来源：http://im.9csxet.cn

[U55] PHP：match 表达式
来源：http://cd.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fk.gzmigu.cn

[U56] PHP：命名参数
来源：http://am.hnjuh.cn

f(a: 1, b: 2)
来源：http://qs.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://kn.bookmarksfly.cn

"值: {$a}"
来源：http://ka.panjiajie.cn

[U58] PHP：数组三件套
来源：http://hv.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xi.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://ci.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zo.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://ft.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ua.muxihuayi.cn

[U61] PHP：正则
来源：http://io.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ot.nszjky.cn

[U62] PHP：日期对象
来源：http://eu.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ih.9csxet.cn

[U63] PHP：文件读写
来源：http://js.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pp.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://zu.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://pc.szxytkj.cn

[U65] PHP：会话
来源：http://kj.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ys.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://ub.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jc.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://ok.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xd.newstarts.cn

[U68] PHP：PDO 连接
来源：http://mm.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xn.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://sv.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dj.nicolike.cn

[U70] PHP：PDO 事务
来源：http://qu.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wt.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://iq.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://cz.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://oj.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://go.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://hn.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://jq.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://af.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://eq.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://ar.hnjuh.cn

composer require psr/container
来源：http://wb.lnxyls.cn

[U76] PHP：简单路由
来源：http://lu.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nf.521024.cn

[U77] PHP：模板渲染
来源：http://rx.gzmigu.cn

composer require twig/twig
来源：http://li.jctech888.com.cn

[U78] PHP：单元测试
来源：http://iv.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://uv.9csxet.cn

[U79] PHP：静态分析
来源：http://rc.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://cg.nszjky.cn

[U80] PHP：代码规范修复
来源：http://yb.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bs.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://xp.bookmarksfly.cn

npm init -y;  npm i express
来源：http://zs.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://en.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tf.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://ky.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mt.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://dm.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xw.521024.cn

[U85] JS：可选链
来源：http://wf.panjiajie.cn

a?.b?.c
来源：http://vk.muxihuayi.cn

[U86] JS：空值合并
来源：http://mf.yuexingan06.cn

a ?? b
来源：http://qg.muxihuayi.cn

[U87] JS：解构默认值
来源：http://bn.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://dq.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://pf.bookmarksfly.cn

{ ...a, ...b }
来源：http://tl.haigaiapp.cn

[U89] JS：数组去重
来源：http://st.colortex.cn

[...new Set(arr)]
来源：http://uv.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://uf.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://it.newstarts.cn

[U91] JS：对象键值遍历
来源：http://yx.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cb.szxytkj.cn

[U92] JS：深拷贝
来源：http://zo.colortex.cn

structuredClone(obj)
来源：http://rk.chemitech.net.cn

[U93] JS：模板字符串
来源：http://az.huixinmuqiang.cn

`共 ${n} 条`
来源：http://wj.chemitech.net.cn

[U94] JS：箭头函数
来源：http://eg.hnjuh.cn

const double = x => x * 2;
来源：http://la.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://ee.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://ua.newstarts.cn

[U96] JS：async/await 与异常
来源：http://tb.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://df.hahajie.cn

[U97] JS：并发请求
来源：http://jd.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gg.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ex.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ss.shtwfgs.cn

[U99] JS：事件监听
来源：http://ka.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://am.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://ot.szsharing.cn

document.querySelector(".item")
来源：http://ih.szsharing.cn

[U101] JS：classList 操作
来源：http://mx.yuexingan06.cn

el.classList.toggle("active")
来源：http://il.shxzukj.cn

[U102] JS：本地存储
来源：http://bw.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rk.9csxet.cn

[U103] JS：定时器
来源：http://gk.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zq.shxzskj.cn

[U104] JS：防抖
来源：http://og.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ns.asd995.cn

[U105] JS：节流
来源：http://mc.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hc.521024.cn

[U106] JS：日期格式化
来源：http://vw.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zh.asd995.cn

[U107] JS：数字千分位
来源：http://pw.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cv.newstarts.cn

[U108] JS：随机整数
来源：http://gu.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hx.jctech888.com.cn

[U109] JS：数组分组
来源：http://ki.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://vn.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://qf.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uk.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://nt.newstarts.cn

new Map(Object.entries(obj))
来源：http://jx.yuexingan06.cn

[U112] JS：字符串补位
来源：http://hc.bjjhwx.cn

"7".padStart(3, "0")
来源：http://mz.shxzukj.cn

[U113] JS：正则替换全部
来源：http://kh.shxzskj.cn

s.replaceAll("a", "b")
来源：http://bi.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://tg.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://om.nicolike.cn

[U115] JS：生成 UUID
来源：http://oo.521024.cn

crypto.randomUUID()
来源：http://ub.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://hc.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://pa.hahajie.cn

[U117] JS：单元测试
来源：http://gk.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://zn.newstarts.cn

[U118] JS：开发服务器
来源：http://cx.panjiajie.cn

npm i -D vite;  npx vite
来源：http://qv.panjiajie.cn

[U119] JS：生产构建
来源：http://fn.asd995.cn

npx vite build
来源：http://kv.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://ay.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://db.jianghongdianzi.cn

================================================================================
来源：http://nf.asd995.cn

统计汇总
来源：http://pb.shxzukj.cn

================================================================================
来源：http://al.huixiangedu.cn

按语言统计（条）：
来源：http://uu.shxzskj.cn

Python ......... 252
来源：http://ct.bjjhwx.cn

PHP ............ 252
来源：http://lh.bookmarksfly.cn

JavaScript ..... 252
来源：http://ke.lnxyls.cn

TypeScript ..... 212
来源：http://er.huixiangedu.cn

Java ........... 212
来源：http://ij.chemitech.net.cn

Go ............. 212
来源：http://hs.szxytkj.cn

Ruby ........... 212
来源：http://ed.shxzskj.cn

C# ............. 212
来源：http://lz.shtwfgs.cn

C .............. 30
来源：http://qb.jianghongdianzi.cn

C++ ............ 30
来源：http://mq.nszjky.cn

SQL ............ 90
来源：http://kj.yuntaijiaju.cn

Bash ........... 80
来源：http://pj.jianghongdianzi.cn

Kotlin ......... 15
来源：http://fo.nicolike.cn

Swift .......... 15
来源：http://uu.yuntaijiaju.cn

Lua ............ 10
来源：http://ul.hahajie.cn

Perl ........... 10
来源：http://vs.szsharing.cn

Scala .......... 10
来源：http://gc.jianghongdianzi.cn

------------------------------------
来源：http://ll.shxzskj.cn

合计 ........... 2106 条
来源：http://fz.shtwfgs.cn

按章节统计：
来源：http://fe.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fs.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yp.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cu.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rm.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rb.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ug.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nr.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ag.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vf.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rg.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uw.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gn.9csxet.cn


<!-- 参考信息 -->