代发 wailian999

[T45] Perl：数组遍历
来源：http://lq.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://qx.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://bz.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pf.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://ip.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rr.9csxet.cn

[T48] Perl：正则替换
来源：http://cd.hahajie.cn

$s =~ s/old/new/g;
来源：http://bs.nszjky.cn

[T49] Perl：函数
来源：http://av.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qa.9csxet.cn

[T50] Perl：逐行读文件
来源：http://zl.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cu.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ac.hahajie.cn

[T51] Scala：Hello World
来源：http://eu.szsharing.cn

println("Hello")
来源：http://qq.lnxyls.cn

[T52] Scala：变量
来源：http://gb.colortex.cn

val a = 1;  var b = 2
来源：http://eh.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://lk.hnjuh.cn

s"值: $b"
来源：http://sp.bjjhwx.cn

[T54] Scala：集合映射
来源：http://pg.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://sw.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ui.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xe.haigaiapp.cn

[T56] Scala：样例类
来源：http://te.colortex.cn

case class User(name: String, age: Int)
来源：http://bb.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://ff.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uy.shxzskj.cn

[T58] Scala：函数定义
来源：http://lf.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rb.nicolike.cn

[T59] Scala：循环
来源：http://om.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://xa.521024.cn

[T60] Scala：折叠
来源：http://pu.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iy.shxzukj.cn

================================================================================
来源：http://wz.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cp.szsharing.cn

================================================================================
来源：http://td.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://ba.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://da.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://cj.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ox.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://hd.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rr.asd995.cn

[U04] Py：变量调试打印
来源：http://pv.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ek.colortex.cn

[U05] Py：列表去重且保序
来源：http://nu.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://pk.shxzskj.cn

[U06] Py：合并两个字典
来源：http://ld.huanxung.cn

{**a, **b}
来源：http://gg.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://ot.huanxung.cn

{v: k for k, v in d.items()}
来源：http://ir.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://ew.huanxung.cn

[y for x in nested for y in x]
来源：http://cz.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://du.bookmarksfly.cn

max(d, key=d.get)
来源：http://jv.gzmigu.cn

[U10] Py：按值排序字典
来源：http://tx.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xm.shxzskj.cn

[U11] Py：生成器表达式
来源：http://td.wgjwhj.cn

(x * 2 for x in arr)
来源：http://wv.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nt.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://jl.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://se.nicolike.cn

deque(maxlen=10)
来源：http://bi.asd995.cn

[U14] Py：分组收集到列表
来源：http://hi.bookmarksfly.cn

defaultdict(list)
来源：http://zo.szsharing.cn

[U15] Py：高精度计时
来源：http://xo.colortex.cn

t = time.perf_counter()
来源：http://hv.hahajie.cn

[U16] Py：命令行参数解析
来源：http://yu.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ex.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://ol.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ge.nicolike.cn

[U18] Py：预编译正则
来源：http://ih.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://ju.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://ch.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qv.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://wf.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://ny.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://nc.lnxyls.cn

@contextlib.contextmanager
来源：http://zp.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://cs.gzmigu.cn

list(zip(*m))
来源：http://ns.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://gw.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qq.nszjky.cn

[U24] Py：路径操作
来源：http://qp.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zi.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://so.gzmigu.cn

csv.DictReader(f)
来源：http://wb.bookmarksfly.cn

[U26] Py：并发下载
来源：http://zo.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xa.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://qy.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://tv.huixiangedu.cn

[U28] Py：类型别名
来源：http://tc.muxihuayi.cn

UserId = int
来源：http://ro.9csxet.cn

[U29] Py：属性校验
来源：http://ox.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://cu.jctech888.com.cn

[U30] Py：数据类
来源：http://ug.huanxung.cn

@dataclass(slots=True)
来源：http://ok.muxihuayi.cn

[U31] Py：单测
来源：http://ls.muxihuayi.cn

python -m pytest -q
来源：http://hl.shtwfgs.cn

[U32] Py：代码格式化
来源：http://cd.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://vo.bjjhwx.cn

[U33] Py：打包发布
来源：http://yh.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://ri.bjjhwx.cn

[U34] Py：判断编码
来源：http://fe.huanxung.cn

