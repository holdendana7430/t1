代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ir.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://hk.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ml.nszjky.cn

[T56] Scala：样例类
来源：http://gq.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://ae.9csxet.cn

[T57] Scala：模式匹配
来源：http://hw.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vu.hahajie.cn

[T58] Scala：函数定义
来源：http://av.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hb.szsharing.cn

[T59] Scala：循环
来源：http://xd.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://zu.nicolike.cn

[T60] Scala：折叠
来源：http://qt.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mv.gzmigu.cn

================================================================================
来源：http://ii.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pp.bjjhwx.cn

================================================================================
来源：http://dv.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://gq.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fb.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://gp.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cy.colortex.cn

[U03] Py：加载 .env 配置
来源：http://dv.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tl.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://nw.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fi.9csxet.cn

[U05] Py：列表去重且保序
来源：http://cl.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://ot.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://cb.bookmarksfly.cn

{**a, **b}
来源：http://nf.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ca.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://my.521024.cn

[U08] Py：展平二维列表
来源：http://ze.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://sl.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://ws.hahajie.cn

max(d, key=d.get)
来源：http://ro.shxzskj.cn

[U10] Py：按值排序字典
来源：http://xv.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ka.hnjuh.cn

[U11] Py：生成器表达式
来源：http://ot.hahajie.cn

(x * 2 for x in arr)
来源：http://gt.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sr.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://yo.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://lw.nicolike.cn

deque(maxlen=10)
来源：http://ng.szsharing.cn

[U14] Py：分组收集到列表
来源：http://db.bookmarksfly.cn

defaultdict(list)
来源：http://og.nszjky.cn

[U15] Py：高精度计时
来源：http://pb.haigaiapp.cn

t = time.perf_counter()
来源：http://mj.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://zl.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zf.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ao.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://sa.9csxet.cn

[U18] Py：预编译正则
来源：http://cp.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://hp.szsharing.cn

[U19] Py：正则替换带回调
来源：http://ee.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gv.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://is.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://ji.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://rh.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://ab.hnjuh.cn

[U22] Py：矩阵转置
来源：http://no.shtwfgs.cn

list(zip(*m))
来源：http://az.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://av.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ey.shtwfgs.cn

[U24] Py：路径操作
来源：http://tz.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://my.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://kc.hnjuh.cn

csv.DictReader(f)
来源：http://ol.chemitech.net.cn

[U26] Py：并发下载
来源：http://ij.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ph.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://th.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://rg.hnjuh.cn

[U28] Py：类型别名
来源：http://qh.9csxet.cn

UserId = int
来源：http://cv.muxihuayi.cn

[U29] Py：属性校验
来源：http://ja.gzmigu.cn

@property 与 @x.setter 配合
来源：http://rl.muxihuayi.cn

[U30] Py：数据类
来源：http://uc.bjjhwx.cn

@dataclass(slots=True)
来源：http://yq.bjjhwx.cn

[U31] Py：单测
来源：http://oq.bjjhwx.cn

python -m pytest -q
来源：http://gp.jctech888.com.cn

[U32] Py：代码格式化
来源：http://rn.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://yh.nszjky.cn

[U33] Py：打包发布
来源：http://mt.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://jw.szsharing.cn

[U34] Py：判断编码
来源：http://sb.huanxung.cn

chardet.detect(raw)
来源：http://my.haigaiapp.cn

[U35] Py：发送邮件
来源：http://yv.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jn.shxzskj.cn

[U36] Py：定时任务
来源：http://ja.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://zv.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://dm.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nj.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://rc.hahajie.cn

Path(__file__).resolve().parent
来源：http://kh.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://dw.asd995.cn

sys.stdout.isatty()
来源：http://qr.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://fa.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://ov.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://fp.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fj.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://of.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wg.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://ga.yuexingan06.cn

namespace App\Http;
来源：http://oy.9csxet.cn

[U44] PHP：开启严格类型
来源：http://hq.nszjky.cn

declare(strict_types=1);
来源：http://dr.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://em.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.asd995.cn

