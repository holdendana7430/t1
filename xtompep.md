代发 wailian999

[T45] Perl：数组遍历
来源：http://hd.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://sk.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://eb.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ya.lnxyls.cn

[T47] Perl：正则捕获
来源：http://hn.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mu.gzmigu.cn

[T48] Perl：正则替换
来源：http://hr.9csxet.cn

$s =~ s/old/new/g;
来源：http://ff.jianghongdianzi.cn

[T49] Perl：函数
来源：http://jb.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wb.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://fa.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gj.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://ht.521024.cn

[T51] Scala：Hello World
来源：http://oi.shtwfgs.cn

println("Hello")
来源：http://vz.panjiajie.cn

[T52] Scala：变量
来源：http://yo.yuexingan06.cn

val a = 1;  var b = 2
来源：http://sv.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://wv.muxihuayi.cn

s"值: $b"
来源：http://il.gzmigu.cn

[T54] Scala：集合映射
来源：http://uv.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ln.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://hu.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kx.bjjhwx.cn

[T56] Scala：样例类
来源：http://ae.szsharing.cn

case class User(name: String, age: Int)
来源：http://ao.9csxet.cn

[T57] Scala：模式匹配
来源：http://fx.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tr.asd995.cn

[T58] Scala：函数定义
来源：http://yj.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hw.chemitech.net.cn

[T59] Scala：循环
来源：http://li.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://nt.bjjhwx.cn

[T60] Scala：折叠
来源：http://kw.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uz.wgjwhj.cn

================================================================================
来源：http://xe.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yi.jianghongdianzi.cn

================================================================================
来源：http://zv.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ly.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mo.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://ks.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yh.521024.cn

[U03] Py：加载 .env 配置
来源：http://ce.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ny.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://vl.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mx.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://tt.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://ai.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://qi.panjiajie.cn

{**a, **b}
来源：http://ni.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://cb.newstarts.cn

{v: k for k, v in d.items()}
来源：http://mv.nszjky.cn

[U08] Py：展平二维列表
来源：http://ml.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://xu.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://xi.newstarts.cn

max(d, key=d.get)
来源：http://te.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://ty.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yj.9csxet.cn

[U11] Py：生成器表达式
来源：http://bt.huanxung.cn

(x * 2 for x in arr)
来源：http://jx.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ed.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://gg.szxytkj.cn

[U13] Py：固定长度队列
来源：http://xn.521024.cn

deque(maxlen=10)
来源：http://ac.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://kj.shxzskj.cn

defaultdict(list)
来源：http://hd.huixiangedu.cn

[U15] Py：高精度计时
来源：http://sg.gzmigu.cn

t = time.perf_counter()
来源：http://fo.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://mm.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iv.lnxyls.cn

[U17] Py：初始化日志
来源：http://yy.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://vq.gzmigu.cn

[U18] Py：预编译正则
来源：http://qn.colortex.cn

pat = re.compile(r"\d+")
来源：http://ot.hahajie.cn

[U19] Py：正则替换带回调
来源：http://rs.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gs.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://pa.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://dv.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://kh.nicolike.cn

@contextlib.contextmanager
来源：http://ud.szsharing.cn

[U22] Py：矩阵转置
来源：http://sa.huixiangedu.cn

list(zip(*m))
来源：http://ll.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://bj.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sc.szxytkj.cn

[U24] Py：路径操作
来源：http://qw.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cy.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://ao.shxzukj.cn

csv.DictReader(f)
来源：http://uk.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://ef.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mh.521024.cn

[U27] Py：异步 HTTP
来源：http://cy.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://hg.lnxyls.cn

[U28] Py：类型别名
来源：http://sh.yuntaijiaju.cn

UserId = int
来源：http://aj.haigaiapp.cn

[U29] Py：属性校验
来源：http://nl.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://lv.lnxyls.cn

[U30] Py：数据类
来源：http://de.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://nt.colortex.cn

[U31] Py：单测
来源：http://yb.9csxet.cn

python -m pytest -q
来源：http://xw.bjjhwx.cn

[U32] Py：代码格式化
来源：http://cu.szsharing.cn

ruff format . && ruff check --fix .
来源：http://de.shxzskj.cn

[U33] Py：打包发布
来源：http://ih.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://pz.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://oa.chemitech.net.cn