chardet.detect(raw)
来源：http://qx.jctech888.com.cn

[U35] Py：发送邮件
来源：http://ve.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pn.bjjhwx.cn

[U36] Py：定时任务
来源：http://tu.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://jc.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://ch.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zk.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://ic.9csxet.cn

Path(__file__).resolve().parent
来源：http://sc.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://ex.gzmigu.cn

sys.stdout.isatty()
来源：http://fk.colortex.cn

[U40] Py：打印到标准错误
来源：http://cv.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://ap.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://zm.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gd.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://tt.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ht.9csxet.cn

[U43] PHP：声明命名空间
来源：http://mp.yuexingan06.cn

namespace App\Http;
来源：http://uo.asd995.cn

[U44] PHP：开启严格类型
来源：http://dv.szsharing.cn

declare(strict_types=1);
来源：http://ye.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://tx.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://pq.wgjwhj.cn

?string $name = null
来源：http://kq.lnxyls.cn

[U47] PHP：联合类型
来源：http://lw.wgjwhj.cn

int|string $id
来源：http://ao.9csxet.cn

[U48] PHP：纯枚举
来源：http://to.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cy.newstarts.cn

[U49] PHP：只读属性
来源：http://hf.521024.cn

public readonly string $name
来源：http://ls.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://sj.shxzukj.cn

public function __construct(private int $id) {}
来源：http://wm.shxzukj.cn

[U51] PHP：数组解构
来源：http://he.huanxung.cn

[$a, $b] = $arr;
来源：http://td.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://wt.521024.cn

$double = fn($x) => $x * 2;
来源：http://vb.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://pn.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://nw.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://xz.shtwfgs.cn

$obj?->method()
来源：http://iw.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://nf.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ls.chemitech.net.cn

[U56] PHP：命名参数
来源：http://dw.lnxyls.cn

f(a: 1, b: 2)
来源：http://eg.colortex.cn

[U57] PHP：字符串插值
来源：http://md.asd995.cn

"值: {$a}"
来源：http://yf.shxzskj.cn

[U58] PHP：数组三件套
来源：http://kg.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mc.9csxet.cn

[U59] PHP：自定义排序
来源：http://no.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jm.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://dg.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aw.hnjuh.cn

[U61] PHP：正则
来源：http://zv.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iu.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://qg.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rh.asd995.cn

[U63] PHP：文件读写
来源：http://st.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zj.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://rc.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://cp.nszjky.cn

[U65] PHP：会话
来源：http://vo.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qr.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://pa.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ks.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://cj.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ok.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://fw.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lo.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://az.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://un.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ir.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://es.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://fm.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://aw.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://qj.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://lv.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://fe.colortex.cn

parse_ini_file("config.ini", true)
来源：http://nh.huanxung.cn

[U74] PHP：读取环境变量
来源：http://pi.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://fn.hahajie.cn

[U75] PHP：依赖注入
来源：http://pb.lnxyls.cn

composer require psr/container
来源：http://uu.nicolike.cn

[U76] PHP：简单路由
来源：http://sv.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uz.nszjky.cn

[U77] PHP：模板渲染
来源：http://xg.panjiajie.cn

composer require twig/twig
来源：http://jd.wgjwhj.cn

[U78] PHP：单元测试
来源：http://qv.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://zt.jctech888.com.cn

[U79] PHP：静态分析
来源：http://oc.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://ct.colortex.cn

[U80] PHP：代码规范修复
来源：http://gg.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eg.panjiajie.cn

[U81] JS：初始化项目
来源：http://yl.panjiajie.cn

npm init -y;  npm i express
来源：http://wv.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://fi.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cd.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://py.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mi.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://pl.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tj.newstarts.cn

[U85] JS：可选链
来源：http://bh.jianghongdianzi.cn

a?.b?.c
来源：http://rp.szxytkj.cn

[U86] JS：空值合并
来源：http://gf.nicolike.cn

a ?? b
来源：http://kj.huixiangedu.cn

[U87] JS：解构默认值
来源：http://yi.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://fn.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://rx.wgjwhj.cn

{ ...a, ...b }
来源：http://zy.szsharing.cn

[U89] JS：数组去重
来源：http://ew.jctech888.com.cn

[...new Set(arr)]
来源：http://ed.521024.cn