[U46] PHP：可空类型
来源：http://kl.wgjwhj.cn

?string $name = null
来源：http://jn.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://yv.lnxyls.cn

int|string $id
来源：http://pz.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://bj.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eg.lnxyls.cn

[U49] PHP：只读属性
来源：http://qz.shtwfgs.cn

public readonly string $name
来源：http://rj.colortex.cn

[U50] PHP：构造器属性提升
来源：http://rc.szxytkj.cn

public function __construct(private int $id) {}
来源：http://fa.nicolike.cn

[U51] PHP：数组解构
来源：http://zh.chemitech.net.cn

[$a, $b] = $arr;
来源：http://uo.szxytkj.cn

[U52] PHP：箭头函数
来源：http://co.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://hv.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://eq.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://fb.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://az.hnjuh.cn

$obj?->method()
来源：http://li.szsharing.cn

[U55] PHP：match 表达式
来源：http://dd.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ss.shxzskj.cn

[U56] PHP：命名参数
来源：http://tp.bjjhwx.cn

f(a: 1, b: 2)
来源：http://nq.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://zc.wgjwhj.cn

"值: {$a}"
来源：http://xw.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://qy.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ny.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://lg.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zp.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://hv.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wb.yuntaijiaju.cn

[U61] PHP：正则
来源：http://pw.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://od.panjiajie.cn

[U62] PHP：日期对象
来源：http://nb.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ys.nicolike.cn

[U63] PHP：文件读写
来源：http://wv.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qt.nicolike.cn

[U64] PHP：目录遍历
来源：http://qb.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://bv.yuexingan06.cn

[U65] PHP：会话
来源：http://xg.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kv.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://rc.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xw.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://hv.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zx.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://jv.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nw.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://ja.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ol.asd995.cn

[U70] PHP：PDO 事务
来源：http://tx.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zg.9csxet.cn

[U71] PHP：抛出异常
来源：http://hy.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://vi.hahajie.cn

[U72] PHP：写错误日志
来源：http://vk.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://se.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://it.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://li.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://hx.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://lo.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://ki.yuntaijiaju.cn

composer require psr/container
来源：http://wh.9csxet.cn

[U76] PHP：简单路由
来源：http://ra.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ug.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://xq.huixiangedu.cn

composer require twig/twig
来源：http://zs.nszjky.cn

[U78] PHP：单元测试
来源：http://ks.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://tr.panjiajie.cn

[U79] PHP：静态分析
来源：http://qs.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://dd.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://vx.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fh.shxzukj.cn

[U81] JS：初始化项目
来源：http://la.lnxyls.cn

npm init -y;  npm i express
来源：http://xi.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://yb.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xe.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://pw.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qa.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://rk.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pw.521024.cn

[U85] JS：可选链
来源：http://fi.hnjuh.cn

a?.b?.c
来源：http://va.colortex.cn

[U86] JS：空值合并
来源：http://fn.jctech888.com.cn

a ?? b
来源：http://ug.haigaiapp.cn

[U87] JS：解构默认值
来源：http://zs.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://xk.asd995.cn

[U88] JS：对象展开合并
来源：http://qo.jctech888.com.cn

{ ...a, ...b }
来源：http://ny.nicolike.cn

[U89] JS：数组去重
来源：http://ih.muxihuayi.cn

[...new Set(arr)]
来源：http://mp.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://wi.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://sy.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://sm.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ez.asd995.cn

[U92] JS：深拷贝
来源：http://jc.9csxet.cn

structuredClone(obj)
来源：http://dd.shtwfgs.cn

[U93] JS：模板字符串
来源：http://vz.gzmigu.cn

`共 ${n} 条`
来源：http://pc.muxihuayi.cn

[U94] JS：箭头函数
来源：http://ek.wgjwhj.cn

const double = x => x * 2;
来源：http://tj.asd995.cn

[U95] JS：Promise 包装
来源：http://wz.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://wp.nszjky.cn

[U96] JS：async/await 与异常
来源：http://vw.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tb.wgjwhj.cn

