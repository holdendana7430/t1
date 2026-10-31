代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://zr.gzmigu.cn

[T51] Scala：Hello World
来源：http://ps.jianghongdianzi.cn

println("Hello")
来源：http://oz.muxihuayi.cn

[T52] Scala：变量
来源：http://ul.521024.cn

val a = 1;  var b = 2
来源：http://kq.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://sd.huixinmuqiang.cn

s"值: $b"
来源：http://au.huixiangedu.cn

[T54] Scala：集合映射
来源：http://ku.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://jz.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://wl.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rs.panjiajie.cn

[T56] Scala：样例类
来源：http://sq.panjiajie.cn

case class User(name: String, age: Int)
来源：http://ia.colortex.cn

[T57] Scala：模式匹配
来源：http://jy.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hr.hnjuh.cn

[T58] Scala：函数定义
来源：http://ma.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ql.shtwfgs.cn

[T59] Scala：循环
来源：http://um.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://fo.muxihuayi.cn

[T60] Scala：折叠
来源：http://ft.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ep.hahajie.cn

================================================================================
来源：http://we.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bj.wgjwhj.cn

================================================================================
来源：http://py.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://mw.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sl.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://hv.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fn.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://jc.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ti.lnxyls.cn

[U04] Py：变量调试打印
来源：http://jl.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://db.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://ue.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://sq.shxzskj.cn

[U06] Py：合并两个字典
来源：http://xl.shtwfgs.cn

{**a, **b}
来源：http://vn.huanxung.cn

[U07] Py：反转字典键值
来源：http://mm.hahajie.cn

{v: k for k, v in d.items()}
来源：http://cj.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://aj.asd995.cn

[y for x in nested for y in x]
来源：http://ot.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://gt.jianghongdianzi.cn

max(d, key=d.get)
来源：http://di.shxzukj.cn

[U10] Py：按值排序字典
来源：http://rk.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iq.szsharing.cn

[U11] Py：生成器表达式
来源：http://ac.chemitech.net.cn

(x * 2 for x in arr)
来源：http://cf.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oc.huanxung.cn

Counter(arr).most_common(3)
来源：http://nm.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://qe.huanxung.cn

deque(maxlen=10)
来源：http://mr.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://zn.jctech888.com.cn

defaultdict(list)
来源：http://tj.panjiajie.cn

[U15] Py：高精度计时
来源：http://dq.521024.cn

t = time.perf_counter()
来源：http://uz.huanxung.cn

[U16] Py：命令行参数解析
来源：http://ym.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pr.shxzukj.cn

[U17] Py：初始化日志
来源：http://py.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zq.chemitech.net.cn

[U18] Py：预编译正则
来源：http://eq.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://my.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://vd.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eu.9csxet.cn

[U20] Py：缓存函数结果
来源：http://th.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://ng.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://yt.muxihuayi.cn

@contextlib.contextmanager
来源：http://nn.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://ov.lnxyls.cn

list(zip(*m))
来源：http://br.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://et.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sr.hnjuh.cn

[U24] Py：路径操作
来源：http://od.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cx.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://zp.shtwfgs.cn

csv.DictReader(f)
来源：http://ir.bookmarksfly.cn

[U26] Py：并发下载
来源：http://jd.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://na.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://tm.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://aq.yuexingan06.cn

[U28] Py：类型别名
来源：http://oz.nicolike.cn

UserId = int
来源：http://ij.chemitech.net.cn

[U29] Py：属性校验
来源：http://aa.shxzukj.cn

@property 与 @x.setter 配合
来源：http://hs.shxzskj.cn

[U30] Py：数据类
来源：http://ko.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://ga.yuexingan06.cn

[U31] Py：单测
来源：http://pc.hnjuh.cn

python -m pytest -q
来源：http://bq.hahajie.cn

[U32] Py：代码格式化
来源：http://yp.nszjky.cn

ruff format . && ruff check --fix .
来源：http://ym.lnxyls.cn

[U33] Py：打包发布
来源：http://fv.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ta.szsharing.cn

[U34] Py：判断编码
来源：http://nt.szxytkj.cn

chardet.detect(raw)
来源：http://vv.huixiangedu.cn

[U35] Py：发送邮件
来源：http://av.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gh.shxzskj.cn

