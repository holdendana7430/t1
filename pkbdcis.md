代发 wailian999

[T49] Perl：函数
来源：http://gn.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://am.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://ip.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ak.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://sw.nicolike.cn

[T51] Scala：Hello World
来源：http://fh.gzmigu.cn

println("Hello")
来源：http://nj.panjiajie.cn

[T52] Scala：变量
来源：http://se.nicolike.cn

val a = 1;  var b = 2
来源：http://aq.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://gp.gzmigu.cn

s"值: $b"
来源：http://jr.szsharing.cn

[T54] Scala：集合映射
来源：http://qu.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://wz.hahajie.cn

[T55] Scala：集合过滤
来源：http://tt.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://za.hnjuh.cn

[T56] Scala：样例类
来源：http://dt.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://xf.szxytkj.cn

[T57] Scala：模式匹配
来源：http://tz.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hw.asd995.cn

[T58] Scala：函数定义
来源：http://rv.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sb.jianghongdianzi.cn

[T59] Scala：循环
来源：http://bk.521024.cn

for (i <- 1 to 10) println(i)
来源：http://mu.nicolike.cn

[T60] Scala：折叠
来源：http://wc.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qo.huixinmuqiang.cn

================================================================================
来源：http://lj.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://le.szsharing.cn

================================================================================
来源：http://js.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://jh.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lc.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://mk.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bq.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://yk.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oc.lnxyls.cn

[U04] Py：变量调试打印
来源：http://ng.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nd.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://hv.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://lj.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://yz.hahajie.cn

{**a, **b}
来源：http://bx.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://rg.nicolike.cn

{v: k for k, v in d.items()}
来源：http://be.lnxyls.cn

[U08] Py：展平二维列表
来源：http://db.colortex.cn

[y for x in nested for y in x]
来源：http://le.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://qt.panjiajie.cn

max(d, key=d.get)
来源：http://hf.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://om.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ec.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://bf.521024.cn

(x * 2 for x in arr)
来源：http://uq.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://od.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://kv.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://oc.yuntaijiaju.cn

deque(maxlen=10)
来源：http://af.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://qn.haigaiapp.cn

defaultdict(list)
来源：http://wx.chemitech.net.cn

[U15] Py：高精度计时
来源：http://le.huixiangedu.cn

t = time.perf_counter()
来源：http://zx.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://bw.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vb.hnjuh.cn

[U17] Py：初始化日志
来源：http://jb.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://dh.521024.cn

[U18] Py：预编译正则
来源：http://gq.521024.cn

pat = re.compile(r"\d+")
来源：http://jl.colortex.cn

[U19] Py：正则替换带回调
来源：http://uc.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tm.521024.cn

[U20] Py：缓存函数结果
来源：http://ch.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://nw.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ir.gzmigu.cn

@contextlib.contextmanager
来源：http://gl.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://hx.yuntaijiaju.cn

list(zip(*m))
来源：http://om.colortex.cn

[U23] Py：分块读取大文件
来源：http://wq.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hp.huanxung.cn

[U24] Py：路径操作
来源：http://ke.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sy.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://iy.bookmarksfly.cn

csv.DictReader(f)
来源：http://ow.huixiangedu.cn

[U26] Py：并发下载
来源：http://ua.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iw.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://pl.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://dt.haigaiapp.cn

[U28] Py：类型别名
来源：http://vy.huanxung.cn

UserId = int
来源：http://sr.haigaiapp.cn

[U29] Py：属性校验
来源：http://gz.lnxyls.cn

@property 与 @x.setter 配合
来源：http://nz.jctech888.com.cn

[U30] Py：数据类
来源：http://qv.newstarts.cn

@dataclass(slots=True)
来源：http://zx.lnxyls.cn

[U31] Py：单测
来源：http://mk.haigaiapp.cn

python -m pytest -q
来源：http://nt.wgjwhj.cn

[U32] Py：代码格式化
来源：http://tw.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://lr.nicolike.cn

[U33] Py：打包发布
来源：http://jy.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://rt.wgjwhj.cn

[U34] Py：判断编码
来源：http://id.hahajie.cn

chardet.detect(raw)
来源：http://ja.9csxet.cn

