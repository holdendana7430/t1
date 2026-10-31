代发 wailian999

val a = 1;  var b = 2
来源：http://ac.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://ib.bookmarksfly.cn

s"值: $b"
来源：http://hd.521024.cn

[T54] Scala：集合映射
来源：http://xe.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://up.szsharing.cn

[T55] Scala：集合过滤
来源：http://qn.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eg.huixiangedu.cn

[T56] Scala：样例类
来源：http://uc.nszjky.cn

case class User(name: String, age: Int)
来源：http://zw.hahajie.cn

[T57] Scala：模式匹配
来源：http://vd.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mz.szxytkj.cn

[T58] Scala：函数定义
来源：http://ro.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vg.panjiajie.cn

[T59] Scala：循环
来源：http://is.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://ud.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://nd.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rt.chemitech.net.cn

================================================================================
来源：http://kf.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sz.gzmigu.cn

================================================================================
来源：http://pe.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://wx.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sb.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://dx.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tf.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://uw.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ge.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://hg.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://od.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://xo.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://uo.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://up.yuexingan06.cn

{**a, **b}
来源：http://hm.9csxet.cn

[U07] Py：反转字典键值
来源：http://mk.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://pu.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://he.hnjuh.cn

[y for x in nested for y in x]
来源：http://zj.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://kj.wgjwhj.cn

max(d, key=d.get)
来源：http://gs.lnxyls.cn

[U10] Py：按值排序字典
来源：http://sv.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ed.asd995.cn

[U11] Py：生成器表达式
来源：http://vl.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ub.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oh.521024.cn

Counter(arr).most_common(3)
来源：http://ul.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://kz.hnjuh.cn

deque(maxlen=10)
来源：http://sb.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://wv.gzmigu.cn

defaultdict(list)
来源：http://et.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://ds.hahajie.cn

t = time.perf_counter()
来源：http://mw.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://rr.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vb.muxihuayi.cn

[U17] Py：初始化日志
来源：http://wp.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://gk.yuexingan06.cn

[U18] Py：预编译正则
来源：http://jp.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://vk.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://df.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iu.nszjky.cn

[U20] Py：缓存函数结果
来源：http://nq.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://rw.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://oc.muxihuayi.cn

@contextlib.contextmanager
来源：http://vu.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://fp.szxytkj.cn

list(zip(*m))
来源：http://zc.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://pu.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wu.shtwfgs.cn

[U24] Py：路径操作
来源：http://na.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pv.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://ge.huixiangedu.cn

csv.DictReader(f)
来源：http://im.shtwfgs.cn

[U26] Py：并发下载
来源：http://bx.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cq.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ev.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://cb.jctech888.com.cn

[U28] Py：类型别名
来源：http://jt.9csxet.cn

UserId = int
来源：http://ag.yuexingan06.cn

[U29] Py：属性校验
来源：http://cv.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://jr.hnjuh.cn

[U30] Py：数据类
来源：http://ny.muxihuayi.cn

@dataclass(slots=True)
来源：http://wt.521024.cn

[U31] Py：单测
来源：http://yy.jianghongdianzi.cn

python -m pytest -q
来源：http://ip.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://qa.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://qo.hnjuh.cn

[U33] Py：打包发布
来源：http://hr.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://up.newstarts.cn

[U34] Py：判断编码
来源：http://iq.hnjuh.cn

chardet.detect(raw)
来源：http://ap.huixiangedu.cn

[U35] Py：发送邮件
来源：http://lg.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nh.haigaiapp.cn

[U36] Py：定时任务
来源：http://bs.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://fo.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://sv.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ap.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://ft.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://gc.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://da.szxytkj.cn

sys.stdout.isatty()
来源：http://bb.9csxet.cn

[U40] Py：打印到标准错误
来源：http://zz.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ur.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://vu.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uy.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://tc.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iy.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://lo.panjiajie.cn

namespace App\Http;
来源：http://oq.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://ei.jianghongdianzi.cn

declare(strict_types=1);
来源：http://hz.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://pf.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yx.hahajie.cn

[U46] PHP：可空类型
来源：http://fs.9csxet.cn

?string $name = null
来源：http://kf.newstarts.cn

[U47] PHP：联合类型
来源：http://bb.shxzskj.cn

int|string $id
来源：http://uz.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://mk.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zn.hnjuh.cn

[U49] PHP：只读属性
来源：http://rp.huixinmuqiang.cn

public readonly string $name
来源：http://be.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://yp.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://nf.nszjky.cn

[U51] PHP：数组解构
来源：http://kj.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://nd.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://rn.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://ng.szsharing.cn

[U53] PHP：空合并运算符
来源：http://vq.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://ec.newstarts.cn

[U54] PHP：空安全调用
来源：http://jk.lnxyls.cn

$obj?->method()
来源：http://hw.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ba.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rz.chemitech.net.cn

[U56] PHP：命名参数
来源：http://jw.chemitech.net.cn

f(a: 1, b: 2)
来源：http://id.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://ho.asd995.cn

"值: {$a}"
来源：http://hq.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://vu.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yn.9csxet.cn

[U59] PHP：自定义排序
来源：http://dp.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fe.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://gy.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://by.huixinmuqiang.cn

[U61] PHP：正则
来源：http://vy.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bi.jctech888.com.cn

[U62] PHP：日期对象
来源：http://pj.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yl.huanxung.cn

[U63] PHP：文件读写
来源：http://lc.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://na.shxzukj.cn

[U64] PHP：目录遍历
来源：http://ot.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://fi.panjiajie.cn

[U65] PHP：会话
来源：http://od.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gu.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://nm.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rb.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://gw.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cu.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://kv.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fi.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://do.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://po.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://se.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fp.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ns.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://ux.shxzukj.cn

