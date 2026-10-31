代发 wailian999

[T41] Perl：Hello World
来源：http://yx.gzmigu.cn

print "Hello\n";
来源：http://qu.jctech888.com.cn

[T42] Perl：变量类型
来源：http://oz.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://az.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://bw.521024.cn

"值: $a"
来源：http://xs.jctech888.com.cn

[T44] Perl：条件
来源：http://xb.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://sl.521024.cn

[T45] Perl：数组遍历
来源：http://ci.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://iv.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://kn.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xe.szxytkj.cn

[T47] Perl：正则捕获
来源：http://tg.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pc.gzmigu.cn

[T48] Perl：正则替换
来源：http://ml.9csxet.cn

$s =~ s/old/new/g;
来源：http://ql.521024.cn

[T49] Perl：函数
来源：http://hz.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yx.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://bd.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xz.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://qb.haigaiapp.cn

[T51] Scala：Hello World
来源：http://og.jctech888.com.cn

println("Hello")
来源：http://sq.9csxet.cn

[T52] Scala：变量
来源：http://ie.shtwfgs.cn

val a = 1;  var b = 2
来源：http://vf.521024.cn

[T53] Scala：字符串插值
来源：http://vo.muxihuayi.cn

s"值: $b"
来源：http://ea.lnxyls.cn

[T54] Scala：集合映射
来源：http://yz.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://hy.nszjky.cn

[T55] Scala：集合过滤
来源：http://th.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jd.chemitech.net.cn

[T56] Scala：样例类
来源：http://dn.521024.cn

case class User(name: String, age: Int)
来源：http://tg.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://mp.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ge.shxzukj.cn

[T58] Scala：函数定义
来源：http://qo.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qw.yuntaijiaju.cn

[T59] Scala：循环
来源：http://kn.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://oi.nicolike.cn

[T60] Scala：折叠
来源：http://mb.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vy.colortex.cn

================================================================================
来源：http://dd.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lb.9csxet.cn

================================================================================
来源：http://zh.521024.cn

[U01] Py：创建虚拟环境
来源：http://wk.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oc.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://gz.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wp.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://hn.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qp.gzmigu.cn

[U04] Py：变量调试打印
来源：http://zt.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vb.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://gm.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ou.521024.cn

[U06] Py：合并两个字典
来源：http://ro.bjjhwx.cn

{**a, **b}
来源：http://em.asd995.cn

[U07] Py：反转字典键值
来源：http://rn.szsharing.cn

{v: k for k, v in d.items()}
来源：http://qw.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://em.hnjuh.cn

[y for x in nested for y in x]
来源：http://xx.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://or.asd995.cn

max(d, key=d.get)
来源：http://jc.gzmigu.cn

[U10] Py：按值排序字典
来源：http://pq.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kk.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://qt.huixiangedu.cn

(x * 2 for x in arr)
来源：http://kj.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yo.lnxyls.cn

Counter(arr).most_common(3)
来源：http://jt.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://sj.9csxet.cn

deque(maxlen=10)
来源：http://lt.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://lb.521024.cn

defaultdict(list)
来源：http://ld.szsharing.cn

[U15] Py：高精度计时
来源：http://qr.bjjhwx.cn

t = time.perf_counter()
来源：http://dg.9csxet.cn

[U16] Py：命令行参数解析
来源：http://ii.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ge.hahajie.cn

[U17] Py：初始化日志
来源：http://ue.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zt.huanxung.cn

[U18] Py：预编译正则
来源：http://td.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://fr.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://qs.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xr.huanxung.cn

[U20] Py：缓存函数结果
来源：http://kf.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://kj.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://lo.gzmigu.cn

@contextlib.contextmanager
来源：http://qs.shxzskj.cn

[U22] Py：矩阵转置
来源：http://ms.wgjwhj.cn

list(zip(*m))
来源：http://qs.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://rq.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oa.muxihuayi.cn

[U24] Py：路径操作
来源：http://px.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qa.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://dn.huixinmuqiang.cn

csv.DictReader(f)
来源：http://gg.haigaiapp.cn

[U26] Py：并发下载
来源：http://pg.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uq.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://bj.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://hq.hahajie.cn

[U28] Py：类型别名
来源：http://si.haigaiapp.cn

UserId = int
来源：http://xj.shtwfgs.cn

