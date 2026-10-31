代发 wailian999

[T35] Lua：字典表
来源：http://id.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://za.shtwfgs.cn

[T36] Lua：函数
来源：http://pr.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://nw.nszjky.cn

[T37] Lua：字符串拼接
来源：http://wa.szxytkj.cn

"a" .. "b"
来源：http://yq.szxytkj.cn

[T38] Lua：条件
来源：http://cf.chemitech.net.cn

if x > 0 then print("正") end
来源：http://ge.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://rk.shtwfgs.cn

string.find(s, "%d+")
来源：http://jy.hnjuh.cn

[T40] Lua：元表
来源：http://tf.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://ya.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://jy.huixinmuqiang.cn

print "Hello\n";
来源：http://mn.colortex.cn

[T42] Perl：变量类型
来源：http://sn.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nd.szxytkj.cn

[T43] Perl：字符串插值
来源：http://dz.haigaiapp.cn

"值: $a"
来源：http://de.jianghongdianzi.cn

[T44] Perl：条件
来源：http://vs.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://pk.nszjky.cn

[T45] Perl：数组遍历
来源：http://tu.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://nz.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ga.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nv.hahajie.cn

[T47] Perl：正则捕获
来源：http://pq.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cj.szxytkj.cn

[T48] Perl：正则替换
来源：http://lh.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://iu.asd995.cn

[T49] Perl：函数
来源：http://hf.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qj.nicolike.cn

[T50] Perl：逐行读文件
来源：http://xs.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://on.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ar.hahajie.cn

[T51] Scala：Hello World
来源：http://sy.9csxet.cn

println("Hello")
来源：http://uc.haigaiapp.cn

[T52] Scala：变量
来源：http://qb.panjiajie.cn

val a = 1;  var b = 2
来源：http://ud.colortex.cn

[T53] Scala：字符串插值
来源：http://ig.panjiajie.cn

s"值: $b"
来源：http://fa.newstarts.cn

[T54] Scala：集合映射
来源：http://yr.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://nw.szxytkj.cn

[T55] Scala：集合过滤
来源：http://cw.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://as.lnxyls.cn

[T56] Scala：样例类
来源：http://wk.hahajie.cn

case class User(name: String, age: Int)
来源：http://yb.shxzskj.cn

[T57] Scala：模式匹配
来源：http://bh.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kq.huanxung.cn

[T58] Scala：函数定义
来源：http://iv.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ho.huixiangedu.cn

[T59] Scala：循环
来源：http://fo.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://yq.bookmarksfly.cn

[T60] Scala：折叠
来源：http://in.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sl.shxzukj.cn

================================================================================
来源：http://pb.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bb.colortex.cn

================================================================================
来源：http://ya.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://yl.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bk.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://ho.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uw.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://mu.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fq.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://vn.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iq.9csxet.cn

[U05] Py：列表去重且保序
来源：http://xa.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://ce.shxzskj.cn

[U06] Py：合并两个字典
来源：http://of.nszjky.cn

{**a, **b}
来源：http://br.szxytkj.cn

[U07] Py：反转字典键值
来源：http://mo.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://jj.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://kw.hnjuh.cn

[y for x in nested for y in x]
来源：http://lg.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://nm.shtwfgs.cn

max(d, key=d.get)
来源：http://lh.gzmigu.cn

[U10] Py：按值排序字典
来源：http://vc.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xp.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://cr.521024.cn

(x * 2 for x in arr)
来源：http://ir.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ei.521024.cn

Counter(arr).most_common(3)
来源：http://rt.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://bg.newstarts.cn

deque(maxlen=10)
来源：http://gx.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://gv.yuntaijiaju.cn

defaultdict(list)
来源：http://pu.wgjwhj.cn

[U15] Py：高精度计时
来源：http://pr.nszjky.cn

t = time.perf_counter()
来源：http://mp.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://zf.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vg.asd995.cn

[U17] Py：初始化日志
来源：http://gt.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://nd.shxzskj.cn

[U18] Py：预编译正则
来源：http://sm.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://em.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://em.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cj.nszjky.cn

[U20] Py：缓存函数结果
来源：http://ur.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://mr.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://hh.hnjuh.cn

@contextlib.contextmanager
来源：http://cj.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://rx.szxytkj.cn

