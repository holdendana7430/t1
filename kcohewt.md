代发 wailian999

[T43] Perl：字符串插值
来源：http://za.jianghongdianzi.cn

"值: $a"
来源：http://ip.asd995.cn

[T44] Perl：条件
来源：http://mf.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://bi.shxzskj.cn

[T45] Perl：数组遍历
来源：http://jj.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://ua.lnxyls.cn

[T46] Perl：哈希操作
来源：http://im.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ey.hahajie.cn

[T47] Perl：正则捕获
来源：http://gc.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://su.szxytkj.cn

[T48] Perl：正则替换
来源：http://iq.panjiajie.cn

$s =~ s/old/new/g;
来源：http://ga.asd995.cn

[T49] Perl：函数
来源：http://pj.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hq.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://gh.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wd.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://uo.panjiajie.cn

[T51] Scala：Hello World
来源：http://zg.haigaiapp.cn

println("Hello")
来源：http://mz.szxytkj.cn

[T52] Scala：变量
来源：http://le.shtwfgs.cn

val a = 1;  var b = 2
来源：http://lg.asd995.cn

[T53] Scala：字符串插值
来源：http://hp.huixiangedu.cn

s"值: $b"
来源：http://fe.chemitech.net.cn

[T54] Scala：集合映射
来源：http://ob.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://lf.shxzukj.cn

[T55] Scala：集合过滤
来源：http://uc.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zd.bookmarksfly.cn

[T56] Scala：样例类
来源：http://yd.huanxung.cn

case class User(name: String, age: Int)
来源：http://em.shxzskj.cn

[T57] Scala：模式匹配
来源：http://nk.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vu.asd995.cn

[T58] Scala：函数定义
来源：http://dc.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fp.yuexingan06.cn

[T59] Scala：循环
来源：http://ga.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://fj.jctech888.com.cn

[T60] Scala：折叠
来源：http://gq.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lm.yuntaijiaju.cn

================================================================================
来源：http://ub.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zv.newstarts.cn

================================================================================
来源：http://ad.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://ea.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://za.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://xn.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eq.521024.cn

[U03] Py：加载 .env 配置
来源：http://zi.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bf.nicolike.cn

[U04] Py：变量调试打印
来源：http://xr.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://we.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://ac.521024.cn

list(dict.fromkeys(arr))
来源：http://oa.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://vl.huanxung.cn

{**a, **b}
来源：http://oa.hahajie.cn

[U07] Py：反转字典键值
来源：http://rw.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://hh.asd995.cn

[U08] Py：展平二维列表
来源：http://gf.nicolike.cn

[y for x in nested for y in x]
来源：http://rs.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://tk.huixinmuqiang.cn

max(d, key=d.get)
来源：http://rc.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://zo.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wp.colortex.cn

[U11] Py：生成器表达式
来源：http://hd.muxihuayi.cn

(x * 2 for x in arr)
来源：http://pb.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bv.nszjky.cn

Counter(arr).most_common(3)
来源：http://qg.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://af.huanxung.cn

deque(maxlen=10)
来源：http://yd.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://ph.hahajie.cn

defaultdict(list)
来源：http://ns.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://te.asd995.cn

t = time.perf_counter()
来源：http://wn.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://je.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ct.huanxung.cn

[U17] Py：初始化日志
来源：http://yo.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://dc.szsharing.cn

[U18] Py：预编译正则
来源：http://un.nszjky.cn

pat = re.compile(r"\d+")
来源：http://wi.9csxet.cn

[U19] Py：正则替换带回调
来源：http://dl.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sa.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://so.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://um.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://vd.yuexingan06.cn

@contextlib.contextmanager
来源：http://uc.521024.cn

[U22] Py：矩阵转置
来源：http://ah.yuntaijiaju.cn

list(zip(*m))
来源：http://dy.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://zl.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mi.bjjhwx.cn

[U24] Py：路径操作
来源：http://js.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ud.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://zi.chemitech.net.cn

csv.DictReader(f)
来源：http://fy.huanxung.cn

[U26] Py：并发下载
来源：http://vg.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gj.asd995.cn

[U27] Py：异步 HTTP
来源：http://ir.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://rw.huixiangedu.cn

[U28] Py：类型别名
来源：http://eu.newstarts.cn

