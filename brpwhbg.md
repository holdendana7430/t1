代发 wailian999

[T47] Perl：正则捕获
来源：http://xe.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pp.szxytkj.cn

[T48] Perl：正则替换
来源：http://xi.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://ii.huixinmuqiang.cn

[T49] Perl：函数
来源：http://ap.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://of.szsharing.cn

[T50] Perl：逐行读文件
来源：http://el.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://km.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://fz.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://yg.yuntaijiaju.cn

println("Hello")
来源：http://zh.lnxyls.cn

[T52] Scala：变量
来源：http://lq.nicolike.cn

val a = 1;  var b = 2
来源：http://ul.shxzskj.cn

[T53] Scala：字符串插值
来源：http://rv.asd995.cn

s"值: $b"
来源：http://rc.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://tl.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://ut.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://kv.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ec.bookmarksfly.cn

[T56] Scala：样例类
来源：http://lz.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ec.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://od.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ea.shxzukj.cn

[T58] Scala：函数定义
来源：http://ua.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lj.huixinmuqiang.cn

[T59] Scala：循环
来源：http://oi.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://qc.chemitech.net.cn

[T60] Scala：折叠
来源：http://yq.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wp.szxytkj.cn

================================================================================
来源：http://xs.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fe.panjiajie.cn

================================================================================
来源：http://mz.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://kl.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kh.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://sg.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cp.521024.cn

[U03] Py：加载 .env 配置
来源：http://rf.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ny.nszjky.cn

[U04] Py：变量调试打印
来源：http://ya.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://az.hahajie.cn

[U05] Py：列表去重且保序
来源：http://by.nszjky.cn

list(dict.fromkeys(arr))
来源：http://qp.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://tg.shxzskj.cn

{**a, **b}
来源：http://az.panjiajie.cn

[U07] Py：反转字典键值
来源：http://hi.nicolike.cn

{v: k for k, v in d.items()}
来源：http://lm.nszjky.cn

[U08] Py：展平二维列表
来源：http://rd.shtwfgs.cn

[y for x in nested for y in x]
来源：http://xx.asd995.cn

[U09] Py：字典取最大值的键
来源：http://uv.nicolike.cn

max(d, key=d.get)
来源：http://bh.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://fw.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kx.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://yk.bjjhwx.cn

(x * 2 for x in arr)
来源：http://ia.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wz.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://pc.lnxyls.cn

[U13] Py：固定长度队列
来源：http://af.yuntaijiaju.cn

deque(maxlen=10)
来源：http://eq.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ir.shxzukj.cn

defaultdict(list)
来源：http://cw.huanxung.cn

[U15] Py：高精度计时
来源：http://xt.jianghongdianzi.cn

t = time.perf_counter()
来源：http://hs.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://ft.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://my.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://rb.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://hx.huanxung.cn

[U18] Py：预编译正则
来源：http://ls.9csxet.cn

pat = re.compile(r"\d+")
来源：http://sm.hahajie.cn

[U19] Py：正则替换带回调
来源：http://gt.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yn.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://hv.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://li.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://yz.haigaiapp.cn

@contextlib.contextmanager
来源：http://mw.9csxet.cn

[U22] Py：矩阵转置
来源：http://wc.jianghongdianzi.cn

list(zip(*m))
来源：http://he.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://rx.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gt.newstarts.cn

[U24] Py：路径操作
来源：http://to.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qm.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://wr.yuntaijiaju.cn

csv.DictReader(f)
来源：http://mo.lnxyls.cn

[U26] Py：并发下载
来源：http://px.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ak.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://zt.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://mw.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://pr.haigaiapp.cn

UserId = int
来源：http://ce.muxihuayi.cn

[U29] Py：属性校验
来源：http://mf.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://zh.wgjwhj.cn

[U30] Py：数据类
来源：http://qo.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://mp.huixinmuqiang.cn

[U31] Py：单测
来源：http://pb.nszjky.cn

python -m pytest -q
来源：http://sm.jctech888.com.cn

[U32] Py：代码格式化
来源：http://ln.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://kh.shxzskj.cn

[U33] Py：打包发布
来源：http://ut.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://mh.gzmigu.cn