[U36] Py：定时任务
来源：http://zp.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://mq.szxytkj.cn

[U37] Py：读写 Excel
来源：http://sn.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ck.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://no.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://oy.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://vi.chemitech.net.cn

sys.stdout.isatty()
来源：http://uo.521024.cn

[U40] Py：打印到标准错误
来源：http://pc.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://vv.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ie.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xz.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://lk.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tg.colortex.cn

[U43] PHP：声明命名空间
来源：http://vc.huanxung.cn

namespace App\Http;
来源：http://ij.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://jq.yuexingan06.cn

declare(strict_types=1);
来源：http://io.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://da.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ho.szsharing.cn

[U46] PHP：可空类型
来源：http://os.nicolike.cn

?string $name = null
来源：http://lg.panjiajie.cn

[U47] PHP：联合类型
来源：http://kt.asd995.cn

int|string $id
来源：http://ci.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://oy.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sj.lnxyls.cn

[U49] PHP：只读属性
来源：http://ts.wgjwhj.cn

public readonly string $name
来源：http://yu.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ct.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://cg.nicolike.cn

[U51] PHP：数组解构
来源：http://ln.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://sj.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ca.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://vs.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://oa.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://ah.newstarts.cn

[U54] PHP：空安全调用
来源：http://do.gzmigu.cn

$obj?->method()
来源：http://tv.lnxyls.cn

[U55] PHP：match 表达式
来源：http://fu.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qd.szxytkj.cn

[U56] PHP：命名参数
来源：http://mi.colortex.cn

f(a: 1, b: 2)
来源：http://mw.nicolike.cn

[U57] PHP：字符串插值
来源：http://cv.shxzskj.cn

"值: {$a}"
来源：http://fz.huanxung.cn

[U58] PHP：数组三件套
来源：http://vx.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ch.szsharing.cn

[U59] PHP：自定义排序
来源：http://ej.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vp.colortex.cn

[U60] PHP：JSON 编解码
来源：http://er.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://md.huixinmuqiang.cn

[U61] PHP：正则
来源：http://ur.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rg.szxytkj.cn

[U62] PHP：日期对象
来源：http://uc.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hm.szsharing.cn

[U63] PHP：文件读写
来源：http://tn.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vh.nicolike.cn

[U64] PHP：目录遍历
来源：http://jd.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://io.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ln.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ct.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://xc.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xp.asd995.cn

[U67] PHP：处理文件上传
来源：http://dv.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ot.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://rc.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bu.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://yd.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pi.9csxet.cn

[U70] PHP：PDO 事务
来源：http://bp.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jc.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://ve.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://kn.huanxung.cn

[U72] PHP：写错误日志
来源：http://ib.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://wv.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://by.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://un.nszjky.cn

[U74] PHP：读取环境变量
来源：http://pm.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://pw.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://lt.colortex.cn

composer require psr/container
来源：http://mm.521024.cn

[U76] PHP：简单路由
来源：http://kd.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://is.shxzskj.cn

[U77] PHP：模板渲染
来源：http://ip.newstarts.cn

composer require twig/twig
来源：http://wc.asd995.cn

[U78] PHP：单元测试
来源：http://tv.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://xo.hahajie.cn

[U79] PHP：静态分析
来源：http://tt.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://le.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://il.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sj.hnjuh.cn

[U81] JS：初始化项目
来源：http://ee.huanxung.cn

npm init -y;  npm i express
来源：http://da.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://qs.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rx.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ku.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lq.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://iv.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xr.panjiajie.cn

[U85] JS：可选链
来源：http://eo.shtwfgs.cn

a?.b?.c
来源：http://mw.521024.cn

[U86] JS：空值合并
来源：http://fo.newstarts.cn

a ?? b
来源：http://ov.yuexingan06.cn

[U87] JS：解构默认值
来源：http://vz.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://us.gzmigu.cn

[U88] JS：对象展开合并
来源：http://lg.chemitech.net.cn

{ ...a, ...b }
来源：http://zr.shxzskj.cn

[U89] JS：数组去重
来源：http://kn.hahajie.cn

[...new Set(arr)]
来源：http://ka.colortex.cn

[U90] JS：数字数组排序
来源：http://vi.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://bq.huanxung.cn

