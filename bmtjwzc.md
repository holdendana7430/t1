代发 wailian999

[T47] Perl：正则捕获
来源：http://mt.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ad.shxzskj.cn

[T48] Perl：正则替换
来源：http://fn.shxzukj.cn

$s =~ s/old/new/g;
来源：http://iq.521024.cn

[T49] Perl：函数
来源：http://je.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dt.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://hm.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fp.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://am.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://tg.chemitech.net.cn

println("Hello")
来源：http://xn.bookmarksfly.cn

[T52] Scala：变量
来源：http://yl.521024.cn

val a = 1;  var b = 2
来源：http://cr.shxzukj.cn

[T53] Scala：字符串插值
来源：http://kh.newstarts.cn

s"值: $b"
来源：http://ev.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://tt.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://dc.panjiajie.cn

[T55] Scala：集合过滤
来源：http://pm.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ds.haigaiapp.cn

[T56] Scala：样例类
来源：http://ws.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://si.huanxung.cn

[T57] Scala：模式匹配
来源：http://kv.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tq.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://wg.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://br.szxytkj.cn

[T59] Scala：循环
来源：http://bb.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://sv.hahajie.cn

[T60] Scala：折叠
来源：http://rz.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ch.9csxet.cn

================================================================================
来源：http://sd.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dl.shtwfgs.cn

================================================================================
来源：http://wg.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://uh.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vs.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://gv.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nc.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://rl.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zc.huanxung.cn

[U04] Py：变量调试打印
来源：http://pk.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ff.szsharing.cn

[U05] Py：列表去重且保序
来源：http://fd.521024.cn

list(dict.fromkeys(arr))
来源：http://un.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://mg.gzmigu.cn

{**a, **b}
来源：http://uz.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://fo.newstarts.cn

{v: k for k, v in d.items()}
来源：http://kj.lnxyls.cn

[U08] Py：展平二维列表
来源：http://gx.haigaiapp.cn

[y for x in nested for y in x]
来源：http://ww.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://sr.nszjky.cn

max(d, key=d.get)
来源：http://zn.shxzukj.cn

[U10] Py：按值排序字典
来源：http://yt.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mm.521024.cn

[U11] Py：生成器表达式
来源：http://ee.9csxet.cn

(x * 2 for x in arr)
来源：http://yv.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nk.hnjuh.cn

Counter(arr).most_common(3)
来源：http://xh.shxzskj.cn

[U13] Py：固定长度队列
来源：http://yq.wgjwhj.cn

deque(maxlen=10)
来源：http://nh.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://wx.jctech888.com.cn

defaultdict(list)
来源：http://ri.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://nw.huixinmuqiang.cn

t = time.perf_counter()
来源：http://bj.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://hi.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uq.jctech888.com.cn

[U17] Py：初始化日志
来源：http://qd.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://tf.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://ow.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://gd.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://es.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pb.szsharing.cn

[U20] Py：缓存函数结果
来源：http://fk.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://ij.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://xk.asd995.cn

@contextlib.contextmanager
来源：http://wx.huanxung.cn

[U22] Py：矩阵转置
来源：http://ux.shxzskj.cn

list(zip(*m))
来源：http://sf.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://vo.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://li.muxihuayi.cn

[U24] Py：路径操作
来源：http://xx.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mm.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://ub.bookmarksfly.cn

csv.DictReader(f)
来源：http://cf.nszjky.cn

[U26] Py：并发下载
来源：http://im.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qt.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://df.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://ft.bookmarksfly.cn

[U28] Py：类型别名
来源：http://ey.shxzskj.cn

UserId = int
来源：http://dl.wgjwhj.cn

[U29] Py：属性校验
来源：http://dc.colortex.cn

@property 与 @x.setter 配合
来源：http://uw.shxzskj.cn

[U30] Py：数据类
来源：http://og.bookmarksfly.cn

@dataclass(slots=True)
来源：http://ji.chemitech.net.cn

[U31] Py：单测
来源：http://hm.szsharing.cn

python -m pytest -q
来源：http://hk.shtwfgs.cn

