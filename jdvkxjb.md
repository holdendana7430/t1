代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://xi.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ts.9csxet.cn

println("Hello")
来源：http://la.yuntaijiaju.cn

[T52] Scala：变量
来源：http://vg.colortex.cn

val a = 1;  var b = 2
来源：http://ia.lnxyls.cn

[T53] Scala：字符串插值
来源：http://ti.nszjky.cn

s"值: $b"
来源：http://zs.szxytkj.cn

[T54] Scala：集合映射
来源：http://hj.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ch.shxzskj.cn

[T55] Scala：集合过滤
来源：http://pi.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zf.yuexingan06.cn

[T56] Scala：样例类
来源：http://ty.hahajie.cn

case class User(name: String, age: Int)
来源：http://tk.lnxyls.cn

[T57] Scala：模式匹配
来源：http://xl.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ls.newstarts.cn

[T58] Scala：函数定义
来源：http://ie.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pi.shxzskj.cn

[T59] Scala：循环
来源：http://qu.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://mw.shtwfgs.cn

[T60] Scala：折叠
来源：http://bz.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://db.chemitech.net.cn

================================================================================
来源：http://uv.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ln.bookmarksfly.cn

================================================================================
来源：http://ec.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://da.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nt.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://om.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://an.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://sn.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hd.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://mo.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://le.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://nn.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://aj.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://rc.nicolike.cn

{**a, **b}
来源：http://mp.lnxyls.cn

[U07] Py：反转字典键值
来源：http://kp.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ga.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://jv.shtwfgs.cn

[y for x in nested for y in x]
来源：http://tx.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://gn.521024.cn

max(d, key=d.get)
来源：http://ht.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://dt.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://re.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ie.wgjwhj.cn

(x * 2 for x in arr)
来源：http://ct.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dc.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://xt.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://sg.lnxyls.cn

deque(maxlen=10)
来源：http://rs.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://yv.bookmarksfly.cn

defaultdict(list)
来源：http://zc.hnjuh.cn

[U15] Py：高精度计时
来源：http://cq.colortex.cn

t = time.perf_counter()
来源：http://qv.521024.cn

[U16] Py：命令行参数解析
来源：http://pb.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cd.lnxyls.cn

[U17] Py：初始化日志
来源：http://bm.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nn.chemitech.net.cn

[U18] Py：预编译正则
来源：http://zn.huanxung.cn

pat = re.compile(r"\d+")
来源：http://rl.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://wr.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://px.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ti.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ht.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://iq.huixiangedu.cn

@contextlib.contextmanager
来源：http://ad.panjiajie.cn

[U22] Py：矩阵转置
来源：http://qf.huixiangedu.cn

list(zip(*m))
来源：http://ld.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://aa.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yd.chemitech.net.cn

[U24] Py：路径操作
来源：http://if.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wy.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://mo.nicolike.cn

csv.DictReader(f)
来源：http://po.bookmarksfly.cn

[U26] Py：并发下载
来源：http://bo.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cw.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://bp.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://tx.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://qb.gzmigu.cn

UserId = int
来源：http://pv.asd995.cn

[U29] Py：属性校验
来源：http://zi.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://gk.jctech888.com.cn

[U30] Py：数据类
来源：http://lf.chemitech.net.cn

@dataclass(slots=True)
来源：http://db.gzmigu.cn

[U31] Py：单测
来源：http://sz.yuntaijiaju.cn

python -m pytest -q
来源：http://id.muxihuayi.cn

[U32] Py：代码格式化
来源：http://wg.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://rt.nszjky.cn

[U33] Py：打包发布
来源：http://mq.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://cw.521024.cn

[U34] Py：判断编码
来源：http://zf.szxytkj.cn

chardet.detect(raw)
来源：http://bw.521024.cn

[U35] Py：发送邮件
来源：http://bq.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zm.shxzukj.cn

[U36] Py：定时任务
来源：http://mi.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://lg.gzmigu.cn