[U35] Py：发送邮件
来源：http://hb.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qi.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://sg.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ap.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://rp.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rx.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://jk.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://sd.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://ip.shxzukj.cn

sys.stdout.isatty()
来源：http://bs.hahajie.cn

[U40] Py：打印到标准错误
来源：http://cv.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://hb.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://sn.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sg.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://id.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zy.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://lz.wgjwhj.cn

namespace App\Http;
来源：http://nh.szsharing.cn

[U44] PHP：开启严格类型
来源：http://bg.yuntaijiaju.cn

declare(strict_types=1);
来源：http://ve.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://cy.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.521024.cn

[U46] PHP：可空类型
来源：http://bt.gzmigu.cn

?string $name = null
来源：http://tc.shxzskj.cn

[U47] PHP：联合类型
来源：http://xp.gzmigu.cn

int|string $id
来源：http://az.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://dy.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cz.hnjuh.cn

[U49] PHP：只读属性
来源：http://ui.szxytkj.cn

public readonly string $name
来源：http://hw.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://ya.colortex.cn

public function __construct(private int $id) {}
来源：http://ns.muxihuayi.cn

[U51] PHP：数组解构
来源：http://nz.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ct.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://wj.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://er.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://iy.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://ub.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://nc.wgjwhj.cn

$obj?->method()
来源：http://iv.panjiajie.cn

[U55] PHP：match 表达式
来源：http://ye.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kn.gzmigu.cn

[U56] PHP：命名参数
来源：http://xx.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://lj.huanxung.cn

[U57] PHP：字符串插值
来源：http://nq.szxytkj.cn

"值: {$a}"
来源：http://cb.lnxyls.cn

[U58] PHP：数组三件套
来源：http://hm.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yg.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://wl.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sg.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://qh.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zu.newstarts.cn

[U61] PHP：正则
来源：http://tj.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bk.haigaiapp.cn

[U62] PHP：日期对象
来源：http://lb.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dh.asd995.cn

[U63] PHP：文件读写
来源：http://pu.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://li.newstarts.cn

[U64] PHP：目录遍历
来源：http://hc.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://oj.szxytkj.cn

[U65] PHP：会话
来源：http://yn.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ky.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://wf.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qg.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://io.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zn.nszjky.cn

[U68] PHP：PDO 连接
来源：http://vn.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jn.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://wa.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bw.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://mp.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nj.nszjky.cn

[U71] PHP：抛出异常
来源：http://tx.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://en.shxzukj.cn

[U72] PHP：写错误日志
来源：http://np.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://zy.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://rk.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://ha.521024.cn

[U74] PHP：读取环境变量
来源：http://qq.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://cv.nicolike.cn

[U75] PHP：依赖注入
来源：http://ib.szsharing.cn

composer require psr/container
来源：http://to.nicolike.cn

[U76] PHP：简单路由
来源：http://pu.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hi.hahajie.cn

[U77] PHP：模板渲染
来源：http://wf.jctech888.com.cn

composer require twig/twig
来源：http://nu.szsharing.cn

[U78] PHP：单元测试
来源：http://cm.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://uj.huanxung.cn

[U79] PHP：静态分析
来源：http://aj.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://lv.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://sl.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sg.521024.cn

[U81] JS：初始化项目
来源：http://hv.hnjuh.cn

npm init -y;  npm i express
来源：http://dq.521024.cn

[U82] JS：package.json 脚本
来源：http://yn.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ym.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ah.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://di.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://la.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tn.bookmarksfly.cn

[U85] JS：可选链
来源：http://gz.nszjky.cn

a?.b?.c
来源：http://sm.wgjwhj.cn

[U86] JS：空值合并
来源：http://eg.jianghongdianzi.cn

a ?? b
来源：http://de.huixiangedu.cn

[U87] JS：解构默认值
来源：http://yx.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://xq.shxzukj.cn

[U88] JS：对象展开合并
来源：http://ji.haigaiapp.cn

{ ...a, ...b }
来源：http://kx.chemitech.net.cn

[U89] JS：数组去重
来源：http://br.huixiangedu.cn

[...new Set(arr)]
来源：http://sl.huanxung.cn

[U90] JS：数字数组排序
来源：http://sr.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://bb.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://ui.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lz.yuexingan06.cn