[U29] Py：属性校验
来源：http://im.szxytkj.cn

@property 与 @x.setter 配合
来源：http://kt.szsharing.cn

[U30] Py：数据类
来源：http://ub.lnxyls.cn

@dataclass(slots=True)
来源：http://cg.chemitech.net.cn

[U31] Py：单测
来源：http://om.bjjhwx.cn

python -m pytest -q
来源：http://od.9csxet.cn

[U32] Py：代码格式化
来源：http://gx.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://da.szsharing.cn

[U33] Py：打包发布
来源：http://gi.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://vl.jctech888.com.cn

[U34] Py：判断编码
来源：http://zm.haigaiapp.cn

chardet.detect(raw)
来源：http://ky.nszjky.cn

[U35] Py：发送邮件
来源：http://zg.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pw.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://hk.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://fb.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ka.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cb.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://al.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://dq.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://au.yuexingan06.cn

sys.stdout.isatty()
来源：http://no.nszjky.cn

[U40] Py：打印到标准错误
来源：http://lh.gzmigu.cn

print("err", file=sys.stderr)
来源：http://to.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://gl.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dn.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://ev.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aa.szsharing.cn

[U43] PHP：声明命名空间
来源：http://hn.colortex.cn

namespace App\Http;
来源：http://qj.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://cq.wgjwhj.cn

declare(strict_types=1);
来源：http://sq.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://js.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uk.huixiangedu.cn

[U46] PHP：可空类型
来源：http://dx.bjjhwx.cn

?string $name = null
来源：http://jj.521024.cn

[U47] PHP：联合类型
来源：http://om.bjjhwx.cn

int|string $id
来源：http://co.lnxyls.cn

[U48] PHP：纯枚举
来源：http://ya.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wb.lnxyls.cn

[U49] PHP：只读属性
来源：http://in.huixinmuqiang.cn

public readonly string $name
来源：http://fz.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://ff.nicolike.cn

public function __construct(private int $id) {}
来源：http://vs.muxihuayi.cn

[U51] PHP：数组解构
来源：http://li.gzmigu.cn

[$a, $b] = $arr;
来源：http://no.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ir.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://jv.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://qg.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://bi.szsharing.cn

[U54] PHP：空安全调用
来源：http://sp.panjiajie.cn

$obj?->method()
来源：http://bp.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://wr.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dc.jctech888.com.cn

[U56] PHP：命名参数
来源：http://pw.szxytkj.cn

f(a: 1, b: 2)
来源：http://tv.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://xl.nszjky.cn

"值: {$a}"
来源：http://sj.nicolike.cn

[U58] PHP：数组三件套
来源：http://bg.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://us.shxzskj.cn

[U59] PHP：自定义排序
来源：http://wz.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sb.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://mj.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cs.huanxung.cn

[U61] PHP：正则
来源：http://sj.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pq.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://ge.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sw.shxzskj.cn

[U63] PHP：文件读写
来源：http://gt.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fw.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://ua.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://kg.jctech888.com.cn

[U65] PHP：会话
来源：http://md.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ch.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://uu.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tp.521024.cn

[U67] PHP：处理文件上传
来源：http://kh.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://af.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://oo.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kz.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://eh.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wx.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://bp.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://en.shxzukj.cn

[U71] PHP：抛出异常
来源：http://hh.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://th.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://eh.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://gh.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://bk.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://lw.newstarts.cn

[U74] PHP：读取环境变量
来源：http://ty.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://lf.panjiajie.cn

[U75] PHP：依赖注入
来源：http://yu.shxzskj.cn

composer require psr/container
来源：http://tk.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://jq.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://js.szxytkj.cn

[U77] PHP：模板渲染
来源：http://bb.huixiangedu.cn

composer require twig/twig
来源：http://fx.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://bh.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://jg.newstarts.cn

[U79] PHP：静态分析
来源：http://pq.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://cw.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://fv.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://la.szxytkj.cn

[U81] JS：初始化项目
来源：http://kt.newstarts.cn

npm init -y;  npm i express
来源：http://sx.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://zs.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ws.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://rj.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ac.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://qh.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qc.haigaiapp.cn

[U85] JS：可选链
来源：http://ve.colortex.cn

a?.b?.c
来源：http://ov.521024.cn