[U37] Py：读写 Excel
来源：http://ww.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uf.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://tu.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://gy.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ls.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://dj.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://hf.newstarts.cn

print("err", file=sys.stderr)
来源：http://mu.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://em.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ur.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://fa.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sg.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://wp.newstarts.cn

namespace App\Http;
来源：http://dh.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://jj.521024.cn

declare(strict_types=1);
来源：http://eq.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://rs.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://di.gzmigu.cn

[U46] PHP：可空类型
来源：http://an.hnjuh.cn

?string $name = null
来源：http://ld.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://fq.shxzukj.cn

int|string $id
来源：http://bu.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://ad.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rz.nszjky.cn

[U49] PHP：只读属性
来源：http://rf.haigaiapp.cn

public readonly string $name
来源：http://qa.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://xn.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://dc.newstarts.cn

[U51] PHP：数组解构
来源：http://yo.szxytkj.cn

[$a, $b] = $arr;
来源：http://yj.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://fd.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://du.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://if.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://qr.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ri.colortex.cn

$obj?->method()
来源：http://kj.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ni.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rv.shxzukj.cn

[U56] PHP：命名参数
来源：http://tm.szsharing.cn

f(a: 1, b: 2)
来源：http://ob.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://pv.chemitech.net.cn

"值: {$a}"
来源：http://sn.nicolike.cn

[U58] PHP：数组三件套
来源：http://rv.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://un.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://ih.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://si.521024.cn

[U60] PHP：JSON 编解码
来源：http://yr.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zv.lnxyls.cn

[U61] PHP：正则
来源：http://vn.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rl.szxytkj.cn

[U62] PHP：日期对象
来源：http://ot.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mc.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://fr.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yh.hahajie.cn

[U64] PHP：目录遍历
来源：http://ss.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://dq.yuntaijiaju.cn

[U65] PHP：会话
来源：http://qk.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pf.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://sk.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://py.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://zx.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ad.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://tg.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uc.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://nw.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rc.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://vh.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sx.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://di.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://pr.szsharing.cn

[U72] PHP：写错误日志
来源：http://af.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://ie.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://db.colortex.cn

parse_ini_file("config.ini", true)
来源：http://wv.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://ch.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://qa.asd995.cn

[U75] PHP：依赖注入
来源：http://wb.bjjhwx.cn

composer require psr/container
来源：http://tu.shtwfgs.cn

[U76] PHP：简单路由
来源：http://ag.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mt.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://jk.bookmarksfly.cn

composer require twig/twig
来源：http://xn.bjjhwx.cn

[U78] PHP：单元测试
来源：http://rg.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://le.hnjuh.cn

[U79] PHP：静态分析
来源：http://vc.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://km.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://jd.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uj.asd995.cn

[U81] JS：初始化项目
来源：http://sd.muxihuayi.cn

npm init -y;  npm i express
来源：http://kf.asd995.cn

[U82] JS：package.json 脚本
来源：http://ev.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ah.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://bz.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kg.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://fk.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yf.chemitech.net.cn

[U85] JS：可选链
来源：http://sz.panjiajie.cn

a?.b?.c
来源：http://nb.chemitech.net.cn

[U86] JS：空值合并
来源：http://mk.yuexingan06.cn

a ?? b
来源：http://df.chemitech.net.cn

[U87] JS：解构默认值
来源：http://pu.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://mn.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://md.yuexingan06.cn

{ ...a, ...b }
来源：http://th.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://pi.yuexingan06.cn

[...new Set(arr)]
来源：http://dk.shxzskj.cn

[U90] JS：数字数组排序
来源：http://gi.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://do.asd995.cn

[U91] JS：对象键值遍历
来源：http://dl.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ka.shxzskj.cn

[U92] JS：深拷贝
来源：http://fm.nszjky.cn

structuredClone(obj)
来源：http://gz.jctech888.com.cn

[U93] JS：模板字符串
来源：http://oi.huanxung.cn

`共 ${n} 条`
来源：http://kv.bjjhwx.cn

