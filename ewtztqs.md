代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://qm.9csxet.cn

[T51] Scala：Hello World
来源：http://nq.shtwfgs.cn

println("Hello")
来源：http://np.panjiajie.cn

[T52] Scala：变量
来源：http://cv.9csxet.cn

val a = 1;  var b = 2
来源：http://id.nszjky.cn

[T53] Scala：字符串插值
来源：http://qo.muxihuayi.cn

s"值: $b"
来源：http://fr.chemitech.net.cn

[T54] Scala：集合映射
来源：http://oz.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://rk.panjiajie.cn

[T55] Scala：集合过滤
来源：http://mq.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lz.szsharing.cn

[T56] Scala：样例类
来源：http://wy.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://hj.szxytkj.cn

[T57] Scala：模式匹配
来源：http://dz.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bz.muxihuayi.cn

[T58] Scala：函数定义
来源：http://fn.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://he.nicolike.cn

[T59] Scala：循环
来源：http://wy.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://cf.bookmarksfly.cn

[T60] Scala：折叠
来源：http://jc.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oj.shtwfgs.cn

================================================================================
来源：http://xw.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eq.huixinmuqiang.cn

================================================================================
来源：http://il.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://za.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ve.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://dp.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://co.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://vo.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ib.521024.cn

[U04] Py：变量调试打印
来源：http://ad.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zy.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://po.newstarts.cn

list(dict.fromkeys(arr))
来源：http://og.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://gf.huixinmuqiang.cn

{**a, **b}
来源：http://wj.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://jo.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://ua.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://pl.shxzukj.cn

[y for x in nested for y in x]
来源：http://xr.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://yl.haigaiapp.cn

max(d, key=d.get)
来源：http://ev.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://wv.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ix.shxzskj.cn

[U11] Py：生成器表达式
来源：http://tu.521024.cn

(x * 2 for x in arr)
来源：http://iy.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ng.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://yx.szsharing.cn

[U13] Py：固定长度队列
来源：http://wm.huanxung.cn

deque(maxlen=10)
来源：http://tk.9csxet.cn

[U14] Py：分组收集到列表
来源：http://al.panjiajie.cn

defaultdict(list)
来源：http://bn.521024.cn

[U15] Py：高精度计时
来源：http://zm.hahajie.cn

t = time.perf_counter()
来源：http://ky.szsharing.cn

[U16] Py：命令行参数解析
来源：http://hk.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ve.hnjuh.cn

[U17] Py：初始化日志
来源：http://zh.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://qb.bjjhwx.cn

[U18] Py：预编译正则
来源：http://fz.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://kp.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://vy.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sy.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://wd.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://sa.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://ou.nszjky.cn

@contextlib.contextmanager
来源：http://mu.lnxyls.cn

[U22] Py：矩阵转置
来源：http://tz.huixinmuqiang.cn

list(zip(*m))
来源：http://gz.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://tr.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mb.shxzskj.cn

[U24] Py：路径操作
来源：http://tv.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ss.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://wy.jianghongdianzi.cn

csv.DictReader(f)
来源：http://kj.szxytkj.cn

[U26] Py：并发下载
来源：http://hh.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bv.hahajie.cn

[U27] Py：异步 HTTP
来源：http://tq.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://pn.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://eq.shtwfgs.cn

UserId = int
来源：http://lc.szxytkj.cn

[U29] Py：属性校验
来源：http://ix.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://pd.huixinmuqiang.cn

[U30] Py：数据类
来源：http://wt.yuexingan06.cn

@dataclass(slots=True)
来源：http://dv.nicolike.cn

[U31] Py：单测
来源：http://fl.nicolike.cn

python -m pytest -q
来源：http://ya.gzmigu.cn

[U32] Py：代码格式化
来源：http://bc.szsharing.cn

ruff format . && ruff check --fix .
来源：http://of.shxzukj.cn

[U33] Py：打包发布
来源：http://gw.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://zl.bjjhwx.cn

[U34] Py：判断编码
来源：http://sp.nicolike.cn

chardet.detect(raw)
来源：http://kg.szsharing.cn

