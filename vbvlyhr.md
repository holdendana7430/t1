代发 wailian999

val a = 1;  var b = 2
来源：http://at.colortex.cn

[T53] Scala：字符串插值
来源：http://tg.lnxyls.cn

s"值: $b"
来源：http://bj.muxihuayi.cn

[T54] Scala：集合映射
来源：http://pz.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://sl.nszjky.cn

[T55] Scala：集合过滤
来源：http://ov.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tv.gzmigu.cn

[T56] Scala：样例类
来源：http://hj.panjiajie.cn

case class User(name: String, age: Int)
来源：http://tl.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://vk.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yh.wgjwhj.cn

[T58] Scala：函数定义
来源：http://cz.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://us.newstarts.cn

[T59] Scala：循环
来源：http://af.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://gm.gzmigu.cn

[T60] Scala：折叠
来源：http://mh.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ya.asd995.cn

================================================================================
来源：http://jl.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hb.yuntaijiaju.cn

================================================================================
来源：http://nd.asd995.cn

[U01] Py：创建虚拟环境
来源：http://ot.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yo.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://gi.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yl.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://gl.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://un.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://gf.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rk.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://hu.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ow.gzmigu.cn

[U06] Py：合并两个字典
来源：http://mv.shxzukj.cn

{**a, **b}
来源：http://ve.szxytkj.cn

[U07] Py：反转字典键值
来源：http://nc.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://je.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://rz.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://js.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://ai.521024.cn

max(d, key=d.get)
来源：http://lh.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://si.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vk.hnjuh.cn

[U11] Py：生成器表达式
来源：http://yd.muxihuayi.cn

(x * 2 for x in arr)
来源：http://uc.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ke.nicolike.cn

Counter(arr).most_common(3)
来源：http://zf.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://jh.lnxyls.cn

deque(maxlen=10)
来源：http://np.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://ez.bjjhwx.cn

defaultdict(list)
来源：http://yr.chemitech.net.cn

[U15] Py：高精度计时
来源：http://yc.9csxet.cn

t = time.perf_counter()
来源：http://kg.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://cd.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lp.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://pc.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://wo.muxihuayi.cn

[U18] Py：预编译正则
来源：http://hu.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ut.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://pl.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rx.newstarts.cn

[U20] Py：缓存函数结果
来源：http://ub.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://av.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://kz.521024.cn

@contextlib.contextmanager
来源：http://pg.asd995.cn

[U22] Py：矩阵转置
来源：http://wa.yuexingan06.cn

list(zip(*m))
来源：http://cp.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://kq.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fl.panjiajie.cn

[U24] Py：路径操作
来源：http://zn.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://el.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://ps.yuexingan06.cn

csv.DictReader(f)
来源：http://za.hnjuh.cn

[U26] Py：并发下载
来源：http://hx.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ck.nicolike.cn

[U27] Py：异步 HTTP
来源：http://hz.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://vr.hnjuh.cn

[U28] Py：类型别名
来源：http://sg.shxzskj.cn

UserId = int
来源：http://sr.521024.cn

[U29] Py：属性校验
来源：http://kn.panjiajie.cn

@property 与 @x.setter 配合
来源：http://ge.shxzukj.cn

[U30] Py：数据类
来源：http://og.asd995.cn

@dataclass(slots=True)
来源：http://aj.yuexingan06.cn

[U31] Py：单测
来源：http://dl.9csxet.cn

python -m pytest -q
来源：http://kv.yuexingan06.cn

[U32] Py：代码格式化
来源：http://yf.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://bm.9csxet.cn

[U33] Py：打包发布
来源：http://eu.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://xn.szxytkj.cn

[U34] Py：判断编码
来源：http://au.haigaiapp.cn

chardet.detect(raw)
来源：http://rc.panjiajie.cn

[U35] Py：发送邮件
来源：http://yf.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xq.lnxyls.cn

[U36] Py：定时任务
来源：http://yb.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://gl.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://dv.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mo.521024.cn

[U38] Py：获取脚本所在目录
来源：http://ej.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://xb.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://gr.yuexingan06.cn

sys.stdout.isatty()
来源：http://ef.newstarts.cn