UserId = int
来源：http://oy.colortex.cn

[U29] Py：属性校验
来源：http://ih.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://jc.chemitech.net.cn

[U30] Py：数据类
来源：http://nl.bjjhwx.cn

@dataclass(slots=True)
来源：http://uz.9csxet.cn

[U31] Py：单测
来源：http://yf.chemitech.net.cn

python -m pytest -q
来源：http://nh.huanxung.cn

[U32] Py：代码格式化
来源：http://dj.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://gq.wgjwhj.cn

[U33] Py：打包发布
来源：http://kz.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://ya.521024.cn

[U34] Py：判断编码
来源：http://fd.hahajie.cn

chardet.detect(raw)
来源：http://az.yuexingan06.cn

[U35] Py：发送邮件
来源：http://aq.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://es.nicolike.cn

[U36] Py：定时任务
来源：http://sm.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://bj.shxzskj.cn

[U37] Py：读写 Excel
来源：http://gj.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lo.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://fd.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://xg.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://lx.huixiangedu.cn

sys.stdout.isatty()
来源：http://xj.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://oi.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://fb.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://no.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ib.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://hj.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bu.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://mz.yuntaijiaju.cn

namespace App\Http;
来源：http://zt.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://yq.huanxung.cn

declare(strict_types=1);
来源：http://pd.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://gi.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ie.shtwfgs.cn

[U46] PHP：可空类型
来源：http://wc.shxzskj.cn

?string $name = null
来源：http://mv.jctech888.com.cn

[U47] PHP：联合类型
来源：http://vx.szsharing.cn

int|string $id
来源：http://de.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://gf.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fq.muxihuayi.cn

[U49] PHP：只读属性
来源：http://fw.gzmigu.cn

public readonly string $name
来源：http://zj.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://yv.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://jk.shxzskj.cn

[U51] PHP：数组解构
来源：http://js.hnjuh.cn

[$a, $b] = $arr;
来源：http://te.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://vd.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://iz.asd995.cn

[U53] PHP：空合并运算符
来源：http://gk.521024.cn

$v = $a ?? $b ?? "default";
来源：http://dn.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://sx.9csxet.cn

$obj?->method()
来源：http://fs.hahajie.cn

[U55] PHP：match 表达式
来源：http://rd.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ts.jctech888.com.cn

[U56] PHP：命名参数
来源：http://hq.hahajie.cn

f(a: 1, b: 2)
来源：http://mz.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://xo.haigaiapp.cn

"值: {$a}"
来源：http://mg.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://db.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pb.9csxet.cn

[U59] PHP：自定义排序
来源：http://mf.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kp.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://za.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://th.muxihuayi.cn

[U61] PHP：正则
来源：http://cy.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ag.chemitech.net.cn

[U62] PHP：日期对象
来源：http://ji.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ob.huanxung.cn

[U63] PHP：文件读写
来源：http://xj.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ys.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://op.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://nd.colortex.cn

[U65] PHP：会话
来源：http://hs.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xk.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://ko.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gm.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://kt.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ok.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://mq.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dg.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://ad.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://py.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://sh.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pe.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://pg.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://cz.panjiajie.cn

[U72] PHP：写错误日志
来源：http://cg.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://au.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://ph.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://jb.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://rs.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://oj.panjiajie.cn

[U75] PHP：依赖注入
来源：http://tl.jianghongdianzi.cn

composer require psr/container
来源：http://vv.9csxet.cn

[U76] PHP：简单路由
来源：http://vw.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qi.shxzskj.cn

[U77] PHP：模板渲染
来源：http://gh.huanxung.cn

composer require twig/twig
来源：http://nc.shxzukj.cn

[U78] PHP：单元测试
来源：http://mn.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://lt.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://zf.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://zy.newstarts.cn

[U80] PHP：代码规范修复
来源：http://eg.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://id.asd995.cn

[U81] JS：初始化项目
来源：http://rb.asd995.cn

npm init -y;  npm i express
来源：http://po.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://pg.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://br.521024.cn

[U83] JS：ES Module 导入导出
来源：http://la.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dq.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://vb.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yk.hahajie.cn

[U85] JS：可选链
来源：http://tp.nicolike.cn

a?.b?.c
来源：http://zl.muxihuayi.cn

[U86] JS：空值合并
来源：http://mr.szsharing.cn

