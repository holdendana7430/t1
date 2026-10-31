代发 wailian999

[T47] Perl：正则捕获
来源：http://ac.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vd.newstarts.cn

[T48] Perl：正则替换
来源：http://cb.szxytkj.cn

$s =~ s/old/new/g;
来源：http://il.colortex.cn

[T49] Perl：函数
来源：http://xq.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ur.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://od.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ur.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://rf.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://us.bookmarksfly.cn

println("Hello")
来源：http://zq.jctech888.com.cn

[T52] Scala：变量
来源：http://op.colortex.cn

val a = 1;  var b = 2
来源：http://nv.521024.cn

[T53] Scala：字符串插值
来源：http://tp.chemitech.net.cn

s"值: $b"
来源：http://vv.asd995.cn

[T54] Scala：集合映射
来源：http://pj.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://cp.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://ma.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gs.yuexingan06.cn

[T56] Scala：样例类
来源：http://di.9csxet.cn

case class User(name: String, age: Int)
来源：http://iu.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ge.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zb.szxytkj.cn

[T58] Scala：函数定义
来源：http://dt.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cs.lnxyls.cn

[T59] Scala：循环
来源：http://vo.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://qa.9csxet.cn

[T60] Scala：折叠
来源：http://nn.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vq.szxytkj.cn

================================================================================
来源：http://sy.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bm.szsharing.cn

================================================================================
来源：http://xt.colortex.cn

[U01] Py：创建虚拟环境
来源：http://yd.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ut.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://ca.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wj.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://yq.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mj.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://yv.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jl.huanxung.cn

[U05] Py：列表去重且保序
来源：http://xu.nszjky.cn

list(dict.fromkeys(arr))
来源：http://nd.lnxyls.cn

[U06] Py：合并两个字典
来源：http://ji.shxzukj.cn

{**a, **b}
来源：http://in.panjiajie.cn

[U07] Py：反转字典键值
来源：http://or.nicolike.cn

{v: k for k, v in d.items()}
来源：http://dw.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://mi.shxzskj.cn

[y for x in nested for y in x]
来源：http://ub.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://du.szsharing.cn

max(d, key=d.get)
来源：http://qt.panjiajie.cn

[U10] Py：按值排序字典
来源：http://bz.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bb.nicolike.cn

[U11] Py：生成器表达式
来源：http://qb.nszjky.cn

(x * 2 for x in arr)
来源：http://lo.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wm.szsharing.cn

Counter(arr).most_common(3)
来源：http://bp.huanxung.cn

[U13] Py：固定长度队列
来源：http://sa.szsharing.cn

deque(maxlen=10)
来源：http://xz.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://vu.9csxet.cn

defaultdict(list)
来源：http://vw.szsharing.cn

[U15] Py：高精度计时
来源：http://jz.asd995.cn

t = time.perf_counter()
来源：http://nc.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://cu.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mh.haigaiapp.cn

[U17] Py：初始化日志
来源：http://oy.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://yk.nszjky.cn

[U18] Py：预编译正则
来源：http://ok.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://gd.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://wc.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wy.nszjky.cn

[U20] Py：缓存函数结果
来源：http://cj.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://iq.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://bz.colortex.cn

@contextlib.contextmanager
来源：http://ll.szxytkj.cn

[U22] Py：矩阵转置
来源：http://cs.shxzukj.cn

list(zip(*m))
来源：http://re.newstarts.cn

[U23] Py：分块读取大文件
来源：http://jx.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yx.gzmigu.cn

[U24] Py：路径操作
来源：http://eu.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fb.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://xv.muxihuayi.cn

csv.DictReader(f)
来源：http://qr.9csxet.cn

[U26] Py：并发下载
来源：http://av.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fq.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://br.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://es.chemitech.net.cn

[U28] Py：类型别名
来源：http://ap.hnjuh.cn

UserId = int
来源：http://qa.lnxyls.cn

[U29] Py：属性校验
来源：http://xh.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://fi.9csxet.cn

[U30] Py：数据类
来源：http://rk.jctech888.com.cn

@dataclass(slots=True)
来源：http://ox.shxzukj.cn

[U31] Py：单测
来源：http://pl.yuntaijiaju.cn

python -m pytest -q
来源：http://mp.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://xl.nszjky.cn