[U40] Py：打印到标准错误
来源：http://bz.nszjky.cn

print("err", file=sys.stderr)
来源：http://fa.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ni.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ee.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://qs.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lm.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://uo.wgjwhj.cn

namespace App\Http;
来源：http://ng.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://oa.jctech888.com.cn

declare(strict_types=1);
来源：http://fq.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://xl.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ly.huixiangedu.cn

[U46] PHP：可空类型
来源：http://mr.hahajie.cn

?string $name = null
来源：http://rm.shtwfgs.cn

[U47] PHP：联合类型
来源：http://uc.shtwfgs.cn

int|string $id
来源：http://we.hnjuh.cn

[U48] PHP：纯枚举
来源：http://oh.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zh.huanxung.cn

[U49] PHP：只读属性
来源：http://ai.nicolike.cn

public readonly string $name
来源：http://ql.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://bg.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://sg.nszjky.cn

[U51] PHP：数组解构
来源：http://gu.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://bg.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://hf.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://za.nszjky.cn

[U53] PHP：空合并运算符
来源：http://rv.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://mp.newstarts.cn

[U54] PHP：空安全调用
来源：http://ny.nicolike.cn

$obj?->method()
来源：http://tc.panjiajie.cn

[U55] PHP：match 表达式
来源：http://pq.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xh.521024.cn

[U56] PHP：命名参数
来源：http://gu.asd995.cn

f(a: 1, b: 2)
来源：http://ki.521024.cn

[U57] PHP：字符串插值
来源：http://gg.bookmarksfly.cn

"值: {$a}"
来源：http://fv.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://gy.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tc.521024.cn

[U59] PHP：自定义排序
来源：http://rg.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dm.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://fy.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ks.shxzukj.cn

[U61] PHP：正则
来源：http://va.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eh.hnjuh.cn

[U62] PHP：日期对象
来源：http://kj.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ms.jctech888.com.cn

[U63] PHP：文件读写
来源：http://wg.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bg.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://ln.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://mn.colortex.cn

[U65] PHP：会话
来源：http://zf.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yj.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://re.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wo.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://or.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ns.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://qs.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kh.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://jk.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dg.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://ph.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yu.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://gw.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://ip.521024.cn

[U72] PHP：写错误日志
来源：http://ua.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://kj.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://yn.asd995.cn

parse_ini_file("config.ini", true)
来源：http://cz.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://do.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://ii.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://um.colortex.cn

composer require psr/container
来源：http://ha.haigaiapp.cn

[U76] PHP：简单路由
来源：http://gv.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qz.521024.cn

[U77] PHP：模板渲染
来源：http://yh.szsharing.cn

composer require twig/twig
来源：http://su.shxzukj.cn

[U78] PHP：单元测试
来源：http://zu.521024.cn

composer require --dev phpunit/phpunit
来源：http://rj.muxihuayi.cn

[U79] PHP：静态分析
来源：http://mb.521024.cn

composer require --dev phpstan/phpstan
来源：http://ox.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://de.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://at.hnjuh.cn

[U81] JS：初始化项目
来源：http://et.jctech888.com.cn

npm init -y;  npm i express
来源：http://jb.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://yi.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xg.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://wz.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tx.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://gm.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ru.hnjuh.cn

[U85] JS：可选链
来源：http://fq.nicolike.cn

a?.b?.c
来源：http://pa.hnjuh.cn

[U86] JS：空值合并
来源：http://en.shxzukj.cn

a ?? b
来源：http://ug.9csxet.cn

[U87] JS：解构默认值
来源：http://ox.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://yl.nicolike.cn

[U88] JS：对象展开合并
来源：http://sk.huanxung.cn

{ ...a, ...b }
来源：http://ey.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://lc.shxzukj.cn

[...new Set(arr)]
来源：http://yb.521024.cn

[U90] JS：数字数组排序
来源：http://kp.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://cd.szsharing.cn

[U91] JS：对象键值遍历
来源：http://wm.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ov.shtwfgs.cn

[U92] JS：深拷贝
来源：http://do.huixiangedu.cn

structuredClone(obj)
来源：http://zs.huixiangedu.cn

[U93] JS：模板字符串
来源：http://qz.jctech888.com.cn

