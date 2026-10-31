代发 wailian999

val a = 1;  var b = 2
来源：http://vq.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://lq.asd995.cn

s"值: $b"
来源：http://ep.shxzukj.cn

[T54] Scala：集合映射
来源：http://ql.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://kj.nszjky.cn

[T55] Scala：集合过滤
来源：http://mm.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qg.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://bl.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://tb.newstarts.cn

[T57] Scala：模式匹配
来源：http://mv.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://do.521024.cn

[T58] Scala：函数定义
来源：http://uz.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wp.nszjky.cn

[T59] Scala：循环
来源：http://tw.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://dn.panjiajie.cn

[T60] Scala：折叠
来源：http://uh.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://su.newstarts.cn

================================================================================
来源：http://kh.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bw.szsharing.cn

================================================================================
来源：http://vu.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://wp.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fp.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://qv.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dm.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://hx.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iv.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://bd.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kk.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://lt.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://ex.9csxet.cn

[U06] Py：合并两个字典
来源：http://wn.jianghongdianzi.cn

{**a, **b}
来源：http://ql.521024.cn

[U07] Py：反转字典键值
来源：http://yz.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://ve.huanxung.cn

[U08] Py：展平二维列表
来源：http://nq.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://di.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://hy.colortex.cn

max(d, key=d.get)
来源：http://qv.nicolike.cn

[U10] Py：按值排序字典
来源：http://vp.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jj.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://pj.szxytkj.cn

(x * 2 for x in arr)
来源：http://le.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ed.hahajie.cn

Counter(arr).most_common(3)
来源：http://yq.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://sn.haigaiapp.cn

deque(maxlen=10)
来源：http://db.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://qe.bjjhwx.cn

defaultdict(list)
来源：http://xs.lnxyls.cn

[U15] Py：高精度计时
来源：http://fd.szxytkj.cn

t = time.perf_counter()
来源：http://um.huanxung.cn

[U16] Py：命令行参数解析
来源：http://pb.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cw.wgjwhj.cn

[U17] Py：初始化日志
来源：http://xt.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://az.shtwfgs.cn

[U18] Py：预编译正则
来源：http://tc.hahajie.cn

pat = re.compile(r"\d+")
来源：http://yv.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://tm.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ym.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://pk.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://mg.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://uy.haigaiapp.cn

@contextlib.contextmanager
来源：http://gl.shxzskj.cn

[U22] Py：矩阵转置
来源：http://vi.asd995.cn

list(zip(*m))
来源：http://gq.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://jw.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sp.asd995.cn

[U24] Py：路径操作
来源：http://rj.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pw.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://vl.szsharing.cn

csv.DictReader(f)
来源：http://iz.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://pt.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://em.nszjky.cn

[U27] Py：异步 HTTP
来源：http://jd.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://fc.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://wd.nicolike.cn

UserId = int
来源：http://hr.jctech888.com.cn

[U29] Py：属性校验
来源：http://sj.szsharing.cn

@property 与 @x.setter 配合
来源：http://ik.hahajie.cn

[U30] Py：数据类
来源：http://fe.szxytkj.cn

@dataclass(slots=True)
来源：http://dn.lnxyls.cn

[U31] Py：单测
来源：http://id.9csxet.cn

python -m pytest -q
来源：http://jn.nicolike.cn

[U32] Py：代码格式化
来源：http://eu.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://ab.shtwfgs.cn

[U33] Py：打包发布
来源：http://xs.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://ni.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://kt.wgjwhj.cn

chardet.detect(raw)
来源：http://nb.shtwfgs.cn

[U35] Py：发送邮件
来源：http://pn.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nw.nszjky.cn

[U36] Py：定时任务
来源：http://qv.521024.cn

schedule.every(10).minutes.do(job)
来源：http://co.szxytkj.cn

[U37] Py：读写 Excel
来源：http://ir.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wg.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://gm.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://op.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://uq.521024.cn

sys.stdout.isatty()
来源：http://qg.nicolike.cn

[U40] Py：打印到标准错误
来源：http://oi.panjiajie.cn

print("err", file=sys.stderr)
来源：http://nj.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://da.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://le.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://fi.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qy.nszjky.cn

