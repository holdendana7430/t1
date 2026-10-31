代发 wailian999

[T41] Perl：Hello World
来源：http://ja.wgjwhj.cn

print "Hello\n";
来源：http://zd.lnxyls.cn

[T42] Perl：变量类型
来源：http://nd.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fr.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://kw.nszjky.cn

"值: $a"
来源：http://zf.yuntaijiaju.cn

[T44] Perl：条件
来源：http://dh.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://gj.panjiajie.cn

[T45] Perl：数组遍历
来源：http://eq.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://br.nszjky.cn

[T46] Perl：哈希操作
来源：http://te.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vc.nszjky.cn

[T47] Perl：正则捕获
来源：http://po.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ri.newstarts.cn

[T48] Perl：正则替换
来源：http://hr.szxytkj.cn

$s =~ s/old/new/g;
来源：http://po.muxihuayi.cn

[T49] Perl：函数
来源：http://ny.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cs.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://xs.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bk.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://zh.asd995.cn

[T51] Scala：Hello World
来源：http://kx.yuntaijiaju.cn

println("Hello")
来源：http://pm.huixiangedu.cn

[T52] Scala：变量
来源：http://ae.9csxet.cn

val a = 1;  var b = 2
来源：http://ai.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://pp.huixinmuqiang.cn

s"值: $b"
来源：http://gm.nicolike.cn

[T54] Scala：集合映射
来源：http://hv.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://wq.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://yv.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gb.yuexingan06.cn

[T56] Scala：样例类
来源：http://mv.lnxyls.cn

case class User(name: String, age: Int)
来源：http://bm.hnjuh.cn

[T57] Scala：模式匹配
来源：http://qt.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ip.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://lo.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ew.nszjky.cn

[T59] Scala：循环
来源：http://fe.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://is.szxytkj.cn

[T60] Scala：折叠
来源：http://lv.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cm.jctech888.com.cn

================================================================================
来源：http://pu.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kv.haigaiapp.cn

================================================================================
来源：http://fe.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://mw.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rg.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://ae.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://id.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://rp.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mn.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://vo.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fn.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://ka.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ld.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://pw.jctech888.com.cn

{**a, **b}
来源：http://gc.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://sl.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://dq.nszjky.cn

[U08] Py：展平二维列表
来源：http://jg.yuexingan06.cn

[y for x in nested for y in x]
来源：http://pd.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://sh.hnjuh.cn

max(d, key=d.get)
来源：http://hn.panjiajie.cn

[U10] Py：按值排序字典
来源：http://uu.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ub.nszjky.cn

[U11] Py：生成器表达式
来源：http://pe.huixiangedu.cn

(x * 2 for x in arr)
来源：http://qc.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gy.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://tf.shxzskj.cn

[U13] Py：固定长度队列
来源：http://sx.huanxung.cn

deque(maxlen=10)
来源：http://by.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://sn.nszjky.cn

defaultdict(list)
来源：http://qr.hahajie.cn

[U15] Py：高精度计时
来源：http://te.szsharing.cn

t = time.perf_counter()
来源：http://lj.nicolike.cn

[U16] Py：命令行参数解析
来源：http://uw.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xh.bjjhwx.cn

[U17] Py：初始化日志
来源：http://id.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://yh.huixiangedu.cn

[U18] Py：预编译正则
来源：http://nm.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://na.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://wr.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://am.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ft.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://fk.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://lp.gzmigu.cn

@contextlib.contextmanager
来源：http://ux.szxytkj.cn

[U22] Py：矩阵转置
来源：http://lb.muxihuayi.cn

list(zip(*m))
来源：http://jn.nicolike.cn

[U23] Py：分块读取大文件
来源：http://xu.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sh.jctech888.com.cn

[U24] Py：路径操作
来源：http://gm.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ga.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://sq.huixiangedu.cn

csv.DictReader(f)
来源：http://ef.shtwfgs.cn

[U26] Py：并发下载
来源：http://hx.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zp.hahajie.cn

[U27] Py：异步 HTTP
来源：http://mv.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://vs.szxytkj.cn

[U28] Py：类型别名
来源：http://xc.nszjky.cn