list(zip(*m))
来源：http://ht.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://fd.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wl.521024.cn

[U24] Py：路径操作
来源：http://nh.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vo.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://oa.newstarts.cn

csv.DictReader(f)
来源：http://kl.nszjky.cn

[U26] Py：并发下载
来源：http://ug.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gf.hahajie.cn

[U27] Py：异步 HTTP
来源：http://bm.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uj.muxihuayi.cn

[U28] Py：类型别名
来源：http://hl.newstarts.cn

UserId = int
来源：http://ba.jctech888.com.cn

[U29] Py：属性校验
来源：http://bf.gzmigu.cn

@property 与 @x.setter 配合
来源：http://wa.lnxyls.cn

[U30] Py：数据类
来源：http://bi.wgjwhj.cn

@dataclass(slots=True)
来源：http://hi.szxytkj.cn

[U31] Py：单测
来源：http://ks.nicolike.cn

python -m pytest -q
来源：http://hl.panjiajie.cn

[U32] Py：代码格式化
来源：http://fs.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://ur.9csxet.cn

[U33] Py：打包发布
来源：http://er.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://dg.9csxet.cn

[U34] Py：判断编码
来源：http://rh.haigaiapp.cn

chardet.detect(raw)
来源：http://us.chemitech.net.cn

[U35] Py：发送邮件
来源：http://qi.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://te.9csxet.cn

[U36] Py：定时任务
来源：http://sn.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://zu.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://zp.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nb.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://vr.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://gu.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://ye.yuexingan06.cn

sys.stdout.isatty()
来源：http://ob.szsharing.cn

[U40] Py：打印到标准错误
来源：http://xy.huanxung.cn

print("err", file=sys.stderr)
来源：http://ya.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ii.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gf.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://id.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ql.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://cq.hnjuh.cn

namespace App\Http;
来源：http://yu.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://lp.yuntaijiaju.cn

declare(strict_types=1);
来源：http://bt.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://rx.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qa.shxzukj.cn

[U46] PHP：可空类型
来源：http://zo.colortex.cn

?string $name = null
来源：http://aa.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://zw.yuntaijiaju.cn

int|string $id
来源：http://hu.nicolike.cn

[U48] PHP：纯枚举
来源：http://kh.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zt.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://mt.panjiajie.cn

public readonly string $name
来源：http://iu.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ea.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ir.gzmigu.cn

[U51] PHP：数组解构
来源：http://io.muxihuayi.cn

[$a, $b] = $arr;
来源：http://do.lnxyls.cn

[U52] PHP：箭头函数
来源：http://xu.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://ee.szsharing.cn

[U53] PHP：空合并运算符
来源：http://xh.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://xs.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://ll.gzmigu.cn

$obj?->method()
来源：http://ci.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://mp.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hh.panjiajie.cn

[U56] PHP：命名参数
来源：http://fs.haigaiapp.cn

f(a: 1, b: 2)
来源：http://hb.nicolike.cn

[U57] PHP：字符串插值
来源：http://ek.bookmarksfly.cn

"值: {$a}"
来源：http://kk.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://dy.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xc.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://kl.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ne.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://yp.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ns.shtwfgs.cn

[U61] PHP：正则
来源：http://fa.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ms.haigaiapp.cn

[U62] PHP：日期对象
来源：http://un.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yj.muxihuayi.cn

[U63] PHP：文件读写
来源：http://lh.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://re.colortex.cn

[U64] PHP：目录遍历
来源：http://zy.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://zo.szsharing.cn

[U65] PHP：会话
来源：http://sl.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vz.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://qz.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ef.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://sr.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wf.huanxung.cn

[U68] PHP：PDO 连接
来源：http://ie.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rx.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://bh.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ut.hahajie.cn

[U70] PHP：PDO 事务
来源：http://pa.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sj.panjiajie.cn

[U71] PHP：抛出异常
来源：http://ps.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://vu.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://yy.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://sm.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://yk.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://zh.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ib.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://vi.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://yv.huanxung.cn

composer require psr/container
来源：http://wh.hahajie.cn

[U76] PHP：简单路由
来源：http://ez.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lm.hahajie.cn

[U77] PHP：模板渲染
来源：http://ft.521024.cn

