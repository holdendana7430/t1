代发 wailian999

[T41] Perl：Hello World
来源：http://aj.nszjky.cn

print "Hello\n";
来源：http://dr.shxzukj.cn

[T42] Perl：变量类型
来源：http://ve.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fm.szsharing.cn

[T43] Perl：字符串插值
来源：http://kw.szsharing.cn

"值: $a"
来源：http://xr.huixinmuqiang.cn

[T44] Perl：条件
来源：http://fk.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://he.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://qp.colortex.cn

for my $x (@arr) { print $x; }
来源：http://mg.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://nm.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cw.colortex.cn

[T47] Perl：正则捕获
来源：http://ko.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wu.colortex.cn

[T48] Perl：正则替换
来源：http://ml.lnxyls.cn

$s =~ s/old/new/g;
来源：http://ta.jctech888.com.cn

[T49] Perl：函数
来源：http://hu.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ro.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://gi.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mr.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://fg.asd995.cn

[T51] Scala：Hello World
来源：http://xu.colortex.cn

println("Hello")
来源：http://uw.yuexingan06.cn

[T52] Scala：变量
来源：http://lf.shxzskj.cn

val a = 1;  var b = 2
来源：http://bd.gzmigu.cn

[T53] Scala：字符串插值
来源：http://gm.huanxung.cn

s"值: $b"
来源：http://fu.colortex.cn

[T54] Scala：集合映射
来源：http://bl.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://nk.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://pb.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ll.shtwfgs.cn

[T56] Scala：样例类
来源：http://xi.newstarts.cn

case class User(name: String, age: Int)
来源：http://su.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://oy.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://be.yuexingan06.cn

[T58] Scala：函数定义
来源：http://yn.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pd.huixiangedu.cn

[T59] Scala：循环
来源：http://pb.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://jc.gzmigu.cn

[T60] Scala：折叠
来源：http://ih.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mo.nszjky.cn

================================================================================
来源：http://hd.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ot.9csxet.cn

================================================================================
来源：http://yx.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://hv.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dt.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://hx.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lt.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://uh.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sw.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://np.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fx.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://yh.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://eo.asd995.cn

[U06] Py：合并两个字典
来源：http://nr.haigaiapp.cn

{**a, **b}
来源：http://tz.9csxet.cn

[U07] Py：反转字典键值
来源：http://nb.newstarts.cn

{v: k for k, v in d.items()}
来源：http://kz.shxzskj.cn

[U08] Py：展平二维列表
来源：http://hs.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://ia.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://iy.shxzskj.cn

max(d, key=d.get)
来源：http://ud.lnxyls.cn

[U10] Py：按值排序字典
来源：http://jx.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kz.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://yw.haigaiapp.cn

(x * 2 for x in arr)
来源：http://ft.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nj.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://yz.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://wz.asd995.cn

deque(maxlen=10)
来源：http://oa.huanxung.cn

[U14] Py：分组收集到列表
来源：http://dq.gzmigu.cn

defaultdict(list)
来源：http://xl.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://gw.jianghongdianzi.cn

t = time.perf_counter()
来源：http://dv.newstarts.cn

[U16] Py：命令行参数解析
来源：http://vn.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ux.szxytkj.cn

[U17] Py：初始化日志
来源：http://tq.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://qe.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://zk.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ah.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://uo.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uf.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://lc.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://cx.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://pa.szsharing.cn

@contextlib.contextmanager
来源：http://yi.huanxung.cn

[U22] Py：矩阵转置
来源：http://xz.wgjwhj.cn

list(zip(*m))
来源：http://dj.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://gn.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ny.huanxung.cn

[U24] Py：路径操作
来源：http://yw.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ic.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://xz.shtwfgs.cn

csv.DictReader(f)
来源：http://eh.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://xj.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bx.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://gs.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://om.panjiajie.cn

[U28] Py：类型别名
来源：http://dw.asd995.cn

UserId = int
来源：http://ar.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://lu.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://gm.nicolike.cn

[U30] Py：数据类
来源：http://yq.nszjky.cn

@dataclass(slots=True)
来源：http://pk.huixinmuqiang.cn

