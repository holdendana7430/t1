代发 wailian999

[T41] Perl：Hello World
来源：http://ya.muxihuayi.cn

print "Hello\n";
来源：http://jz.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ux.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kl.huanxung.cn

[T43] Perl：字符串插值
来源：http://sq.asd995.cn

"值: $a"
来源：http://vw.nszjky.cn

[T44] Perl：条件
来源：http://lx.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://xg.hnjuh.cn

[T45] Perl：数组遍历
来源：http://qg.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://dr.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://gr.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fj.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://ox.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wb.szxytkj.cn

[T48] Perl：正则替换
来源：http://fg.gzmigu.cn

$s =~ s/old/new/g;
来源：http://iq.colortex.cn

[T49] Perl：函数
来源：http://ry.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://li.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://pe.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eb.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://an.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://jp.bjjhwx.cn

println("Hello")
来源：http://uw.asd995.cn

[T52] Scala：变量
来源：http://yw.shtwfgs.cn

val a = 1;  var b = 2
来源：http://wo.hnjuh.cn

[T53] Scala：字符串插值
来源：http://hx.521024.cn

s"值: $b"
来源：http://ng.colortex.cn

[T54] Scala：集合映射
来源：http://kl.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://hy.szsharing.cn

[T55] Scala：集合过滤
来源：http://hy.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mm.yuexingan06.cn

[T56] Scala：样例类
来源：http://zx.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://pb.szxytkj.cn

[T57] Scala：模式匹配
来源：http://gi.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tv.hnjuh.cn

[T58] Scala：函数定义
来源：http://ft.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ud.jianghongdianzi.cn

[T59] Scala：循环
来源：http://gw.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://vd.newstarts.cn

[T60] Scala：折叠
来源：http://lu.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fj.shtwfgs.cn

================================================================================
来源：http://cd.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zw.521024.cn

================================================================================
来源：http://sd.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://ob.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://us.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://qj.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tw.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://rl.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xu.521024.cn

[U04] Py：变量调试打印
来源：http://ak.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ao.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://dn.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://qp.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://sl.huanxung.cn

{**a, **b}
来源：http://uc.gzmigu.cn

[U07] Py：反转字典键值
来源：http://uq.nszjky.cn

{v: k for k, v in d.items()}
来源：http://mx.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ua.colortex.cn

[y for x in nested for y in x]
来源：http://qu.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://py.shxzskj.cn

max(d, key=d.get)
来源：http://zq.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://gm.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qg.panjiajie.cn

[U11] Py：生成器表达式
来源：http://ik.asd995.cn

(x * 2 for x in arr)
来源：http://li.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jw.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://rp.newstarts.cn

[U13] Py：固定长度队列
来源：http://ea.nszjky.cn

deque(maxlen=10)
来源：http://go.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://gl.jctech888.com.cn

defaultdict(list)
来源：http://yg.bjjhwx.cn

[U15] Py：高精度计时
来源：http://vz.panjiajie.cn

t = time.perf_counter()
来源：http://jg.nicolike.cn

[U16] Py：命令行参数解析
来源：http://op.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cw.szsharing.cn

[U17] Py：初始化日志
来源：http://qm.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://wh.szsharing.cn

[U18] Py：预编译正则
来源：http://tw.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://jt.521024.cn

[U19] Py：正则替换带回调
来源：http://yv.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ha.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://fk.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://lp.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://ll.bjjhwx.cn

@contextlib.contextmanager
来源：http://pn.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://fh.szsharing.cn

list(zip(*m))
来源：http://gn.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://hw.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eu.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ep.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ce.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://ae.szxytkj.cn

csv.DictReader(f)
来源：http://el.9csxet.cn

[U26] Py：并发下载
来源：http://ir.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vt.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://te.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ti.shxzukj.cn

[U28] Py：类型别名
来源：http://xx.nszjky.cn

UserId = int
来源：http://zp.521024.cn

[U29] Py：属性校验
来源：http://kh.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://nx.shxzskj.cn

[U30] Py：数据类
来源：http://hy.nicolike.cn

@dataclass(slots=True)
来源：http://yn.colortex.cn

