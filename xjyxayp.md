代发 wailian999

[T39] Lua：模式匹配
来源：http://qi.nicolike.cn

string.find(s, "%d+")
来源：http://fe.wgjwhj.cn

[T40] Lua：元表
来源：http://vv.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://tt.bjjhwx.cn

[T41] Perl：Hello World
来源：http://lv.muxihuayi.cn

print "Hello\n";
来源：http://po.shxzukj.cn

[T42] Perl：变量类型
来源：http://cw.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ca.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://xg.jctech888.com.cn

"值: $a"
来源：http://ol.521024.cn

[T44] Perl：条件
来源：http://wr.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://xe.521024.cn

[T45] Perl：数组遍历
来源：http://wf.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ld.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://ll.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xj.newstarts.cn

[T47] Perl：正则捕获
来源：http://rv.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uc.bjjhwx.cn

[T48] Perl：正则替换
来源：http://jb.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://dw.huixinmuqiang.cn

[T49] Perl：函数
来源：http://va.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oe.colortex.cn

[T50] Perl：逐行读文件
来源：http://zq.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jh.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://tn.wgjwhj.cn

[T51] Scala：Hello World
来源：http://qi.hnjuh.cn

println("Hello")
来源：http://ed.hnjuh.cn

[T52] Scala：变量
来源：http://tk.szsharing.cn

val a = 1;  var b = 2
来源：http://ss.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://lq.shxzukj.cn

s"值: $b"
来源：http://gn.huixiangedu.cn

[T54] Scala：集合映射
来源：http://rr.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://qw.colortex.cn

[T55] Scala：集合过滤
来源：http://ai.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ck.521024.cn

[T56] Scala：样例类
来源：http://yp.gzmigu.cn

case class User(name: String, age: Int)
来源：http://bg.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://by.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mi.szsharing.cn

[T58] Scala：函数定义
来源：http://fn.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bs.gzmigu.cn

[T59] Scala：循环
来源：http://tz.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://cg.9csxet.cn

[T60] Scala：折叠
来源：http://lh.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ba.gzmigu.cn

================================================================================
来源：http://bk.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cr.shxzukj.cn

================================================================================
来源：http://bh.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://ae.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cu.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://zn.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nm.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://aa.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://of.nicolike.cn

[U04] Py：变量调试打印
来源：http://py.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nn.nszjky.cn

[U05] Py：列表去重且保序
来源：http://vj.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://uf.newstarts.cn

[U06] Py：合并两个字典
来源：http://ej.shtwfgs.cn

{**a, **b}
来源：http://ki.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://yl.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://ml.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://cn.nicolike.cn

[y for x in nested for y in x]
来源：http://rv.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://vw.huanxung.cn

max(d, key=d.get)
来源：http://ch.lnxyls.cn

[U10] Py：按值排序字典
来源：http://ok.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ai.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://cp.chemitech.net.cn

(x * 2 for x in arr)
来源：http://sh.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://px.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://su.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ns.haigaiapp.cn

deque(maxlen=10)
来源：http://rm.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://ek.huixinmuqiang.cn

defaultdict(list)
来源：http://zm.huixiangedu.cn

[U15] Py：高精度计时
来源：http://yv.muxihuayi.cn

t = time.perf_counter()
来源：http://zw.hahajie.cn

[U16] Py：命令行参数解析
来源：http://kt.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nc.colortex.cn

[U17] Py：初始化日志
来源：http://gd.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://gi.nicolike.cn

[U18] Py：预编译正则
来源：http://gv.newstarts.cn

pat = re.compile(r"\d+")
来源：http://qs.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://lf.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lt.asd995.cn

[U20] Py：缓存函数结果
来源：http://ew.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://hg.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://tx.hahajie.cn

@contextlib.contextmanager
来源：http://gu.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://tz.huanxung.cn

list(zip(*m))
来源：http://zt.colortex.cn

[U23] Py：分块读取大文件
来源：http://ze.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mb.muxihuayi.cn

[U24] Py：路径操作
来源：http://ia.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ye.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://qz.bookmarksfly.cn

csv.DictReader(f)
来源：http://fb.panjiajie.cn

[U26] Py：并发下载
来源：http://af.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ik.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://yq.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://za.chemitech.net.cn

