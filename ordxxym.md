代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://lu.nszjky.cn

[T55] Scala：集合过滤
来源：http://zx.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rn.chemitech.net.cn

[T56] Scala：样例类
来源：http://fy.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://cr.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://gd.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jl.newstarts.cn

[T58] Scala：函数定义
来源：http://mt.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ur.shxzukj.cn

[T59] Scala：循环
来源：http://iy.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://gh.newstarts.cn

[T60] Scala：折叠
来源：http://ef.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ag.shtwfgs.cn

================================================================================
来源：http://lw.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pz.huixiangedu.cn

================================================================================
来源：http://bw.521024.cn

[U01] Py：创建虚拟环境
来源：http://uw.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rc.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://od.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wx.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://bu.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xf.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://qi.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jl.huanxung.cn

[U05] Py：列表去重且保序
来源：http://wz.521024.cn

list(dict.fromkeys(arr))
来源：http://wb.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://wh.shtwfgs.cn

{**a, **b}
来源：http://rd.panjiajie.cn

[U07] Py：反转字典键值
来源：http://dd.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://iq.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://en.shxzskj.cn

[y for x in nested for y in x]
来源：http://iv.521024.cn

[U09] Py：字典取最大值的键
来源：http://py.muxihuayi.cn

max(d, key=d.get)
来源：http://ci.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://dz.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ta.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://nx.shxzukj.cn

(x * 2 for x in arr)
来源：http://ks.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fk.521024.cn

Counter(arr).most_common(3)
来源：http://mb.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://tk.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ih.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://ar.shxzskj.cn

defaultdict(list)
来源：http://zc.huanxung.cn

[U15] Py：高精度计时
来源：http://zv.yuexingan06.cn

t = time.perf_counter()
来源：http://os.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://vl.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fk.lnxyls.cn

[U17] Py：初始化日志
来源：http://fk.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://lk.newstarts.cn

[U18] Py：预编译正则
来源：http://jx.asd995.cn

pat = re.compile(r"\d+")
来源：http://he.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://hz.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pa.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://ev.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://od.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ir.haigaiapp.cn

@contextlib.contextmanager
来源：http://ih.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://ph.hnjuh.cn

list(zip(*m))
来源：http://je.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://ca.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dx.chemitech.net.cn

[U24] Py：路径操作
来源：http://qd.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dx.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://hg.szsharing.cn

csv.DictReader(f)
来源：http://gr.shxzskj.cn

[U26] Py：并发下载
来源：http://vc.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://la.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://ee.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://dr.colortex.cn

[U28] Py：类型别名
来源：http://wh.bjjhwx.cn

UserId = int
来源：http://bp.colortex.cn

[U29] Py：属性校验
来源：http://or.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://rn.asd995.cn

[U30] Py：数据类
来源：http://qh.asd995.cn

@dataclass(slots=True)
来源：http://je.hnjuh.cn

[U31] Py：单测
来源：http://om.asd995.cn

python -m pytest -q
来源：http://vz.newstarts.cn

[U32] Py：代码格式化
来源：http://bj.hahajie.cn

ruff format . && ruff check --fix .
来源：http://fh.jctech888.com.cn

[U33] Py：打包发布
来源：http://rz.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://tr.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://jv.panjiajie.cn

chardet.detect(raw)
来源：http://dr.huanxung.cn

[U35] Py：发送邮件
来源：http://qk.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tg.nicolike.cn

[U36] Py：定时任务
来源：http://pt.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://or.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://zv.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gh.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://hh.nicolike.cn

Path(__file__).resolve().parent
来源：http://qy.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://lq.huanxung.cn

sys.stdout.isatty()
来源：http://pu.asd995.cn

[U40] Py：打印到标准错误
来源：http://gd.hahajie.cn

print("err", file=sys.stderr)
来源：http://er.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://rw.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ya.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://gf.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fn.colortex.cn

[U43] PHP：声明命名空间
来源：http://cg.hnjuh.cn

namespace App\Http;
来源：http://ei.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://tf.yuexingan06.cn

