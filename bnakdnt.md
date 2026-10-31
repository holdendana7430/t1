代发 wailian999

[T43] Perl：字符串插值
来源：http://cc.panjiajie.cn

"值: $a"
来源：http://rc.nszjky.cn

[T44] Perl：条件
来源：http://ak.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://oy.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ct.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://ds.newstarts.cn

[T46] Perl：哈希操作
来源：http://hp.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ur.asd995.cn

[T47] Perl：正则捕获
来源：http://yz.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vu.huanxung.cn

[T48] Perl：正则替换
来源：http://vl.nszjky.cn

$s =~ s/old/new/g;
来源：http://ku.wgjwhj.cn

[T49] Perl：函数
来源：http://ou.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hc.nszjky.cn

[T50] Perl：逐行读文件
来源：http://ob.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rs.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://sx.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://nu.gzmigu.cn

println("Hello")
来源：http://ct.shtwfgs.cn

[T52] Scala：变量
来源：http://oq.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://bi.huanxung.cn

[T53] Scala：字符串插值
来源：http://eq.szxytkj.cn

s"值: $b"
来源：http://vd.newstarts.cn

[T54] Scala：集合映射
来源：http://kz.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://ej.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://zl.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://av.panjiajie.cn

[T56] Scala：样例类
来源：http://sm.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://hm.shxzskj.cn

[T57] Scala：模式匹配
来源：http://pw.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ej.gzmigu.cn

[T58] Scala：函数定义
来源：http://tl.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iw.bjjhwx.cn

[T59] Scala：循环
来源：http://ym.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://oj.lnxyls.cn

[T60] Scala：折叠
来源：http://is.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wg.yuexingan06.cn

================================================================================
来源：http://nc.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vo.newstarts.cn

================================================================================
来源：http://ao.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://js.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://od.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://dt.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hh.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://dc.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uk.nicolike.cn

[U04] Py：变量调试打印
来源：http://hh.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kh.newstarts.cn

[U05] Py：列表去重且保序
来源：http://aj.nicolike.cn

list(dict.fromkeys(arr))
来源：http://ge.lnxyls.cn

[U06] Py：合并两个字典
来源：http://nj.huanxung.cn

{**a, **b}
来源：http://db.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://ud.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://bi.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://ut.huixiangedu.cn

[y for x in nested for y in x]
来源：http://go.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://js.shxzukj.cn

max(d, key=d.get)
来源：http://vf.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://un.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zl.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://fp.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://yd.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fz.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://ql.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://vg.szsharing.cn

deque(maxlen=10)
来源：http://ay.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://sa.jctech888.com.cn

defaultdict(list)
来源：http://cm.gzmigu.cn

[U15] Py：高精度计时
来源：http://re.bjjhwx.cn

t = time.perf_counter()
来源：http://fu.nszjky.cn

[U16] Py：命令行参数解析
来源：http://jj.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zn.jctech888.com.cn

[U17] Py：初始化日志
来源：http://ow.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ip.szxytkj.cn

[U18] Py：预编译正则
来源：http://gf.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://yh.newstarts.cn

[U19] Py：正则替换带回调
来源：http://zf.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hc.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://sp.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://gl.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://lc.gzmigu.cn

@contextlib.contextmanager
来源：http://qi.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://tw.huixinmuqiang.cn

list(zip(*m))
来源：http://mc.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://oy.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pt.hnjuh.cn

[U24] Py：路径操作
来源：http://sc.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zn.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://cd.jianghongdianzi.cn

csv.DictReader(f)
来源：http://eu.huanxung.cn

[U26] Py：并发下载
来源：http://vw.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gy.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://rf.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://eb.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://xo.huixiangedu.cn

UserId = int
来源：http://vq.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://am.shxzukj.cn

@property 与 @x.setter 配合
来源：http://xs.nszjky.cn

[U30] Py：数据类
来源：http://zi.jctech888.com.cn

@dataclass(slots=True)
来源：http://gy.panjiajie.cn

[U31] Py：单测
来源：http://in.huixinmuqiang.cn

python -m pytest -q
来源：http://px.muxihuayi.cn