[U31] Py：单测
来源：http://ak.shxzskj.cn

python -m pytest -q
来源：http://fm.jctech888.com.cn

[U32] Py：代码格式化
来源：http://mc.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://jl.bookmarksfly.cn

[U33] Py：打包发布
来源：http://ci.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://cm.wgjwhj.cn

[U34] Py：判断编码
来源：http://wt.wgjwhj.cn

chardet.detect(raw)
来源：http://mj.huixiangedu.cn

[U35] Py：发送邮件
来源：http://oy.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nj.chemitech.net.cn

[U36] Py：定时任务
来源：http://km.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://qf.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://hk.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ec.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://kl.szxytkj.cn

Path(__file__).resolve().parent
来源：http://hg.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://zu.bjjhwx.cn

sys.stdout.isatty()
来源：http://hj.nszjky.cn

[U40] Py：打印到标准错误
来源：http://im.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://zx.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://ji.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rn.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://zb.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vb.asd995.cn

[U43] PHP：声明命名空间
来源：http://xn.jctech888.com.cn

namespace App\Http;
来源：http://zr.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://vh.huanxung.cn

declare(strict_types=1);
来源：http://db.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://dd.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fj.shxzskj.cn

[U46] PHP：可空类型
来源：http://tx.gzmigu.cn

?string $name = null
来源：http://nz.chemitech.net.cn

[U47] PHP：联合类型
来源：http://bo.gzmigu.cn

int|string $id
来源：http://wf.hnjuh.cn

[U48] PHP：纯枚举
来源：http://nx.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zk.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://cu.szxytkj.cn

public readonly string $name
来源：http://lo.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://ey.panjiajie.cn

public function __construct(private int $id) {}
来源：http://nt.panjiajie.cn

[U51] PHP：数组解构
来源：http://er.nicolike.cn

[$a, $b] = $arr;
来源：http://ce.nszjky.cn

[U52] PHP：箭头函数
来源：http://bd.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://wu.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://dl.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://fp.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://rk.huixinmuqiang.cn

$obj?->method()
来源：http://ao.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://mx.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gz.jctech888.com.cn

[U56] PHP：命名参数
来源：http://zx.haigaiapp.cn

f(a: 1, b: 2)
来源：http://tt.newstarts.cn

[U57] PHP：字符串插值
来源：http://fc.521024.cn

"值: {$a}"
来源：http://ft.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://ln.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ux.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://yi.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ju.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://gj.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hv.wgjwhj.cn

[U61] PHP：正则
来源：http://aw.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bg.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ke.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cc.huanxung.cn

[U63] PHP：文件读写
来源：http://mn.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://he.nicolike.cn

[U64] PHP：目录遍历
来源：http://lf.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://md.jctech888.com.cn

[U65] PHP：会话
来源：http://kb.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vk.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://ip.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ea.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://uj.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xq.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://ak.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fv.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://kt.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qa.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://rj.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tj.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://dj.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://iw.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://fa.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://io.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://rh.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://tn.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://fu.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://jt.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://bs.gzmigu.cn

composer require psr/container
来源：http://dz.jctech888.com.cn

[U76] PHP：简单路由
来源：http://gq.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ic.szxytkj.cn

[U77] PHP：模板渲染
来源：http://gu.wgjwhj.cn

composer require twig/twig
来源：http://pv.haigaiapp.cn

[U78] PHP：单元测试
来源：http://vt.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://cq.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://rc.colortex.cn

composer require --dev phpstan/phpstan
来源：http://un.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://ua.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ka.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://su.shtwfgs.cn

npm init -y;  npm i express
来源：http://qj.9csxet.cn

[U82] JS：package.json 脚本
来源：http://tl.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ll.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://pp.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://me.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://wi.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ul.chemitech.net.cn

[U85] JS：可选链
来源：http://gc.hahajie.cn

a?.b?.c
来源：http://ug.521024.cn

[U86] JS：空值合并
来源：http://ee.gzmigu.cn

a ?? b
来源：http://nl.huixiangedu.cn

[U87] JS：解构默认值
来源：http://yb.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ae.nszjky.cn