[U91] JS：对象键值遍历
来源：http://lf.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ex.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://is.bookmarksfly.cn

structuredClone(obj)
来源：http://jd.shxzskj.cn

[U93] JS：模板字符串
来源：http://nk.lnxyls.cn

`共 ${n} 条`
来源：http://kq.shxzskj.cn

[U94] JS：箭头函数
来源：http://cs.chemitech.net.cn

const double = x => x * 2;
来源：http://dr.nszjky.cn

[U95] JS：Promise 包装
来源：http://mo.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://an.colortex.cn

[U96] JS：async/await 与异常
来源：http://et.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fa.colortex.cn

[U97] JS：并发请求
来源：http://id.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yx.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://ko.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bp.bookmarksfly.cn

[U99] JS：事件监听
来源：http://gk.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://nv.hahajie.cn

[U100] JS：DOM 查询
来源：http://ri.huanxung.cn

document.querySelector(".item")
来源：http://yp.panjiajie.cn

[U101] JS：classList 操作
来源：http://xu.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://zo.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://ai.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gj.9csxet.cn

[U103] JS：定时器
来源：http://gz.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dq.jianghongdianzi.cn

[U104] JS：防抖
来源：http://ue.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cj.huixinmuqiang.cn

[U105] JS：节流
来源：http://gi.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ne.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://ql.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yr.gzmigu.cn

[U107] JS：数字千分位
来源：http://vi.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ve.muxihuayi.cn

[U108] JS：随机整数
来源：http://ue.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qa.yuexingan06.cn

[U109] JS：数组分组
来源：http://vn.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://ha.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://bv.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dx.shxzukj.cn

[U111] JS：对象转 Map
来源：http://yg.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://au.chemitech.net.cn

[U112] JS：字符串补位
来源：http://of.jctech888.com.cn

"7".padStart(3, "0")
来源：http://va.newstarts.cn

[U113] JS：正则替换全部
来源：http://df.szsharing.cn

s.replaceAll("a", "b")
来源：http://xz.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://bb.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://da.newstarts.cn

[U115] JS：生成 UUID
来源：http://co.hahajie.cn

crypto.randomUUID()
来源：http://az.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://no.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://im.bookmarksfly.cn

[U117] JS：单元测试
来源：http://gj.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://tf.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://sr.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://mh.panjiajie.cn

[U119] JS：生产构建
来源：http://yy.huixinmuqiang.cn

npx vite build
来源：http://rx.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://py.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://fp.hnjuh.cn

================================================================================
来源：http://oj.yuntaijiaju.cn

统计汇总
来源：http://hm.9csxet.cn

================================================================================
来源：http://fp.huixiangedu.cn

按语言统计（条）：
来源：http://mk.newstarts.cn

Python ......... 252
来源：http://nv.lnxyls.cn

PHP ............ 252
来源：http://pp.jctech888.com.cn

JavaScript ..... 252
来源：http://kp.jctech888.com.cn

TypeScript ..... 212
来源：http://ty.chemitech.net.cn

Java ........... 212
来源：http://vr.gzmigu.cn

Go ............. 212
来源：http://fp.haigaiapp.cn

Ruby ........... 212
来源：http://ac.chemitech.net.cn

C# ............. 212
来源：http://ho.huixinmuqiang.cn

C .............. 30
来源：http://jb.chemitech.net.cn

C++ ............ 30
来源：http://su.shxzukj.cn

SQL ............ 90
来源：http://zf.shtwfgs.cn

Bash ........... 80
来源：http://bh.szsharing.cn

Kotlin ......... 15
来源：http://oo.chemitech.net.cn

Swift .......... 15
来源：http://mi.huixiangedu.cn

Lua ............ 10
来源：http://um.shxzskj.cn

Perl ........... 10
来源：http://po.huanxung.cn

Scala .......... 10
来源：http://wm.hnjuh.cn

------------------------------------
来源：http://eu.haigaiapp.cn

合计 ........... 2106 条
来源：http://da.newstarts.cn

按章节统计：
来源：http://lz.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://to.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zn.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gq.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zh.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gm.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zk.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qz.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lz.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bo.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ol.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dz.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zh.haigaiapp.cn


<!-- 参考信息 -->