[U34] Py：判断编码
来源：http://pr.shxzskj.cn

chardet.detect(raw)
来源：http://qk.jctech888.com.cn

[U35] Py：发送邮件
来源：http://tj.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://so.huanxung.cn

[U36] Py：定时任务
来源：http://lj.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://ae.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ln.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bk.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://fe.colortex.cn

Path(__file__).resolve().parent
来源：http://qx.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://qx.szxytkj.cn

sys.stdout.isatty()
来源：http://ta.newstarts.cn

[U40] Py：打印到标准错误
来源：http://jn.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://mb.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://bq.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ya.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://lj.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gb.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://cr.shxzukj.cn

namespace App\Http;
来源：http://nw.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://mj.huixinmuqiang.cn

declare(strict_types=1);
来源：http://jz.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://kr.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ib.nszjky.cn

[U46] PHP：可空类型
来源：http://mu.yuntaijiaju.cn

?string $name = null
来源：http://pp.jctech888.com.cn

[U47] PHP：联合类型
来源：http://ef.bookmarksfly.cn

int|string $id
来源：http://ts.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://pw.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zh.szsharing.cn

[U49] PHP：只读属性
来源：http://vm.shxzukj.cn

public readonly string $name
来源：http://mx.521024.cn

[U50] PHP：构造器属性提升
来源：http://oh.panjiajie.cn

public function __construct(private int $id) {}
来源：http://tr.muxihuayi.cn

[U51] PHP：数组解构
来源：http://jg.szsharing.cn

[$a, $b] = $arr;
来源：http://xl.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://hi.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://xi.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://wd.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://mh.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://dd.shxzukj.cn

$obj?->method()
来源：http://ki.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://di.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ni.haigaiapp.cn

[U56] PHP：命名参数
来源：http://qg.shxzskj.cn

f(a: 1, b: 2)
来源：http://to.lnxyls.cn

[U57] PHP：字符串插值
来源：http://mq.shtwfgs.cn

"值: {$a}"
来源：http://en.hahajie.cn

[U58] PHP：数组三件套
来源：http://qi.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ve.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://fr.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ff.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://wa.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ng.hnjuh.cn

[U61] PHP：正则
来源：http://od.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qd.521024.cn

[U62] PHP：日期对象
来源：http://wg.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nl.shtwfgs.cn

[U63] PHP：文件读写
来源：http://wy.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://di.hahajie.cn

[U64] PHP：目录遍历
来源：http://qk.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://zk.jianghongdianzi.cn

[U65] PHP：会话
来源：http://gy.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://to.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://om.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://el.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://fv.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gn.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://ot.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bs.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://oi.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rs.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://us.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lv.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://au.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ay.gzmigu.cn

[U72] PHP：写错误日志
来源：http://uq.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://wy.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://hk.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://gh.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://eq.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://sq.colortex.cn

[U75] PHP：依赖注入
来源：http://xq.hnjuh.cn

composer require psr/container
来源：http://jh.panjiajie.cn

[U76] PHP：简单路由
来源：http://ws.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kg.shxzukj.cn

[U77] PHP：模板渲染
来源：http://qn.shxzskj.cn

composer require twig/twig
来源：http://bx.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://gb.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://vc.lnxyls.cn

[U79] PHP：静态分析
来源：http://fb.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://cj.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://ek.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wr.asd995.cn

[U81] JS：初始化项目
来源：http://dg.wgjwhj.cn

npm init -y;  npm i express
来源：http://uy.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://no.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://on.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://cm.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ux.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://ir.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wo.bjjhwx.cn

[U85] JS：可选链
来源：http://po.yuexingan06.cn

a?.b?.c
来源：http://mk.gzmigu.cn

[U86] JS：空值合并
来源：http://iv.bjjhwx.cn

a ?? b
来源：http://ws.wgjwhj.cn

[U87] JS：解构默认值
来源：http://mg.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://mm.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://ul.hnjuh.cn

{ ...a, ...b }
来源：http://rp.chemitech.net.cn

[U89] JS：数组去重
来源：http://mx.jianghongdianzi.cn

[...new Set(arr)]
来源：http://rp.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://xi.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://hg.colortex.cn

