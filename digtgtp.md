代发 wailian999

[T41] Perl：Hello World
来源：http://hr.yuntaijiaju.cn

print "Hello\n";
来源：http://hd.bjjhwx.cn

[T42] Perl：变量类型
来源：http://wf.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lg.shxzukj.cn

[T43] Perl：字符串插值
来源：http://hc.yuntaijiaju.cn

"值: $a"
来源：http://pr.hnjuh.cn

[T44] Perl：条件
来源：http://uh.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://so.lnxyls.cn

[T45] Perl：数组遍历
来源：http://xa.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://lt.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://fb.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zy.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://zz.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ih.nicolike.cn

[T48] Perl：正则替换
来源：http://pf.hnjuh.cn

$s =~ s/old/new/g;
来源：http://zh.huanxung.cn

[T49] Perl：函数
来源：http://or.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cb.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://ff.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sr.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://jd.huanxung.cn

[T51] Scala：Hello World
来源：http://yr.9csxet.cn

println("Hello")
来源：http://hs.hnjuh.cn

[T52] Scala：变量
来源：http://um.szxytkj.cn

val a = 1;  var b = 2
来源：http://hx.nicolike.cn

[T53] Scala：字符串插值
来源：http://ya.panjiajie.cn

s"值: $b"
来源：http://ga.huixiangedu.cn

[T54] Scala：集合映射
来源：http://zs.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://rk.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://tt.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mp.muxihuayi.cn

[T56] Scala：样例类
来源：http://ha.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ft.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://we.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hk.9csxet.cn

[T58] Scala：函数定义
来源：http://jp.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ca.muxihuayi.cn

[T59] Scala：循环
来源：http://zf.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://xd.lnxyls.cn

[T60] Scala：折叠
来源：http://vn.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://it.yuexingan06.cn

================================================================================
来源：http://sg.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ib.wgjwhj.cn

================================================================================
来源：http://jm.521024.cn

[U01] Py：创建虚拟环境
来源：http://ej.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hs.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ri.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://se.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://ud.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://er.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://ts.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ii.newstarts.cn

[U05] Py：列表去重且保序
来源：http://os.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://vv.hnjuh.cn

[U06] Py：合并两个字典
来源：http://qy.nszjky.cn

{**a, **b}
来源：http://zt.hnjuh.cn

[U07] Py：反转字典键值
来源：http://sj.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://fl.nszjky.cn

[U08] Py：展平二维列表
来源：http://xp.shxzskj.cn

[y for x in nested for y in x]
来源：http://vo.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://bg.muxihuayi.cn

max(d, key=d.get)
来源：http://jr.521024.cn

[U10] Py：按值排序字典
来源：http://zx.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ga.shxzskj.cn

[U11] Py：生成器表达式
来源：http://yj.wgjwhj.cn

(x * 2 for x in arr)
来源：http://if.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vq.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://re.hahajie.cn

[U13] Py：固定长度队列
来源：http://qc.muxihuayi.cn

deque(maxlen=10)
来源：http://dk.colortex.cn

[U14] Py：分组收集到列表
来源：http://zz.muxihuayi.cn

defaultdict(list)
来源：http://td.hnjuh.cn

[U15] Py：高精度计时
来源：http://ld.yuexingan06.cn

t = time.perf_counter()
来源：http://qx.nicolike.cn

[U16] Py：命令行参数解析
来源：http://dn.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://us.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://mn.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://xx.nszjky.cn

[U18] Py：预编译正则
来源：http://vy.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://le.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://al.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ol.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://fi.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://ep.521024.cn

[U21] Py：自定义上下文管理器
来源：http://mg.muxihuayi.cn

@contextlib.contextmanager
来源：http://qw.nicolike.cn

[U22] Py：矩阵转置
来源：http://rx.9csxet.cn

list(zip(*m))
来源：http://ya.nszjky.cn

[U23] Py：分块读取大文件
来源：http://cq.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mg.hnjuh.cn

[U24] Py：路径操作
来源：http://sl.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ye.asd995.cn

[U25] Py：CSV 按字典读
来源：http://sz.huixinmuqiang.cn

csv.DictReader(f)
来源：http://xz.nszjky.cn

[U26] Py：并发下载
来源：http://ey.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lq.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://rg.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ap.colortex.cn

[U28] Py：类型别名
来源：http://qs.shtwfgs.cn

