代发 wailian999

[T35] Lua：字典表
来源：http://hf.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://yk.9csxet.cn

[T36] Lua：函数
来源：http://bu.muxihuayi.cn

function add(a, b) return a + b end
来源：http://pf.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://pt.asd995.cn

"a" .. "b"
来源：http://za.9csxet.cn

[T38] Lua：条件
来源：http://ga.asd995.cn

if x > 0 then print("正") end
来源：http://nn.szsharing.cn

[T39] Lua：模式匹配
来源：http://mh.hahajie.cn

string.find(s, "%d+")
来源：http://gk.colortex.cn

[T40] Lua：元表
来源：http://tl.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://jw.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://bn.chemitech.net.cn

print "Hello\n";
来源：http://lh.hnjuh.cn

[T42] Perl：变量类型
来源：http://uz.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nq.huanxung.cn

[T43] Perl：字符串插值
来源：http://tt.bjjhwx.cn

"值: $a"
来源：http://uu.nszjky.cn

[T44] Perl：条件
来源：http://tw.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://wi.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://jx.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://br.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://ib.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://al.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ea.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cq.gzmigu.cn

[T48] Perl：正则替换
来源：http://sh.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://or.nszjky.cn

[T49] Perl：函数
来源：http://qp.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cn.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://ff.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lq.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://bo.panjiajie.cn

[T51] Scala：Hello World
来源：http://lh.huixinmuqiang.cn

println("Hello")
来源：http://nh.huixinmuqiang.cn

[T52] Scala：变量
来源：http://hp.shxzukj.cn

val a = 1;  var b = 2
来源：http://rj.hahajie.cn

[T53] Scala：字符串插值
来源：http://xy.yuntaijiaju.cn

s"值: $b"
来源：http://nm.muxihuayi.cn

[T54] Scala：集合映射
来源：http://gj.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://td.szxytkj.cn

[T55] Scala：集合过滤
来源：http://rn.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jw.bjjhwx.cn

[T56] Scala：样例类
来源：http://rl.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://uf.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://dg.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dx.huixiangedu.cn

[T58] Scala：函数定义
来源：http://wx.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jy.asd995.cn

[T59] Scala：循环
来源：http://pu.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://wr.shxzukj.cn

[T60] Scala：折叠
来源：http://qo.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lr.huixiangedu.cn

================================================================================
来源：http://pw.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://is.9csxet.cn

================================================================================
来源：http://ic.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://sj.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vt.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://cd.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zn.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://tv.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qh.hahajie.cn

[U04] Py：变量调试打印
来源：http://zg.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mw.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://ew.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://kp.lnxyls.cn

[U06] Py：合并两个字典
来源：http://fa.bookmarksfly.cn

{**a, **b}
来源：http://cm.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://bo.nicolike.cn

{v: k for k, v in d.items()}
来源：http://ww.shxzukj.cn

[U08] Py：展平二维列表
来源：http://pg.haigaiapp.cn

[y for x in nested for y in x]
来源：http://df.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://st.huixiangedu.cn

max(d, key=d.get)
来源：http://wv.nicolike.cn

[U10] Py：按值排序字典
来源：http://fh.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yd.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://ay.521024.cn

(x * 2 for x in arr)
来源：http://kb.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ej.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://xs.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://ze.lnxyls.cn

deque(maxlen=10)
来源：http://ik.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ym.shtwfgs.cn

defaultdict(list)
来源：http://rx.shxzskj.cn

[U15] Py：高精度计时
来源：http://wn.szsharing.cn

t = time.perf_counter()
来源：http://xd.nicolike.cn

[U16] Py：命令行参数解析
来源：http://ex.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ut.jctech888.com.cn

[U17] Py：初始化日志
来源：http://xy.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ug.asd995.cn

[U18] Py：预编译正则
来源：http://jh.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://ak.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://dq.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://re.9csxet.cn

[U20] Py：缓存函数结果
来源：http://wh.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://ij.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://mq.szsharing.cn

@contextlib.contextmanager
来源：http://br.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://pk.9csxet.cn

list(zip(*m))
来源：http://qg.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://bk.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qj.521024.cn

[U24] Py：路径操作
来源：http://ou.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yy.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://mt.lnxyls.cn

csv.DictReader(f)
来源：http://bw.9csxet.cn

