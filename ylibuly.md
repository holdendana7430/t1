代发 wailian999

[T49] Perl：函数
来源：http://ls.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dk.colortex.cn

[T50] Perl：逐行读文件
来源：http://nc.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xm.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://wr.panjiajie.cn

[T51] Scala：Hello World
来源：http://th.yuntaijiaju.cn

println("Hello")
来源：http://or.shxzukj.cn

[T52] Scala：变量
来源：http://ns.shxzskj.cn

val a = 1;  var b = 2
来源：http://sk.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://vl.huixiangedu.cn

s"值: $b"
来源：http://cx.shtwfgs.cn

[T54] Scala：集合映射
来源：http://mg.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://az.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://kb.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qt.szsharing.cn

[T56] Scala：样例类
来源：http://iy.asd995.cn

case class User(name: String, age: Int)
来源：http://nb.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://rd.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sg.lnxyls.cn

[T58] Scala：函数定义
来源：http://vo.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mv.huixiangedu.cn

[T59] Scala：循环
来源：http://ai.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://up.huanxung.cn

[T60] Scala：折叠
来源：http://np.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tb.newstarts.cn

================================================================================
来源：http://zt.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cr.huixiangedu.cn

================================================================================
来源：http://az.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://ku.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iq.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://rn.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mn.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://bt.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mg.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://ds.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ck.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://ih.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://gn.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://fg.newstarts.cn

{**a, **b}
来源：http://di.521024.cn

[U07] Py：反转字典键值
来源：http://gd.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://hn.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://sz.521024.cn

[y for x in nested for y in x]
来源：http://df.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://wz.bjjhwx.cn

max(d, key=d.get)
来源：http://ws.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://nh.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ed.9csxet.cn

[U11] Py：生成器表达式
来源：http://fz.newstarts.cn

(x * 2 for x in arr)
来源：http://mj.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ko.shxzukj.cn

Counter(arr).most_common(3)
来源：http://oj.colortex.cn

[U13] Py：固定长度队列
来源：http://ni.huixiangedu.cn

deque(maxlen=10)
来源：http://cx.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://to.szxytkj.cn

defaultdict(list)
来源：http://bz.bjjhwx.cn

[U15] Py：高精度计时
来源：http://eb.hahajie.cn

t = time.perf_counter()
来源：http://em.asd995.cn

[U16] Py：命令行参数解析
来源：http://gv.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wk.nszjky.cn

[U17] Py：初始化日志
来源：http://vs.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://dv.chemitech.net.cn

[U18] Py：预编译正则
来源：http://zs.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://pw.nszjky.cn

[U19] Py：正则替换带回调
来源：http://tp.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mt.asd995.cn

[U20] Py：缓存函数结果
来源：http://ca.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://as.521024.cn

[U21] Py：自定义上下文管理器
来源：http://qk.hahajie.cn

@contextlib.contextmanager
来源：http://fg.shxzukj.cn

[U22] Py：矩阵转置
来源：http://qq.huixiangedu.cn

list(zip(*m))
来源：http://iv.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://fm.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nc.shxzskj.cn

[U24] Py：路径操作
来源：http://mp.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jo.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://xe.huixiangedu.cn

csv.DictReader(f)
来源：http://nt.nicolike.cn

[U26] Py：并发下载
来源：http://ay.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ar.hahajie.cn

[U27] Py：异步 HTTP
来源：http://kp.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://op.bjjhwx.cn

[U28] Py：类型别名
来源：http://gj.bjjhwx.cn

UserId = int
来源：http://zz.asd995.cn

[U29] Py：属性校验
来源：http://wz.asd995.cn

@property 与 @x.setter 配合
来源：http://yv.szsharing.cn

[U30] Py：数据类
来源：http://ey.nszjky.cn

@dataclass(slots=True)
来源：http://nu.9csxet.cn

[U31] Py：单测
来源：http://st.wgjwhj.cn

python -m pytest -q
来源：http://ty.shtwfgs.cn

[U32] Py：代码格式化
来源：http://qy.newstarts.cn

ruff format . && ruff check --fix .
来源：http://ak.asd995.cn

[U33] Py：打包发布
来源：http://tv.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://qc.shxzskj.cn

[U34] Py：判断编码
来源：http://sn.hahajie.cn

