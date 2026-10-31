代发 wailian999

[T43] Perl：字符串插值
来源：http://ax.9csxet.cn

"值: $a"
来源：http://tb.lnxyls.cn

[T44] Perl：条件
来源：http://bf.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ja.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://yo.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://zr.panjiajie.cn

[T46] Perl：哈希操作
来源：http://ou.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hy.lnxyls.cn

[T47] Perl：正则捕获
来源：http://hy.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lh.newstarts.cn

[T48] Perl：正则替换
来源：http://gr.panjiajie.cn

$s =~ s/old/new/g;
来源：http://re.shxzskj.cn

[T49] Perl：函数
来源：http://ye.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gm.huanxung.cn

[T50] Perl：逐行读文件
来源：http://qx.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gf.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://hw.hahajie.cn

[T51] Scala：Hello World
来源：http://oj.hahajie.cn

println("Hello")
来源：http://ou.shxzskj.cn

[T52] Scala：变量
来源：http://oq.panjiajie.cn

val a = 1;  var b = 2
来源：http://en.shxzukj.cn

[T53] Scala：字符串插值
来源：http://zl.nszjky.cn

s"值: $b"
来源：http://sb.colortex.cn

[T54] Scala：集合映射
来源：http://mz.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ys.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://nf.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lp.huixiangedu.cn

[T56] Scala：样例类
来源：http://tt.lnxyls.cn

case class User(name: String, age: Int)
来源：http://cl.asd995.cn

[T57] Scala：模式匹配
来源：http://zb.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oz.szsharing.cn

[T58] Scala：函数定义
来源：http://hg.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tz.huixiangedu.cn

[T59] Scala：循环
来源：http://cb.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://yl.lnxyls.cn

[T60] Scala：折叠
来源：http://kv.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://on.wgjwhj.cn

================================================================================
来源：http://ai.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ea.shxzskj.cn

================================================================================
来源：http://tm.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://qj.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cj.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://ss.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xg.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://ql.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xo.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://rh.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zj.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://wh.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://cy.hnjuh.cn

[U06] Py：合并两个字典
来源：http://bd.huixiangedu.cn

{**a, **b}
来源：http://ey.asd995.cn

[U07] Py：反转字典键值
来源：http://ri.nszjky.cn

{v: k for k, v in d.items()}
来源：http://cb.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://qr.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://ov.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://gn.lnxyls.cn

max(d, key=d.get)
来源：http://ng.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://ce.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ms.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://cj.haigaiapp.cn

(x * 2 for x in arr)
来源：http://ve.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ln.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://ue.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://as.shtwfgs.cn

deque(maxlen=10)
来源：http://zc.newstarts.cn

[U14] Py：分组收集到列表
来源：http://cy.shxzskj.cn

defaultdict(list)
来源：http://uc.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://zn.521024.cn

t = time.perf_counter()
来源：http://nq.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://jb.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bm.panjiajie.cn

[U17] Py：初始化日志
来源：http://kf.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://ij.muxihuayi.cn

[U18] Py：预编译正则
来源：http://jy.asd995.cn

pat = re.compile(r"\d+")
来源：http://jp.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://es.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oz.asd995.cn

[U20] Py：缓存函数结果
来源：http://aa.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://fj.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://tv.lnxyls.cn

@contextlib.contextmanager
来源：http://eg.gzmigu.cn

[U22] Py：矩阵转置
来源：http://ji.wgjwhj.cn

list(zip(*m))
来源：http://tg.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://th.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ed.lnxyls.cn

[U24] Py：路径操作
来源：http://qq.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kz.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://ph.szsharing.cn

csv.DictReader(f)
来源：http://rr.asd995.cn

[U26] Py：并发下载
来源：http://pv.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aq.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://xh.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ld.shxzukj.cn

[U28] Py：类型别名
来源：http://ok.jctech888.com.cn

UserId = int
来源：http://hg.lnxyls.cn

[U29] Py：属性校验
来源：http://hy.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://zf.bookmarksfly.cn

[U30] Py：数据类
来源：http://ge.hahajie.cn

@dataclass(slots=True)
来源：http://ug.szsharing.cn