[U43] PHP：声明命名空间
来源：http://xr.wgjwhj.cn

namespace App\Http;
来源：http://vp.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://nj.szsharing.cn

declare(strict_types=1);
来源：http://sy.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://ra.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ta.wgjwhj.cn

[U46] PHP：可空类型
来源：http://es.9csxet.cn

?string $name = null
来源：http://pp.shxzukj.cn

[U47] PHP：联合类型
来源：http://li.yuexingan06.cn

int|string $id
来源：http://ev.shxzukj.cn

[U48] PHP：纯枚举
来源：http://sj.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ul.muxihuayi.cn

[U49] PHP：只读属性
来源：http://et.haigaiapp.cn

public readonly string $name
来源：http://al.521024.cn

[U50] PHP：构造器属性提升
来源：http://bv.9csxet.cn

public function __construct(private int $id) {}
来源：http://fq.nszjky.cn

[U51] PHP：数组解构
来源：http://ww.szsharing.cn

[$a, $b] = $arr;
来源：http://is.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://az.521024.cn

$double = fn($x) => $x * 2;
来源：http://oy.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://bh.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://ni.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://ae.colortex.cn

$obj?->method()
来源：http://dj.hnjuh.cn

[U55] PHP：match 表达式
来源：http://ss.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gq.shxzukj.cn

[U56] PHP：命名参数
来源：http://lu.shtwfgs.cn

f(a: 1, b: 2)
来源：http://dw.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://sb.newstarts.cn

"值: {$a}"
来源：http://bp.newstarts.cn

[U58] PHP：数组三件套
来源：http://xk.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hi.newstarts.cn

[U59] PHP：自定义排序
来源：http://ak.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lr.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://yh.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oz.9csxet.cn

[U61] PHP：正则
来源：http://ft.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ec.lnxyls.cn

[U62] PHP：日期对象
来源：http://mi.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nk.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://wx.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hg.newstarts.cn

[U64] PHP：目录遍历
来源：http://ef.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://nm.jianghongdianzi.cn

[U65] PHP：会话
来源：http://nj.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dp.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://lb.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hd.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://so.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vp.nicolike.cn

[U68] PHP：PDO 连接
来源：http://us.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lu.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://zh.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zc.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://or.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pu.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://hg.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ei.lnxyls.cn

[U72] PHP：写错误日志
来源：http://ui.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://th.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://yp.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://tv.colortex.cn

[U74] PHP：读取环境变量
来源：http://ie.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://jx.9csxet.cn

[U75] PHP：依赖注入
来源：http://sl.9csxet.cn

composer require psr/container
来源：http://sa.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://fx.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sx.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://uy.newstarts.cn

composer require twig/twig
来源：http://pp.huixiangedu.cn

[U78] PHP：单元测试
来源：http://qb.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://uv.bjjhwx.cn

[U79] PHP：静态分析
来源：http://yj.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://lt.9csxet.cn

[U80] PHP：代码规范修复
来源：http://yv.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gr.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://ml.shxzukj.cn

npm init -y;  npm i express
来源：http://ur.huanxung.cn

[U82] JS：package.json 脚本
来源：http://wu.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sl.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://iw.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wv.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://gr.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zg.nicolike.cn

[U85] JS：可选链
来源：http://kr.shxzukj.cn

a?.b?.c
来源：http://rg.nszjky.cn

[U86] JS：空值合并
来源：http://cg.jctech888.com.cn

a ?? b
来源：http://rs.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://qn.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://cm.newstarts.cn

[U88] JS：对象展开合并
来源：http://es.jctech888.com.cn

{ ...a, ...b }
来源：http://ml.wgjwhj.cn

[U89] JS：数组去重
来源：http://tu.shxzukj.cn

[...new Set(arr)]
来源：http://ax.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://jq.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://pm.nicolike.cn

[U91] JS：对象键值遍历
来源：http://kk.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qb.szsharing.cn

[U92] JS：深拷贝
来源：http://ck.9csxet.cn

structuredClone(obj)
来源：http://mx.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://tw.yuexingan06.cn

`共 ${n} 条`
来源：http://fb.9csxet.cn

[U94] JS：箭头函数
来源：http://td.szsharing.cn