[U90] JS：数字数组排序
来源：http://xu.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://dl.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://bj.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iw.asd995.cn

[U92] JS：深拷贝
来源：http://jd.chemitech.net.cn

structuredClone(obj)
来源：http://rr.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://ms.bookmarksfly.cn

`共 ${n} 条`
来源：http://sn.hnjuh.cn

[U94] JS：箭头函数
来源：http://ga.nszjky.cn

const double = x => x * 2;
来源：http://em.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://zz.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://ht.newstarts.cn

[U96] JS：async/await 与异常
来源：http://eu.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hf.newstarts.cn

[U97] JS：并发请求
来源：http://dt.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xh.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://lv.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xx.yuexingan06.cn

[U99] JS：事件监听
来源：http://qv.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://dm.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://fi.wgjwhj.cn

document.querySelector(".item")
来源：http://no.nicolike.cn

[U101] JS：classList 操作
来源：http://xr.yuexingan06.cn

el.classList.toggle("active")
来源：http://fr.muxihuayi.cn

[U102] JS：本地存储
来源：http://vr.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kt.9csxet.cn

[U103] JS：定时器
来源：http://ac.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mc.521024.cn

[U104] JS：防抖
来源：http://zq.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zx.newstarts.cn

[U105] JS：节流
来源：http://gd.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bz.hnjuh.cn

[U106] JS：日期格式化
来源：http://vx.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ec.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://xk.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://se.hahajie.cn

[U108] JS：随机整数
来源：http://rd.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kg.haigaiapp.cn

[U109] JS：数组分组
来源：http://td.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://dj.nszjky.cn

[U110] JS：数组分块
来源：http://qi.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kd.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://rc.lnxyls.cn

new Map(Object.entries(obj))
来源：http://xi.shtwfgs.cn

[U112] JS：字符串补位
来源：http://wu.asd995.cn

"7".padStart(3, "0")
来源：http://kd.panjiajie.cn

[U113] JS：正则替换全部
来源：http://oc.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://zp.9csxet.cn

[U114] JS：JSON 深比较
来源：http://rn.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ci.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://nf.huixiangedu.cn

crypto.randomUUID()
来源：http://th.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://ef.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://qw.newstarts.cn

[U117] JS：单元测试
来源：http://ar.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://pi.nszjky.cn

[U118] JS：开发服务器
来源：http://fg.lnxyls.cn

npm i -D vite;  npx vite
来源：http://bv.nszjky.cn

[U119] JS：生产构建
来源：http://tz.bjjhwx.cn

npx vite build
来源：http://nk.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://gh.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ix.huixiangedu.cn

================================================================================
来源：http://vi.jianghongdianzi.cn

统计汇总
来源：http://jd.wgjwhj.cn

================================================================================
来源：http://ui.jctech888.com.cn

按语言统计（条）：
来源：http://fs.jctech888.com.cn

Python ......... 252
来源：http://jg.colortex.cn

PHP ............ 252
来源：http://wg.9csxet.cn

JavaScript ..... 252
来源：http://zz.lnxyls.cn

TypeScript ..... 212
来源：http://rt.shxzskj.cn

Java ........... 212
来源：http://ka.chemitech.net.cn

Go ............. 212
来源：http://lv.haigaiapp.cn

Ruby ........... 212
来源：http://vv.9csxet.cn

C# ............. 212
来源：http://lt.nszjky.cn

C .............. 30
来源：http://oc.hahajie.cn

C++ ............ 30
来源：http://fh.panjiajie.cn

SQL ............ 90
来源：http://jy.huixiangedu.cn

Bash ........... 80
来源：http://um.bookmarksfly.cn

Kotlin ......... 15
来源：http://og.shxzskj.cn

Swift .......... 15
来源：http://lk.bookmarksfly.cn

Lua ............ 10
来源：http://je.nszjky.cn

Perl ........... 10
来源：http://rl.huixiangedu.cn

Scala .......... 10
来源：http://xb.haigaiapp.cn

------------------------------------
来源：http://el.bookmarksfly.cn

合计 ........... 2106 条
来源：http://pi.huixiangedu.cn

按章节统计：
来源：http://yr.yuntaijiaju.cn


<!-- 参考信息 -->