[U26] Py：并发下载
来源：http://nx.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vn.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://gy.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://wa.huanxung.cn

[U28] Py：类型别名
来源：http://xm.yuntaijiaju.cn

UserId = int
来源：http://tn.bookmarksfly.cn

[U29] Py：属性校验
来源：http://hw.szsharing.cn

@property 与 @x.setter 配合
来源：http://is.yuexingan06.cn

[U30] Py：数据类
来源：http://ib.gzmigu.cn

@dataclass(slots=True)
来源：http://cj.shtwfgs.cn

[U31] Py：单测
来源：http://qo.haigaiapp.cn

python -m pytest -q
来源：http://pr.9csxet.cn

[U32] Py：代码格式化
来源：http://gu.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://zx.hahajie.cn

[U33] Py：打包发布
来源：http://bm.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://ks.hnjuh.cn

[U34] Py：判断编码
来源：http://xf.hnjuh.cn

chardet.detect(raw)
来源：http://hb.nicolike.cn

[U35] Py：发送邮件
来源：http://ib.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ja.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://mp.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://ca.panjiajie.cn

[U37] Py：读写 Excel
来源：http://nv.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vz.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://hc.panjiajie.cn

Path(__file__).resolve().parent
来源：http://gx.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://hy.hahajie.cn

sys.stdout.isatty()
来源：http://qu.colortex.cn

[U40] Py：打印到标准错误
来源：http://yc.colortex.cn

print("err", file=sys.stderr)
来源：http://po.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://eu.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ya.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://vc.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mi.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://sf.hnjuh.cn

namespace App\Http;
来源：http://ny.szsharing.cn

[U44] PHP：开启严格类型
来源：http://vs.shxzukj.cn

declare(strict_types=1);
来源：http://sx.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://ms.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jo.wgjwhj.cn

[U46] PHP：可空类型
来源：http://tw.chemitech.net.cn

?string $name = null
来源：http://tc.huixiangedu.cn

[U47] PHP：联合类型
来源：http://sq.panjiajie.cn

int|string $id
来源：http://fv.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://qp.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uw.wgjwhj.cn

[U49] PHP：只读属性
来源：http://eh.huixiangedu.cn

public readonly string $name
来源：http://xy.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://wu.asd995.cn

public function __construct(private int $id) {}
来源：http://ou.asd995.cn

[U51] PHP：数组解构
来源：http://ss.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://lj.szxytkj.cn

[U52] PHP：箭头函数
来源：http://ma.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://bg.521024.cn

[U53] PHP：空合并运算符
来源：http://zw.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://ia.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://gr.shxzskj.cn

$obj?->method()
来源：http://vq.521024.cn

[U55] PHP：match 表达式
来源：http://jo.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ta.gzmigu.cn

[U56] PHP：命名参数
来源：http://ox.shxzukj.cn

f(a: 1, b: 2)
来源：http://yx.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://na.shxzukj.cn

"值: {$a}"
来源：http://oi.gzmigu.cn

[U58] PHP：数组三件套
来源：http://lb.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uk.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://yp.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mt.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://mo.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://on.hahajie.cn

[U61] PHP：正则
来源：http://gz.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cz.asd995.cn

[U62] PHP：日期对象
来源：http://qh.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xc.huanxung.cn

[U63] PHP：文件读写
来源：http://pe.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tk.szsharing.cn

[U64] PHP：目录遍历
来源：http://cw.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://gb.chemitech.net.cn

[U65] PHP：会话
来源：http://tf.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vs.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://ei.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lt.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://rq.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wv.9csxet.cn

[U68] PHP：PDO 连接
来源：http://xx.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ps.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://xa.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ww.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://lh.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wl.lnxyls.cn

[U71] PHP：抛出异常
来源：http://pq.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://oy.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://gz.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://ig.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://tu.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://bu.nszjky.cn

[U74] PHP：读取环境变量
来源：http://nx.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://tv.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://kf.chemitech.net.cn

composer require psr/container
来源：http://ta.bjjhwx.cn

[U76] PHP：简单路由
来源：http://lf.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eb.gzmigu.cn

[U77] PHP：模板渲染
来源：http://qz.haigaiapp.cn

composer require twig/twig
来源：http://td.nicolike.cn