[U86] JS：空值合并
来源：http://mk.shxzskj.cn

a ?? b
来源：http://hc.nicolike.cn

[U87] JS：解构默认值
来源：http://sm.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://qj.nicolike.cn

[U88] JS：对象展开合并
来源：http://xr.hahajie.cn

{ ...a, ...b }
来源：http://mv.shtwfgs.cn

[U89] JS：数组去重
来源：http://ru.521024.cn

[...new Set(arr)]
来源：http://uz.newstarts.cn

[U90] JS：数字数组排序
来源：http://ee.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://dd.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://yj.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xe.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://fj.nszjky.cn

structuredClone(obj)
来源：http://pr.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ko.hahajie.cn

`共 ${n} 条`
来源：http://eg.lnxyls.cn

[U94] JS：箭头函数
来源：http://wn.wgjwhj.cn

const double = x => x * 2;
来源：http://cm.nicolike.cn

[U95] JS：Promise 包装
来源：http://of.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://cw.newstarts.cn

[U96] JS：async/await 与异常
来源：http://dd.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nh.huanxung.cn

[U97] JS：并发请求
来源：http://qf.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yd.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://wh.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ns.colortex.cn

[U99] JS：事件监听
来源：http://az.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://qb.shxzskj.cn

[U100] JS：DOM 查询
来源：http://pb.bookmarksfly.cn

document.querySelector(".item")
来源：http://pj.jctech888.com.cn

[U101] JS：classList 操作
来源：http://ry.bjjhwx.cn

el.classList.toggle("active")
来源：http://yx.shtwfgs.cn

[U102] JS：本地存储
来源：http://lf.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mi.huixinmuqiang.cn

[U103] JS：定时器
来源：http://wx.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iy.gzmigu.cn

[U104] JS：防抖
来源：http://iv.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kb.lnxyls.cn

[U105] JS：节流
来源：http://vc.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kc.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://vc.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vr.szsharing.cn

[U107] JS：数字千分位
来源：http://ew.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ua.9csxet.cn

[U108] JS：随机整数
来源：http://ml.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yt.chemitech.net.cn

[U109] JS：数组分组
来源：http://fy.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://il.wgjwhj.cn

[U110] JS：数组分块
来源：http://zp.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ft.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://xk.lnxyls.cn

new Map(Object.entries(obj))
来源：http://np.nszjky.cn

[U112] JS：字符串补位
来源：http://zu.szsharing.cn

"7".padStart(3, "0")
来源：http://bn.asd995.cn

[U113] JS：正则替换全部
来源：http://vx.lnxyls.cn

s.replaceAll("a", "b")
来源：http://zo.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://uo.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nt.shxzukj.cn

[U115] JS：生成 UUID
来源：http://zm.gzmigu.cn

crypto.randomUUID()
来源：http://zv.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ur.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://on.asd995.cn

[U117] JS：单元测试
来源：http://le.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://nr.szsharing.cn

[U118] JS：开发服务器
来源：http://nf.asd995.cn

npm i -D vite;  npx vite
来源：http://ya.hahajie.cn

[U119] JS：生产构建
来源：http://bl.yuexingan06.cn

npx vite build
来源：http://mt.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://oo.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://ey.gzmigu.cn

================================================================================
来源：http://km.huixinmuqiang.cn

统计汇总
来源：http://ts.gzmigu.cn

================================================================================
来源：http://xs.521024.cn

按语言统计（条）：
来源：http://cx.huanxung.cn

Python ......... 252
来源：http://mx.colortex.cn

PHP ............ 252
来源：http://gh.panjiajie.cn

JavaScript ..... 252
来源：http://ks.szsharing.cn

TypeScript ..... 212
来源：http://ap.shxzskj.cn

Java ........... 212
来源：http://dj.huixiangedu.cn

Go ............. 212
来源：http://wi.gzmigu.cn

Ruby ........... 212
来源：http://aj.bookmarksfly.cn

C# ............. 212
来源：http://dj.muxihuayi.cn

C .............. 30
来源：http://hw.9csxet.cn

C++ ............ 30
来源：http://xr.colortex.cn

SQL ............ 90
来源：http://ws.yuntaijiaju.cn

Bash ........... 80
来源：http://jt.szxytkj.cn


<!-- 参考信息 -->