[U92] JS：深拷贝
来源：http://ij.huanxung.cn

structuredClone(obj)
来源：http://qc.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://mc.colortex.cn

`共 ${n} 条`
来源：http://iv.hnjuh.cn

[U94] JS：箭头函数
来源：http://mp.haigaiapp.cn

const double = x => x * 2;
来源：http://uy.panjiajie.cn

[U95] JS：Promise 包装
来源：http://nl.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://am.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://vg.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zb.panjiajie.cn

[U97] JS：并发请求
来源：http://df.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yo.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://ki.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rj.asd995.cn

[U99] JS：事件监听
来源：http://xq.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://hy.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://ql.nicolike.cn

document.querySelector(".item")
来源：http://bc.newstarts.cn

[U101] JS：classList 操作
来源：http://hp.bjjhwx.cn

el.classList.toggle("active")
来源：http://ry.shtwfgs.cn

[U102] JS：本地存储
来源：http://ax.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://om.huixiangedu.cn

[U103] JS：定时器
来源：http://bl.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ad.shxzukj.cn

[U104] JS：防抖
来源：http://yz.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pd.newstarts.cn

[U105] JS：节流
来源：http://fb.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gx.lnxyls.cn

[U106] JS：日期格式化
来源：http://uu.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gr.lnxyls.cn

[U107] JS：数字千分位
来源：http://nj.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://al.colortex.cn

[U108] JS：随机整数
来源：http://jt.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xg.wgjwhj.cn

[U109] JS：数组分组
来源：http://yg.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://ts.asd995.cn

[U110] JS：数组分块
来源：http://wc.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kx.szxytkj.cn

[U111] JS：对象转 Map
来源：http://ok.lnxyls.cn

new Map(Object.entries(obj))
来源：http://dx.521024.cn

[U112] JS：字符串补位
来源：http://ow.jctech888.com.cn

"7".padStart(3, "0")
来源：http://vh.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://da.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://qi.newstarts.cn

[U114] JS：JSON 深比较
来源：http://as.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ky.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://xz.szxytkj.cn

crypto.randomUUID()
来源：http://cs.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://zg.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://by.bookmarksfly.cn

[U117] JS：单元测试
来源：http://nz.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://bx.muxihuayi.cn

[U118] JS：开发服务器
来源：http://do.lnxyls.cn

npm i -D vite;  npx vite
来源：http://se.nicolike.cn

[U119] JS：生产构建
来源：http://wt.lnxyls.cn

npx vite build
来源：http://up.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://es.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://ma.szsharing.cn

================================================================================
来源：http://gi.chemitech.net.cn

统计汇总
来源：http://fn.hnjuh.cn

================================================================================
来源：http://cm.wgjwhj.cn

按语言统计（条）：
来源：http://xg.asd995.cn

Python ......... 252
来源：http://it.521024.cn

PHP ............ 252
来源：http://zb.panjiajie.cn

JavaScript ..... 252
来源：http://mh.jctech888.com.cn

TypeScript ..... 212
来源：http://rd.nszjky.cn

Java ........... 212
来源：http://ni.muxihuayi.cn

Go ............. 212
来源：http://ec.bjjhwx.cn

Ruby ........... 212
来源：http://zo.yuexingan06.cn

C# ............. 212
来源：http://pg.haigaiapp.cn

C .............. 30
来源：http://jx.shxzskj.cn

C++ ............ 30
来源：http://mg.yuexingan06.cn

SQL ............ 90
来源：http://hg.hnjuh.cn

Bash ........... 80
来源：http://lm.szsharing.cn

Kotlin ......... 15
来源：http://is.yuexingan06.cn

Swift .......... 15
来源：http://np.muxihuayi.cn

Lua ............ 10
来源：http://wq.newstarts.cn

Perl ........... 10
来源：http://im.panjiajie.cn

Scala .......... 10
来源：http://vy.nicolike.cn

------------------------------------
来源：http://ia.yuexingan06.cn

合计 ........... 2106 条
来源：http://hm.hahajie.cn

按章节统计：
来源：http://aa.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qb.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ma.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yl.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://os.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cv.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bj.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nv.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ze.panjiajie.cn


<!-- 参考信息 -->