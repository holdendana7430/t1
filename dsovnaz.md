代发 wailian999

[T47] Perl：正则捕获
来源：http://qs.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zx.newstarts.cn

[T48] Perl：正则替换
来源：http://ht.shxzskj.cn

$s =~ s/old/new/g;
来源：http://gv.9csxet.cn

[T49] Perl：函数
来源：http://hd.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xb.szsharing.cn

[T50] Perl：逐行读文件
来源：http://jc.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://di.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ps.nicolike.cn

[T51] Scala：Hello World
来源：http://qc.bjjhwx.cn

println("Hello")
来源：http://he.yuexingan06.cn

[T52] Scala：变量
来源：http://pf.haigaiapp.cn

val a = 1;  var b = 2
来源：http://kd.521024.cn

[T53] Scala：字符串插值
来源：http://zc.nicolike.cn

s"值: $b"
来源：http://ee.nszjky.cn

[T54] Scala：集合映射
来源：http://kf.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://ys.shxzukj.cn

[T55] Scala：集合过滤
来源：http://hl.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://db.panjiajie.cn

[T56] Scala：样例类
来源：http://ou.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://tm.szxytkj.cn

[T57] Scala：模式匹配
来源：http://vz.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vg.newstarts.cn

[T58] Scala：函数定义
来源：http://jm.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qa.yuexingan06.cn

[T59] Scala：循环
来源：http://yx.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://vf.9csxet.cn

[T60] Scala：折叠
来源：http://wp.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fd.chemitech.net.cn

================================================================================
来源：http://gt.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ns.muxihuayi.cn

================================================================================
来源：http://pn.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://ic.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nt.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ii.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ie.asd995.cn

[U03] Py：加载 .env 配置
来源：http://ei.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oq.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://oi.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rh.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://fy.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://vb.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://pz.huanxung.cn

{**a, **b}
来源：http://ub.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://ku.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://gz.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://ty.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://pa.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://xc.huixiangedu.cn

max(d, key=d.get)
来源：http://ju.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://iu.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qa.521024.cn

[U11] Py：生成器表达式
来源：http://ox.muxihuayi.cn

(x * 2 for x in arr)
来源：http://iv.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oc.lnxyls.cn

Counter(arr).most_common(3)
来源：http://wp.panjiajie.cn

[U13] Py：固定长度队列
来源：http://rv.newstarts.cn

deque(maxlen=10)
来源：http://cf.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://de.szsharing.cn

defaultdict(list)
来源：http://rn.hahajie.cn

[U15] Py：高精度计时
来源：http://in.nszjky.cn

t = time.perf_counter()
来源：http://lf.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://ov.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rw.bjjhwx.cn

[U17] Py：初始化日志
来源：http://mr.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://yb.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://tr.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://oa.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://wa.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jk.szsharing.cn

[U20] Py：缓存函数结果
来源：http://au.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://vc.521024.cn

[U21] Py：自定义上下文管理器
来源：http://uz.wgjwhj.cn

@contextlib.contextmanager
来源：http://ra.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://fq.huanxung.cn

list(zip(*m))
来源：http://zw.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://uf.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zz.jctech888.com.cn

[U24] Py：路径操作
来源：http://pl.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://be.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://ar.haigaiapp.cn

csv.DictReader(f)
来源：http://oz.panjiajie.cn

[U26] Py：并发下载
来源：http://zj.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xp.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://pv.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://ou.lnxyls.cn

[U28] Py：类型别名
来源：http://is.jctech888.com.cn

UserId = int
来源：http://jz.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://ch.colortex.cn

@property 与 @x.setter 配合
来源：http://hl.asd995.cn

[U30] Py：数据类
来源：http://vn.haigaiapp.cn

@dataclass(slots=True)
来源：http://so.muxihuayi.cn

[U31] Py：单测
来源：http://tz.jianghongdianzi.cn

python -m pytest -q
来源：http://vz.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://lg.colortex.cn

ruff format . && ruff check --fix .
来源：http://hk.hahajie.cn

[U33] Py：打包发布
来源：http://fa.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://ga.szsharing.cn

[U34] Py：判断编码
来源：http://xx.muxihuayi.cn

chardet.detect(raw)
来源：http://na.colortex.cn