[U35] Py：发送邮件
来源：http://xv.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oy.521024.cn

[U36] Py：定时任务
来源：http://wj.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://hm.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://hj.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wo.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://hw.colortex.cn

Path(__file__).resolve().parent
来源：http://ff.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://ia.colortex.cn

sys.stdout.isatty()
来源：http://hl.9csxet.cn

[U40] Py：打印到标准错误
来源：http://zr.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://cn.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://je.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tf.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://rg.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ks.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://cd.chemitech.net.cn

namespace App\Http;
来源：http://sb.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://mf.chemitech.net.cn

declare(strict_types=1);
来源：http://wz.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://yv.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xr.gzmigu.cn

[U46] PHP：可空类型
来源：http://av.chemitech.net.cn

?string $name = null
来源：http://zk.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://fa.huanxung.cn

int|string $id
来源：http://oz.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://vj.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sl.yuexingan06.cn

[U49] PHP：只读属性
来源：http://ov.szxytkj.cn

public readonly string $name
来源：http://ow.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://zu.asd995.cn

public function __construct(private int $id) {}
来源：http://ez.nicolike.cn

[U51] PHP：数组解构
来源：http://bc.bjjhwx.cn

[$a, $b] = $arr;
来源：http://ui.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://kk.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://mf.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://gx.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://bm.lnxyls.cn

[U54] PHP：空安全调用
来源：http://zx.shxzskj.cn

$obj?->method()
来源：http://mu.nicolike.cn

[U55] PHP：match 表达式
来源：http://ju.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ee.shtwfgs.cn

[U56] PHP：命名参数
来源：http://ja.hnjuh.cn

f(a: 1, b: 2)
来源：http://qf.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://lp.gzmigu.cn

"值: {$a}"
来源：http://ew.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://sm.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ni.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://es.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vn.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://tb.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ck.huixinmuqiang.cn

[U61] PHP：正则
来源：http://wa.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qs.nszjky.cn

[U62] PHP：日期对象
来源：http://dy.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jw.hahajie.cn

[U63] PHP：文件读写
来源：http://ez.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jz.newstarts.cn

[U64] PHP：目录遍历
来源：http://bq.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://sz.shxzukj.cn

[U65] PHP：会话
来源：http://sh.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ci.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://dl.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kw.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://sb.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pu.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://vz.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mw.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://nw.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dk.nicolike.cn

[U70] PHP：PDO 事务
来源：http://ku.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zs.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://jk.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://xf.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://si.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://tv.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://sk.asd995.cn

parse_ini_file("config.ini", true)
来源：http://ak.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://nd.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ec.newstarts.cn

[U75] PHP：依赖注入
来源：http://ab.shxzukj.cn

composer require psr/container
来源：http://vf.haigaiapp.cn

[U76] PHP：简单路由
来源：http://wf.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mz.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://xn.hahajie.cn

composer require twig/twig
来源：http://la.asd995.cn

[U78] PHP：单元测试
来源：http://lf.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://gd.hnjuh.cn

[U79] PHP：静态分析
来源：http://qz.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://ja.huanxung.cn

[U80] PHP：代码规范修复
来源：http://gs.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dt.lnxyls.cn

[U81] JS：初始化项目
来源：http://kk.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://rt.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://yx.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ia.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://nd.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oo.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://tm.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ys.shxzskj.cn

[U85] JS：可选链
来源：http://wp.hahajie.cn

a?.b?.c
来源：http://yb.wgjwhj.cn

[U86] JS：空值合并
来源：http://fh.bjjhwx.cn

a ?? b
来源：http://vb.yuexingan06.cn

[U87] JS：解构默认值
来源：http://ff.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://td.panjiajie.cn

[U88] JS：对象展开合并
来源：http://zt.hnjuh.cn

{ ...a, ...b }
来源：http://se.yuexingan06.cn

[U89] JS：数组去重
来源：http://og.asd995.cn

[...new Set(arr)]
来源：http://mu.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://gs.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://cm.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://un.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bn.nicolike.cn

[U92] JS：深拷贝
来源：http://zq.wgjwhj.cn