chardet.detect(raw)
来源：http://pp.yuexingan06.cn

[U35] Py：发送邮件
来源：http://ji.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pv.gzmigu.cn

[U36] Py：定时任务
来源：http://ov.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://nx.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://ec.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kq.521024.cn

[U38] Py：获取脚本所在目录
来源：http://ax.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://gw.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://ql.colortex.cn

sys.stdout.isatty()
来源：http://ln.huanxung.cn

[U40] Py：打印到标准错误
来源：http://zb.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://tu.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://qp.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zy.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://np.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qp.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://gf.shxzskj.cn

namespace App\Http;
来源：http://sl.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://oa.muxihuayi.cn

declare(strict_types=1);
来源：http://ry.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ny.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fa.wgjwhj.cn

[U46] PHP：可空类型
来源：http://sz.panjiajie.cn

?string $name = null
来源：http://en.szsharing.cn

[U47] PHP：联合类型
来源：http://sj.yuntaijiaju.cn

int|string $id
来源：http://nj.asd995.cn

[U48] PHP：纯枚举
来源：http://bg.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bz.chemitech.net.cn

[U49] PHP：只读属性
来源：http://ed.hnjuh.cn

public readonly string $name
来源：http://ql.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://ow.panjiajie.cn

public function __construct(private int $id) {}
来源：http://pm.lnxyls.cn

[U51] PHP：数组解构
来源：http://wh.shxzukj.cn

[$a, $b] = $arr;
来源：http://hy.shxzukj.cn

[U52] PHP：箭头函数
来源：http://gb.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://mq.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://fq.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://av.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://kl.panjiajie.cn

$obj?->method()
来源：http://zn.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ip.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pg.huanxung.cn

[U56] PHP：命名参数
来源：http://kb.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://vh.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://ud.nszjky.cn

"值: {$a}"
来源：http://ph.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://wn.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bt.nicolike.cn

[U59] PHP：自定义排序
来源：http://jx.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wm.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://fi.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ed.wgjwhj.cn

[U61] PHP：正则
来源：http://gh.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xy.wgjwhj.cn

[U62] PHP：日期对象
来源：http://fl.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ay.hahajie.cn

[U63] PHP：文件读写
来源：http://uh.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pj.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://tu.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ni.shxzskj.cn

[U65] PHP：会话
来源：http://zn.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vx.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://ui.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yj.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://wv.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bp.szsharing.cn

[U68] PHP：PDO 连接
来源：http://kh.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qo.colortex.cn

[U69] PHP：PDO 预处理
来源：http://ds.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dc.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://hn.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ss.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://ek.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://qu.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://eo.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://ty.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://lp.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://hx.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://wq.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://ge.nicolike.cn

[U75] PHP：依赖注入
来源：http://hm.huixiangedu.cn

composer require psr/container
来源：http://kt.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://ni.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ls.shxzukj.cn

[U77] PHP：模板渲染
来源：http://xk.huixiangedu.cn

composer require twig/twig
来源：http://bx.hnjuh.cn

[U78] PHP：单元测试
来源：http://uc.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://jy.hnjuh.cn

[U79] PHP：静态分析
来源：http://yo.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://xu.hahajie.cn

[U80] PHP：代码规范修复
来源：http://oh.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cj.lnxyls.cn

[U81] JS：初始化项目
来源：http://vw.asd995.cn

npm init -y;  npm i express
来源：http://yv.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://wj.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lq.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://bq.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mo.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ji.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nm.haigaiapp.cn

[U85] JS：可选链
来源：http://iw.nicolike.cn

a?.b?.c
来源：http://um.bjjhwx.cn

[U86] JS：空值合并
来源：http://qj.gzmigu.cn

a ?? b
来源：http://xz.colortex.cn

[U87] JS：解构默认值
来源：http://zc.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://xw.shxzukj.cn

[U88] JS：对象展开合并
来源：http://ab.nszjky.cn

{ ...a, ...b }
来源：http://va.shxzskj.cn

[U89] JS：数组去重
来源：http://zp.bjjhwx.cn

[...new Set(arr)]
来源：http://px.shxzukj.cn

[U90] JS：数字数组排序
来源：http://ku.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://az.colortex.cn

[U91] JS：对象键值遍历
来源：http://dh.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rr.wgjwhj.cn