`共 ${n} 条`
来源：http://bx.bjjhwx.cn

[U94] JS：箭头函数
来源：http://vm.szsharing.cn

const double = x => x * 2;
来源：http://ne.9csxet.cn

[U95] JS：Promise 包装
来源：http://fa.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://bf.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://gp.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yh.shxzskj.cn

[U97] JS：并发请求
来源：http://cb.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ww.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://vw.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://st.521024.cn

[U99] JS：事件监听
来源：http://nh.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://gf.shxzskj.cn

[U100] JS：DOM 查询
来源：http://mq.bookmarksfly.cn

document.querySelector(".item")
来源：http://lf.newstarts.cn

[U101] JS：classList 操作
来源：http://iz.chemitech.net.cn

el.classList.toggle("active")
来源：http://xi.shxzskj.cn

[U102] JS：本地存储
来源：http://ct.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ka.yuexingan06.cn

[U103] JS：定时器
来源：http://ui.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mo.shxzukj.cn

[U104] JS：防抖
来源：http://jj.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://za.521024.cn

[U105] JS：节流
来源：http://lq.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pw.chemitech.net.cn

[U106] JS：日期格式化
来源：http://sw.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vd.huixiangedu.cn

[U107] JS：数字千分位
来源：http://yd.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://co.wgjwhj.cn

[U108] JS：随机整数
来源：http://ya.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://co.muxihuayi.cn

[U109] JS：数组分组
来源：http://oo.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://kj.shxzskj.cn

[U110] JS：数组分块
来源：http://ns.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zq.hnjuh.cn

[U111] JS：对象转 Map
来源：http://oc.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ix.jctech888.com.cn

[U112] JS：字符串补位
来源：http://uo.9csxet.cn

"7".padStart(3, "0")
来源：http://cl.521024.cn

[U113] JS：正则替换全部
来源：http://dr.hnjuh.cn

s.replaceAll("a", "b")
来源：http://nm.colortex.cn

[U114] JS：JSON 深比较
来源：http://qu.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qg.nicolike.cn

[U115] JS：生成 UUID
来源：http://be.huixiangedu.cn

crypto.randomUUID()
来源：http://ai.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://sg.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://sp.shxzukj.cn

[U117] JS：单元测试
来源：http://qc.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://yu.521024.cn

[U118] JS：开发服务器
来源：http://gz.521024.cn

npm i -D vite;  npx vite
来源：http://xr.shxzskj.cn

[U119] JS：生产构建
来源：http://ce.asd995.cn

npx vite build
来源：http://ru.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://mg.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://sr.gzmigu.cn

================================================================================
来源：http://uv.bjjhwx.cn

统计汇总
来源：http://uv.bookmarksfly.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

按语言统计（条）：
来源：http://ch.shxzukj.cn

Python ......... 252
来源：http://ij.huixiangedu.cn

PHP ............ 252
来源：http://oo.shxzskj.cn

JavaScript ..... 252
来源：http://sy.lnxyls.cn

TypeScript ..... 212
来源：http://sj.shtwfgs.cn

Java ........... 212
来源：http://am.huixinmuqiang.cn

Go ............. 212
来源：http://rb.shxzukj.cn

Ruby ........... 212
来源：http://og.nszjky.cn

C# ............. 212
来源：http://uf.haigaiapp.cn

C .............. 30
来源：http://nf.wgjwhj.cn

C++ ............ 30
来源：http://vv.521024.cn

SQL ............ 90
来源：http://qr.shxzukj.cn

Bash ........... 80
来源：http://uk.newstarts.cn

Kotlin ......... 15
来源：http://xm.chemitech.net.cn

Swift .......... 15
来源：http://ea.9csxet.cn

Lua ............ 10
来源：http://dk.521024.cn

Perl ........... 10
来源：http://cd.colortex.cn

Scala .......... 10
来源：http://pk.szsharing.cn

------------------------------------
来源：http://co.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://nn.521024.cn

按章节统计：
来源：http://hn.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bj.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ob.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uo.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ai.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gr.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wh.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cu.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dx.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ek.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vu.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gv.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gt.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qw.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sp.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vt.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dy.yuexingan06.cn


<!-- 参考信息 -->