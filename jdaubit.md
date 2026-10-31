代发 wailian999

case class User(name: String, age: Int)
来源：http://iu.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://bs.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vi.szxytkj.cn

[T58] Scala：函数定义
来源：http://ou.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jf.wgjwhj.cn

[T59] Scala：循环
来源：http://ua.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://tm.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ir.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jc.nszjky.cn

================================================================================
来源：http://um.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nx.szsharing.cn

================================================================================
来源：http://qf.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://oc.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dv.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://ok.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mf.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://tv.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dc.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ed.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tv.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://xt.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://fx.gzmigu.cn

[U06] Py：合并两个字典
来源：http://pd.bookmarksfly.cn

{**a, **b}
来源：http://iy.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://rs.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://ju.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://dh.huanxung.cn

[y for x in nested for y in x]
来源：http://py.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://rh.colortex.cn

max(d, key=d.get)
来源：http://fg.521024.cn

[U10] Py：按值排序字典
来源：http://zj.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jc.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://ph.huixiangedu.cn

(x * 2 for x in arr)
来源：http://ix.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qw.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://wx.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://bl.lnxyls.cn

deque(maxlen=10)
来源：http://qs.nszjky.cn

[U14] Py：分组收集到列表
来源：http://xw.jctech888.com.cn

defaultdict(list)
来源：http://ny.panjiajie.cn

[U15] Py：高精度计时
来源：http://xu.bookmarksfly.cn

t = time.perf_counter()
来源：http://aj.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://so.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hi.wgjwhj.cn

[U17] Py：初始化日志
来源：http://so.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://rm.nszjky.cn

[U18] Py：预编译正则
来源：http://os.521024.cn

pat = re.compile(r"\d+")
来源：http://ej.newstarts.cn

[U19] Py：正则替换带回调
来源：http://tv.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vf.nszjky.cn

[U20] Py：缓存函数结果
来源：http://ri.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://yf.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://ek.szsharing.cn

@contextlib.contextmanager
来源：http://pv.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://rx.szsharing.cn

list(zip(*m))
来源：http://kq.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://kk.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pm.panjiajie.cn

[U24] Py：路径操作
来源：http://er.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qg.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://lw.panjiajie.cn

csv.DictReader(f)
来源：http://vp.shxzukj.cn

[U26] Py：并发下载
来源：http://om.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hc.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://eo.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://or.jctech888.com.cn

[U28] Py：类型别名
来源：http://zr.wgjwhj.cn

UserId = int
来源：http://ct.9csxet.cn

[U29] Py：属性校验
来源：http://kl.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://na.panjiajie.cn

[U30] Py：数据类
来源：http://ge.521024.cn

@dataclass(slots=True)
来源：http://tq.jianghongdianzi.cn

[U31] Py：单测
来源：http://nc.newstarts.cn

python -m pytest -q
来源：http://zh.nszjky.cn

[U32] Py：代码格式化
来源：http://gd.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://dk.chemitech.net.cn

[U33] Py：打包发布
来源：http://fp.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://yi.chemitech.net.cn

[U34] Py：判断编码
来源：http://fl.nszjky.cn

chardet.detect(raw)
来源：http://or.nicolike.cn

[U35] Py：发送邮件
来源：http://lb.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wy.newstarts.cn

[U36] Py：定时任务
来源：http://lk.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://go.nicolike.cn

[U37] Py：读写 Excel
来源：http://ur.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gx.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://kr.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://dr.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://sk.szxytkj.cn

sys.stdout.isatty()
来源：http://mh.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://sh.shxzskj.cn

print("err", file=sys.stderr)
来源：http://rx.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://vh.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eu.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://li.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dl.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ej.panjiajie.cn

namespace App\Http;
来源：http://xr.nicolike.cn

[U44] PHP：开启严格类型
来源：http://ra.colortex.cn

declare(strict_types=1);
来源：http://lf.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://hc.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xt.lnxyls.cn

[U46] PHP：可空类型
来源：http://xx.shxzukj.cn

?string $name = null
来源：http://kc.muxihuayi.cn

[U47] PHP：联合类型
来源：http://ln.chemitech.net.cn

int|string $id
来源：http://wa.lnxyls.cn