declare(strict_types=1);
来源：http://zm.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://oe.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lo.huanxung.cn

[U46] PHP：可空类型
来源：http://gv.bookmarksfly.cn

?string $name = null
来源：http://en.szxytkj.cn

[U47] PHP：联合类型
来源：http://uk.shxzukj.cn

int|string $id
来源：http://qn.nicolike.cn

[U48] PHP：纯枚举
来源：http://zt.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yq.haigaiapp.cn

[U49] PHP：只读属性
来源：http://du.jianghongdianzi.cn

public readonly string $name
来源：http://nj.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://fh.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ap.haigaiapp.cn

[U51] PHP：数组解构
来源：http://cv.gzmigu.cn

[$a, $b] = $arr;
来源：http://gl.huanxung.cn

[U52] PHP：箭头函数
来源：http://qb.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://xk.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://xb.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://gi.szsharing.cn

[U54] PHP：空安全调用
来源：http://ma.huixinmuqiang.cn

$obj?->method()
来源：http://dk.newstarts.cn

[U55] PHP：match 表达式
来源：http://oc.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qr.521024.cn

[U56] PHP：命名参数
来源：http://ff.shtwfgs.cn

f(a: 1, b: 2)
来源：http://hd.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://rc.jctech888.com.cn

"值: {$a}"
来源：http://ga.newstarts.cn

[U58] PHP：数组三件套
来源：http://cb.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gn.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://cg.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ec.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://go.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ds.yuexingan06.cn

[U61] PHP：正则
来源：http://wv.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ue.asd995.cn

[U62] PHP：日期对象
来源：http://db.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://no.shxzukj.cn

[U63] PHP：文件读写
来源：http://oz.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ps.newstarts.cn

[U64] PHP：目录遍历
来源：http://ge.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://uh.panjiajie.cn

[U65] PHP：会话
来源：http://yp.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://he.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://sn.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vb.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://yo.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hj.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://xr.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uj.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://dn.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oz.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://qq.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qj.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://po.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://am.nicolike.cn

[U72] PHP：写错误日志
来源：http://md.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://en.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://rk.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://vq.szsharing.cn

[U74] PHP：读取环境变量
来源：http://gf.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://hq.hahajie.cn

[U75] PHP：依赖注入
来源：http://ed.bjjhwx.cn

composer require psr/container
来源：http://pc.shxzskj.cn

[U76] PHP：简单路由
来源：http://zn.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zw.panjiajie.cn

[U77] PHP：模板渲染
来源：http://fb.szxytkj.cn

composer require twig/twig
来源：http://gx.nicolike.cn

[U78] PHP：单元测试
来源：http://em.asd995.cn

composer require --dev phpunit/phpunit
来源：http://ob.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://io.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://nn.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://lz.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jc.lnxyls.cn

[U81] JS：初始化项目
来源：http://jc.hnjuh.cn

npm init -y;  npm i express
来源：http://fa.521024.cn

[U82] JS：package.json 脚本
来源：http://tq.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zq.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://bi.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zz.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://qb.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tv.colortex.cn

[U85] JS：可选链
来源：http://bm.lnxyls.cn

a?.b?.c
来源：http://ps.wgjwhj.cn

[U86] JS：空值合并
来源：http://jm.nszjky.cn

a ?? b
来源：http://ww.newstarts.cn

[U87] JS：解构默认值
来源：http://ze.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://hu.nszjky.cn

[U88] JS：对象展开合并
来源：http://hc.huixiangedu.cn

{ ...a, ...b }
来源：http://zs.yuexingan06.cn

[U89] JS：数组去重
来源：http://ke.asd995.cn

[...new Set(arr)]
来源：http://zd.panjiajie.cn

[U90] JS：数字数组排序
来源：http://ya.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://um.colortex.cn

[U91] JS：对象键值遍历
来源：http://hv.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pr.szxytkj.cn

[U92] JS：深拷贝
来源：http://at.521024.cn

structuredClone(obj)
来源：http://wi.yuexingan06.cn

