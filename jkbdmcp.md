代发 wailian999

[T47] Perl：正则捕获
来源：http://xe.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iz.szsharing.cn

[T48] Perl：正则替换
来源：http://xt.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ek.jianghongdianzi.cn

[T49] Perl：函数
来源：http://um.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rf.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://bk.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gu.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://mq.hnjuh.cn

[T51] Scala：Hello World
来源：http://gd.huixiangedu.cn

println("Hello")
来源：http://ll.shtwfgs.cn

[T52] Scala：变量
来源：http://wb.szsharing.cn

val a = 1;  var b = 2
来源：http://fr.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://dw.shtwfgs.cn

s"值: $b"
来源：http://zs.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://kx.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://ze.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://en.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nz.hnjuh.cn

[T56] Scala：样例类
来源：http://gk.hahajie.cn

case class User(name: String, age: Int)
来源：http://uz.panjiajie.cn

[T57] Scala：模式匹配
来源：http://lx.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zl.panjiajie.cn

[T58] Scala：函数定义
来源：http://up.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://so.shxzukj.cn

[T59] Scala：循环
来源：http://cw.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://ty.huanxung.cn

[T60] Scala：折叠
来源：http://jb.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bt.shxzukj.cn

================================================================================
来源：http://im.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oo.jctech888.com.cn

================================================================================
来源：http://hb.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://gj.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xr.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://jj.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oj.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://dx.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ms.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://vf.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ty.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://gf.hahajie.cn

list(dict.fromkeys(arr))
来源：http://if.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ne.panjiajie.cn

{**a, **b}
来源：http://xf.huanxung.cn

[U07] Py：反转字典键值
来源：http://jw.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://ih.hahajie.cn

[U08] Py：展平二维列表
来源：http://ze.asd995.cn

[y for x in nested for y in x]
来源：http://ud.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://hh.szxytkj.cn

max(d, key=d.get)
来源：http://ri.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://zf.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ej.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://ed.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://ya.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://go.newstarts.cn

Counter(arr).most_common(3)
来源：http://se.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://zp.panjiajie.cn

deque(maxlen=10)
来源：http://fb.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://na.huixinmuqiang.cn

defaultdict(list)
来源：http://zv.jctech888.com.cn

[U15] Py：高精度计时
来源：http://js.yuexingan06.cn

t = time.perf_counter()
来源：http://wx.521024.cn

[U16] Py：命令行参数解析
来源：http://rc.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ay.szsharing.cn

[U17] Py：初始化日志
来源：http://tb.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://uj.nicolike.cn

[U18] Py：预编译正则
来源：http://pq.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://nv.huanxung.cn

[U19] Py：正则替换带回调
来源：http://tx.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jf.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://fl.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://cd.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://ig.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://pt.9csxet.cn

[U22] Py：矩阵转置
来源：http://ga.jianghongdianzi.cn

list(zip(*m))
来源：http://rt.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://bk.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ns.shtwfgs.cn

[U24] Py：路径操作
来源：http://ox.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yy.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://nl.huixiangedu.cn

csv.DictReader(f)
来源：http://my.huixiangedu.cn

[U26] Py：并发下载
来源：http://dp.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jo.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://zz.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://gy.panjiajie.cn

[U28] Py：类型别名
来源：http://nt.jctech888.com.cn

UserId = int
来源：http://sc.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://ek.newstarts.cn

@property 与 @x.setter 配合
来源：http://ii.lnxyls.cn

[U30] Py：数据类
来源：http://bc.chemitech.net.cn

@dataclass(slots=True)
来源：http://rh.shxzukj.cn

[U31] Py：单测
来源：http://mc.yuntaijiaju.cn

python -m pytest -q
来源：http://ld.9csxet.cn

[U32] Py：代码格式化
来源：http://su.szsharing.cn

ruff format . && ruff check --fix .
来源：http://tl.hahajie.cn

[U33] Py：打包发布
来源：http://ly.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ij.bookmarksfly.cn

[U34] Py：判断编码
来源：http://rt.colortex.cn

chardet.detect(raw)
来源：http://yo.hnjuh.cn

[U35] Py：发送邮件
来源：http://qg.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://by.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://vk.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://ho.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://fa.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vl.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ro.asd995.cn