[U91] JS：对象键值遍历
来源：http://ek.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uj.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://mp.lnxyls.cn

structuredClone(obj)
来源：http://fi.shtwfgs.cn

[U93] JS：模板字符串
来源：http://sx.muxihuayi.cn

`共 ${n} 条`
来源：http://lv.szsharing.cn

[U94] JS：箭头函数
来源：http://ej.nszjky.cn

const double = x => x * 2;
来源：http://my.hahajie.cn

[U95] JS：Promise 包装
来源：http://pq.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://jg.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://kq.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vh.shxzskj.cn

[U97] JS：并发请求
来源：http://bb.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://sr.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ap.yuexingan06.cn

[U99] JS：事件监听
来源：http://tm.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://lx.huanxung.cn

[U100] JS：DOM 查询
来源：http://sz.szxytkj.cn

document.querySelector(".item")
来源：http://wy.szsharing.cn

[U101] JS：classList 操作
来源：http://ge.hnjuh.cn

el.classList.toggle("active")
来源：http://cw.panjiajie.cn

[U102] JS：本地存储
来源：http://uc.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ha.jctech888.com.cn

[U103] JS：定时器
来源：http://ha.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://io.hahajie.cn

[U104] JS：防抖
来源：http://kx.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sf.9csxet.cn

[U105] JS：节流
来源：http://vn.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bo.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://fj.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nf.wgjwhj.cn

[U107] JS：数字千分位
来源：http://uo.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sp.chemitech.net.cn

[U108] JS：随机整数
来源：http://az.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iw.9csxet.cn

[U109] JS：数组分组
来源：http://yb.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://sh.szsharing.cn

[U110] JS：数组分块
来源：http://qr.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yj.nicolike.cn

[U111] JS：对象转 Map
来源：http://py.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://vo.shxzukj.cn

[U112] JS：字符串补位
来源：http://dp.9csxet.cn

"7".padStart(3, "0")
来源：http://kf.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://zz.9csxet.cn

s.replaceAll("a", "b")
来源：http://vt.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://an.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kk.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ip.hahajie.cn

crypto.randomUUID()
来源：http://qf.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://zw.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://bm.muxihuayi.cn

[U117] JS：单元测试
来源：http://zo.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://vp.huixiangedu.cn

[U118] JS：开发服务器
来源：http://bl.hahajie.cn

npm i -D vite;  npx vite
来源：http://jw.jctech888.com.cn

[U119] JS：生产构建
来源：http://nj.shxzskj.cn

npx vite build
来源：http://ux.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://pk.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://rw.huixinmuqiang.cn

================================================================================
来源：http://rz.shxzukj.cn

统计汇总
来源：http://ww.hahajie.cn

================================================================================
来源：http://fc.yuexingan06.cn

按语言统计（条）：
来源：http://ya.newstarts.cn

Python ......... 252
来源：http://ra.nicolike.cn

PHP ............ 252
来源：http://ax.jianghongdianzi.cn

JavaScript ..... 252
来源：http://vs.shtwfgs.cn

TypeScript ..... 212
来源：http://dt.szsharing.cn

Java ........... 212
来源：http://ag.gzmigu.cn

Go ............. 212
来源：http://iw.nszjky.cn

Ruby ........... 212
来源：http://tq.521024.cn

C# ............. 212
来源：http://mc.haigaiapp.cn

C .............. 30
来源：http://wq.nicolike.cn

C++ ............ 30
来源：http://qo.bjjhwx.cn

SQL ............ 90
来源：http://zq.szxytkj.cn

Bash ........... 80
来源：http://iw.gzmigu.cn

Kotlin ......... 15
来源：http://lb.hnjuh.cn

Swift .......... 15
来源：http://nc.bookmarksfly.cn

Lua ............ 10
来源：http://va.szsharing.cn

Perl ........... 10
来源：http://ps.shxzskj.cn

Scala .......... 10
来源：http://wu.szsharing.cn

------------------------------------
来源：http://nv.nszjky.cn

合计 ........... 2106 条
来源：http://sc.shxzskj.cn

按章节统计：
来源：http://fn.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://se.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ax.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uu.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ph.hnjuh.cn


<!-- 参考信息 -->