[U94] JS：箭头函数
来源：http://dp.nszjky.cn

const double = x => x * 2;
来源：http://tn.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://bl.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://fr.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://zk.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qv.chemitech.net.cn

[U97] JS：并发请求
来源：http://xk.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://de.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://eb.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zs.haigaiapp.cn

[U99] JS：事件监听
来源：http://hp.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://hh.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://bk.yuexingan06.cn

document.querySelector(".item")
来源：http://uh.szxytkj.cn

[U101] JS：classList 操作
来源：http://cj.nicolike.cn

el.classList.toggle("active")
来源：http://vj.gzmigu.cn

[U102] JS：本地存储
来源：http://ft.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vd.asd995.cn

[U103] JS：定时器
来源：http://qb.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ol.szsharing.cn

[U104] JS：防抖
来源：http://xi.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dg.yuexingan06.cn

[U105] JS：节流
来源：http://km.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zy.haigaiapp.cn

[U106] JS：日期格式化
来源：http://kt.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uw.521024.cn

[U107] JS：数字千分位
来源：http://iu.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lw.shtwfgs.cn

[U108] JS：随机整数
来源：http://xh.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dn.wgjwhj.cn

[U109] JS：数组分组
来源：http://rn.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://be.szsharing.cn

[U110] JS：数组分块
来源：http://oa.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sw.hahajie.cn

[U111] JS：对象转 Map
来源：http://xv.colortex.cn

new Map(Object.entries(obj))
来源：http://yx.colortex.cn

[U112] JS：字符串补位
来源：http://bv.yuexingan06.cn

"7".padStart(3, "0")
来源：http://mf.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://aa.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://dr.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://xh.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eu.newstarts.cn

[U115] JS：生成 UUID
来源：http://ck.huixiangedu.cn

crypto.randomUUID()
来源：http://rb.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://km.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://ol.newstarts.cn

[U117] JS：单元测试
来源：http://uf.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://xi.jctech888.com.cn

[U118] JS：开发服务器
来源：http://rz.521024.cn

npm i -D vite;  npx vite
来源：http://tw.huanxung.cn

[U119] JS：生产构建
来源：http://mj.huixinmuqiang.cn

npx vite build
来源：http://lq.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://kf.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://mj.asd995.cn

================================================================================
来源：http://dd.panjiajie.cn

统计汇总
来源：http://fv.yuexingan06.cn

================================================================================
来源：http://lp.lnxyls.cn

按语言统计（条）：
来源：http://zq.shtwfgs.cn

Python ......... 252
来源：http://za.jctech888.com.cn

PHP ............ 252
来源：http://te.nicolike.cn

JavaScript ..... 252
来源：http://sr.shxzukj.cn

TypeScript ..... 212
来源：http://ri.szxytkj.cn

Java ........... 212
来源：http://rp.hnjuh.cn

Go ............. 212
来源：http://wa.bookmarksfly.cn

Ruby ........... 212
来源：http://ei.szsharing.cn

C# ............. 212
来源：http://rk.panjiajie.cn

C .............. 30
来源：http://ae.szsharing.cn

C++ ............ 30
来源：http://ix.huanxung.cn

SQL ............ 90
来源：http://zx.bjjhwx.cn

Bash ........... 80
来源：http://wl.521024.cn

Kotlin ......... 15
来源：http://bc.huixiangedu.cn

Swift .......... 15
来源：http://vo.lnxyls.cn

Lua ............ 10
来源：http://sq.muxihuayi.cn

Perl ........... 10
来源：http://vz.yuntaijiaju.cn

Scala .......... 10
来源：http://tj.gzmigu.cn

------------------------------------
来源：http://jz.jctech888.com.cn

合计 ........... 2106 条
来源：http://xj.hahajie.cn

按章节统计：
来源：http://ni.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wi.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://om.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ys.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gi.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kh.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ri.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ao.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://up.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ni.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yd.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dy.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://my.lnxyls.cn


<!-- 参考信息 -->