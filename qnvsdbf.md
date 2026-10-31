代发 wailian999

[T49] Perl：函数
来源：http://lx.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://es.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://ny.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gb.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://rk.shxzskj.cn

[T51] Scala：Hello World
来源：http://ik.shxzskj.cn

println("Hello")
来源：http://bj.lnxyls.cn

[T52] Scala：变量
来源：http://gq.9csxet.cn

val a = 1;  var b = 2
来源：http://gr.hahajie.cn

[T53] Scala：字符串插值
来源：http://dm.jianghongdianzi.cn

s"值: $b"
来源：http://na.haigaiapp.cn

[T54] Scala：集合映射
来源：http://vr.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ib.newstarts.cn

[T55] Scala：集合过滤
来源：http://nh.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kn.szsharing.cn

[T56] Scala：样例类
来源：http://fg.szsharing.cn

case class User(name: String, age: Int)
来源：http://vr.nicolike.cn

[T57] Scala：模式匹配
来源：http://zo.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://df.colortex.cn

[T58] Scala：函数定义
来源：http://rh.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gz.asd995.cn

[T59] Scala：循环
来源：http://vl.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://aj.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://dn.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gw.asd995.cn

================================================================================
来源：http://am.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ud.shtwfgs.cn

================================================================================
来源：http://sb.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://pb.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ul.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://hd.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gc.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://ep.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sd.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://tl.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vt.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://ks.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://tz.szxytkj.cn

[U06] Py：合并两个字典
来源：http://fu.gzmigu.cn

{**a, **b}
来源：http://th.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://dw.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://hk.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://sy.huanxung.cn

[y for x in nested for y in x]
来源：http://bl.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://tk.521024.cn

max(d, key=d.get)
来源：http://ob.szsharing.cn

[U10] Py：按值排序字典
来源：http://wj.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wb.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://ie.hnjuh.cn

(x * 2 for x in arr)
来源：http://pn.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ic.hahajie.cn

Counter(arr).most_common(3)
来源：http://zj.asd995.cn

[U13] Py：固定长度队列
来源：http://uj.muxihuayi.cn

deque(maxlen=10)
来源：http://ke.9csxet.cn

[U14] Py：分组收集到列表
来源：http://gc.haigaiapp.cn

defaultdict(list)
来源：http://ov.szxytkj.cn

[U15] Py：高精度计时
来源：http://wc.jctech888.com.cn

t = time.perf_counter()
来源：http://su.9csxet.cn

[U16] Py：命令行参数解析
来源：http://bh.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ob.jctech888.com.cn

[U17] Py：初始化日志
来源：http://oe.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://tj.haigaiapp.cn

[U18] Py：预编译正则
来源：http://sj.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://pd.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://dx.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ql.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://ro.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://zo.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://sh.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://bx.hnjuh.cn

[U22] Py：矩阵转置
来源：http://sl.nicolike.cn

list(zip(*m))
来源：http://sm.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ns.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lq.huixiangedu.cn

[U24] Py：路径操作
来源：http://rc.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mm.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://yt.lnxyls.cn

csv.DictReader(f)
来源：http://xq.asd995.cn

[U26] Py：并发下载
来源：http://wx.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://li.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://zt.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://ck.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://oo.panjiajie.cn

UserId = int
来源：http://tc.lnxyls.cn

[U29] Py：属性校验
来源：http://kf.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://cx.gzmigu.cn

[U30] Py：数据类
来源：http://jb.shtwfgs.cn

@dataclass(slots=True)
来源：http://qz.lnxyls.cn

[U31] Py：单测
来源：http://mq.huanxung.cn

python -m pytest -q
来源：http://zi.chemitech.net.cn

[U32] Py：代码格式化
来源：http://gc.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://hd.hnjuh.cn

[U33] Py：打包发布
来源：http://el.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://bi.bookmarksfly.cn

[U34] Py：判断编码
来源：http://xw.huixiangedu.cn

chardet.detect(raw)
来源：http://qq.haigaiapp.cn