chardet.detect(raw)
来源：http://yh.9csxet.cn

[U35] Py：发送邮件
来源：http://os.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nk.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://jf.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://xi.shxzukj.cn

[U37] Py：读写 Excel
来源：http://vp.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yp.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://ff.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://pp.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://jd.chemitech.net.cn

sys.stdout.isatty()
来源：http://qw.newstarts.cn

[U40] Py：打印到标准错误
来源：http://xh.hnjuh.cn

print("err", file=sys.stderr)
来源：http://bs.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://tz.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ln.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://mc.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://im.szsharing.cn

[U43] PHP：声明命名空间
来源：http://iv.szsharing.cn

namespace App\Http;
来源：http://oe.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://tu.szxytkj.cn

declare(strict_types=1);
来源：http://aa.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://jm.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nb.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://tt.bjjhwx.cn

?string $name = null
来源：http://xt.panjiajie.cn

[U47] PHP：联合类型
来源：http://ru.asd995.cn

int|string $id
来源：http://mt.colortex.cn

[U48] PHP：纯枚举
来源：http://bn.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jh.shxzukj.cn

[U49] PHP：只读属性
来源：http://ov.shxzskj.cn

public readonly string $name
来源：http://qj.asd995.cn

[U50] PHP：构造器属性提升
来源：http://pb.nicolike.cn

public function __construct(private int $id) {}
来源：http://jf.panjiajie.cn

[U51] PHP：数组解构
来源：http://ed.newstarts.cn

[$a, $b] = $arr;
来源：http://bp.asd995.cn

[U52] PHP：箭头函数
来源：http://pw.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://nb.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://ku.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://np.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://tg.lnxyls.cn

$obj?->method()
来源：http://zq.panjiajie.cn

[U55] PHP：match 表达式
来源：http://ni.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zf.hahajie.cn

[U56] PHP：命名参数
来源：http://zw.asd995.cn

f(a: 1, b: 2)
来源：http://mr.lnxyls.cn

[U57] PHP：字符串插值
来源：http://nl.colortex.cn

"值: {$a}"
来源：http://qb.hnjuh.cn

[U58] PHP：数组三件套
来源：http://cv.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oh.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://zs.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qc.asd995.cn

[U60] PHP：JSON 编解码
来源：http://ah.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vk.bookmarksfly.cn

[U61] PHP：正则
来源：http://zv.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hj.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://fh.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hd.nicolike.cn

[U63] PHP：文件读写
来源：http://uv.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fa.nszjky.cn

[U64] PHP：目录遍历
来源：http://yt.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ys.yuntaijiaju.cn

[U65] PHP：会话
来源：http://ap.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yc.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://sp.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gr.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://zg.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fv.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://pn.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aq.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://cf.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://my.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://rn.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iw.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://ii.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://vv.shxzskj.cn

[U72] PHP：写错误日志
来源：http://zf.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://nt.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://nk.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://qk.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://th.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://ts.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fr.jianghongdianzi.cn

composer require psr/container
来源：http://ja.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://fu.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mf.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://eo.szsharing.cn

composer require twig/twig
来源：http://mr.newstarts.cn

[U78] PHP：单元测试
来源：http://dm.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://ko.asd995.cn

[U79] PHP：静态分析
来源：http://bs.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://vj.521024.cn

[U80] PHP：代码规范修复
来源：http://kq.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://il.asd995.cn

[U81] JS：初始化项目
来源：http://mx.lnxyls.cn

npm init -y;  npm i express
来源：http://fn.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://eq.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kd.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://fp.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xr.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://ya.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rc.shxzukj.cn

[U85] JS：可选链
来源：http://dm.gzmigu.cn

a?.b?.c
来源：http://ty.asd995.cn

[U86] JS：空值合并
来源：http://sk.jianghongdianzi.cn

a ?? b
来源：http://kq.huixiangedu.cn

[U87] JS：解构默认值
来源：http://rp.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://dw.hnjuh.cn

[U88] JS：对象展开合并
来源：http://nt.bookmarksfly.cn

{ ...a, ...b }
来源：http://pg.chemitech.net.cn

[U89] JS：数组去重
来源：http://fx.nicolike.cn

[...new Set(arr)]
来源：http://mx.nicolike.cn

