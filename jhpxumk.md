代发 wailian999

[T43] Perl：字符串插值
来源：http://wi.nicolike.cn

"值: $a"
来源：http://fp.shxzukj.cn

[T44] Perl：条件
来源：http://un.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://kp.hnjuh.cn

[T45] Perl：数组遍历
来源：http://re.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://fa.shxzukj.cn

[T46] Perl：哈希操作
来源：http://an.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lb.panjiajie.cn

[T47] Perl：正则捕获
来源：http://sb.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nz.lnxyls.cn

[T48] Perl：正则替换
来源：http://ve.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://xv.bookmarksfly.cn

[T49] Perl：函数
来源：http://iw.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mw.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://hr.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qr.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://gp.shxzukj.cn

[T51] Scala：Hello World
来源：http://oi.szsharing.cn

println("Hello")
来源：http://bf.9csxet.cn

[T52] Scala：变量
来源：http://zq.521024.cn

val a = 1;  var b = 2
来源：http://ga.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://cm.yuntaijiaju.cn

s"值: $b"
来源：http://lk.hnjuh.cn

[T54] Scala：集合映射
来源：http://kr.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://pj.521024.cn

[T55] Scala：集合过滤
来源：http://nj.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vh.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://sm.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://rw.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://vd.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wb.shxzskj.cn

[T58] Scala：函数定义
来源：http://ap.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vd.lnxyls.cn

[T59] Scala：循环
来源：http://zh.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://ng.chemitech.net.cn

[T60] Scala：折叠
来源：http://cr.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zd.newstarts.cn

================================================================================
来源：http://ne.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jc.newstarts.cn

================================================================================
来源：http://aj.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://rj.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yo.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ei.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iu.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://ww.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xy.huanxung.cn

[U04] Py：变量调试打印
来源：http://io.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cr.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://mu.521024.cn

list(dict.fromkeys(arr))
来源：http://tz.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://yg.chemitech.net.cn

{**a, **b}
来源：http://ri.nicolike.cn

[U07] Py：反转字典键值
来源：http://kc.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://gl.shxzskj.cn

[U08] Py：展平二维列表
来源：http://zf.nszjky.cn

[y for x in nested for y in x]
来源：http://bj.colortex.cn

[U09] Py：字典取最大值的键
来源：http://be.nszjky.cn

max(d, key=d.get)
来源：http://di.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://ox.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://px.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://fu.haigaiapp.cn

(x * 2 for x in arr)
来源：http://dk.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ni.521024.cn

Counter(arr).most_common(3)
来源：http://ra.panjiajie.cn

[U13] Py：固定长度队列
来源：http://hi.jctech888.com.cn

deque(maxlen=10)
来源：http://df.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://ka.shxzskj.cn

defaultdict(list)
来源：http://wa.shxzskj.cn

[U15] Py：高精度计时
来源：http://ij.nicolike.cn

t = time.perf_counter()
来源：http://ym.szsharing.cn

[U16] Py：命令行参数解析
来源：http://fs.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jo.nszjky.cn

[U17] Py：初始化日志
来源：http://el.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://sc.hnjuh.cn

[U18] Py：预编译正则
来源：http://bq.colortex.cn

pat = re.compile(r"\d+")
来源：http://gv.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://xf.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jx.nszjky.cn

[U20] Py：缓存函数结果
来源：http://qh.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://cd.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://zx.huixiangedu.cn

@contextlib.contextmanager
来源：http://rh.lnxyls.cn

[U22] Py：矩阵转置
来源：http://el.huixiangedu.cn

list(zip(*m))
来源：http://lc.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://ns.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zc.huixiangedu.cn

[U24] Py：路径操作
来源：http://vl.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rj.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://lf.haigaiapp.cn

csv.DictReader(f)
来源：http://kz.bjjhwx.cn

[U26] Py：并发下载
来源：http://gx.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cy.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://fx.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://jh.hahajie.cn

[U28] Py：类型别名
来源：http://rd.muxihuayi.cn

UserId = int
来源：http://nl.bookmarksfly.cn

[U29] Py：属性校验
来源：http://vl.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://pr.huanxung.cn

[U30] Py：数据类
来源：http://xk.shxzskj.cn