[U32] Py：代码格式化
来源：http://va.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ca.asd995.cn

[U33] Py：打包发布
来源：http://tu.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://dk.asd995.cn

[U34] Py：判断编码
来源：http://uv.hahajie.cn

chardet.detect(raw)
来源：http://rf.shtwfgs.cn

[U35] Py：发送邮件
来源：http://hk.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yd.shxzskj.cn

[U36] Py：定时任务
来源：http://uc.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://qb.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ri.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zh.521024.cn

[U38] Py：获取脚本所在目录
来源：http://vg.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://it.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://ab.chemitech.net.cn

sys.stdout.isatty()
来源：http://dn.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://lk.521024.cn

print("err", file=sys.stderr)
来源：http://fw.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://go.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tz.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://lv.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://az.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://ax.bookmarksfly.cn

namespace App\Http;
来源：http://ji.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://im.gzmigu.cn

declare(strict_types=1);
来源：http://fa.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://yd.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.nszjky.cn

[U46] PHP：可空类型
来源：http://zv.panjiajie.cn

?string $name = null
来源：http://lh.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ed.szsharing.cn

int|string $id
来源：http://rg.colortex.cn

[U48] PHP：纯枚举
来源：http://nd.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mk.panjiajie.cn

[U49] PHP：只读属性
来源：http://sj.shxzskj.cn

public readonly string $name
来源：http://ug.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://gl.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://ec.huanxung.cn

[U51] PHP：数组解构
来源：http://kc.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://zz.newstarts.cn

[U52] PHP：箭头函数
来源：http://kg.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://pi.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://oh.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://oi.9csxet.cn

[U54] PHP：空安全调用
来源：http://ik.521024.cn

$obj?->method()
来源：http://oz.newstarts.cn

[U55] PHP：match 表达式
来源：http://xc.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yc.asd995.cn

[U56] PHP：命名参数
来源：http://ex.szxytkj.cn

f(a: 1, b: 2)
来源：http://ao.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://mf.haigaiapp.cn

"值: {$a}"
来源：http://ii.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://hj.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://di.nszjky.cn

[U59] PHP：自定义排序
来源：http://ub.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lv.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://ys.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ln.nszjky.cn

[U61] PHP：正则
来源：http://ms.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tp.jctech888.com.cn

[U62] PHP：日期对象
来源：http://cp.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kd.yuexingan06.cn

[U63] PHP：文件读写
来源：http://fr.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tr.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://xn.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://bi.yuntaijiaju.cn

[U65] PHP：会话
来源：http://cr.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yc.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://tn.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hb.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://lz.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yp.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://rw.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xw.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://lj.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ks.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://yb.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uj.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://cr.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://lc.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://lz.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://dw.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://ce.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://tl.hahajie.cn

[U74] PHP：读取环境变量
来源：http://sx.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://ik.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://iw.gzmigu.cn

composer require psr/container
来源：http://op.hnjuh.cn

[U76] PHP：简单路由
来源：http://hj.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dm.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://ul.chemitech.net.cn

composer require twig/twig
来源：http://fz.nicolike.cn

[U78] PHP：单元测试
来源：http://ea.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://fv.9csxet.cn

[U79] PHP：静态分析
来源：http://kp.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://qa.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ac.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cs.huixiangedu.cn

[U81] JS：初始化项目
来源：http://am.shxzukj.cn

npm init -y;  npm i express
来源：http://vp.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://kx.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ju.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://vi.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rt.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://pi.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ce.huixinmuqiang.cn

[U85] JS：可选链
来源：http://dd.lnxyls.cn

a?.b?.c
来源：http://ve.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://tq.wgjwhj.cn

a ?? b
来源：http://td.shtwfgs.cn

[U87] JS：解构默认值
来源：http://pa.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://gv.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://vr.hnjuh.cn

{ ...a, ...b }
来源：http://ug.colortex.cn

[U89] JS：数组去重
来源：http://hp.chemitech.net.cn

[...new Set(arr)]
来源：http://tk.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://gb.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://yc.hahajie.cn