const double = x => x * 2;
来源：http://fw.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://za.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://aw.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://xq.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uu.nicolike.cn

[U97] JS：并发请求
来源：http://sm.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fx.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://wl.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xe.huanxung.cn

[U99] JS：事件监听
来源：http://hn.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ta.hnjuh.cn

[U100] JS：DOM 查询
来源：http://vv.muxihuayi.cn

document.querySelector(".item")
来源：http://vr.gzmigu.cn

[U101] JS：classList 操作
来源：http://pf.huixiangedu.cn

el.classList.toggle("active")
来源：http://yz.szsharing.cn

[U102] JS：本地存储
来源：http://bm.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xw.nszjky.cn

[U103] JS：定时器
来源：http://wj.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pc.shxzukj.cn

[U104] JS：防抖
来源：http://do.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pf.colortex.cn

[U105] JS：节流
来源：http://ri.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lm.yuexingan06.cn

[U106] JS：日期格式化
来源：http://jf.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dw.szxytkj.cn

[U107] JS：数字千分位
来源：http://sm.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wq.newstarts.cn

[U108] JS：随机整数
来源：http://hl.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sk.panjiajie.cn

[U109] JS：数组分组
来源：http://sf.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://st.panjiajie.cn

[U110] JS：数组分块
来源：http://ni.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iz.gzmigu.cn

[U111] JS：对象转 Map
来源：http://ct.521024.cn

new Map(Object.entries(obj))
来源：http://qf.521024.cn

[U112] JS：字符串补位
来源：http://ik.chemitech.net.cn

"7".padStart(3, "0")
来源：http://yv.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://ae.newstarts.cn

s.replaceAll("a", "b")
来源：http://od.huanxung.cn

[U114] JS：JSON 深比较
来源：http://aw.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ak.9csxet.cn

[U115] JS：生成 UUID
来源：http://ci.huixinmuqiang.cn

crypto.randomUUID()
来源：http://mg.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://al.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://gc.nicolike.cn

[U117] JS：单元测试
来源：http://me.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://oq.nicolike.cn

[U118] JS：开发服务器
来源：http://jv.nicolike.cn

npm i -D vite;  npx vite
来源：http://cb.shxzskj.cn

[U119] JS：生产构建
来源：http://zh.lnxyls.cn

npx vite build
来源：http://ls.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://cd.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://zv.panjiajie.cn

================================================================================
来源：http://qa.jianghongdianzi.cn

统计汇总
来源：http://ah.huixiangedu.cn

================================================================================
来源：http://le.szsharing.cn

按语言统计（条）：
来源：http://sw.jianghongdianzi.cn

Python ......... 252
来源：http://ze.haigaiapp.cn

PHP ............ 252
来源：http://gq.newstarts.cn

JavaScript ..... 252
来源：http://pl.shxzskj.cn

TypeScript ..... 212
来源：http://gb.gzmigu.cn

Java ........... 212
来源：http://ce.bookmarksfly.cn

Go ............. 212
来源：http://eu.bjjhwx.cn

Ruby ........... 212
来源：http://ox.huixinmuqiang.cn

C# ............. 212
来源：http://ch.shxzukj.cn

C .............. 30
来源：http://im.muxihuayi.cn

C++ ............ 30
来源：http://hv.gzmigu.cn

SQL ............ 90
来源：http://pl.9csxet.cn

Bash ........... 80
来源：http://nv.yuntaijiaju.cn

Kotlin ......... 15
来源：http://ag.yuntaijiaju.cn

Swift .......... 15
来源：http://ux.jctech888.com.cn

Lua ............ 10
来源：http://an.lnxyls.cn

Perl ........... 10
来源：http://sx.9csxet.cn

Scala .......... 10
来源：http://kb.jianghongdianzi.cn

------------------------------------
来源：http://up.shxzukj.cn

合计 ........... 2106 条
来源：http://el.huanxung.cn

按章节统计：
来源：http://oc.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ie.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bj.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ir.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fc.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fs.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xn.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eo.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zs.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ly.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wa.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://li.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://au.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hy.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ru.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zh.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gx.szxytkj.cn


<!-- 参考信息 -->