[U93] JS：模板字符串
来源：http://oj.szsharing.cn

`共 ${n} 条`
来源：http://ft.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://ze.haigaiapp.cn

const double = x => x * 2;
来源：http://wz.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://ox.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://py.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://bv.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fo.huixiangedu.cn

[U97] JS：并发请求
来源：http://gb.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rn.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://ym.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uo.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://wn.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://cc.nicolike.cn

[U100] JS：DOM 查询
来源：http://ev.bookmarksfly.cn

document.querySelector(".item")
来源：http://jd.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://oc.haigaiapp.cn

el.classList.toggle("active")
来源：http://zp.wgjwhj.cn

[U102] JS：本地存储
来源：http://du.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sp.shxzskj.cn

[U103] JS：定时器
来源：http://lp.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pr.jctech888.com.cn

[U104] JS：防抖
来源：http://cf.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vg.jctech888.com.cn

[U105] JS：节流
来源：http://kl.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tj.panjiajie.cn

[U106] JS：日期格式化
来源：http://ml.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vs.yuexingan06.cn

[U107] JS：数字千分位
来源：http://xm.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fx.hahajie.cn

[U108] JS：随机整数
来源：http://ef.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tm.colortex.cn

[U109] JS：数组分组
来源：http://yf.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://ng.bookmarksfly.cn

[U110] JS：数组分块
来源：http://er.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pj.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://wf.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://wd.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://qv.szxytkj.cn

"7".padStart(3, "0")
来源：http://ds.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ti.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://wl.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://kw.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tw.lnxyls.cn

[U115] JS：生成 UUID
来源：http://kr.nicolike.cn

crypto.randomUUID()
来源：http://ar.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://oy.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://mp.szxytkj.cn

[U117] JS：单元测试
来源：http://ct.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://hk.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://gp.asd995.cn

npm i -D vite;  npx vite
来源：http://eu.9csxet.cn

[U119] JS：生产构建
来源：http://bu.muxihuayi.cn

npx vite build
来源：http://mw.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://el.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://ir.jianghongdianzi.cn

================================================================================
来源：http://pt.bjjhwx.cn

统计汇总
来源：http://nu.bookmarksfly.cn

================================================================================
来源：http://id.asd995.cn

按语言统计（条）：
来源：http://ov.bjjhwx.cn

Python ......... 252
来源：http://is.9csxet.cn

PHP ............ 252
来源：http://sh.szsharing.cn

JavaScript ..... 252
来源：http://em.lnxyls.cn

TypeScript ..... 212
来源：http://ba.asd995.cn

Java ........... 212
来源：http://ve.lnxyls.cn

Go ............. 212
来源：http://hu.asd995.cn

Ruby ........... 212
来源：http://xo.bjjhwx.cn

C# ............. 212
来源：http://ay.huixiangedu.cn

C .............. 30
来源：http://ij.huixinmuqiang.cn

C++ ............ 30
来源：http://bf.9csxet.cn

SQL ............ 90
来源：http://ec.bookmarksfly.cn

Bash ........... 80
来源：http://nq.haigaiapp.cn

Kotlin ......... 15
来源：http://ye.panjiajie.cn

Swift .......... 15
来源：http://vp.huixinmuqiang.cn

Lua ............ 10
来源：http://dh.jctech888.com.cn

Perl ........... 10
来源：http://cy.chemitech.net.cn

Scala .......... 10
来源：http://br.nszjky.cn

------------------------------------
来源：http://yw.shxzskj.cn

合计 ........... 2106 条
来源：http://km.shxzskj.cn

按章节统计：
来源：http://pj.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mo.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xr.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ik.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sc.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://su.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lk.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://od.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dv.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wl.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zu.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oc.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ra.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xj.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yj.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kf.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oe.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://he.panjiajie.cn

R Bash 专题                             80
来源：http://ru.bjjhwx.cn

S C / C++ 专题                          60
来源：http://ta.colortex.cn

T 其他语言补充                          60
来源：http://qi.shxzukj.cn


<!-- 参考信息 -->