[U35] Py：发送邮件
来源：http://qv.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lb.haigaiapp.cn

[U36] Py：定时任务
来源：http://kc.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://er.panjiajie.cn

[U37] Py：读写 Excel
来源：http://hi.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vm.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://hy.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://el.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://hp.chemitech.net.cn

sys.stdout.isatty()
来源：http://du.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://mo.asd995.cn

print("err", file=sys.stderr)
来源：http://wr.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://kb.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hy.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://ne.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yc.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://eb.muxihuayi.cn

namespace App\Http;
来源：http://aj.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://yl.szsharing.cn

declare(strict_types=1);
来源：http://vo.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://bg.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sk.colortex.cn

[U46] PHP：可空类型
来源：http://yv.jianghongdianzi.cn

?string $name = null
来源：http://cn.wgjwhj.cn

[U47] PHP：联合类型
来源：http://oh.9csxet.cn

int|string $id
来源：http://mp.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://ng.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uj.wgjwhj.cn

[U49] PHP：只读属性
来源：http://he.nszjky.cn

public readonly string $name
来源：http://da.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://cf.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://kh.asd995.cn

[U51] PHP：数组解构
来源：http://xp.nicolike.cn

[$a, $b] = $arr;
来源：http://ih.hahajie.cn

[U52] PHP：箭头函数
来源：http://sa.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://dx.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://sv.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://rw.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://bk.panjiajie.cn

$obj?->method()
来源：http://ip.lnxyls.cn

[U55] PHP：match 表达式
来源：http://ny.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hi.panjiajie.cn

[U56] PHP：命名参数
来源：http://cj.lnxyls.cn

f(a: 1, b: 2)
来源：http://za.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://uo.asd995.cn

"值: {$a}"
来源：http://ro.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://is.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pl.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ko.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xp.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://mt.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ur.bjjhwx.cn

[U61] PHP：正则
来源：http://ix.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zk.newstarts.cn

[U62] PHP：日期对象
来源：http://yq.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qr.shxzukj.cn

[U63] PHP：文件读写
来源：http://hs.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vl.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://vs.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://dz.asd995.cn

[U65] PHP：会话
来源：http://dh.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gb.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://ve.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bs.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://kn.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ew.szsharing.cn

[U68] PHP：PDO 连接
来源：http://ya.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qe.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://vm.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jo.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://sh.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://im.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://ej.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://sf.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://qw.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://sz.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://sx.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://ly.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://iu.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://bw.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://du.colortex.cn

composer require psr/container
来源：http://wm.chemitech.net.cn

[U76] PHP：简单路由
来源：http://ip.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ri.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://mk.nicolike.cn

composer require twig/twig
来源：http://qx.newstarts.cn

[U78] PHP：单元测试
来源：http://tr.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://je.nszjky.cn

[U79] PHP：静态分析
来源：http://ji.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://ue.521024.cn

[U80] PHP：代码规范修复
来源：http://by.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vg.hnjuh.cn

[U81] JS：初始化项目
来源：http://xq.nicolike.cn

npm init -y;  npm i express
来源：http://vf.521024.cn

[U82] JS：package.json 脚本
来源：http://pc.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://go.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://hk.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vh.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://dz.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pe.muxihuayi.cn

[U85] JS：可选链
来源：http://mh.bjjhwx.cn

a?.b?.c
来源：http://iy.wgjwhj.cn

[U86] JS：空值合并
来源：http://je.haigaiapp.cn

a ?? b
来源：http://jl.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://eu.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ko.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://qz.wgjwhj.cn

{ ...a, ...b }
来源：http://za.gzmigu.cn

[U89] JS：数组去重
来源：http://vh.yuexingan06.cn

[...new Set(arr)]
来源：http://hd.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://ft.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://do.hahajie.cn

[U91] JS：对象键值遍历
来源：http://cm.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ek.wgjwhj.cn

[U92] JS：深拷贝
来源：http://yh.szsharing.cn

structuredClone(obj)
来源：http://xq.muxihuayi.cn