Path(__file__).resolve().parent
来源：http://gt.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://zl.jctech888.com.cn

sys.stdout.isatty()
来源：http://na.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://al.huanxung.cn

print("err", file=sys.stderr)
来源：http://fj.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://kr.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pc.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://an.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qe.nszjky.cn

[U43] PHP：声明命名空间
来源：http://jv.hnjuh.cn

namespace App\Http;
来源：http://cj.hahajie.cn

[U44] PHP：开启严格类型
来源：http://gk.huixiangedu.cn

declare(strict_types=1);
来源：http://wn.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://gv.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bn.nszjky.cn

[U46] PHP：可空类型
来源：http://zt.haigaiapp.cn

?string $name = null
来源：http://wk.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://yi.asd995.cn

int|string $id
来源：http://za.shxzukj.cn

[U48] PHP：纯枚举
来源：http://ft.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ia.9csxet.cn

[U49] PHP：只读属性
来源：http://bw.shxzukj.cn

public readonly string $name
来源：http://xi.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://zy.521024.cn

public function __construct(private int $id) {}
来源：http://qq.panjiajie.cn

[U51] PHP：数组解构
来源：http://qm.szsharing.cn

[$a, $b] = $arr;
来源：http://km.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://yk.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://oi.colortex.cn

[U53] PHP：空合并运算符
来源：http://kx.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://jl.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://lo.hahajie.cn

$obj?->method()
来源：http://no.hahajie.cn

[U55] PHP：match 表达式
来源：http://dn.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yu.9csxet.cn

[U56] PHP：命名参数
来源：http://ks.gzmigu.cn

f(a: 1, b: 2)
来源：http://za.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://bf.nszjky.cn

"值: {$a}"
来源：http://zn.nszjky.cn

[U58] PHP：数组三件套
来源：http://gk.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://to.szsharing.cn

[U59] PHP：自定义排序
来源：http://xh.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qb.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://ef.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wf.asd995.cn

[U61] PHP：正则
来源：http://ql.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ox.shxzskj.cn

[U62] PHP：日期对象
来源：http://bx.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zj.huanxung.cn

[U63] PHP：文件读写
来源：http://as.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hl.shxzskj.cn

[U64] PHP：目录遍历
来源：http://js.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://ik.shxzskj.cn

[U65] PHP：会话
来源：http://ee.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xq.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://om.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eq.nszjky.cn

[U67] PHP：处理文件上传
来源：http://oe.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sy.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://gk.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vt.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://ao.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gb.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ku.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hy.hahajie.cn

[U71] PHP：抛出异常
来源：http://ho.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://vx.hnjuh.cn

[U72] PHP：写错误日志
来源：http://gy.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://pm.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://ck.colortex.cn

parse_ini_file("config.ini", true)
来源：http://yc.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://es.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://og.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://vv.jianghongdianzi.cn

composer require psr/container
来源：http://rg.haigaiapp.cn

[U76] PHP：简单路由
来源：http://xv.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ma.huanxung.cn

[U77] PHP：模板渲染
来源：http://uj.colortex.cn

composer require twig/twig
来源：http://nc.hnjuh.cn

[U78] PHP：单元测试
来源：http://fr.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://js.yuexingan06.cn

[U79] PHP：静态分析
来源：http://ya.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://rl.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://qi.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ms.lnxyls.cn

[U81] JS：初始化项目
来源：http://rf.hahajie.cn

npm init -y;  npm i express
来源：http://ia.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://qe.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vr.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://en.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gy.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://an.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qp.panjiajie.cn

[U85] JS：可选链
来源：http://en.szsharing.cn

a?.b?.c
来源：http://sq.panjiajie.cn

[U86] JS：空值合并
来源：http://hy.hahajie.cn

a ?? b
来源：http://se.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://uh.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://cw.lnxyls.cn

[U88] JS：对象展开合并
来源：http://rf.szxytkj.cn

{ ...a, ...b }
来源：http://ji.hahajie.cn

[U89] JS：数组去重
来源：http://co.newstarts.cn

[...new Set(arr)]
来源：http://zd.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://vk.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://gn.9csxet.cn

[U91] JS：对象键值遍历
来源：http://oz.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ig.huanxung.cn