[U28] Py：类型别名
来源：http://fo.huanxung.cn

UserId = int
来源：http://xm.nicolike.cn

[U29] Py：属性校验
来源：http://kb.nszjky.cn

@property 与 @x.setter 配合
来源：http://jp.newstarts.cn

[U30] Py：数据类
来源：http://cm.chemitech.net.cn

@dataclass(slots=True)
来源：http://sf.chemitech.net.cn

[U31] Py：单测
来源：http://ej.haigaiapp.cn

python -m pytest -q
来源：http://to.hnjuh.cn

[U32] Py：代码格式化
来源：http://ep.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://np.huanxung.cn

[U33] Py：打包发布
来源：http://kh.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://cg.panjiajie.cn

[U34] Py：判断编码
来源：http://of.wgjwhj.cn

chardet.detect(raw)
来源：http://wa.nszjky.cn

[U35] Py：发送邮件
来源：http://no.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pc.nszjky.cn

[U36] Py：定时任务
来源：http://qz.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://xx.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://lc.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ww.521024.cn

[U38] Py：获取脚本所在目录
来源：http://fz.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://mg.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://rc.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://kk.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://yi.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://sn.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://he.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wn.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://ym.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pa.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://wq.nszjky.cn

namespace App\Http;
来源：http://md.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://dh.shtwfgs.cn

declare(strict_types=1);
来源：http://wi.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://rw.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vj.nszjky.cn

[U46] PHP：可空类型
来源：http://af.huanxung.cn

?string $name = null
来源：http://ch.shtwfgs.cn

[U47] PHP：联合类型
来源：http://hp.haigaiapp.cn

int|string $id
来源：http://ku.lnxyls.cn

[U48] PHP：纯枚举
来源：http://mg.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tt.asd995.cn

[U49] PHP：只读属性
来源：http://ba.jctech888.com.cn

public readonly string $name
来源：http://ds.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://uc.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://cl.lnxyls.cn

[U51] PHP：数组解构
来源：http://dl.colortex.cn

[$a, $b] = $arr;
来源：http://ez.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://om.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://br.newstarts.cn

[U53] PHP：空合并运算符
来源：http://bi.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://tg.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ap.shtwfgs.cn

$obj?->method()
来源：http://zs.521024.cn

[U55] PHP：match 表达式
来源：http://iu.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xf.wgjwhj.cn

[U56] PHP：命名参数
来源：http://co.haigaiapp.cn

f(a: 1, b: 2)
来源：http://cs.panjiajie.cn

[U57] PHP：字符串插值
来源：http://kg.nicolike.cn

"值: {$a}"
来源：http://zp.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://zc.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jz.gzmigu.cn

[U59] PHP：自定义排序
来源：http://mp.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zk.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://lf.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pf.chemitech.net.cn

[U61] PHP：正则
来源：http://ei.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ui.newstarts.cn

[U62] PHP：日期对象
来源：http://pe.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ps.chemitech.net.cn

[U63] PHP：文件读写
来源：http://wl.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kw.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://xv.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://db.yuntaijiaju.cn

[U65] PHP：会话
来源：http://ka.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qk.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://al.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zt.hahajie.cn

[U67] PHP：处理文件上传
来源：http://bw.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zh.colortex.cn

[U68] PHP：PDO 连接
来源：http://xq.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rv.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://rb.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qs.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://ph.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ys.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://ag.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://zn.lnxyls.cn

[U72] PHP：写错误日志
来源：http://ht.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://ny.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://pk.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://pa.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://ee.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://zt.asd995.cn

[U75] PHP：依赖注入
来源：http://fs.huanxung.cn

composer require psr/container
来源：http://wd.chemitech.net.cn

[U76] PHP：简单路由
来源：http://bx.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ke.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://jx.szsharing.cn

composer require twig/twig
来源：http://ij.hahajie.cn

[U78] PHP：单元测试
来源：http://pq.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://jh.newstarts.cn

[U79] PHP：静态分析
来源：http://vm.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://kw.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://it.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tj.lnxyls.cn

[U81] JS：初始化项目
来源：http://lt.shtwfgs.cn

npm init -y;  npm i express
来源：http://mo.9csxet.cn