[U31] Py：单测
来源：http://wu.muxihuayi.cn

python -m pytest -q
来源：http://ju.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://ts.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://dc.lnxyls.cn

[U33] Py：打包发布
来源：http://ne.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://mj.asd995.cn

[U34] Py：判断编码
来源：http://ru.lnxyls.cn

chardet.detect(raw)
来源：http://mp.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://rq.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rq.panjiajie.cn

[U36] Py：定时任务
来源：http://dk.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://oj.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://gd.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://em.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://eq.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://uu.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://kj.bookmarksfly.cn

sys.stdout.isatty()
来源：http://fo.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://cf.panjiajie.cn

print("err", file=sys.stderr)
来源：http://zg.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://cj.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://me.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://vc.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rw.huanxung.cn

[U43] PHP：声明命名空间
来源：http://id.szsharing.cn

namespace App\Http;
来源：http://ja.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://hv.shxzukj.cn

declare(strict_types=1);
来源：http://qt.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://zy.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://om.hnjuh.cn

[U46] PHP：可空类型
来源：http://vk.shxzukj.cn

?string $name = null
来源：http://mr.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://fw.521024.cn

int|string $id
来源：http://in.nicolike.cn

[U48] PHP：纯枚举
来源：http://yx.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fb.gzmigu.cn

[U49] PHP：只读属性
来源：http://qj.szsharing.cn

public readonly string $name
来源：http://uj.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://un.szsharing.cn

public function __construct(private int $id) {}
来源：http://dw.szxytkj.cn

[U51] PHP：数组解构
来源：http://fy.huanxung.cn

[$a, $b] = $arr;
来源：http://xl.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://fu.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://lu.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://vh.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://zp.9csxet.cn

[U54] PHP：空安全调用
来源：http://ha.bjjhwx.cn

$obj?->method()
来源：http://ra.panjiajie.cn

[U55] PHP：match 表达式
来源：http://un.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://px.yuexingan06.cn

[U56] PHP：命名参数
来源：http://tx.521024.cn

f(a: 1, b: 2)
来源：http://tk.asd995.cn

[U57] PHP：字符串插值
来源：http://ek.hnjuh.cn

"值: {$a}"
来源：http://wn.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://af.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bv.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://cr.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://il.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://jc.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pa.huanxung.cn

[U61] PHP：正则
来源：http://mt.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jl.wgjwhj.cn

[U62] PHP：日期对象
来源：http://mf.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gr.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://sv.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gy.newstarts.cn

[U64] PHP：目录遍历
来源：http://oq.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://rv.shxzukj.cn

[U65] PHP：会话
来源：http://zg.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qt.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://cr.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gb.newstarts.cn

[U67] PHP：处理文件上传
来源：http://nj.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wc.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://tt.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vn.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://td.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eu.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://ak.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sd.asd995.cn

[U71] PHP：抛出异常
来源：http://ng.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://yz.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://bp.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ms.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://pq.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://wk.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ih.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://kl.szsharing.cn

[U75] PHP：依赖注入
来源：http://bz.hnjuh.cn

composer require psr/container
来源：http://jh.yuexingan06.cn

[U76] PHP：简单路由
来源：http://nx.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wy.asd995.cn

[U77] PHP：模板渲染
来源：http://vj.9csxet.cn

composer require twig/twig
来源：http://lb.jctech888.com.cn

[U78] PHP：单元测试
来源：http://fq.colortex.cn

composer require --dev phpunit/phpunit
来源：http://fu.chemitech.net.cn

[U79] PHP：静态分析
来源：http://dn.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://lk.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://rc.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lg.huanxung.cn

[U81] JS：初始化项目
来源：http://vk.wgjwhj.cn

npm init -y;  npm i express
来源：http://el.huanxung.cn

[U82] JS：package.json 脚本
来源：http://yr.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ga.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://gx.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vn.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://zy.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fw.wgjwhj.cn

[U85] JS：可选链
来源：http://xa.lnxyls.cn

a?.b?.c
来源：http://vw.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ue.yuexingan06.cn

a ?? b
来源：http://bx.wgjwhj.cn

[U87] JS：解构默认值
来源：http://lu.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://jk.9csxet.cn

