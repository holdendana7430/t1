代发 wailian999

[T45] Perl：数组遍历
来源：http://hb.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://js.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://ko.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nr.521024.cn

[T47] Perl：正则捕获
来源：http://pg.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hv.shxzskj.cn

[T48] Perl：正则替换
来源：http://hq.lnxyls.cn

$s =~ s/old/new/g;
来源：http://pt.asd995.cn

[T49] Perl：函数
来源：http://wg.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sd.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ea.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ce.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://xp.jctech888.com.cn

[T51] Scala：Hello World
来源：http://hd.lnxyls.cn

println("Hello")
来源：http://ez.huixinmuqiang.cn

[T52] Scala：变量
来源：http://af.wgjwhj.cn

val a = 1;  var b = 2
来源：http://ak.9csxet.cn

[T53] Scala：字符串插值
来源：http://io.szsharing.cn

s"值: $b"
来源：http://cn.lnxyls.cn

[T54] Scala：集合映射
来源：http://ma.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://nh.nszjky.cn

[T55] Scala：集合过滤
来源：http://ln.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uq.hnjuh.cn

[T56] Scala：样例类
来源：http://ot.9csxet.cn

case class User(name: String, age: Int)
来源：http://hy.nszjky.cn

[T57] Scala：模式匹配
来源：http://xo.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sl.gzmigu.cn

[T58] Scala：函数定义
来源：http://ss.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ww.wgjwhj.cn

[T59] Scala：循环
来源：http://wn.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://jl.panjiajie.cn

[T60] Scala：折叠
来源：http://fz.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zt.huixiangedu.cn

================================================================================
来源：http://zt.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dg.9csxet.cn

================================================================================
来源：http://fz.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://nk.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://si.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://ly.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jn.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://yp.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zs.szsharing.cn

[U04] Py：变量调试打印
来源：http://he.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zj.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://gn.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://wj.nszjky.cn

[U06] Py：合并两个字典
来源：http://lm.wgjwhj.cn

{**a, **b}
来源：http://xc.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://go.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://dc.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://qo.asd995.cn

[y for x in nested for y in x]
来源：http://fh.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://mu.muxihuayi.cn

max(d, key=d.get)
来源：http://wk.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://xa.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kd.shxzukj.cn

[U11] Py：生成器表达式
来源：http://hm.asd995.cn

(x * 2 for x in arr)
来源：http://an.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uj.szxytkj.cn

Counter(arr).most_common(3)
来源：http://jr.nszjky.cn

[U13] Py：固定长度队列
来源：http://ks.huixinmuqiang.cn

deque(maxlen=10)
来源：http://sr.newstarts.cn

[U14] Py：分组收集到列表
来源：http://nt.bookmarksfly.cn

defaultdict(list)
来源：http://og.shtwfgs.cn

[U15] Py：高精度计时
来源：http://tp.9csxet.cn

t = time.perf_counter()
来源：http://ye.nszjky.cn

[U16] Py：命令行参数解析
来源：http://vt.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gl.huixiangedu.cn

[U17] Py：初始化日志
来源：http://gd.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://ds.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://gb.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://vd.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://wj.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ui.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://yi.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://hb.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://eo.hahajie.cn

@contextlib.contextmanager
来源：http://te.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://th.nszjky.cn

list(zip(*m))
来源：http://ju.colortex.cn

[U23] Py：分块读取大文件
来源：http://tf.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wx.colortex.cn

[U24] Py：路径操作
来源：http://tg.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mi.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://dr.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ic.chemitech.net.cn

[U26] Py：并发下载
来源：http://gk.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://as.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://oq.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://hd.lnxyls.cn

[U28] Py：类型别名
来源：http://ig.hahajie.cn

UserId = int
来源：http://lx.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://xa.521024.cn

@property 与 @x.setter 配合
来源：http://ea.szsharing.cn

[U30] Py：数据类
来源：http://sm.shxzukj.cn

@dataclass(slots=True)
来源：http://ww.chemitech.net.cn

[U31] Py：单测
来源：http://ju.jianghongdianzi.cn

python -m pytest -q
来源：http://ct.haigaiapp.cn

[U32] Py：代码格式化
来源：http://jj.hahajie.cn

ruff format . && ruff check --fix .
来源：http://nh.chemitech.net.cn