a ?? b
来源：http://xl.asd995.cn

[U87] JS：解构默认值
来源：http://tx.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://tt.lnxyls.cn

[U88] JS：对象展开合并
来源：http://fl.newstarts.cn

{ ...a, ...b }
来源：http://jr.yuexingan06.cn

[U89] JS：数组去重
来源：http://nr.nszjky.cn

[...new Set(arr)]
来源：http://ve.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://hv.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ig.521024.cn

[U91] JS：对象键值遍历
来源：http://gt.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://av.colortex.cn

[U92] JS：深拷贝
来源：http://iw.newstarts.cn

structuredClone(obj)
来源：http://hy.chemitech.net.cn

[U93] JS：模板字符串
来源：http://zh.jctech888.com.cn

`共 ${n} 条`
来源：http://lm.wgjwhj.cn

[U94] JS：箭头函数
来源：http://tt.lnxyls.cn

const double = x => x * 2;
来源：http://es.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://je.colortex.cn

new Promise((resolve, reject) => {})
来源：http://jp.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://fd.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jc.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://vp.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://us.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://nc.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ng.colortex.cn

[U99] JS：事件监听
来源：http://hy.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://pf.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://gp.haigaiapp.cn

document.querySelector(".item")
来源：http://ka.asd995.cn

[U101] JS：classList 操作
来源：http://ra.panjiajie.cn

el.classList.toggle("active")
来源：http://lb.yuexingan06.cn

[U102] JS：本地存储
来源：http://cy.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ou.yuexingan06.cn

[U103] JS：定时器
来源：http://rd.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hh.szsharing.cn

[U104] JS：防抖
来源：http://zx.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wu.hahajie.cn

[U105] JS：节流
来源：http://fd.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qi.szsharing.cn

[U106] JS：日期格式化
来源：http://pg.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ed.bjjhwx.cn

[U107] JS：数字千分位
来源：http://hg.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://at.newstarts.cn

[U108] JS：随机整数
来源：http://be.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dt.nszjky.cn

[U109] JS：数组分组
来源：http://la.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://df.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://xk.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://si.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://mk.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://fe.szxytkj.cn

[U112] JS：字符串补位
来源：http://fm.szsharing.cn

"7".padStart(3, "0")
来源：http://ae.nicolike.cn

[U113] JS：正则替换全部
来源：http://iz.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://hv.nicolike.cn

[U114] JS：JSON 深比较
来源：http://wb.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tq.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://bi.nicolike.cn

crypto.randomUUID()
来源：http://yo.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ik.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://gq.gzmigu.cn

[U117] JS：单元测试
来源：http://sn.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://dl.nicolike.cn

[U118] JS：开发服务器
来源：http://dm.nicolike.cn

npm i -D vite;  npx vite
来源：http://ty.bjjhwx.cn

[U119] JS：生产构建
来源：http://da.szsharing.cn

npx vite build
来源：http://oc.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ro.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://oc.szxytkj.cn

================================================================================
来源：http://wz.bookmarksfly.cn

统计汇总
来源：http://yq.huanxung.cn

================================================================================
来源：http://wi.nszjky.cn

按语言统计（条）：
来源：http://jp.muxihuayi.cn

Python ......... 252
来源：http://xx.huixiangedu.cn

PHP ............ 252
来源：http://hd.gzmigu.cn

JavaScript ..... 252
来源：http://uk.nszjky.cn

TypeScript ..... 212
来源：http://mb.hnjuh.cn

Java ........... 212
来源：http://ab.hnjuh.cn

Go ............. 212
来源：http://nl.yuntaijiaju.cn

Ruby ........... 212
来源：http://fq.haigaiapp.cn

C# ............. 212
来源：http://gp.nszjky.cn

C .............. 30
来源：http://kd.szxytkj.cn

C++ ............ 30
来源：http://qk.gzmigu.cn

SQL ............ 90
来源：http://ed.newstarts.cn

Bash ........... 80
来源：http://xo.jianghongdianzi.cn

Kotlin ......... 15
来源：http://hk.hahajie.cn

Swift .......... 15
来源：http://cf.nszjky.cn

Lua ............ 10
来源：http://ip.hnjuh.cn

Perl ........... 10
来源：http://ng.muxihuayi.cn


<!-- 参考信息 -->