ruff format . && ruff check --fix .
来源：http://wu.szsharing.cn

[U33] Py：打包发布
来源：http://me.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://zc.muxihuayi.cn

[U34] Py：判断编码
来源：http://pq.nszjky.cn

chardet.detect(raw)
来源：http://jd.nicolike.cn

[U35] Py：发送邮件
来源：http://jl.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zj.yuexingan06.cn

[U36] Py：定时任务
来源：http://le.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://sn.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://gb.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dy.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://ls.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://vv.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ex.panjiajie.cn

sys.stdout.isatty()
来源：http://hl.nszjky.cn

[U40] Py：打印到标准错误
来源：http://cq.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://zk.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://lc.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gk.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://ms.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iv.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://gt.panjiajie.cn

namespace App\Http;
来源：http://nq.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://wi.yuntaijiaju.cn

declare(strict_types=1);
来源：http://ex.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://zh.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uh.jctech888.com.cn

[U46] PHP：可空类型
来源：http://su.nszjky.cn

?string $name = null
来源：http://lv.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://zt.huixiangedu.cn

int|string $id
来源：http://uo.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://tr.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gm.huixiangedu.cn

[U49] PHP：只读属性
来源：http://fp.huixinmuqiang.cn

public readonly string $name
来源：http://um.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://us.9csxet.cn

public function __construct(private int $id) {}
来源：http://tx.shtwfgs.cn

[U51] PHP：数组解构
来源：http://zc.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://ks.shxzukj.cn

[U52] PHP：箭头函数
来源：http://qv.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://zn.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://px.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://mf.hnjuh.cn

[U54] PHP：空安全调用
来源：http://rb.shxzskj.cn

$obj?->method()
来源：http://im.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://xz.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ij.wgjwhj.cn

[U56] PHP：命名参数
来源：http://eu.shxzskj.cn

f(a: 1, b: 2)
来源：http://qg.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://lx.9csxet.cn

"值: {$a}"
来源：http://xb.521024.cn

[U58] PHP：数组三件套
来源：http://tk.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qu.asd995.cn

[U59] PHP：自定义排序
来源：http://hp.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eb.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://fx.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ag.asd995.cn

[U61] PHP：正则
来源：http://fb.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sb.9csxet.cn

[U62] PHP：日期对象
来源：http://rg.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ce.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://lh.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ym.9csxet.cn

[U64] PHP：目录遍历
来源：http://os.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://iu.colortex.cn

[U65] PHP：会话
来源：http://vy.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ox.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://qi.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mo.hahajie.cn

[U67] PHP：处理文件上传
来源：http://im.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tu.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://ij.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zh.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://al.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ji.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://qh.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jo.panjiajie.cn

[U71] PHP：抛出异常
来源：http://ac.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://xx.hahajie.cn

[U72] PHP：写错误日志
来源：http://um.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://sj.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://gj.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://vn.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://jk.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://bl.asd995.cn

[U75] PHP：依赖注入
来源：http://bl.521024.cn

composer require psr/container
来源：http://il.nszjky.cn

[U76] PHP：简单路由
来源：http://ce.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ae.gzmigu.cn

[U77] PHP：模板渲染
来源：http://vp.huixiangedu.cn

composer require twig/twig
来源：http://wg.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://od.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://nh.shxzskj.cn

[U79] PHP：静态分析
来源：http://lr.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://il.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://ou.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://se.yuexingan06.cn

[U81] JS：初始化项目
来源：http://dz.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://hy.521024.cn

[U82] JS：package.json 脚本
来源：http://kx.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gd.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://of.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ri.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://xi.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cw.colortex.cn

[U85] JS：可选链
来源：http://cw.gzmigu.cn

a?.b?.c
来源：http://ti.huixiangedu.cn

[U86] JS：空值合并
来源：http://wa.chemitech.net.cn

a ?? b
来源：http://ub.panjiajie.cn

[U87] JS：解构默认值
来源：http://zz.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ev.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://xk.9csxet.cn

{ ...a, ...b }
来源：http://gh.muxihuayi.cn

[U89] JS：数组去重
来源：http://md.wgjwhj.cn

[...new Set(arr)]
来源：http://ea.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://xg.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://mr.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://iz.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ds.9csxet.cn