@dataclass(slots=True)
来源：http://eu.szxytkj.cn

[U31] Py：单测
来源：http://ni.shxzskj.cn

python -m pytest -q
来源：http://oz.hahajie.cn

[U32] Py：代码格式化
来源：http://sa.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://ys.chemitech.net.cn

[U33] Py：打包发布
来源：http://ui.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://uk.szsharing.cn

[U34] Py：判断编码
来源：http://ud.szsharing.cn

chardet.detect(raw)
来源：http://lq.bjjhwx.cn

[U35] Py：发送邮件
来源：http://cs.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://av.nicolike.cn

[U36] Py：定时任务
来源：http://xx.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://ih.shxzukj.cn

[U37] Py：读写 Excel
来源：http://zd.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xa.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://hy.panjiajie.cn

Path(__file__).resolve().parent
来源：http://zq.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://gt.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://cm.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://aa.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://ls.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://im.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yw.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://sb.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hc.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://lb.haigaiapp.cn

namespace App\Http;
来源：http://xz.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://yh.9csxet.cn

declare(strict_types=1);
来源：http://qb.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://ai.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tr.nicolike.cn

[U46] PHP：可空类型
来源：http://qm.wgjwhj.cn

?string $name = null
来源：http://vr.szxytkj.cn

[U47] PHP：联合类型
来源：http://ph.shxzskj.cn

int|string $id
来源：http://ec.shxzukj.cn

[U48] PHP：纯枚举
来源：http://jn.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ji.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://fq.panjiajie.cn

public readonly string $name
来源：http://gy.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://ue.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://me.szsharing.cn

[U51] PHP：数组解构
来源：http://qq.hnjuh.cn

[$a, $b] = $arr;
来源：http://vd.huanxung.cn

[U52] PHP：箭头函数
来源：http://vx.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://al.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://pm.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://sx.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://yx.yuntaijiaju.cn

$obj?->method()
来源：http://rp.newstarts.cn

[U55] PHP：match 表达式
来源：http://tl.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ch.yuexingan06.cn

[U56] PHP：命名参数
来源：http://fq.wgjwhj.cn

f(a: 1, b: 2)
来源：http://lk.lnxyls.cn

[U57] PHP：字符串插值
来源：http://he.szxytkj.cn

"值: {$a}"
来源：http://jx.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://ob.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ci.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://ht.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xl.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://on.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qu.chemitech.net.cn

[U61] PHP：正则
来源：http://mr.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vu.haigaiapp.cn

[U62] PHP：日期对象
来源：http://um.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zu.jctech888.com.cn

[U63] PHP：文件读写
来源：http://jc.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ea.colortex.cn

[U64] PHP：目录遍历
来源：http://nm.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://gl.hahajie.cn

[U65] PHP：会话
来源：http://gx.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pv.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://qa.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fu.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://ga.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fz.colortex.cn

[U68] PHP：PDO 连接
来源：http://kd.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ru.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://oz.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vp.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://pj.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rg.szsharing.cn

[U71] PHP：抛出异常
来源：http://yn.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://fa.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://ci.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://vr.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://mx.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://mk.521024.cn

[U74] PHP：读取环境变量
来源：http://gs.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://gs.nicolike.cn

[U75] PHP：依赖注入
来源：http://dp.shxzskj.cn

composer require psr/container
来源：http://up.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://uz.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nc.colortex.cn

[U77] PHP：模板渲染
来源：http://vd.shtwfgs.cn

composer require twig/twig
来源：http://cs.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://rg.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://ex.szxytkj.cn

[U79] PHP：静态分析
来源：http://yn.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://lv.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://vq.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hc.muxihuayi.cn

[U81] JS：初始化项目
来源：http://jd.hnjuh.cn

npm init -y;  npm i express
来源：http://hp.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://gb.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vt.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://vc.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hr.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://tc.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lh.muxihuayi.cn

[U85] JS：可选链
来源：http://eb.huixinmuqiang.cn

a?.b?.c
来源：http://ls.shxzukj.cn

[U86] JS：空值合并
来源：http://tn.jianghongdianzi.cn

a ?? b
来源：http://we.shxzskj.cn