[U88] JS：对象展开合并
来源：http://fq.bjjhwx.cn

{ ...a, ...b }
来源：http://cd.shtwfgs.cn

[U89] JS：数组去重
来源：http://ez.bjjhwx.cn

[...new Set(arr)]
来源：http://vx.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://fm.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://xl.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://oi.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oz.nszjky.cn

[U92] JS：深拷贝
来源：http://cq.colortex.cn

structuredClone(obj)
来源：http://pr.chemitech.net.cn

[U93] JS：模板字符串
来源：http://es.asd995.cn

`共 ${n} 条`
来源：http://kf.hahajie.cn

[U94] JS：箭头函数
来源：http://pf.huixiangedu.cn

const double = x => x * 2;
来源：http://ms.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://dv.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://et.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://ie.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wm.hnjuh.cn

[U97] JS：并发请求
来源：http://rg.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zi.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://ml.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ju.hnjuh.cn

[U99] JS：事件监听
来源：http://xh.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://js.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://gr.huixinmuqiang.cn

document.querySelector(".item")
来源：http://cj.521024.cn

[U101] JS：classList 操作
来源：http://gj.bjjhwx.cn

el.classList.toggle("active")
来源：http://qx.yuexingan06.cn

[U102] JS：本地存储
来源：http://cg.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hr.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ak.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yn.szsharing.cn

[U104] JS：防抖
来源：http://qg.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://od.asd995.cn

[U105] JS：节流
来源：http://nv.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uv.huixiangedu.cn

[U106] JS：日期格式化
来源：http://vr.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jv.yuexingan06.cn

[U107] JS：数字千分位
来源：http://zv.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fz.panjiajie.cn

[U108] JS：随机整数
来源：http://fm.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nm.muxihuayi.cn

[U109] JS：数组分组
来源：http://sy.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://sl.wgjwhj.cn

[U110] JS：数组分块
来源：http://wb.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qo.huanxung.cn

[U111] JS：对象转 Map
来源：http://fx.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://dn.lnxyls.cn

[U112] JS：字符串补位
来源：http://qo.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://si.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://qj.521024.cn

s.replaceAll("a", "b")
来源：http://zp.nicolike.cn

[U114] JS：JSON 深比较
来源：http://bz.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fb.hahajie.cn

[U115] JS：生成 UUID
来源：http://kc.szxytkj.cn

crypto.randomUUID()
来源：http://dk.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://rd.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://hf.bjjhwx.cn

[U117] JS：单元测试
来源：http://ze.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://yl.huanxung.cn

[U118] JS：开发服务器
来源：http://rt.shxzukj.cn

npm i -D vite;  npx vite
来源：http://wo.shtwfgs.cn

[U119] JS：生产构建
来源：http://wa.haigaiapp.cn

npx vite build
来源：http://pz.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://vs.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://zo.huixiangedu.cn

================================================================================
来源：http://vr.huanxung.cn

统计汇总
来源：http://yc.huanxung.cn

================================================================================
来源：http://fz.bjjhwx.cn

按语言统计（条）：
来源：http://ky.bookmarksfly.cn

Python ......... 252
来源：http://oz.panjiajie.cn

PHP ............ 252
来源：http://qh.haigaiapp.cn

JavaScript ..... 252
来源：http://dh.panjiajie.cn

TypeScript ..... 212
来源：http://df.521024.cn

Java ........... 212
来源：http://ls.huanxung.cn

Go ............. 212
来源：http://uu.huixiangedu.cn

Ruby ........... 212
来源：http://hc.nszjky.cn

C# ............. 212
来源：http://lm.huixinmuqiang.cn

C .............. 30
来源：http://ui.wgjwhj.cn

C++ ............ 30
来源：http://ka.yuexingan06.cn

SQL ............ 90
来源：http://mc.lnxyls.cn

Bash ........... 80
来源：http://xv.haigaiapp.cn

Kotlin ......... 15
来源：http://up.nszjky.cn

Swift .......... 15
来源：http://si.chemitech.net.cn

Lua ............ 10
来源：http://tg.colortex.cn

Perl ........... 10
来源：http://dg.asd995.cn


<!-- 参考信息 -->