[U35] Py：发送邮件
来源：http://lo.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hm.gzmigu.cn

[U36] Py：定时任务
来源：http://xt.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://ai.asd995.cn

[U37] Py：读写 Excel
来源：http://pt.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rp.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://yv.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://gu.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://ju.hahajie.cn

sys.stdout.isatty()
来源：http://lb.huanxung.cn

[U40] Py：打印到标准错误
来源：http://qo.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://jb.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://pz.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gm.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://wn.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xf.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://ym.gzmigu.cn

namespace App\Http;
来源：http://ze.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://cm.panjiajie.cn

declare(strict_types=1);
来源：http://oi.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://ub.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jl.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://fr.asd995.cn

?string $name = null
来源：http://xs.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://eh.haigaiapp.cn

int|string $id
来源：http://nz.szxytkj.cn

[U48] PHP：纯枚举
来源：http://yl.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cc.szxytkj.cn

[U49] PHP：只读属性
来源：http://od.muxihuayi.cn

public readonly string $name
来源：http://pt.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://ie.shxzskj.cn

public function __construct(private int $id) {}
来源：http://yj.shxzukj.cn

[U51] PHP：数组解构
来源：http://xs.colortex.cn

[$a, $b] = $arr;
来源：http://ia.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://ot.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://dm.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ie.521024.cn

$v = $a ?? $b ?? "default";
来源：http://ls.nicolike.cn

[U54] PHP：空安全调用
来源：http://ag.huixinmuqiang.cn

$obj?->method()
来源：http://ii.newstarts.cn

[U55] PHP：match 表达式
来源：http://gl.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bp.bjjhwx.cn

[U56] PHP：命名参数
来源：http://xg.nicolike.cn

f(a: 1, b: 2)
来源：http://hd.szxytkj.cn

[U57] PHP：字符串插值
来源：http://gh.szsharing.cn

"值: {$a}"
来源：http://bi.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ff.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rd.colortex.cn

[U59] PHP：自定义排序
来源：http://dz.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hi.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://rj.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dr.haigaiapp.cn

[U61] PHP：正则
来源：http://sd.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dm.colortex.cn

[U62] PHP：日期对象
来源：http://cw.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yl.lnxyls.cn

[U63] PHP：文件读写
来源：http://tp.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dj.521024.cn

[U64] PHP：目录遍历
来源：http://mf.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://kh.hnjuh.cn

[U65] PHP：会话
来源：http://rx.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rv.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://ly.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pv.hahajie.cn

[U67] PHP：处理文件上传
来源：http://hb.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bi.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://zf.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ag.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://ax.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vg.asd995.cn

[U70] PHP：PDO 事务
来源：http://pl.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dw.szsharing.cn

[U71] PHP：抛出异常
来源：http://gp.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ko.asd995.cn

[U72] PHP：写错误日志
来源：http://pu.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://my.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://jt.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://ez.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://jr.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://mx.nszjky.cn

[U75] PHP：依赖注入
来源：http://aj.wgjwhj.cn

composer require psr/container
来源：http://ih.haigaiapp.cn

[U76] PHP：简单路由
来源：http://eb.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dt.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://nr.lnxyls.cn

composer require twig/twig
来源：http://rz.wgjwhj.cn

[U78] PHP：单元测试
来源：http://wz.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://ng.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ko.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://gb.9csxet.cn

[U80] PHP：代码规范修复
来源：http://ot.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xr.nszjky.cn

[U81] JS：初始化项目
来源：http://jh.newstarts.cn

npm init -y;  npm i express
来源：http://sr.huanxung.cn

[U82] JS：package.json 脚本
来源：http://lh.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nj.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://kk.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wi.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://yx.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tf.yuntaijiaju.cn

[U85] JS：可选链
来源：http://vp.wgjwhj.cn

a?.b?.c
来源：http://zo.szxytkj.cn

[U86] JS：空值合并
来源：http://wy.newstarts.cn

a ?? b
来源：http://en.wgjwhj.cn

[U87] JS：解构默认值
来源：http://ir.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://oi.521024.cn

[U88] JS：对象展开合并
来源：http://nn.huixinmuqiang.cn

{ ...a, ...b }
来源：http://zj.yuexingan06.cn

[U89] JS：数组去重
来源：http://st.gzmigu.cn