[U90] JS：数字数组排序
来源：http://si.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://wq.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://ub.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://na.hahajie.cn

[U92] JS：深拷贝
来源：http://rb.lnxyls.cn

structuredClone(obj)
来源：http://zt.szsharing.cn

[U93] JS：模板字符串
来源：http://tx.huixinmuqiang.cn

`共 ${n} 条`
来源：http://zg.panjiajie.cn

[U94] JS：箭头函数
来源：http://lg.nszjky.cn

const double = x => x * 2;
来源：http://ij.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://kq.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://kw.nszjky.cn

[U96] JS：async/await 与异常
来源：http://sg.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sk.muxihuayi.cn

[U97] JS：并发请求
来源：http://ul.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hb.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://df.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cq.shxzskj.cn

[U99] JS：事件监听
来源：http://jt.nszjky.cn

el.addEventListener("click", e => {})
来源：http://ly.colortex.cn

[U100] JS：DOM 查询
来源：http://lf.bookmarksfly.cn

document.querySelector(".item")
来源：http://gg.colortex.cn

[U101] JS：classList 操作
来源：http://zw.chemitech.net.cn

el.classList.toggle("active")
来源：http://ay.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://vr.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ej.shxzskj.cn

[U103] JS：定时器
来源：http://uk.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ku.newstarts.cn

[U104] JS：防抖
来源：http://is.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fd.bjjhwx.cn

[U105] JS：节流
来源：http://ww.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://th.haigaiapp.cn

[U106] JS：日期格式化
来源：http://hq.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hc.huixiangedu.cn

[U107] JS：数字千分位
来源：http://jt.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uf.huixiangedu.cn

[U108] JS：随机整数
来源：http://ui.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hp.nszjky.cn

[U109] JS：数组分组
来源：http://qf.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://af.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://xi.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ih.hahajie.cn

[U111] JS：对象转 Map
来源：http://sy.hnjuh.cn

new Map(Object.entries(obj))
来源：http://hu.hahajie.cn

[U112] JS：字符串补位
来源：http://sl.chemitech.net.cn

"7".padStart(3, "0")
来源：http://sb.asd995.cn

[U113] JS：正则替换全部
来源：http://fn.colortex.cn

s.replaceAll("a", "b")
来源：http://tx.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://in.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://le.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://rp.jianghongdianzi.cn

crypto.randomUUID()
来源：http://vx.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://gb.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://wm.huanxung.cn

[U117] JS：单元测试
来源：http://ob.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://ju.szxytkj.cn

[U118] JS：开发服务器
来源：http://rr.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://du.wgjwhj.cn

[U119] JS：生产构建
来源：http://lk.huixinmuqiang.cn

npx vite build
来源：http://gx.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://fi.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://df.colortex.cn

================================================================================
来源：http://tg.huanxung.cn

统计汇总
来源：http://yr.hnjuh.cn

================================================================================
来源：http://ye.shxzukj.cn

按语言统计（条）：
来源：http://ic.yuntaijiaju.cn

Python ......... 252
来源：http://pt.newstarts.cn

PHP ............ 252
来源：http://li.hahajie.cn

JavaScript ..... 252
来源：http://gd.huixiangedu.cn

TypeScript ..... 212
来源：http://od.colortex.cn

Java ........... 212
来源：http://xi.shxzukj.cn

Go ............. 212
来源：http://zm.huixinmuqiang.cn

Ruby ........... 212
来源：http://ja.bookmarksfly.cn

C# ............. 212
来源：http://kt.huixiangedu.cn

C .............. 30
来源：http://ty.yuntaijiaju.cn

C++ ............ 30
来源：http://mh.521024.cn

SQL ............ 90
来源：http://hh.shxzskj.cn

Bash ........... 80
来源：http://we.huixiangedu.cn

Kotlin ......... 15
来源：http://no.huanxung.cn

Swift .......... 15
来源：http://lq.yuexingan06.cn

Lua ............ 10
来源：http://yd.bookmarksfly.cn

Perl ........... 10
来源：http://xy.9csxet.cn

Scala .......... 10
来源：http://iy.gzmigu.cn

------------------------------------
来源：http://yd.hahajie.cn

合计 ........... 2106 条
来源：http://zg.bjjhwx.cn

按章节统计：
来源：http://bu.jctech888.com.cn


<!-- 参考信息 -->