[U92] JS：深拷贝
来源：http://mb.nicolike.cn

structuredClone(obj)
来源：http://fj.nicolike.cn

[U93] JS：模板字符串
来源：http://ma.newstarts.cn

`共 ${n} 条`
来源：http://br.nicolike.cn

[U94] JS：箭头函数
来源：http://xi.jctech888.com.cn

const double = x => x * 2;
来源：http://yq.shxzskj.cn

[U95] JS：Promise 包装
来源：http://ot.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://do.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://pe.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bo.szxytkj.cn

[U97] JS：并发请求
来源：http://oq.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://py.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://ie.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yi.lnxyls.cn

[U99] JS：事件监听
来源：http://up.521024.cn

el.addEventListener("click", e => {})
来源：http://yu.colortex.cn

[U100] JS：DOM 查询
来源：http://uq.521024.cn

document.querySelector(".item")
来源：http://zc.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://il.szxytkj.cn

el.classList.toggle("active")
来源：http://mx.jctech888.com.cn

[U102] JS：本地存储
来源：http://vs.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ka.nszjky.cn

[U103] JS：定时器
来源：http://ve.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://om.jctech888.com.cn

[U104] JS：防抖
来源：http://vk.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tk.hnjuh.cn

[U105] JS：节流
来源：http://da.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pk.lnxyls.cn

[U106] JS：日期格式化
来源：http://lx.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qr.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://rw.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fr.shxzukj.cn

[U108] JS：随机整数
来源：http://gx.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bj.chemitech.net.cn

[U109] JS：数组分组
来源：http://sd.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://kx.shtwfgs.cn

[U110] JS：数组分块
来源：http://vt.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ts.shxzukj.cn

[U111] JS：对象转 Map
来源：http://yp.panjiajie.cn

new Map(Object.entries(obj))
来源：http://zk.jctech888.com.cn

[U112] JS：字符串补位
来源：http://tg.newstarts.cn

"7".padStart(3, "0")
来源：http://qh.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://zc.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://ea.9csxet.cn

[U114] JS：JSON 深比较
来源：http://ng.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fb.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://wb.shxzskj.cn

crypto.randomUUID()
来源：http://oh.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ix.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://bp.521024.cn

[U117] JS：单元测试
来源：http://kc.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://ok.newstarts.cn

[U118] JS：开发服务器
来源：http://di.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://ob.hnjuh.cn

[U119] JS：生产构建
来源：http://gd.szsharing.cn

npx vite build
来源：http://pb.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://xf.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ee.lnxyls.cn

================================================================================
来源：http://kv.panjiajie.cn

统计汇总
来源：http://co.haigaiapp.cn

================================================================================
来源：http://pz.szsharing.cn

按语言统计（条）：
来源：http://sb.muxihuayi.cn

Python ......... 252
来源：http://iy.jctech888.com.cn

PHP ............ 252
来源：http://qu.jctech888.com.cn

JavaScript ..... 252
来源：http://jl.szxytkj.cn

TypeScript ..... 212
来源：http://hl.jianghongdianzi.cn

Java ........... 212
来源：http://nx.szsharing.cn

Go ............. 212
来源：http://fj.huixiangedu.cn

Ruby ........... 212
来源：http://gp.shtwfgs.cn

C# ............. 212
来源：http://xy.yuexingan06.cn

C .............. 30
来源：http://wr.huanxung.cn

C++ ............ 30
来源：http://oc.chemitech.net.cn

SQL ............ 90
来源：http://nb.lnxyls.cn

Bash ........... 80
来源：http://dt.jianghongdianzi.cn

Kotlin ......... 15
来源：http://pf.bookmarksfly.cn

Swift .......... 15
来源：http://qn.shxzskj.cn

Lua ............ 10
来源：http://ds.hnjuh.cn

Perl ........... 10
来源：http://hv.szsharing.cn

Scala .......... 10
来源：http://nf.newstarts.cn

------------------------------------
来源：http://nm.colortex.cn

合计 ........... 2106 条
来源：http://nf.nszjky.cn

按章节统计：
来源：http://yt.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hg.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aw.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hq.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://um.wgjwhj.cn


<!-- 参考信息 -->