UserId = int
来源：http://ni.521024.cn

[U29] Py：属性校验
来源：http://yz.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ph.jctech888.com.cn

[U30] Py：数据类
来源：http://kj.hahajie.cn

@dataclass(slots=True)
来源：http://ll.colortex.cn

[U31] Py：单测
来源：http://dj.521024.cn

python -m pytest -q
来源：http://fi.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://zu.hahajie.cn

ruff format . && ruff check --fix .
来源：http://zw.shtwfgs.cn

[U33] Py：打包发布
来源：http://qe.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://rx.asd995.cn

[U34] Py：判断编码
来源：http://ct.huixinmuqiang.cn

chardet.detect(raw)
来源：http://vt.colortex.cn

[U35] Py：发送邮件
来源：http://ak.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yd.yuexingan06.cn

[U36] Py：定时任务
来源：http://uz.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://iu.newstarts.cn

[U37] Py：读写 Excel
来源：http://hs.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://df.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://vy.nicolike.cn

Path(__file__).resolve().parent
来源：http://cb.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ht.chemitech.net.cn

sys.stdout.isatty()
来源：http://ao.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://dl.szxytkj.cn

print("err", file=sys.stderr)
来源：http://us.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ql.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zx.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://lm.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ee.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://jc.lnxyls.cn

namespace App\Http;
来源：http://qt.nszjky.cn

[U44] PHP：开启严格类型
来源：http://hz.yuexingan06.cn

declare(strict_types=1);
来源：http://bj.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://eo.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.hnjuh.cn

[U46] PHP：可空类型
来源：http://gq.wgjwhj.cn

?string $name = null
来源：http://ns.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ln.521024.cn

int|string $id
来源：http://nd.shxzskj.cn

[U48] PHP：纯枚举
来源：http://uf.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vd.shxzskj.cn

[U49] PHP：只读属性
来源：http://kf.yuexingan06.cn

public readonly string $name
来源：http://so.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://jt.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://hh.lnxyls.cn

[U51] PHP：数组解构
来源：http://xm.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://mk.panjiajie.cn

[U52] PHP：箭头函数
来源：http://oz.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://uc.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://lt.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://mt.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://wz.nicolike.cn

$obj?->method()
来源：http://eh.gzmigu.cn

[U55] PHP：match 表达式
来源：http://de.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://on.gzmigu.cn

[U56] PHP：命名参数
来源：http://cj.asd995.cn

f(a: 1, b: 2)
来源：http://yr.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://so.shxzskj.cn

"值: {$a}"
来源：http://lt.521024.cn

[U58] PHP：数组三件套
来源：http://hf.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rv.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://jm.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://oy.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ze.colortex.cn

[U61] PHP：正则
来源：http://ni.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bc.9csxet.cn

[U62] PHP：日期对象
来源：http://na.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ld.9csxet.cn

[U63] PHP：文件读写
来源：http://wc.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rt.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://jm.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://eh.asd995.cn

[U65] PHP：会话
来源：http://im.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iy.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://lb.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ed.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://jt.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zq.newstarts.cn

[U68] PHP：PDO 连接
来源：http://jl.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pl.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://bx.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kp.nszjky.cn

[U70] PHP：PDO 事务
来源：http://qd.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bl.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://cu.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://fj.521024.cn

[U72] PHP：写错误日志
来源：http://vc.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://rs.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://bt.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://qk.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://co.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://dl.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://iq.yuntaijiaju.cn

composer require psr/container
来源：http://mn.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://ot.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ph.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://pd.haigaiapp.cn

composer require twig/twig
来源：http://ta.hnjuh.cn

[U78] PHP：单元测试
来源：http://kh.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://fb.521024.cn

[U79] PHP：静态分析
来源：http://iy.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://hf.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://zz.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xh.colortex.cn

[U81] JS：初始化项目
来源：http://fz.haigaiapp.cn

npm init -y;  npm i express
来源：http://zu.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://aq.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tq.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://md.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rb.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://hj.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ng.hahajie.cn

[U85] JS：可选链
来源：http://hn.521024.cn

a?.b?.c
来源：http://xb.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://hm.bookmarksfly.cn

a ?? b
来源：http://yq.hnjuh.cn