[U48] PHP：纯枚举
来源：http://me.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://go.huanxung.cn

[U49] PHP：只读属性
来源：http://ke.szsharing.cn

public readonly string $name
来源：http://ss.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://cx.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://uk.9csxet.cn

[U51] PHP：数组解构
来源：http://bt.bjjhwx.cn

[$a, $b] = $arr;
来源：http://gr.lnxyls.cn

[U52] PHP：箭头函数
来源：http://gs.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://et.nszjky.cn

[U53] PHP：空合并运算符
来源：http://aw.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://jf.shxzukj.cn

[U54] PHP：空安全调用
来源：http://lb.shxzukj.cn

$obj?->method()
来源：http://lp.nszjky.cn

[U55] PHP：match 表达式
来源：http://mo.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ab.yuexingan06.cn

[U56] PHP：命名参数
来源：http://wm.szsharing.cn

f(a: 1, b: 2)
来源：http://fc.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ff.asd995.cn

"值: {$a}"
来源：http://qg.nszjky.cn

[U58] PHP：数组三件套
来源：http://ac.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zk.521024.cn

[U59] PHP：自定义排序
来源：http://af.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kl.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://dv.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yt.muxihuayi.cn

[U61] PHP：正则
来源：http://ar.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jm.shtwfgs.cn

[U62] PHP：日期对象
来源：http://uv.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cd.wgjwhj.cn

[U63] PHP：文件读写
来源：http://ns.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zp.shxzukj.cn

[U64] PHP：目录遍历
来源：http://go.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://io.panjiajie.cn

[U65] PHP：会话
来源：http://rw.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kl.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ze.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pw.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://uo.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wm.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://gz.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vb.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://jx.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vh.521024.cn

[U70] PHP：PDO 事务
来源：http://gl.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://by.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://tj.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://hd.szsharing.cn

[U72] PHP：写错误日志
来源：http://mp.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://ya.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://bj.521024.cn

parse_ini_file("config.ini", true)
来源：http://pr.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://kl.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://zt.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://xb.chemitech.net.cn

composer require psr/container
来源：http://zy.asd995.cn

[U76] PHP：简单路由
来源：http://qc.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bs.nszjky.cn

[U77] PHP：模板渲染
来源：http://hq.szsharing.cn

composer require twig/twig
来源：http://me.huixiangedu.cn

[U78] PHP：单元测试
来源：http://gi.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://sh.huixiangedu.cn

[U79] PHP：静态分析
来源：http://te.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://vq.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://bn.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nc.wgjwhj.cn

[U81] JS：初始化项目
来源：http://go.nszjky.cn

npm init -y;  npm i express
来源：http://gt.szsharing.cn

[U82] JS：package.json 脚本
来源：http://ap.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fd.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ab.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oj.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://jz.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ta.bookmarksfly.cn

[U85] JS：可选链
来源：http://sc.gzmigu.cn

a?.b?.c
来源：http://hr.szxytkj.cn

[U86] JS：空值合并
来源：http://gk.nszjky.cn

a ?? b
来源：http://gy.gzmigu.cn

[U87] JS：解构默认值
来源：http://wv.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://wi.szsharing.cn

[U88] JS：对象展开合并
来源：http://mb.bjjhwx.cn

{ ...a, ...b }
来源：http://xw.haigaiapp.cn

[U89] JS：数组去重
来源：http://ee.yuexingan06.cn

[...new Set(arr)]
来源：http://pr.colortex.cn

[U90] JS：数字数组排序
来源：http://yq.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://gr.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://lg.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ok.yuexingan06.cn

[U92] JS：深拷贝
来源：http://sa.hnjuh.cn

structuredClone(obj)
来源：http://qb.wgjwhj.cn

[U93] JS：模板字符串
来源：http://fx.521024.cn

`共 ${n} 条`
来源：http://fd.shtwfgs.cn

[U94] JS：箭头函数
来源：http://qe.jianghongdianzi.cn

const double = x => x * 2;
来源：http://um.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://kw.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://ob.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://pf.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ei.muxihuayi.cn

[U97] JS：并发请求
来源：http://gl.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kd.521024.cn

[U98] JS：fetch 带 JSON
来源：http://hf.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ps.shxzukj.cn