[U82] JS：package.json 脚本
来源：http://ba.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ci.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://yo.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yk.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://ug.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ax.haigaiapp.cn

[U85] JS：可选链
来源：http://ri.shxzskj.cn

a?.b?.c
来源：http://no.chemitech.net.cn

[U86] JS：空值合并
来源：http://we.wgjwhj.cn

a ?? b
来源：http://zc.huanxung.cn

[U87] JS：解构默认值
来源：http://sq.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://ck.asd995.cn

[U88] JS：对象展开合并
来源：http://ze.panjiajie.cn

{ ...a, ...b }
来源：http://ii.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://be.9csxet.cn

[...new Set(arr)]
来源：http://ek.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://yf.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://fx.huanxung.cn

[U91] JS：对象键值遍历
来源：http://pv.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jb.szxytkj.cn

[U92] JS：深拷贝
来源：http://av.nicolike.cn

structuredClone(obj)
来源：http://zp.huixiangedu.cn

[U93] JS：模板字符串
来源：http://pl.yuexingan06.cn

`共 ${n} 条`
来源：http://xm.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://hg.muxihuayi.cn

const double = x => x * 2;
来源：http://qk.gzmigu.cn

[U95] JS：Promise 包装
来源：http://qp.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://oh.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://hb.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cp.nicolike.cn

[U97] JS：并发请求
来源：http://qy.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ec.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://bc.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mk.chemitech.net.cn

[U99] JS：事件监听
来源：http://qg.asd995.cn

el.addEventListener("click", e => {})
来源：http://hr.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://pk.lnxyls.cn

document.querySelector(".item")
来源：http://gb.9csxet.cn

[U101] JS：classList 操作
来源：http://wt.hnjuh.cn

el.classList.toggle("active")
来源：http://na.hahajie.cn

[U102] JS：本地存储
来源：http://xp.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xt.jctech888.com.cn

[U103] JS：定时器
来源：http://rg.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rb.nszjky.cn

[U104] JS：防抖
来源：http://gc.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ev.shtwfgs.cn

[U105] JS：节流
来源：http://vw.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oa.yuexingan06.cn

[U106] JS：日期格式化
来源：http://jp.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bg.lnxyls.cn

[U107] JS：数字千分位
来源：http://kk.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gr.szxytkj.cn

[U108] JS：随机整数
来源：http://qd.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://da.panjiajie.cn

[U109] JS：数组分组
来源：http://zz.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://yk.huixiangedu.cn

[U110] JS：数组分块
来源：http://lh.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hj.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://ab.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ri.colortex.cn

[U112] JS：字符串补位
来源：http://hy.wgjwhj.cn

"7".padStart(3, "0")
来源：http://ho.hahajie.cn

[U113] JS：正则替换全部
来源：http://ty.szsharing.cn

s.replaceAll("a", "b")
来源：http://de.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://zx.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tr.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://qv.hahajie.cn

crypto.randomUUID()
来源：http://im.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://mc.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://ds.panjiajie.cn

[U117] JS：单元测试
来源：http://sl.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://re.colortex.cn

[U118] JS：开发服务器
来源：http://og.lnxyls.cn

npm i -D vite;  npx vite
来源：http://ng.wgjwhj.cn

[U119] JS：生产构建
来源：http://ep.shxzskj.cn

npx vite build
来源：http://tw.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://ff.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://uq.huixiangedu.cn

================================================================================
来源：http://vr.9csxet.cn

统计汇总
来源：http://yo.wgjwhj.cn

================================================================================
来源：http://ws.yuexingan06.cn

按语言统计（条）：
来源：http://ui.yuexingan06.cn

Python ......... 252
来源：http://zr.bookmarksfly.cn

PHP ............ 252
来源：http://yf.yuntaijiaju.cn

JavaScript ..... 252
来源：http://co.521024.cn

TypeScript ..... 212
来源：http://re.jianghongdianzi.cn

Java ........... 212
来源：http://zd.bjjhwx.cn

Go ............. 212
来源：http://bf.nszjky.cn

Ruby ........... 212
来源：http://jo.wgjwhj.cn

C# ............. 212
来源：http://sd.jianghongdianzi.cn


<!-- 参考信息 -->