[U31] Py：单测
来源：http://ul.hahajie.cn

python -m pytest -q
来源：http://tt.nicolike.cn

[U32] Py：代码格式化
来源：http://bs.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://cv.haigaiapp.cn

[U33] Py：打包发布
来源：http://vn.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://ei.newstarts.cn

[U34] Py：判断编码
来源：http://ue.huanxung.cn

chardet.detect(raw)
来源：http://mz.huanxung.cn

[U35] Py：发送邮件
来源：http://tc.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://to.szxytkj.cn

[U36] Py：定时任务
来源：http://to.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://nh.asd995.cn

[U37] Py：读写 Excel
来源：http://yl.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zx.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ts.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://rp.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://ix.shxzskj.cn

sys.stdout.isatty()
来源：http://aw.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://jd.szxytkj.cn

print("err", file=sys.stderr)
来源：http://xs.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://vg.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bb.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://mq.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xh.nicolike.cn

[U43] PHP：声明命名空间
来源：http://wt.hnjuh.cn

namespace App\Http;
来源：http://cv.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://bw.nszjky.cn

declare(strict_types=1);
来源：http://ep.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://at.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dk.shxzukj.cn

[U46] PHP：可空类型
来源：http://of.nszjky.cn

?string $name = null
来源：http://ul.panjiajie.cn

[U47] PHP：联合类型
来源：http://ps.shxzukj.cn

int|string $id
来源：http://jr.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://bs.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pk.nszjky.cn

[U49] PHP：只读属性
来源：http://kn.521024.cn

public readonly string $name
来源：http://xr.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://fs.shxzukj.cn

public function __construct(private int $id) {}
来源：http://xm.hahajie.cn

[U51] PHP：数组解构
来源：http://fn.hnjuh.cn

[$a, $b] = $arr;
来源：http://mt.nszjky.cn

[U52] PHP：箭头函数
来源：http://mz.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://it.hahajie.cn

[U53] PHP：空合并运算符
来源：http://gr.521024.cn

$v = $a ?? $b ?? "default";
来源：http://gq.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://wy.gzmigu.cn

$obj?->method()
来源：http://es.panjiajie.cn

[U55] PHP：match 表达式
来源：http://ju.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dy.nszjky.cn

[U56] PHP：命名参数
来源：http://an.hahajie.cn

f(a: 1, b: 2)
来源：http://hu.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://nn.gzmigu.cn

"值: {$a}"
来源：http://im.nicolike.cn

[U58] PHP：数组三件套
来源：http://se.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qx.colortex.cn

[U59] PHP：自定义排序
来源：http://cg.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jd.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://nc.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qz.szxytkj.cn

[U61] PHP：正则
来源：http://da.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lp.nszjky.cn

[U62] PHP：日期对象
来源：http://pq.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yr.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://lb.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hx.shxzukj.cn

[U64] PHP：目录遍历
来源：http://oe.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://gr.9csxet.cn

[U65] PHP：会话
来源：http://zz.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bw.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://jg.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gt.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://oz.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rg.nicolike.cn

[U68] PHP：PDO 连接
来源：http://hf.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ct.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://cb.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://og.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://rg.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ld.nszjky.cn

[U71] PHP：抛出异常
来源：http://oa.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://ps.panjiajie.cn

[U72] PHP：写错误日志
来源：http://zw.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ms.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://nb.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://ym.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://sc.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://rp.colortex.cn

[U75] PHP：依赖注入
来源：http://xb.shtwfgs.cn

composer require psr/container
来源：http://qc.szxytkj.cn

[U76] PHP：简单路由
来源：http://ep.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ys.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://qg.9csxet.cn

composer require twig/twig
来源：http://hm.muxihuayi.cn

[U78] PHP：单元测试
来源：http://sb.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://xk.huanxung.cn

[U79] PHP：静态分析
来源：http://av.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://pe.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://qm.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sw.wgjwhj.cn

[U81] JS：初始化项目
来源：http://jl.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://er.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://uk.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ir.521024.cn

[U83] JS：ES Module 导入导出
来源：http://tu.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iu.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://co.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gf.shxzskj.cn