[U99] JS：事件监听
来源：http://zf.szsharing.cn

el.addEventListener("click", e => {})
来源：http://dz.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://pu.bjjhwx.cn

document.querySelector(".item")
来源：http://ek.gzmigu.cn

[U101] JS：classList 操作
来源：http://ha.huixiangedu.cn

el.classList.toggle("active")
来源：http://qj.jctech888.com.cn

[U102] JS：本地存储
来源：http://uh.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bg.yuexingan06.cn

[U103] JS：定时器
来源：http://ks.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://up.shxzukj.cn

[U104] JS：防抖
来源：http://lf.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jr.bjjhwx.cn

[U105] JS：节流
来源：http://xn.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://if.panjiajie.cn

[U106] JS：日期格式化
来源：http://ya.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ub.hnjuh.cn

[U107] JS：数字千分位
来源：http://tc.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ry.jctech888.com.cn

[U108] JS：随机整数
来源：http://ni.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ut.huanxung.cn

[U109] JS：数组分组
来源：http://gn.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://sf.panjiajie.cn

[U110] JS：数组分块
来源：http://mv.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ws.shxzukj.cn

[U111] JS：对象转 Map
来源：http://iv.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://dg.asd995.cn

[U112] JS：字符串补位
来源：http://lm.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://hq.panjiajie.cn

[U113] JS：正则替换全部
来源：http://vi.521024.cn

s.replaceAll("a", "b")
来源：http://nu.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://mq.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gc.szxytkj.cn

[U115] JS：生成 UUID
来源：http://ja.wgjwhj.cn

crypto.randomUUID()
来源：http://of.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://ho.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://nq.lnxyls.cn

[U117] JS：单元测试
来源：http://dk.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://br.nicolike.cn

[U118] JS：开发服务器
来源：http://ay.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://jq.colortex.cn

[U119] JS：生产构建
来源：http://si.yuntaijiaju.cn

npx vite build
来源：http://ge.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://pi.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://jz.huanxung.cn

================================================================================
来源：http://mt.panjiajie.cn

统计汇总
来源：http://zn.huixiangedu.cn

================================================================================
来源：http://rn.chemitech.net.cn

按语言统计（条）：
来源：http://iy.newstarts.cn

Python ......... 252
来源：http://au.muxihuayi.cn

PHP ............ 252
来源：http://ks.shxzskj.cn

JavaScript ..... 252
来源：http://lx.asd995.cn

TypeScript ..... 212
来源：http://fw.yuexingan06.cn

Java ........... 212
来源：http://fc.huanxung.cn

Go ............. 212
来源：http://zr.chemitech.net.cn

Ruby ........... 212
来源：http://vh.nszjky.cn

C# ............. 212
来源：http://nu.panjiajie.cn

C .............. 30
来源：http://zb.muxihuayi.cn

C++ ............ 30
来源：http://zh.chemitech.net.cn

SQL ............ 90
来源：http://kk.nicolike.cn

Bash ........... 80
来源：http://ne.hahajie.cn

Kotlin ......... 15
来源：http://ho.panjiajie.cn

Swift .......... 15
来源：http://ob.colortex.cn

Lua ............ 10
来源：http://um.panjiajie.cn

Perl ........... 10
来源：http://zi.bjjhwx.cn

Scala .......... 10
来源：http://lz.huixiangedu.cn

------------------------------------
来源：http://yc.shxzskj.cn

合计 ........... 2106 条
来源：http://bj.yuntaijiaju.cn

按章节统计：
来源：http://es.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jg.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pt.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jg.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ut.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ne.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wn.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bm.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sl.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yn.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ba.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xm.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ce.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oo.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://di.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kr.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ez.lnxyls.cn

Q SQL 专题                              90
来源：http://ar.colortex.cn

R Bash 专题                             80
来源：http://fh.jctech888.com.cn

S C / C++ 专题                          60
来源：http://du.hnjuh.cn

T 其他语言补充                          60
来源：http://rl.haigaiapp.cn

U 高频实用片段                         120
来源：http://vr.muxihuayi.cn

------------------------------------
来源：http://kt.szsharing.cn

合计                                  2106 条
来源：http://nl.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://xg.nszjky.cn


<!-- 参考信息 -->