[U91] JS：对象键值遍历
来源：http://gd.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iw.asd995.cn

[U92] JS：深拷贝
来源：http://fm.jctech888.com.cn

structuredClone(obj)
来源：http://go.hahajie.cn

[U93] JS：模板字符串
来源：http://gd.huixiangedu.cn

`共 ${n} 条`
来源：http://dj.9csxet.cn

[U94] JS：箭头函数
来源：http://yd.huixinmuqiang.cn

const double = x => x * 2;
来源：http://lw.gzmigu.cn

[U95] JS：Promise 包装
来源：http://nm.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://ju.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://yo.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oq.521024.cn

[U97] JS：并发请求
来源：http://qm.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://by.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://dh.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wv.wgjwhj.cn

[U99] JS：事件监听
来源：http://up.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://wn.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ly.yuntaijiaju.cn

document.querySelector(".item")
来源：http://az.newstarts.cn

[U101] JS：classList 操作
来源：http://qq.szxytkj.cn

el.classList.toggle("active")
来源：http://za.jctech888.com.cn

[U102] JS：本地存储
来源：http://dj.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jw.muxihuayi.cn

[U103] JS：定时器
来源：http://ly.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ua.yuexingan06.cn

[U104] JS：防抖
来源：http://gv.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xq.hahajie.cn

[U105] JS：节流
来源：http://ge.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://da.chemitech.net.cn

[U106] JS：日期格式化
来源：http://eb.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xb.szxytkj.cn

[U107] JS：数字千分位
来源：http://hz.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gn.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://wz.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gd.wgjwhj.cn

[U109] JS：数组分组
来源：http://oz.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://eb.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ap.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qe.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ry.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://qc.huixiangedu.cn

[U112] JS：字符串补位
来源：http://bt.colortex.cn

"7".padStart(3, "0")
来源：http://ss.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://rk.huanxung.cn

s.replaceAll("a", "b")
来源：http://wd.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://fj.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gy.colortex.cn

[U115] JS：生成 UUID
来源：http://da.lnxyls.cn

crypto.randomUUID()
来源：http://an.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://qn.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://cd.jctech888.com.cn

[U117] JS：单元测试
来源：http://ee.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://kx.gzmigu.cn

[U118] JS：开发服务器
来源：http://xv.hnjuh.cn

npm i -D vite;  npx vite
来源：http://vy.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://sv.haigaiapp.cn

npx vite build
来源：http://vn.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ut.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://us.nicolike.cn

================================================================================
来源：http://bb.panjiajie.cn

统计汇总
来源：http://zf.asd995.cn

================================================================================
来源：http://ih.szsharing.cn

按语言统计（条）：
来源：http://tn.9csxet.cn

Python ......... 252
来源：http://fd.szxytkj.cn

PHP ............ 252
来源：http://gb.muxihuayi.cn

JavaScript ..... 252
来源：http://kg.hahajie.cn

TypeScript ..... 212
来源：http://gb.newstarts.cn

Java ........... 212
来源：http://ub.shxzskj.cn

Go ............. 212
来源：http://fj.521024.cn

Ruby ........... 212
来源：http://nf.hnjuh.cn

C# ............. 212
来源：http://fb.hahajie.cn

C .............. 30
来源：http://bu.huixiangedu.cn

C++ ............ 30
来源：http://uo.shtwfgs.cn

SQL ............ 90
来源：http://ic.asd995.cn

Bash ........... 80
来源：http://ih.bjjhwx.cn

Kotlin ......... 15
来源：http://lw.chemitech.net.cn

Swift .......... 15
来源：http://cu.newstarts.cn

Lua ............ 10
来源：http://rm.newstarts.cn

Perl ........... 10
来源：http://lz.shxzskj.cn

Scala .......... 10
来源：http://ee.colortex.cn

------------------------------------
来源：http://vn.jctech888.com.cn

合计 ........... 2106 条
来源：http://jd.jianghongdianzi.cn

按章节统计：
来源：http://yk.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vj.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yi.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cd.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sg.yuntaijiaju.cn


<!-- 参考信息 -->