[U33] Py：打包发布
来源：http://je.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://br.wgjwhj.cn

[U34] Py：判断编码
来源：http://io.jianghongdianzi.cn

chardet.detect(raw)
来源：http://th.shxzukj.cn

[U35] Py：发送邮件
来源：http://gi.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dc.colortex.cn

[U36] Py：定时任务
来源：http://fw.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://fr.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://oq.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rj.521024.cn

[U38] Py：获取脚本所在目录
来源：http://in.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://py.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://rc.chemitech.net.cn

sys.stdout.isatty()
来源：http://hq.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://hk.shxzskj.cn

print("err", file=sys.stderr)
来源：http://jp.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://qt.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gx.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://da.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gv.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://id.huixiangedu.cn

namespace App\Http;
来源：http://se.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://xb.huixinmuqiang.cn

declare(strict_types=1);
来源：http://xi.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://wp.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kg.nicolike.cn

[U46] PHP：可空类型
来源：http://nz.huixiangedu.cn

?string $name = null
来源：http://mr.nicolike.cn

[U47] PHP：联合类型
来源：http://vb.szxytkj.cn

int|string $id
来源：http://lb.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://cf.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vu.szsharing.cn

[U49] PHP：只读属性
来源：http://ci.bookmarksfly.cn

public readonly string $name
来源：http://yq.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://mz.hnjuh.cn

public function __construct(private int $id) {}
来源：http://uk.newstarts.cn

[U51] PHP：数组解构
来源：http://zh.wgjwhj.cn

[$a, $b] = $arr;
来源：http://zi.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://nz.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://jx.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ae.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://ab.newstarts.cn

[U54] PHP：空安全调用
来源：http://um.jianghongdianzi.cn

$obj?->method()
来源：http://zb.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://wm.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qc.asd995.cn

[U56] PHP：命名参数
来源：http://ka.hahajie.cn

f(a: 1, b: 2)
来源：http://cq.521024.cn

[U57] PHP：字符串插值
来源：http://dl.shxzskj.cn

"值: {$a}"
来源：http://rb.szsharing.cn

[U58] PHP：数组三件套
来源：http://cp.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uf.9csxet.cn

[U59] PHP：自定义排序
来源：http://bd.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zc.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://bw.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bx.yuntaijiaju.cn

[U61] PHP：正则
来源：http://wl.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vx.shxzukj.cn

[U62] PHP：日期对象
来源：http://rg.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rw.nszjky.cn

[U63] PHP：文件读写
来源：http://ln.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gh.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://cp.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://nc.huanxung.cn

[U65] PHP：会话
来源：http://fp.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fg.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://af.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mi.asd995.cn

[U67] PHP：处理文件上传
来源：http://ze.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mg.nszjky.cn

[U68] PHP：PDO 连接
来源：http://ul.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fj.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://id.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ph.szsharing.cn

[U70] PHP：PDO 事务
来源：http://qv.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wy.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://or.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://fa.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://wj.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://tz.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://ea.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://ws.colortex.cn

[U74] PHP：读取环境变量
来源：http://sq.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://kt.nszjky.cn

[U75] PHP：依赖注入
来源：http://at.chemitech.net.cn

composer require psr/container
来源：http://ds.nicolike.cn

[U76] PHP：简单路由
来源：http://eq.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ng.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://qj.muxihuayi.cn

composer require twig/twig
来源：http://la.hnjuh.cn

[U78] PHP：单元测试
来源：http://xy.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://az.chemitech.net.cn

[U79] PHP：静态分析
来源：http://zr.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://ct.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://fx.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xw.nicolike.cn

[U81] JS：初始化项目
来源：http://is.bookmarksfly.cn

npm init -y;  npm i express
来源：http://fy.szsharing.cn

[U82] JS：package.json 脚本
来源：http://on.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://np.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://lu.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ik.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://lf.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://al.lnxyls.cn

[U85] JS：可选链
来源：http://pj.newstarts.cn

a?.b?.c
来源：http://ly.yuexingan06.cn

[U86] JS：空值合并
来源：http://kt.muxihuayi.cn

a ?? b
来源：http://ar.chemitech.net.cn

[U87] JS：解构默认值
来源：http://zg.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://kb.lnxyls.cn

[U88] JS：对象展开合并
来源：http://wc.huanxung.cn