[U92] JS：深拷贝
来源：http://gp.colortex.cn

structuredClone(obj)
来源：http://xa.521024.cn

[U93] JS：模板字符串
来源：http://nh.gzmigu.cn

`共 ${n} 条`
来源：http://yp.colortex.cn

[U94] JS：箭头函数
来源：http://xf.szxytkj.cn

const double = x => x * 2;
来源：http://tm.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://ak.colortex.cn

new Promise((resolve, reject) => {})
来源：http://jq.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://vw.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://df.chemitech.net.cn

[U97] JS：并发请求
来源：http://fi.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://my.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://kb.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oy.nicolike.cn

[U99] JS：事件监听
来源：http://eu.huanxung.cn

el.addEventListener("click", e => {})
来源：http://rb.hahajie.cn

[U100] JS：DOM 查询
来源：http://co.huixinmuqiang.cn

document.querySelector(".item")
来源：http://xi.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://pu.bjjhwx.cn

el.classList.toggle("active")
来源：http://mv.chemitech.net.cn

[U102] JS：本地存储
来源：http://ch.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uq.lnxyls.cn

[U103] JS：定时器
来源：http://he.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pu.panjiajie.cn

[U104] JS：防抖
来源：http://fq.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sx.bjjhwx.cn

[U105] JS：节流
来源：http://za.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fo.newstarts.cn

[U106] JS：日期格式化
来源：http://ui.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://si.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://kg.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uv.lnxyls.cn

[U108] JS：随机整数
来源：http://ne.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rp.bjjhwx.cn

[U109] JS：数组分组
来源：http://ep.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://hm.shxzskj.cn

[U110] JS：数组分块
来源：http://ju.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ty.shxzskj.cn

[U111] JS：对象转 Map
来源：http://ok.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://sd.shtwfgs.cn

[U112] JS：字符串补位
来源：http://pn.yuexingan06.cn

"7".padStart(3, "0")
来源：http://la.shxzskj.cn

[U113] JS：正则替换全部
来源：http://fs.hahajie.cn

s.replaceAll("a", "b")
来源：http://dt.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://ud.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hw.521024.cn

[U115] JS：生成 UUID
来源：http://tf.nicolike.cn

crypto.randomUUID()
来源：http://tu.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://zh.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://qv.szsharing.cn

[U117] JS：单元测试
来源：http://tv.asd995.cn

npm i -D vitest;  npx vitest
来源：http://rh.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://zj.gzmigu.cn

npm i -D vite;  npx vite
来源：http://rw.newstarts.cn

[U119] JS：生产构建
来源：http://je.asd995.cn

npx vite build
来源：http://mh.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://ac.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://ad.nicolike.cn

================================================================================
来源：http://og.huanxung.cn

统计汇总
来源：http://gx.hahajie.cn

================================================================================
来源：http://hs.9csxet.cn

按语言统计（条）：
来源：http://ob.szxytkj.cn

Python ......... 252
来源：http://si.521024.cn

PHP ............ 252
来源：http://nh.yuexingan06.cn

JavaScript ..... 252
来源：http://sw.asd995.cn

TypeScript ..... 212
来源：http://xk.bookmarksfly.cn

Java ........... 212
来源：http://ao.gzmigu.cn

Go ............. 212
来源：http://bw.9csxet.cn

Ruby ........... 212
来源：http://qx.shxzskj.cn

C# ............. 212
来源：http://gb.huixinmuqiang.cn

C .............. 30
来源：http://is.yuntaijiaju.cn

C++ ............ 30
来源：http://go.panjiajie.cn

SQL ............ 90
来源：http://ov.hahajie.cn

Bash ........... 80
来源：http://zy.lnxyls.cn

Kotlin ......... 15
来源：http://nv.yuntaijiaju.cn

Swift .......... 15
来源：http://uu.jianghongdianzi.cn

Lua ............ 10
来源：http://iq.newstarts.cn

Perl ........... 10
来源：http://uw.wgjwhj.cn

Scala .......... 10
来源：http://wx.chemitech.net.cn

------------------------------------
来源：http://tj.bjjhwx.cn

合计 ........... 2106 条
来源：http://ou.muxihuayi.cn

按章节统计：
来源：http://co.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eo.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fg.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pi.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gc.lnxyls.cn


<!-- 参考信息 -->