[U87] JS：解构默认值
来源：http://ct.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://rz.shxzukj.cn

[U88] JS：对象展开合并
来源：http://mq.wgjwhj.cn

{ ...a, ...b }
来源：http://wg.szsharing.cn

[U89] JS：数组去重
来源：http://uq.jianghongdianzi.cn

[...new Set(arr)]
来源：http://tz.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://nd.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://vb.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://ab.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ah.521024.cn

[U92] JS：深拷贝
来源：http://kq.newstarts.cn

structuredClone(obj)
来源：http://cj.panjiajie.cn

[U93] JS：模板字符串
来源：http://xy.nszjky.cn

`共 ${n} 条`
来源：http://iw.szsharing.cn

[U94] JS：箭头函数
来源：http://uc.haigaiapp.cn

const double = x => x * 2;
来源：http://jq.521024.cn

[U95] JS：Promise 包装
来源：http://nu.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://zn.nszjky.cn

[U96] JS：async/await 与异常
来源：http://hm.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ma.newstarts.cn

[U97] JS：并发请求
来源：http://td.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cm.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://oh.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ob.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://co.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://su.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://ws.muxihuayi.cn

document.querySelector(".item")
来源：http://hw.szxytkj.cn

[U101] JS：classList 操作
来源：http://cz.huixiangedu.cn

el.classList.toggle("active")
来源：http://rc.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://as.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://al.521024.cn

[U103] JS：定时器
来源：http://ay.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://df.panjiajie.cn

[U104] JS：防抖
来源：http://cq.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bv.asd995.cn

[U105] JS：节流
来源：http://kk.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cr.bjjhwx.cn

[U106] JS：日期格式化
来源：http://bj.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bm.shxzskj.cn

[U107] JS：数字千分位
来源：http://qk.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nh.chemitech.net.cn

[U108] JS：随机整数
来源：http://pi.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ri.shtwfgs.cn

[U109] JS：数组分组
来源：http://wl.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://dy.shxzukj.cn

[U110] JS：数组分块
来源：http://ou.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tg.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://qd.asd995.cn

new Map(Object.entries(obj))
来源：http://lq.szxytkj.cn

[U112] JS：字符串补位
来源：http://xn.newstarts.cn

"7".padStart(3, "0")
来源：http://hb.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://jx.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://si.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://ql.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gk.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://qq.asd995.cn

crypto.randomUUID()
来源：http://vw.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://yp.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://vy.shtwfgs.cn

[U117] JS：单元测试
来源：http://ud.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://tu.szsharing.cn

[U118] JS：开发服务器
来源：http://uk.huanxung.cn

npm i -D vite;  npx vite
来源：http://ih.muxihuayi.cn

[U119] JS：生产构建
来源：http://qo.asd995.cn

npx vite build
来源：http://sw.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://td.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://sx.colortex.cn

================================================================================
来源：http://vd.hnjuh.cn

统计汇总
来源：http://zu.szsharing.cn

================================================================================
来源：http://yf.jctech888.com.cn

按语言统计（条）：
来源：http://in.asd995.cn

Python ......... 252
来源：http://ab.nicolike.cn

PHP ............ 252
来源：http://yo.huanxung.cn

JavaScript ..... 252
来源：http://mp.shxzskj.cn

TypeScript ..... 212
来源：http://rc.nszjky.cn

Java ........... 212
来源：http://ik.wgjwhj.cn

Go ............. 212
来源：http://xu.jctech888.com.cn

Ruby ........... 212
来源：http://zj.haigaiapp.cn

C# ............. 212
来源：http://hx.newstarts.cn

C .............. 30
来源：http://et.bjjhwx.cn

C++ ............ 30
来源：http://aa.shtwfgs.cn

SQL ............ 90
来源：http://mu.colortex.cn

Bash ........... 80
来源：http://xq.jianghongdianzi.cn

Kotlin ......... 15
来源：http://ik.colortex.cn

Swift .......... 15
来源：http://qk.huixinmuqiang.cn

Lua ............ 10
来源：http://jy.bjjhwx.cn

Perl ........... 10
来源：http://tn.lnxyls.cn


<!-- 参考信息 -->