[U85] JS：可选链
来源：http://ce.szsharing.cn

a?.b?.c
来源：http://uh.panjiajie.cn

[U86] JS：空值合并
来源：http://ka.yuntaijiaju.cn

a ?? b
来源：http://dp.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://oa.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://te.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://rs.asd995.cn

{ ...a, ...b }
来源：http://cb.nicolike.cn

[U89] JS：数组去重
来源：http://xw.shxzskj.cn

[...new Set(arr)]
来源：http://pl.newstarts.cn

[U90] JS：数字数组排序
来源：http://vj.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://xr.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://ah.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vl.hahajie.cn

[U92] JS：深拷贝
来源：http://mp.yuntaijiaju.cn

structuredClone(obj)
来源：http://yy.gzmigu.cn

[U93] JS：模板字符串
来源：http://pq.huixiangedu.cn

`共 ${n} 条`
来源：http://bw.bjjhwx.cn

[U94] JS：箭头函数
来源：http://vq.szxytkj.cn

const double = x => x * 2;
来源：http://eg.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://vc.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://si.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://ri.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yj.hahajie.cn

[U97] JS：并发请求
来源：http://qp.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mx.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://pp.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eb.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://si.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://cj.hahajie.cn

[U100] JS：DOM 查询
来源：http://jk.panjiajie.cn

document.querySelector(".item")
来源：http://ew.521024.cn

[U101] JS：classList 操作
来源：http://qy.szxytkj.cn

el.classList.toggle("active")
来源：http://he.shxzskj.cn

[U102] JS：本地存储
来源：http://at.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oq.szxytkj.cn

[U103] JS：定时器
来源：http://bg.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mb.newstarts.cn

[U104] JS：防抖
来源：http://jz.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yf.bookmarksfly.cn

[U105] JS：节流
来源：http://hq.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sg.szxytkj.cn

[U106] JS：日期格式化
来源：http://rh.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oz.lnxyls.cn

[U107] JS：数字千分位
来源：http://sf.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wo.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://tx.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://st.colortex.cn

[U109] JS：数组分组
来源：http://oa.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://rl.shxzukj.cn

[U110] JS：数组分块
来源：http://uw.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ds.nicolike.cn

[U111] JS：对象转 Map
来源：http://uf.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://gz.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://ym.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://mp.colortex.cn

[U113] JS：正则替换全部
来源：http://iw.panjiajie.cn

s.replaceAll("a", "b")
来源：http://bt.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://fa.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vx.hnjuh.cn

[U115] JS：生成 UUID
来源：http://qc.panjiajie.cn

crypto.randomUUID()
来源：http://qy.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ap.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://cj.asd995.cn

[U117] JS：单元测试
来源：http://ll.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://vr.nicolike.cn

[U118] JS：开发服务器
来源：http://tg.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://dn.shxzskj.cn

[U119] JS：生产构建
来源：http://fm.wgjwhj.cn

npx vite build
来源：http://uk.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://xr.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://dn.lnxyls.cn

================================================================================
来源：http://td.shxzskj.cn

统计汇总
来源：http://pt.shxzskj.cn

================================================================================
来源：http://un.yuntaijiaju.cn

按语言统计（条）：
来源：http://fo.nszjky.cn

Python ......... 252
来源：http://wr.jctech888.com.cn

PHP ............ 252
来源：http://ev.9csxet.cn

JavaScript ..... 252
来源：http://rf.huanxung.cn

TypeScript ..... 212
来源：http://hb.haigaiapp.cn

Java ........... 212
来源：http://vw.shxzskj.cn

Go ............. 212
来源：http://uq.szsharing.cn

Ruby ........... 212
来源：http://og.panjiajie.cn

C# ............. 212
来源：http://gn.colortex.cn

C .............. 30
来源：http://vb.huixinmuqiang.cn

C++ ............ 30
来源：http://kj.hnjuh.cn

SQL ............ 90
来源：http://ae.szsharing.cn

Bash ........... 80
来源：http://sy.muxihuayi.cn


<!-- 参考信息 -->