[U92] JS：深拷贝
来源：http://td.521024.cn

structuredClone(obj)
来源：http://jh.hahajie.cn

[U93] JS：模板字符串
来源：http://su.hnjuh.cn

`共 ${n} 条`
来源：http://bc.muxihuayi.cn

[U94] JS：箭头函数
来源：http://zy.asd995.cn

const double = x => x * 2;
来源：http://ek.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://kk.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://wn.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://qb.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mn.gzmigu.cn

[U97] JS：并发请求
来源：http://ll.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://fa.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cv.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://nf.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://qh.hahajie.cn

[U100] JS：DOM 查询
来源：http://jy.hnjuh.cn

document.querySelector(".item")
来源：http://nw.huixiangedu.cn

[U101] JS：classList 操作
来源：http://nc.newstarts.cn

el.classList.toggle("active")
来源：http://qr.yuexingan06.cn

[U102] JS：本地存储
来源：http://es.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gs.hnjuh.cn

[U103] JS：定时器
来源：http://ah.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://na.huanxung.cn

[U104] JS：防抖
来源：http://wx.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sl.jctech888.com.cn

[U105] JS：节流
来源：http://hs.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cj.wgjwhj.cn

[U106] JS：日期格式化
来源：http://cg.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zi.nicolike.cn

[U107] JS：数字千分位
来源：http://sc.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fh.newstarts.cn

[U108] JS：随机整数
来源：http://rj.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fz.nicolike.cn

[U109] JS：数组分组
来源：http://gc.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://au.shxzukj.cn

[U110] JS：数组分块
来源：http://tn.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fj.hahajie.cn

[U111] JS：对象转 Map
来源：http://yq.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://xp.asd995.cn

[U112] JS：字符串补位
来源：http://nx.szsharing.cn

"7".padStart(3, "0")
来源：http://kw.hahajie.cn

[U113] JS：正则替换全部
来源：http://fu.nicolike.cn

s.replaceAll("a", "b")
来源：http://km.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ca.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tb.huanxung.cn

[U115] JS：生成 UUID
来源：http://gv.bookmarksfly.cn

crypto.randomUUID()
来源：http://sb.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://op.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://na.szsharing.cn

[U117] JS：单元测试
来源：http://bo.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://jc.huanxung.cn

[U118] JS：开发服务器
来源：http://wx.colortex.cn

npm i -D vite;  npx vite
来源：http://uk.haigaiapp.cn

[U119] JS：生产构建
来源：http://lt.panjiajie.cn

npx vite build
来源：http://yy.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://nh.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://uh.chemitech.net.cn

================================================================================
来源：http://ww.9csxet.cn

统计汇总
来源：http://oe.nszjky.cn

================================================================================
来源：http://re.colortex.cn

按语言统计（条）：
来源：http://ec.shxzskj.cn

Python ......... 252
来源：http://dx.muxihuayi.cn

PHP ............ 252
来源：http://ot.yuexingan06.cn

JavaScript ..... 252
来源：http://mx.huanxung.cn

TypeScript ..... 212
来源：http://ru.gzmigu.cn

Java ........... 212
来源：http://ks.lnxyls.cn

Go ............. 212
来源：http://an.nicolike.cn

Ruby ........... 212
来源：http://lm.shtwfgs.cn

C# ............. 212
来源：http://fm.lnxyls.cn

C .............. 30
来源：http://gj.huanxung.cn

C++ ............ 30
来源：http://nq.shxzukj.cn

SQL ............ 90
来源：http://yj.chemitech.net.cn

Bash ........... 80
来源：http://gd.gzmigu.cn

Kotlin ......... 15
来源：http://mp.hnjuh.cn

Swift .......... 15
来源：http://ke.hahajie.cn

Lua ............ 10
来源：http://xt.shxzukj.cn

Perl ........... 10
来源：http://hs.asd995.cn

Scala .......... 10
来源：http://qg.chemitech.net.cn

------------------------------------
来源：http://az.yuexingan06.cn

合计 ........... 2106 条
来源：http://ul.jctech888.com.cn

按章节统计：
来源：http://pa.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fi.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ta.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nq.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ye.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qm.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yj.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fw.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ci.colortex.cn


<!-- 参考信息 -->