[U32] Py：代码格式化
来源：http://hy.521024.cn

ruff format . && ruff check --fix .
来源：http://ox.yuexingan06.cn

[U33] Py：打包发布
来源：http://as.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://rr.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://cn.huixiangedu.cn

chardet.detect(raw)
来源：http://jh.lnxyls.cn

[U35] Py：发送邮件
来源：http://qg.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yi.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://kw.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ro.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ra.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bn.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://pk.hahajie.cn

Path(__file__).resolve().parent
来源：http://je.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://qj.shxzskj.cn

sys.stdout.isatty()
来源：http://rl.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://aw.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://ft.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://bl.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ih.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://go.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fj.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://dg.szxytkj.cn

namespace App\Http;
来源：http://oq.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://xd.gzmigu.cn

declare(strict_types=1);
来源：http://bq.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://fn.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qc.hahajie.cn

[U46] PHP：可空类型
来源：http://kb.yuntaijiaju.cn

?string $name = null
来源：http://ut.nszjky.cn

[U47] PHP：联合类型
来源：http://zd.hnjuh.cn

int|string $id
来源：http://rk.szxytkj.cn

[U48] PHP：纯枚举
来源：http://cg.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eu.szxytkj.cn

[U49] PHP：只读属性
来源：http://ln.shxzukj.cn

public readonly string $name
来源：http://jc.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://rr.panjiajie.cn

public function __construct(private int $id) {}
来源：http://yr.gzmigu.cn

[U51] PHP：数组解构
来源：http://mt.9csxet.cn

[$a, $b] = $arr;
来源：http://zv.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://he.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://fv.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://hi.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://mu.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://uk.newstarts.cn

$obj?->method()
来源：http://ld.huanxung.cn

[U55] PHP：match 表达式
来源：http://jd.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://co.szxytkj.cn

[U56] PHP：命名参数
来源：http://vh.bjjhwx.cn

f(a: 1, b: 2)
来源：http://ft.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://gy.shxzskj.cn

"值: {$a}"
来源：http://kb.nszjky.cn

[U58] PHP：数组三件套
来源：http://cp.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ka.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://tt.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aq.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://qy.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ze.szxytkj.cn

[U61] PHP：正则
来源：http://bu.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dh.muxihuayi.cn

[U62] PHP：日期对象
来源：http://eb.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ae.huanxung.cn

[U63] PHP：文件读写
来源：http://ts.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wa.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://pn.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://ch.shxzskj.cn

[U65] PHP：会话
来源：http://yc.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sp.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://zw.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rl.hahajie.cn

[U67] PHP：处理文件上传
来源：http://ct.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bj.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://mz.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zm.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://zv.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sk.colortex.cn

[U70] PHP：PDO 事务
来源：http://mq.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ge.shxzukj.cn

[U71] PHP：抛出异常
来源：http://hr.521024.cn

throw new RuntimeException("失败", 500);
来源：http://dt.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://nf.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://sv.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://bp.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://zq.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://xz.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://sh.gzmigu.cn

[U75] PHP：依赖注入
来源：http://pc.yuntaijiaju.cn

composer require psr/container
来源：http://kd.9csxet.cn

[U76] PHP：简单路由
来源：http://ok.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pp.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://dk.shxzskj.cn

composer require twig/twig
来源：http://ph.muxihuayi.cn

[U78] PHP：单元测试
来源：http://vz.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://un.bjjhwx.cn

[U79] PHP：静态分析
来源：http://zw.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://ne.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://nf.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dc.shxzskj.cn

[U81] JS：初始化项目
来源：http://nh.521024.cn

npm init -y;  npm i express
来源：http://ik.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://mr.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ac.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://rx.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yl.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://jk.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uz.521024.cn

[U85] JS：可选链
来源：http://hw.huixinmuqiang.cn

a?.b?.c
来源：http://hi.shxzskj.cn

[U86] JS：空值合并
来源：http://rv.nszjky.cn

a ?? b
来源：http://pf.szxytkj.cn

[U87] JS：解构默认值
来源：http://cx.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://xe.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://pd.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ip.nicolike.cn