structuredClone(obj)
来源：http://bj.9csxet.cn

[U93] JS：模板字符串
来源：http://id.colortex.cn

`共 ${n} 条`
来源：http://an.panjiajie.cn

[U94] JS：箭头函数
来源：http://vk.huixiangedu.cn

const double = x => x * 2;
来源：http://ic.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://qd.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://gj.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://bt.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://of.gzmigu.cn

[U97] JS：并发请求
来源：http://tk.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://np.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://iz.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ew.nicolike.cn

[U99] JS：事件监听
来源：http://ft.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://ll.gzmigu.cn

[U100] JS：DOM 查询
来源：http://at.huixiangedu.cn

document.querySelector(".item")
来源：http://wi.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://kg.chemitech.net.cn

el.classList.toggle("active")
来源：http://sy.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://ew.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kv.newstarts.cn

[U103] JS：定时器
来源：http://ll.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yt.huanxung.cn

[U104] JS：防抖
来源：http://nh.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ie.bjjhwx.cn

[U105] JS：节流
来源：http://bc.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://np.huixiangedu.cn

[U106] JS：日期格式化
来源：http://fx.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aa.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://kt.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xr.asd995.cn

[U108] JS：随机整数
来源：http://ci.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uy.chemitech.net.cn

[U109] JS：数组分组
来源：http://ma.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://zg.jctech888.com.cn

[U110] JS：数组分块
来源：http://ws.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://or.hahajie.cn

[U111] JS：对象转 Map
来源：http://fq.lnxyls.cn

new Map(Object.entries(obj))
来源：http://ah.nszjky.cn

[U112] JS：字符串补位
来源：http://al.nicolike.cn

"7".padStart(3, "0")
来源：http://hd.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://io.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://do.9csxet.cn

[U114] JS：JSON 深比较
来源：http://sy.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ru.hnjuh.cn

[U115] JS：生成 UUID
来源：http://kk.bjjhwx.cn

crypto.randomUUID()
来源：http://nt.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://fv.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://kc.jctech888.com.cn

[U117] JS：单元测试
来源：http://dd.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://ei.szsharing.cn

[U118] JS：开发服务器
来源：http://dk.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://ig.jctech888.com.cn

[U119] JS：生产构建
来源：http://aj.bookmarksfly.cn

npx vite build
来源：http://cx.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://qs.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://yz.panjiajie.cn

================================================================================
来源：http://tj.asd995.cn

统计汇总
来源：http://jo.chemitech.net.cn

================================================================================
来源：http://tn.shxzskj.cn

按语言统计（条）：
来源：http://pw.yuexingan06.cn

Python ......... 252
来源：http://oh.panjiajie.cn

PHP ............ 252
来源：http://za.hnjuh.cn

JavaScript ..... 252
来源：http://xd.shxzskj.cn

TypeScript ..... 212
来源：http://ej.huixinmuqiang.cn

Java ........... 212
来源：http://wm.shxzskj.cn

Go ............. 212
来源：http://gp.colortex.cn

Ruby ........... 212
来源：http://lg.haigaiapp.cn

C# ............. 212
来源：http://ei.huixinmuqiang.cn

C .............. 30
来源：http://vm.szsharing.cn

C++ ............ 30
来源：http://dp.bjjhwx.cn

SQL ............ 90
来源：http://mz.hnjuh.cn

Bash ........... 80
来源：http://uk.shxzskj.cn

Kotlin ......... 15
来源：http://zb.521024.cn

Swift .......... 15
来源：http://ug.bjjhwx.cn

Lua ............ 10
来源：http://cq.asd995.cn

Perl ........... 10
来源：http://uf.huanxung.cn

Scala .......... 10
来源：http://xm.huixiangedu.cn

------------------------------------
来源：http://pm.521024.cn

合计 ........... 2106 条
来源：http://hh.gzmigu.cn

按章节统计：
来源：http://hx.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ru.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sn.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oq.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sp.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jr.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rv.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qx.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xb.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vs.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kg.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ot.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mr.jianghongdianzi.cn


<!-- 参考信息 -->