[U78] PHP：单元测试
来源：http://rg.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://wx.nszjky.cn

[U79] PHP：静态分析
来源：http://pk.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://hg.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://rr.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kt.szsharing.cn

[U81] JS：初始化项目
来源：http://ei.shxzskj.cn

npm init -y;  npm i express
来源：http://yp.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://ds.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oe.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://iw.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qm.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://nf.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://io.huixiangedu.cn

[U85] JS：可选链
来源：http://uf.bjjhwx.cn

a?.b?.c
来源：http://pz.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://pj.muxihuayi.cn

a ?? b
来源：http://ca.asd995.cn

[U87] JS：解构默认值
来源：http://pr.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://aa.szxytkj.cn

[U88] JS：对象展开合并
来源：http://bw.hnjuh.cn

{ ...a, ...b }
来源：http://jy.shxzskj.cn

[U89] JS：数组去重
来源：http://ps.huixinmuqiang.cn

[...new Set(arr)]
来源：http://il.gzmigu.cn

[U90] JS：数字数组排序
来源：http://yo.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://fw.hahajie.cn

[U91] JS：对象键值遍历
来源：http://qv.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ko.panjiajie.cn

[U92] JS：深拷贝
来源：http://hy.bookmarksfly.cn

structuredClone(obj)
来源：http://ys.nszjky.cn

[U93] JS：模板字符串
来源：http://kk.newstarts.cn

`共 ${n} 条`
来源：http://wh.chemitech.net.cn

[U94] JS：箭头函数
来源：http://sf.yuexingan06.cn

const double = x => x * 2;
来源：http://dw.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://cy.asd995.cn

new Promise((resolve, reject) => {})
来源：http://ub.hahajie.cn

[U96] JS：async/await 与异常
来源：http://kj.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vt.nicolike.cn

[U97] JS：并发请求
来源：http://qa.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sd.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://xs.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hb.bjjhwx.cn

[U99] JS：事件监听
来源：http://jy.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://kk.asd995.cn

[U100] JS：DOM 查询
来源：http://nm.chemitech.net.cn

document.querySelector(".item")
来源：http://fy.shtwfgs.cn

[U101] JS：classList 操作
来源：http://jz.hahajie.cn

el.classList.toggle("active")
来源：http://bt.yuexingan06.cn

[U102] JS：本地存储
来源：http://pn.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nw.chemitech.net.cn

[U103] JS：定时器
来源：http://zh.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ah.hnjuh.cn

[U104] JS：防抖
来源：http://nf.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xa.shtwfgs.cn

[U105] JS：节流
来源：http://ve.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bz.szxytkj.cn

[U106] JS：日期格式化
来源：http://nj.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rx.hnjuh.cn

[U107] JS：数字千分位
来源：http://xi.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ci.nszjky.cn

[U108] JS：随机整数
来源：http://kg.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://av.huixiangedu.cn

[U109] JS：数组分组
来源：http://ov.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://cp.gzmigu.cn

[U110] JS：数组分块
来源：http://cw.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ve.szxytkj.cn

[U111] JS：对象转 Map
来源：http://is.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://lh.asd995.cn

[U112] JS：字符串补位
来源：http://ds.szxytkj.cn

"7".padStart(3, "0")
来源：http://yc.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://jr.colortex.cn

s.replaceAll("a", "b")
来源：http://bi.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://km.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vj.asd995.cn

[U115] JS：生成 UUID
来源：http://fx.shtwfgs.cn

crypto.randomUUID()
来源：http://mf.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://yv.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://uk.bookmarksfly.cn

[U117] JS：单元测试
来源：http://qm.521024.cn

npm i -D vitest;  npx vitest
来源：http://nq.521024.cn

[U118] JS：开发服务器
来源：http://en.lnxyls.cn

npm i -D vite;  npx vite
来源：http://nf.hnjuh.cn

[U119] JS：生产构建
来源：http://vo.huixiangedu.cn

npx vite build
来源：http://nc.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://hi.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://lc.haigaiapp.cn

================================================================================
来源：http://ol.gzmigu.cn

统计汇总
来源：http://ps.gzmigu.cn

================================================================================
来源：http://fh.huixiangedu.cn

按语言统计（条）：
来源：http://hk.colortex.cn


<!-- 参考信息 -->