UserId = int
来源：http://es.hahajie.cn

[U29] Py：属性校验
来源：http://ke.hahajie.cn

@property 与 @x.setter 配合
来源：http://tl.szxytkj.cn

[U30] Py：数据类
来源：http://uo.hahajie.cn

@dataclass(slots=True)
来源：http://sy.wgjwhj.cn

[U31] Py：单测
来源：http://au.muxihuayi.cn

python -m pytest -q
来源：http://kl.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://mt.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://kn.shtwfgs.cn

[U33] Py：打包发布
来源：http://dm.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://sy.huanxung.cn

[U34] Py：判断编码
来源：http://fb.haigaiapp.cn

chardet.detect(raw)
来源：http://ki.chemitech.net.cn

[U35] Py：发送邮件
来源：http://lx.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ig.shtwfgs.cn

[U36] Py：定时任务
来源：http://qu.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://rl.gzmigu.cn

[U37] Py：读写 Excel
来源：http://hs.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mw.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://xz.nicolike.cn

Path(__file__).resolve().parent
来源：http://ij.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://fj.gzmigu.cn

sys.stdout.isatty()
来源：http://xd.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://wr.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://ll.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://qy.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iy.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://un.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://wk.bookmarksfly.cn

namespace App\Http;
来源：http://xa.newstarts.cn

[U44] PHP：开启严格类型
来源：http://iu.asd995.cn

declare(strict_types=1);
来源：http://rc.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://yl.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aw.szxytkj.cn

[U46] PHP：可空类型
来源：http://hw.nicolike.cn

?string $name = null
来源：http://di.chemitech.net.cn

[U47] PHP：联合类型
来源：http://by.szxytkj.cn

int|string $id
来源：http://hp.hnjuh.cn

[U48] PHP：纯枚举
来源：http://md.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://um.shxzukj.cn

[U49] PHP：只读属性
来源：http://gp.jctech888.com.cn

public readonly string $name
来源：http://lf.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://hm.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://vf.gzmigu.cn

[U51] PHP：数组解构
来源：http://fw.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://mq.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://xe.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://wj.9csxet.cn

[U53] PHP：空合并运算符
来源：http://xy.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://xy.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://qy.huixinmuqiang.cn

$obj?->method()
来源：http://bb.nszjky.cn

[U55] PHP：match 表达式
来源：http://os.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kh.shtwfgs.cn

[U56] PHP：命名参数
来源：http://so.hnjuh.cn

f(a: 1, b: 2)
来源：http://qo.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://lv.asd995.cn

"值: {$a}"
来源：http://ut.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://gd.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hf.hahajie.cn

[U59] PHP：自定义排序
来源：http://uy.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://si.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://qk.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lp.gzmigu.cn

[U61] PHP：正则
来源：http://yw.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aj.huixiangedu.cn

[U62] PHP：日期对象
来源：http://hv.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gh.nicolike.cn

[U63] PHP：文件读写
来源：http://qg.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rq.newstarts.cn

[U64] PHP：目录遍历
来源：http://my.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ix.nszjky.cn

[U65] PHP：会话
来源：http://uu.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pv.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://fd.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mb.nicolike.cn

[U67] PHP：处理文件上传
来源：http://zr.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://td.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://dv.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rv.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://bd.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oz.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://sy.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eu.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://na.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://dl.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://ge.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://tn.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://zb.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://mw.521024.cn

[U74] PHP：读取环境变量
来源：http://vt.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://qc.huanxung.cn

[U75] PHP：依赖注入
来源：http://oc.szxytkj.cn

composer require psr/container
来源：http://ar.szxytkj.cn

[U76] PHP：简单路由
来源：http://id.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://op.nszjky.cn

[U77] PHP：模板渲染
来源：http://ch.521024.cn

composer require twig/twig
来源：http://kp.hahajie.cn

[U78] PHP：单元测试
来源：http://ur.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://ah.huixiangedu.cn

[U79] PHP：静态分析
来源：http://ra.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://gv.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://qo.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cm.gzmigu.cn

[U81] JS：初始化项目
来源：http://va.yuexingan06.cn

npm init -y;  npm i express
来源：http://mj.asd995.cn

[U82] JS：package.json 脚本
来源：http://xu.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://du.521024.cn

[U83] JS：ES Module 导入导出
来源：http://hh.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vj.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://wr.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sg.nszjky.cn