[...new Set(arr)]
来源：http://wu.shxzskj.cn

[U90] JS：数字数组排序
来源：http://ni.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://ba.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://de.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wb.bjjhwx.cn

[U92] JS：深拷贝
来源：http://es.nicolike.cn

structuredClone(obj)
来源：http://fb.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://pi.hahajie.cn

`共 ${n} 条`
来源：http://tu.huanxung.cn

[U94] JS：箭头函数
来源：http://km.colortex.cn

const double = x => x * 2;
来源：http://zt.lnxyls.cn

[U95] JS：Promise 包装
来源：http://ey.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://og.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://oj.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gr.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://vk.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://by.521024.cn

[U98] JS：fetch 带 JSON
来源：http://er.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ac.shxzukj.cn

[U99] JS：事件监听
来源：http://be.hahajie.cn

el.addEventListener("click", e => {})
来源：http://so.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://kj.szsharing.cn

document.querySelector(".item")
来源：http://nr.nszjky.cn

[U101] JS：classList 操作
来源：http://go.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://ob.gzmigu.cn

[U102] JS：本地存储
来源：http://ta.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://an.asd995.cn

[U103] JS：定时器
来源：http://ug.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bl.nicolike.cn

[U104] JS：防抖
来源：http://ay.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xt.muxihuayi.cn

[U105] JS：节流
来源：http://nh.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xm.lnxyls.cn

[U106] JS：日期格式化
来源：http://ws.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ab.hnjuh.cn

[U107] JS：数字千分位
来源：http://cr.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://se.haigaiapp.cn

[U108] JS：随机整数
来源：http://pr.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vx.yuexingan06.cn

[U109] JS：数组分组
来源：http://aw.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://jm.chemitech.net.cn

[U110] JS：数组分块
来源：http://qj.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wv.szxytkj.cn

[U111] JS：对象转 Map
来源：http://yj.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://vf.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://ar.bjjhwx.cn

"7".padStart(3, "0")
来源：http://fk.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://eq.colortex.cn

s.replaceAll("a", "b")
来源：http://we.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://wk.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lk.shxzskj.cn

[U115] JS：生成 UUID
来源：http://tc.huixiangedu.cn

crypto.randomUUID()
来源：http://ns.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ma.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ud.newstarts.cn

[U117] JS：单元测试
来源：http://ys.asd995.cn

npm i -D vitest;  npx vitest
来源：http://jy.lnxyls.cn

[U118] JS：开发服务器
来源：http://wz.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://zp.huanxung.cn

[U119] JS：生产构建
来源：http://sn.shxzskj.cn

npx vite build
来源：http://ow.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://zj.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://py.lnxyls.cn

================================================================================
来源：http://gn.szxytkj.cn

统计汇总
来源：http://hd.panjiajie.cn

================================================================================
来源：http://aj.nicolike.cn

按语言统计（条）：
来源：http://lb.9csxet.cn

Python ......... 252
来源：http://vc.jianghongdianzi.cn

PHP ............ 252
来源：http://hy.shtwfgs.cn

JavaScript ..... 252
来源：http://gp.huixinmuqiang.cn

TypeScript ..... 212
来源：http://ey.9csxet.cn

Java ........... 212
来源：http://hx.panjiajie.cn

Go ............. 212
来源：http://zq.521024.cn

Ruby ........... 212
来源：http://vt.huixinmuqiang.cn

C# ............. 212
来源：http://za.shtwfgs.cn

C .............. 30
来源：http://jy.521024.cn

C++ ............ 30
来源：http://iw.521024.cn

SQL ............ 90
来源：http://ud.yuntaijiaju.cn

Bash ........... 80
来源：http://rw.hahajie.cn

Kotlin ......... 15
来源：http://hw.yuntaijiaju.cn

Swift .......... 15
来源：http://xs.jianghongdianzi.cn

Lua ............ 10
来源：http://kj.lnxyls.cn

Perl ........... 10
来源：http://iq.521024.cn

Scala .......... 10
来源：http://uk.huixinmuqiang.cn

------------------------------------
来源：http://oq.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://zb.yuntaijiaju.cn

按章节统计：
来源：http://fq.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uc.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pg.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vr.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ot.nszjky.cn


<!-- 参考信息 -->