[U87] JS：解构默认值
来源：http://lx.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://gk.nicolike.cn

[U88] JS：对象展开合并
来源：http://ak.yuexingan06.cn

{ ...a, ...b }
来源：http://fd.haigaiapp.cn

[U89] JS：数组去重
来源：http://er.lnxyls.cn

[...new Set(arr)]
来源：http://ss.9csxet.cn

[U90] JS：数字数组排序
来源：http://yd.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://fb.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://sy.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ky.nszjky.cn

[U92] JS：深拷贝
来源：http://zs.yuntaijiaju.cn

structuredClone(obj)
来源：http://xv.9csxet.cn

[U93] JS：模板字符串
来源：http://rw.nicolike.cn

`共 ${n} 条`
来源：http://fw.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://ff.9csxet.cn

const double = x => x * 2;
来源：http://sh.newstarts.cn

[U95] JS：Promise 包装
来源：http://oc.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://th.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://jx.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qu.haigaiapp.cn

[U97] JS：并发请求
来源：http://si.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mw.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://ef.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sf.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://tf.9csxet.cn

el.addEventListener("click", e => {})
来源：http://em.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://vc.asd995.cn

document.querySelector(".item")
来源：http://zw.lnxyls.cn

[U101] JS：classList 操作
来源：http://ds.colortex.cn

el.classList.toggle("active")
来源：http://ak.9csxet.cn

[U102] JS：本地存储
来源：http://mv.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jz.nszjky.cn

[U103] JS：定时器
来源：http://ms.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nx.chemitech.net.cn

[U104] JS：防抖
来源：http://ua.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wz.huixiangedu.cn

[U105] JS：节流
来源：http://ev.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oj.szsharing.cn

[U106] JS：日期格式化
来源：http://ir.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ya.szsharing.cn

[U107] JS：数字千分位
来源：http://sm.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lo.muxihuayi.cn

[U108] JS：随机整数
来源：http://vn.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ug.nszjky.cn

[U109] JS：数组分组
来源：http://tn.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://gc.jctech888.com.cn

[U110] JS：数组分块
来源：http://ke.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jy.szxytkj.cn

[U111] JS：对象转 Map
来源：http://lm.newstarts.cn

new Map(Object.entries(obj))
来源：http://vc.huanxung.cn

[U112] JS：字符串补位
来源：http://zf.panjiajie.cn

"7".padStart(3, "0")
来源：http://zt.hahajie.cn

[U113] JS：正则替换全部
来源：http://pa.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://bp.szsharing.cn

[U114] JS：JSON 深比较
来源：http://ty.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ut.colortex.cn

[U115] JS：生成 UUID
来源：http://ei.hnjuh.cn

crypto.randomUUID()
来源：http://dk.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ja.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://eu.hahajie.cn

[U117] JS：单元测试
来源：http://jp.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://zr.9csxet.cn

[U118] JS：开发服务器
来源：http://aj.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://zf.521024.cn

[U119] JS：生产构建
来源：http://vh.gzmigu.cn

npx vite build
来源：http://dj.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://uf.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://pa.hnjuh.cn

================================================================================
来源：http://jv.huanxung.cn

统计汇总
来源：http://nz.bookmarksfly.cn

================================================================================
来源：http://ux.haigaiapp.cn

按语言统计（条）：
来源：http://wi.muxihuayi.cn

Python ......... 252
来源：http://tt.shxzskj.cn

PHP ............ 252
来源：http://tm.newstarts.cn

JavaScript ..... 252
来源：http://oy.colortex.cn

TypeScript ..... 212
来源：http://tz.9csxet.cn

Java ........... 212
来源：http://vl.shxzskj.cn

Go ............. 212
来源：http://qy.nicolike.cn

Ruby ........... 212
来源：http://wj.bookmarksfly.cn

C# ............. 212
来源：http://oh.asd995.cn

C .............. 30
来源：http://nd.bookmarksfly.cn

C++ ............ 30
来源：http://ce.bjjhwx.cn

SQL ............ 90
来源：http://ds.9csxet.cn

Bash ........... 80
来源：http://di.haigaiapp.cn


<!-- 参考信息 -->