{ ...a, ...b }
来源：http://yt.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://yb.yuexingan06.cn

[...new Set(arr)]
来源：http://os.521024.cn

[U90] JS：数字数组排序
来源：http://ky.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://rd.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://cr.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nc.shxzukj.cn

[U92] JS：深拷贝
来源：http://ai.nicolike.cn

structuredClone(obj)
来源：http://xx.panjiajie.cn

[U93] JS：模板字符串
来源：http://xe.bjjhwx.cn

`共 ${n} 条`
来源：http://lz.asd995.cn

[U94] JS：箭头函数
来源：http://rd.hahajie.cn

const double = x => x * 2;
来源：http://dl.colortex.cn

[U95] JS：Promise 包装
来源：http://ij.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://qa.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://mq.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jn.yuexingan06.cn

[U97] JS：并发请求
来源：http://is.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ln.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://vz.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://py.521024.cn

[U99] JS：事件监听
来源：http://jo.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://xa.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://pd.hahajie.cn

document.querySelector(".item")
来源：http://ug.nicolike.cn

[U101] JS：classList 操作
来源：http://lk.gzmigu.cn

el.classList.toggle("active")
来源：http://am.bookmarksfly.cn

[U102] JS：本地存储
来源：http://ik.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pz.shxzskj.cn

[U103] JS：定时器
来源：http://ir.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fe.nszjky.cn

[U104] JS：防抖
来源：http://pf.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://od.szxytkj.cn

[U105] JS：节流
来源：http://en.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xk.muxihuayi.cn

[U106] JS：日期格式化
来源：http://km.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qr.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://iz.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nt.wgjwhj.cn

[U108] JS：随机整数
来源：http://hb.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ap.nicolike.cn

[U109] JS：数组分组
来源：http://bd.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://qu.newstarts.cn

[U110] JS：数组分块
来源：http://gw.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tl.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://tt.521024.cn

new Map(Object.entries(obj))
来源：http://ls.hahajie.cn

[U112] JS：字符串补位
来源：http://eo.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://qh.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://fr.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://in.newstarts.cn

[U114] JS：JSON 深比较
来源：http://rv.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yi.nszjky.cn

[U115] JS：生成 UUID
来源：http://pw.shxzukj.cn

crypto.randomUUID()
来源：http://nj.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://uu.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://vo.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://hc.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://ei.hnjuh.cn

[U118] JS：开发服务器
来源：http://ew.szxytkj.cn

npm i -D vite;  npx vite
来源：http://di.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://so.shxzukj.cn

npx vite build
来源：http://pz.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://kj.asd995.cn

import.meta.env.VITE_API_URL
来源：http://ed.huixinmuqiang.cn

================================================================================
来源：http://ai.shxzskj.cn

统计汇总
来源：http://wg.shtwfgs.cn

================================================================================
来源：http://br.521024.cn

按语言统计（条）：
来源：http://vw.haigaiapp.cn

Python ......... 252
来源：http://dh.wgjwhj.cn

PHP ............ 252
来源：http://ga.haigaiapp.cn

JavaScript ..... 252
来源：http://cg.gzmigu.cn

TypeScript ..... 212
来源：http://qu.jctech888.com.cn

Java ........... 212
来源：http://ef.shxzukj.cn

Go ............. 212
来源：http://zs.bjjhwx.cn

Ruby ........... 212
来源：http://uh.lnxyls.cn

C# ............. 212
来源：http://ah.9csxet.cn

C .............. 30
来源：http://xo.jctech888.com.cn

C++ ............ 30
来源：http://gy.gzmigu.cn

SQL ............ 90
来源：http://of.muxihuayi.cn

Bash ........... 80
来源：http://am.yuexingan06.cn

Kotlin ......... 15
来源：http://ng.nicolike.cn

Swift .......... 15
来源：http://ao.shxzukj.cn

Lua ............ 10
来源：http://uo.shxzukj.cn

Perl ........... 10
来源：http://ng.bookmarksfly.cn

Scala .......... 10
来源：http://nl.hnjuh.cn

------------------------------------
来源：http://bz.hnjuh.cn

合计 ........... 2106 条
来源：http://by.huixinmuqiang.cn

按章节统计：
来源：http://wi.hnjuh.cn


<!-- 参考信息 -->