[U72] PHP：写错误日志
来源：http://xs.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://pc.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ea.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://rg.nicolike.cn

[U74] PHP：读取环境变量
来源：http://zc.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://wa.shxzskj.cn

[U75] PHP：依赖注入
来源：http://mi.shxzukj.cn

composer require psr/container
来源：http://of.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://su.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nw.panjiajie.cn

[U77] PHP：模板渲染
来源：http://od.asd995.cn

composer require twig/twig
来源：http://dy.panjiajie.cn

[U78] PHP：单元测试
来源：http://zy.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://jr.nszjky.cn

[U79] PHP：静态分析
来源：http://ou.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://pm.newstarts.cn

[U80] PHP：代码规范修复
来源：http://ru.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cf.jctech888.com.cn

[U81] JS：初始化项目
来源：http://zj.huixiangedu.cn

npm init -y;  npm i express
来源：http://ef.colortex.cn

[U82] JS：package.json 脚本
来源：http://va.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nx.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://fx.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sl.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://ye.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nl.gzmigu.cn

[U85] JS：可选链
来源：http://he.szxytkj.cn

a?.b?.c
来源：http://wm.shtwfgs.cn

[U86] JS：空值合并
来源：http://bd.bjjhwx.cn

a ?? b
来源：http://nj.newstarts.cn

[U87] JS：解构默认值
来源：http://yc.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://uj.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://ih.shtwfgs.cn

{ ...a, ...b }
来源：http://fw.bjjhwx.cn

[U89] JS：数组去重
来源：http://lc.panjiajie.cn

[...new Set(arr)]
来源：http://nv.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://gq.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://ny.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://dl.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://as.newstarts.cn

[U92] JS：深拷贝
来源：http://hh.nszjky.cn

structuredClone(obj)
来源：http://ce.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://vf.jctech888.com.cn

`共 ${n} 条`
来源：http://vz.bjjhwx.cn

[U94] JS：箭头函数
来源：http://ub.asd995.cn

const double = x => x * 2;
来源：http://yq.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://ac.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://yk.9csxet.cn

[U96] JS：async/await 与异常
来源：http://bh.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jh.haigaiapp.cn

[U97] JS：并发请求
来源：http://rm.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yh.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://ix.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://an.huanxung.cn

[U99] JS：事件监听
来源：http://pr.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://wq.shxzskj.cn

[U100] JS：DOM 查询
来源：http://fa.szxytkj.cn

document.querySelector(".item")
来源：http://yr.wgjwhj.cn

[U101] JS：classList 操作
来源：http://pm.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://cv.wgjwhj.cn

[U102] JS：本地存储
来源：http://qe.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://el.huixinmuqiang.cn

[U103] JS：定时器
来源：http://yr.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xp.nicolike.cn

[U104] JS：防抖
来源：http://se.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://at.nszjky.cn

[U105] JS：节流
来源：http://lu.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sr.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://vv.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bq.bjjhwx.cn

[U107] JS：数字千分位
来源：http://cq.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fp.shtwfgs.cn

[U108] JS：随机整数
来源：http://qg.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hp.bookmarksfly.cn

[U109] JS：数组分组
来源：http://kv.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://rh.shtwfgs.cn

[U110] JS：数组分块
来源：http://kx.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://us.nicolike.cn

[U111] JS：对象转 Map
来源：http://lq.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://tl.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://ot.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://fl.lnxyls.cn

[U113] JS：正则替换全部
来源：http://ar.hahajie.cn

s.replaceAll("a", "b")
来源：http://qf.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://dd.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nk.lnxyls.cn

[U115] JS：生成 UUID
来源：http://rq.bookmarksfly.cn

crypto.randomUUID()
来源：http://yb.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://ti.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://ig.wgjwhj.cn

[U117] JS：单元测试
来源：http://cu.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://ms.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://mr.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://mk.shxzukj.cn

[U119] JS：生产构建
来源：http://tu.asd995.cn

npx vite build
来源：http://ll.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://vl.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://fk.chemitech.net.cn

================================================================================
来源：http://rp.chemitech.net.cn

统计汇总
来源：http://tz.bookmarksfly.cn

================================================================================
来源：http://ev.521024.cn

按语言统计（条）：
来源：http://kq.bookmarksfly.cn

Python ......... 252
来源：http://kc.szsharing.cn

PHP ............ 252
来源：http://dk.chemitech.net.cn

JavaScript ..... 252
来源：http://tg.szsharing.cn

TypeScript ..... 212
来源：http://pu.521024.cn

Java ........... 212
来源：http://ye.hahajie.cn

Go ............. 212
来源：http://mi.huixinmuqiang.cn

Ruby ........... 212
来源：http://gq.chemitech.net.cn

C# ............. 212
来源：http://du.wgjwhj.cn

C .............. 30
来源：http://gb.521024.cn

C++ ............ 30
来源：http://az.gzmigu.cn

SQL ............ 90
来源：http://fu.shxzskj.cn

Bash ........... 80
来源：http://vv.521024.cn

Kotlin ......... 15
来源：http://rv.huixiangedu.cn

Swift .......... 15
来源：http://bs.wgjwhj.cn

Lua ............ 10
来源：http://ae.bjjhwx.cn

Perl ........... 10
来源：http://nj.newstarts.cn

Scala .......... 10
来源：http://ju.nszjky.cn

------------------------------------
来源：http://xn.newstarts.cn

合计 ........... 2106 条
来源：http://ss.colortex.cn

按章节统计：
来源：http://qd.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jk.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rc.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ib.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://up.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://io.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kn.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ad.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://on.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fu.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yx.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wx.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jv.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zu.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ik.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://th.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://po.gzmigu.cn


<!-- 参考信息 -->