[U88] JS：对象展开合并
来源：http://vo.muxihuayi.cn

{ ...a, ...b }
来源：http://vh.hnjuh.cn

[U89] JS：数组去重
来源：http://qx.gzmigu.cn

[...new Set(arr)]
来源：http://wx.gzmigu.cn

[U90] JS：数字数组排序
来源：http://zt.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://zf.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ip.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xu.newstarts.cn

[U92] JS：深拷贝
来源：http://wg.nszjky.cn

structuredClone(obj)
来源：http://kn.9csxet.cn

[U93] JS：模板字符串
来源：http://ef.nicolike.cn

`共 ${n} 条`
来源：http://yo.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://iw.wgjwhj.cn

const double = x => x * 2;
来源：http://nn.521024.cn

[U95] JS：Promise 包装
来源：http://up.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://ul.hahajie.cn

[U96] JS：async/await 与异常
来源：http://ti.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ha.shtwfgs.cn

[U97] JS：并发请求
来源：http://az.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ep.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://qm.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zy.huanxung.cn

[U99] JS：事件监听
来源：http://vb.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://mz.newstarts.cn

[U100] JS：DOM 查询
来源：http://lt.bookmarksfly.cn

document.querySelector(".item")
来源：http://wd.newstarts.cn

[U101] JS：classList 操作
来源：http://ng.lnxyls.cn

el.classList.toggle("active")
来源：http://ba.hnjuh.cn

[U102] JS：本地存储
来源：http://zj.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pw.huixiangedu.cn

[U103] JS：定时器
来源：http://xw.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://on.shxzskj.cn

[U104] JS：防抖
来源：http://se.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nj.chemitech.net.cn

[U105] JS：节流
来源：http://dj.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cp.gzmigu.cn

[U106] JS：日期格式化
来源：http://ca.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hl.huanxung.cn

[U107] JS：数字千分位
来源：http://uq.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gy.521024.cn

[U108] JS：随机整数
来源：http://ty.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wb.haigaiapp.cn

[U109] JS：数组分组
来源：http://hf.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://wa.huanxung.cn

[U110] JS：数组分块
来源：http://ob.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://he.nszjky.cn

[U111] JS：对象转 Map
来源：http://xg.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://oz.shtwfgs.cn

[U112] JS：字符串补位
来源：http://ds.shxzukj.cn

"7".padStart(3, "0")
来源：http://pi.shxzskj.cn

[U113] JS：正则替换全部
来源：http://lr.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://sv.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://yr.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uf.newstarts.cn

[U115] JS：生成 UUID
来源：http://ek.wgjwhj.cn

crypto.randomUUID()
来源：http://ov.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://hk.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://jh.szxytkj.cn

[U117] JS：单元测试
来源：http://jy.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://vn.colortex.cn

[U118] JS：开发服务器
来源：http://bc.gzmigu.cn

npm i -D vite;  npx vite
来源：http://tt.hahajie.cn

[U119] JS：生产构建
来源：http://qf.szsharing.cn

npx vite build
来源：http://mn.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://pk.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://uw.szxytkj.cn

================================================================================
来源：http://ad.yuntaijiaju.cn

统计汇总
来源：http://fl.lnxyls.cn

================================================================================
来源：http://jo.shxzukj.cn

按语言统计（条）：
来源：http://gs.chemitech.net.cn

Python ......... 252
来源：http://mw.colortex.cn

PHP ............ 252
来源：http://kh.gzmigu.cn

JavaScript ..... 252
来源：http://xq.521024.cn

TypeScript ..... 212
来源：http://zy.yuntaijiaju.cn

Java ........... 212
来源：http://pk.hnjuh.cn

Go ............. 212
来源：http://dm.szxytkj.cn

Ruby ........... 212
来源：http://ne.muxihuayi.cn

C# ............. 212
来源：http://uk.yuexingan06.cn

C .............. 30
来源：http://rm.huixiangedu.cn

C++ ............ 30
来源：http://tw.huixinmuqiang.cn

SQL ............ 90
来源：http://nm.huanxung.cn

Bash ........... 80
来源：http://mp.bookmarksfly.cn


<!-- 参考信息 -->