[U89] JS：数组去重
来源：http://ws.asd995.cn

[...new Set(arr)]
来源：http://uc.hahajie.cn

[U90] JS：数字数组排序
来源：http://ao.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://on.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://zw.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nx.chemitech.net.cn

[U92] JS：深拷贝
来源：http://tn.yuexingan06.cn

structuredClone(obj)
来源：http://rw.huanxung.cn

[U93] JS：模板字符串
来源：http://gs.521024.cn

`共 ${n} 条`
来源：http://ih.muxihuayi.cn

[U94] JS：箭头函数
来源：http://dm.nicolike.cn

const double = x => x * 2;
来源：http://yw.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://kr.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://ju.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://qw.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wz.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://cz.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ms.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://je.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ig.chemitech.net.cn

[U99] JS：事件监听
来源：http://ok.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://lt.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ab.chemitech.net.cn

document.querySelector(".item")
来源：http://no.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://ut.bookmarksfly.cn

el.classList.toggle("active")
来源：http://jv.wgjwhj.cn

[U102] JS：本地存储
来源：http://wh.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://id.colortex.cn

[U103] JS：定时器
来源：http://nu.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gc.jctech888.com.cn

[U104] JS：防抖
来源：http://ek.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xu.colortex.cn

[U105] JS：节流
来源：http://go.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuexingan06.cn

[U106] JS：日期格式化
来源：http://wr.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hm.nszjky.cn

[U107] JS：数字千分位
来源：http://as.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ox.chemitech.net.cn

[U108] JS：随机整数
来源：http://zd.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qs.hahajie.cn

[U109] JS：数组分组
来源：http://es.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://yf.lnxyls.cn

[U110] JS：数组分块
来源：http://jr.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://du.gzmigu.cn

[U111] JS：对象转 Map
来源：http://fk.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://vs.chemitech.net.cn

[U112] JS：字符串补位
来源：http://qr.nszjky.cn

"7".padStart(3, "0")
来源：http://ai.nszjky.cn

[U113] JS：正则替换全部
来源：http://an.gzmigu.cn

s.replaceAll("a", "b")
来源：http://ck.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://uo.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hx.szxytkj.cn

[U115] JS：生成 UUID
来源：http://kw.huanxung.cn

crypto.randomUUID()
来源：http://tv.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://te.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://qz.chemitech.net.cn

[U117] JS：单元测试
来源：http://is.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://av.nszjky.cn

[U118] JS：开发服务器
来源：http://hl.newstarts.cn

npm i -D vite;  npx vite
来源：http://nv.bjjhwx.cn

[U119] JS：生产构建
来源：http://lz.521024.cn

npx vite build
来源：http://gf.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://dp.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://ae.nszjky.cn

================================================================================
来源：http://dt.newstarts.cn

统计汇总
来源：http://ig.huixinmuqiang.cn

================================================================================
来源：http://wo.colortex.cn

按语言统计（条）：
来源：http://ob.asd995.cn

Python ......... 252
来源：http://eq.shxzskj.cn

PHP ............ 252
来源：http://hk.haigaiapp.cn

JavaScript ..... 252
来源：http://ev.huixiangedu.cn

TypeScript ..... 212
来源：http://pt.bjjhwx.cn

Java ........... 212
来源：http://no.wgjwhj.cn

Go ............. 212
来源：http://wy.colortex.cn

Ruby ........... 212
来源：http://jw.haigaiapp.cn

C# ............. 212
来源：http://kg.lnxyls.cn

C .............. 30
来源：http://ut.hahajie.cn

C++ ............ 30
来源：http://ux.lnxyls.cn

SQL ............ 90
来源：http://kc.hnjuh.cn

Bash ........... 80
来源：http://fu.hnjuh.cn

Kotlin ......... 15
来源：http://jm.yuexingan06.cn

Swift .......... 15
来源：http://qt.huanxung.cn

Lua ............ 10
来源：http://dz.gzmigu.cn

Perl ........... 10
来源：http://ya.hnjuh.cn


<!-- 参考信息 -->