[U85] JS：可选链
来源：http://zg.shxzskj.cn

a?.b?.c
来源：http://mz.shxzukj.cn

[U86] JS：空值合并
来源：http://py.colortex.cn

a ?? b
来源：http://ir.shxzskj.cn

[U87] JS：解构默认值
来源：http://wq.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://up.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://vh.wgjwhj.cn

{ ...a, ...b }
来源：http://od.9csxet.cn

[U89] JS：数组去重
来源：http://gg.szxytkj.cn

[...new Set(arr)]
来源：http://jc.9csxet.cn

[U90] JS：数字数组排序
来源：http://yi.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://sn.asd995.cn

[U91] JS：对象键值遍历
来源：http://ke.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://op.newstarts.cn

[U92] JS：深拷贝
来源：http://gc.hnjuh.cn

structuredClone(obj)
来源：http://ky.colortex.cn

[U93] JS：模板字符串
来源：http://kr.szxytkj.cn

`共 ${n} 条`
来源：http://gc.haigaiapp.cn

[U94] JS：箭头函数
来源：http://nr.hnjuh.cn

const double = x => x * 2;
来源：http://on.panjiajie.cn

[U95] JS：Promise 包装
来源：http://gg.521024.cn

new Promise((resolve, reject) => {})
来源：http://du.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ci.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hs.nszjky.cn

[U97] JS：并发请求
来源：http://nb.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pg.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://bv.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://as.haigaiapp.cn

[U99] JS：事件监听
来源：http://ol.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://su.shxzukj.cn

[U100] JS：DOM 查询
来源：http://ss.hnjuh.cn

document.querySelector(".item")
来源：http://my.szxytkj.cn

[U101] JS：classList 操作
来源：http://fb.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://lo.szsharing.cn

[U102] JS：本地存储
来源：http://rc.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kf.muxihuayi.cn

[U103] JS：定时器
来源：http://su.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hq.jctech888.com.cn

[U104] JS：防抖
来源：http://af.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nv.shtwfgs.cn

[U105] JS：节流
来源：http://ey.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fa.shtwfgs.cn

[U106] JS：日期格式化
来源：http://qd.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ay.wgjwhj.cn

[U107] JS：数字千分位
来源：http://pl.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qe.hahajie.cn

[U108] JS：随机整数
来源：http://tk.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qj.nicolike.cn

[U109] JS：数组分组
来源：http://sn.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://sw.hahajie.cn

[U110] JS：数组分块
来源：http://ca.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qy.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://iy.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ys.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://ua.chemitech.net.cn

"7".padStart(3, "0")
来源：http://kh.shxzukj.cn

[U113] JS：正则替换全部
来源：http://vh.huanxung.cn

s.replaceAll("a", "b")
来源：http://gp.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://qw.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ja.nszjky.cn

[U115] JS：生成 UUID
来源：http://bd.asd995.cn

crypto.randomUUID()
来源：http://wr.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://dk.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://ic.chemitech.net.cn

[U117] JS：单元测试
来源：http://ek.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://rj.huanxung.cn

[U118] JS：开发服务器
来源：http://hw.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://gh.shxzukj.cn

[U119] JS：生产构建
来源：http://vn.huixiangedu.cn

npx vite build
来源：http://zi.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://se.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://gp.bjjhwx.cn

================================================================================
来源：http://dh.bookmarksfly.cn

统计汇总
来源：http://cg.bjjhwx.cn

================================================================================
来源：http://wy.shxzskj.cn

按语言统计（条）：
来源：http://yy.bookmarksfly.cn

Python ......... 252
来源：http://kt.huixinmuqiang.cn

PHP ............ 252
来源：http://zi.gzmigu.cn

JavaScript ..... 252
来源：http://ny.yuexingan06.cn

TypeScript ..... 212
来源：http://su.nszjky.cn

Java ........... 212
来源：http://jo.chemitech.net.cn

Go ............. 212
来源：http://yn.lnxyls.cn

Ruby ........... 212
来源：http://im.newstarts.cn

C# ............. 212
来源：http://jq.szxytkj.cn

C .............. 30
来源：http://mz.shxzskj.cn

C++ ............ 30
来源：http://gz.chemitech.net.cn

SQL ............ 90
来源：http://po.wgjwhj.cn

Bash ........... 80
来源：http://tc.wgjwhj.cn


<!-- 参考信息 -->