[U97] JS：并发请求
来源：http://bs.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://to.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ak.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pa.panjiajie.cn

[U99] JS：事件监听
来源：http://dv.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://hh.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://si.szsharing.cn

document.querySelector(".item")
来源：http://ec.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://si.huixiangedu.cn

el.classList.toggle("active")
来源：http://gb.newstarts.cn

[U102] JS：本地存储
来源：http://si.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vp.nszjky.cn

[U103] JS：定时器
来源：http://sj.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gb.panjiajie.cn

[U104] JS：防抖
来源：http://ld.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ov.wgjwhj.cn

[U105] JS：节流
来源：http://un.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ue.szxytkj.cn

[U106] JS：日期格式化
来源：http://hp.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ek.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ax.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pb.hnjuh.cn

[U108] JS：随机整数
来源：http://bz.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://se.jctech888.com.cn

[U109] JS：数组分组
来源：http://wg.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://np.nszjky.cn

[U110] JS：数组分块
来源：http://yd.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://co.hnjuh.cn

[U111] JS：对象转 Map
来源：http://gn.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://mt.lnxyls.cn

[U112] JS：字符串补位
来源：http://oh.haigaiapp.cn

"7".padStart(3, "0")
来源：http://xo.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://vf.lnxyls.cn

s.replaceAll("a", "b")
来源：http://no.huanxung.cn

[U114] JS：JSON 深比较
来源：http://tt.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tb.panjiajie.cn

[U115] JS：生成 UUID
来源：http://pa.nicolike.cn

crypto.randomUUID()
来源：http://ev.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://bu.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://cg.yuexingan06.cn

[U117] JS：单元测试
来源：http://nm.521024.cn

npm i -D vitest;  npx vitest
来源：http://dj.hahajie.cn

[U118] JS：开发服务器
来源：http://bb.nszjky.cn

npm i -D vite;  npx vite
来源：http://ii.panjiajie.cn

[U119] JS：生产构建
来源：http://js.hnjuh.cn

npx vite build
来源：http://kv.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://jn.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://fc.nszjky.cn

================================================================================
来源：http://dz.newstarts.cn

统计汇总
来源：http://vh.muxihuayi.cn

================================================================================
来源：http://vt.wgjwhj.cn

按语言统计（条）：
来源：http://sb.yuexingan06.cn

Python ......... 252
来源：http://lz.wgjwhj.cn

PHP ............ 252
来源：http://dv.haigaiapp.cn

JavaScript ..... 252
来源：http://dw.haigaiapp.cn

TypeScript ..... 212
来源：http://fd.bjjhwx.cn

Java ........... 212
来源：http://wi.521024.cn

Go ............. 212
来源：http://si.lnxyls.cn

Ruby ........... 212
来源：http://dx.huixinmuqiang.cn

C# ............. 212
来源：http://jh.521024.cn

C .............. 30
来源：http://kt.colortex.cn

C++ ............ 30
来源：http://ca.lnxyls.cn

SQL ............ 90
来源：http://xe.wgjwhj.cn

Bash ........... 80
来源：http://lp.bjjhwx.cn

Kotlin ......... 15
来源：http://ba.nszjky.cn

Swift .......... 15
来源：http://in.521024.cn

Lua ............ 10
来源：http://zl.newstarts.cn

Perl ........... 10
来源：http://ja.yuntaijiaju.cn

Scala .......... 10
来源：http://ay.wgjwhj.cn

------------------------------------
来源：http://uo.shxzskj.cn

合计 ........... 2106 条
来源：http://uz.colortex.cn

按章节统计：
来源：http://nk.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sa.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lz.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dl.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jf.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nd.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ni.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vz.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lm.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nv.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://be.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ey.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pm.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nx.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ee.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yj.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kh.nszjky.cn

Q SQL 专题                              90
来源：http://ks.szsharing.cn

R Bash 专题                             80
来源：http://ac.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://bp.521024.cn

T 其他语言补充                          60
来源：http://sr.hnjuh.cn


<!-- 参考信息 -->