[U93] JS：模板字符串
来源：http://gv.jianghongdianzi.cn

`共 ${n} 条`
来源：http://au.nicolike.cn

[U94] JS：箭头函数
来源：http://da.nszjky.cn

const double = x => x * 2;
来源：http://ry.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://kd.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://pc.9csxet.cn

[U96] JS：async/await 与异常
来源：http://ur.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://if.hnjuh.cn

[U97] JS：并发请求
来源：http://vd.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://bq.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nx.haigaiapp.cn

[U99] JS：事件监听
来源：http://hu.szsharing.cn

el.addEventListener("click", e => {})
来源：http://yy.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://qb.asd995.cn

document.querySelector(".item")
来源：http://ns.nicolike.cn

[U101] JS：classList 操作
来源：http://vk.asd995.cn

el.classList.toggle("active")
来源：http://ic.nszjky.cn

[U102] JS：本地存储
来源：http://gs.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ul.haigaiapp.cn

[U103] JS：定时器
来源：http://se.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kv.huixiangedu.cn

[U104] JS：防抖
来源：http://pq.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uj.chemitech.net.cn

[U105] JS：节流
来源：http://yp.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lp.yuexingan06.cn

[U106] JS：日期格式化
来源：http://ur.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://og.521024.cn

[U107] JS：数字千分位
来源：http://zp.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zv.gzmigu.cn

[U108] JS：随机整数
来源：http://zp.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ss.szsharing.cn

[U109] JS：数组分组
来源：http://he.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://yo.muxihuayi.cn

[U110] JS：数组分块
来源：http://xm.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xi.shxzukj.cn

[U111] JS：对象转 Map
来源：http://rs.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://qh.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://wk.panjiajie.cn

"7".padStart(3, "0")
来源：http://sa.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://nz.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://ti.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://bc.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://id.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://mr.yuexingan06.cn

crypto.randomUUID()
来源：http://vt.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ex.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://xl.asd995.cn

[U117] JS：单元测试
来源：http://db.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://vk.lnxyls.cn

[U118] JS：开发服务器
来源：http://gg.9csxet.cn

npm i -D vite;  npx vite
来源：http://yl.lnxyls.cn

[U119] JS：生产构建
来源：http://zk.hnjuh.cn

npx vite build
来源：http://gd.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://fb.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://cb.szsharing.cn

================================================================================
来源：http://xu.yuexingan06.cn

统计汇总
来源：http://tp.jctech888.com.cn

================================================================================
来源：http://jr.shxzskj.cn

按语言统计（条）：
来源：http://yx.shtwfgs.cn

Python ......... 252
来源：http://ih.bjjhwx.cn

PHP ............ 252
来源：http://om.panjiajie.cn

JavaScript ..... 252
来源：http://pz.hnjuh.cn

TypeScript ..... 212
来源：http://ar.hahajie.cn

Java ........... 212
来源：http://lf.muxihuayi.cn

Go ............. 212
来源：http://in.nicolike.cn

Ruby ........... 212
来源：http://yu.szsharing.cn

C# ............. 212
来源：http://qy.jianghongdianzi.cn

C .............. 30
来源：http://ts.yuntaijiaju.cn

C++ ............ 30
来源：http://yr.panjiajie.cn

SQL ............ 90
来源：http://hj.jctech888.com.cn

Bash ........... 80
来源：http://ia.hahajie.cn

Kotlin ......... 15
来源：http://cu.9csxet.cn

Swift .......... 15
来源：http://ul.bookmarksfly.cn

Lua ............ 10
来源：http://qd.huixiangedu.cn

Perl ........... 10
来源：http://ts.newstarts.cn

Scala .......... 10
来源：http://ss.chemitech.net.cn

------------------------------------
来源：http://qv.nszjky.cn

合计 ........... 2106 条
来源：http://am.yuntaijiaju.cn

按章节统计：
来源：http://xi.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ce.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bp.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tk.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rn.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://il.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rt.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wu.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gu.hahajie.cn


<!-- 参考信息 -->