composer require twig/twig
来源：http://qg.wgjwhj.cn

[U78] PHP：单元测试
来源：http://iz.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://rb.gzmigu.cn

[U79] PHP：静态分析
来源：http://fc.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://pa.asd995.cn

[U80] PHP：代码规范修复
来源：http://ft.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://om.szsharing.cn

[U81] JS：初始化项目
来源：http://ir.nicolike.cn

npm init -y;  npm i express
来源：http://kx.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://hc.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gb.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://zr.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hj.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://dy.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://px.9csxet.cn

[U85] JS：可选链
来源：http://nw.panjiajie.cn

a?.b?.c
来源：http://pw.hnjuh.cn

[U86] JS：空值合并
来源：http://pr.yuntaijiaju.cn

a ?? b
来源：http://ca.muxihuayi.cn

[U87] JS：解构默认值
来源：http://fl.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://le.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://du.nszjky.cn

{ ...a, ...b }
来源：http://pg.nszjky.cn

[U89] JS：数组去重
来源：http://jc.panjiajie.cn

[...new Set(arr)]
来源：http://dk.shxzukj.cn

[U90] JS：数字数组排序
来源：http://vy.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://xu.521024.cn

[U91] JS：对象键值遍历
来源：http://pj.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qx.szxytkj.cn

[U92] JS：深拷贝
来源：http://jv.panjiajie.cn

structuredClone(obj)
来源：http://gy.nszjky.cn

[U93] JS：模板字符串
来源：http://yk.wgjwhj.cn

`共 ${n} 条`
来源：http://jz.gzmigu.cn

[U94] JS：箭头函数
来源：http://zn.jctech888.com.cn

const double = x => x * 2;
来源：http://fo.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://dj.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://rr.nszjky.cn

[U96] JS：async/await 与异常
来源：http://vq.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uk.lnxyls.cn

[U97] JS：并发请求
来源：http://qt.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tv.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://mu.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ov.wgjwhj.cn

[U99] JS：事件监听
来源：http://sg.nicolike.cn

el.addEventListener("click", e => {})
来源：http://uz.gzmigu.cn

[U100] JS：DOM 查询
来源：http://dq.jianghongdianzi.cn

document.querySelector(".item")
来源：http://ol.asd995.cn

[U101] JS：classList 操作
来源：http://hb.wgjwhj.cn

el.classList.toggle("active")
来源：http://ip.huixiangedu.cn

[U102] JS：本地存储
来源：http://ey.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qp.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ga.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lk.haigaiapp.cn

[U104] JS：防抖
来源：http://vh.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://of.521024.cn

[U105] JS：节流
来源：http://bk.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nn.bjjhwx.cn

[U106] JS：日期格式化
来源：http://zk.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iu.asd995.cn

[U107] JS：数字千分位
来源：http://ce.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sn.jctech888.com.cn

[U108] JS：随机整数
来源：http://hm.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mb.jctech888.com.cn

[U109] JS：数组分组
来源：http://hk.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://do.nszjky.cn

[U110] JS：数组分块
来源：http://wt.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ox.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://bp.lnxyls.cn

new Map(Object.entries(obj))
来源：http://jt.muxihuayi.cn

[U112] JS：字符串补位
来源：http://pz.wgjwhj.cn

"7".padStart(3, "0")
来源：http://iq.asd995.cn

[U113] JS：正则替换全部
来源：http://od.nicolike.cn

s.replaceAll("a", "b")
来源：http://mx.hahajie.cn

[U114] JS：JSON 深比较
来源：http://sl.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nz.shxzskj.cn

[U115] JS：生成 UUID
来源：http://je.newstarts.cn

crypto.randomUUID()
来源：http://yg.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://rx.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://gs.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://ob.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://aj.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://jn.asd995.cn

npm i -D vite;  npx vite
来源：http://wq.521024.cn

[U119] JS：生产构建
来源：http://hd.newstarts.cn

npx vite build
来源：http://dt.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://kp.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://pj.shxzskj.cn

================================================================================
来源：http://yq.huixinmuqiang.cn

统计汇总
来源：http://mt.9csxet.cn

================================================================================
来源：http://qh.shxzukj.cn

按语言统计（条）：
来源：http://yz.nicolike.cn


<!-- 参考信息 -->