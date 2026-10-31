代发 wailian999

[T45] Perl：数组遍历
来源：http://lj.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://wb.shxzukj.cn

[T46] Perl：哈希操作
来源：http://na.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uh.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://fj.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://se.chemitech.net.cn

[T48] Perl：正则替换
来源：http://tq.hahajie.cn

$s =~ s/old/new/g;
来源：http://qi.shxzskj.cn

[T49] Perl：函数
来源：http://ah.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wx.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://uz.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fs.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://gq.bjjhwx.cn

[T51] Scala：Hello World
来源：http://dn.asd995.cn

println("Hello")
来源：http://wq.chemitech.net.cn

[T52] Scala：变量
来源：http://nj.szsharing.cn

val a = 1;  var b = 2
来源：http://ai.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://rs.yuexingan06.cn

s"值: $b"
来源：http://zd.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://rc.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://ig.hahajie.cn

[T55] Scala：集合过滤
来源：http://sf.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zi.jctech888.com.cn

[T56] Scala：样例类
来源：http://bd.nszjky.cn

case class User(name: String, age: Int)
来源：http://af.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://el.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ag.9csxet.cn

[T58] Scala：函数定义
来源：http://ln.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yw.szsharing.cn

[T59] Scala：循环
来源：http://bh.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://xr.huanxung.cn

[T60] Scala：折叠
来源：http://ep.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xj.nicolike.cn

================================================================================
来源：http://av.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dx.shxzskj.cn

================================================================================
来源：http://mk.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://ge.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wt.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://kc.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ug.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://tw.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://su.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://yb.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ug.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://uy.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://nz.szxytkj.cn

[U06] Py：合并两个字典
来源：http://fb.521024.cn

{**a, **b}
来源：http://im.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://nz.521024.cn

{v: k for k, v in d.items()}
来源：http://db.hahajie.cn

[U08] Py：展平二维列表
来源：http://yq.jctech888.com.cn

[y for x in nested for y in x]
来源：http://we.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://wp.huanxung.cn

max(d, key=d.get)
来源：http://hp.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://js.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zp.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://pj.colortex.cn

(x * 2 for x in arr)
来源：http://nb.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jo.nicolike.cn

Counter(arr).most_common(3)
来源：http://sd.huanxung.cn

[U13] Py：固定长度队列
来源：http://wm.huanxung.cn

deque(maxlen=10)
来源：http://cb.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://cm.colortex.cn

defaultdict(list)
来源：http://dm.shtwfgs.cn

[U15] Py：高精度计时
来源：http://lr.colortex.cn

t = time.perf_counter()
来源：http://ls.521024.cn

[U16] Py：命令行参数解析
来源：http://pc.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rw.hnjuh.cn

[U17] Py：初始化日志
来源：http://lt.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ib.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://oy.nszjky.cn

pat = re.compile(r"\d+")
来源：http://aq.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://pv.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xo.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://os.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://kh.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://wb.jctech888.com.cn

@contextlib.contextmanager
来源：http://dp.9csxet.cn

[U22] Py：矩阵转置
来源：http://cx.colortex.cn

list(zip(*m))
来源：http://bz.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://fq.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vi.521024.cn

[U24] Py：路径操作
来源：http://iw.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iu.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://em.yuexingan06.cn

csv.DictReader(f)
来源：http://nk.huixiangedu.cn

[U26] Py：并发下载
来源：http://st.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qo.nicolike.cn

[U27] Py：异步 HTTP
来源：http://kd.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ur.nszjky.cn

[U28] Py：类型别名
来源：http://bd.hnjuh.cn

UserId = int
来源：http://bo.nszjky.cn

[U29] Py：属性校验
来源：http://cu.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://is.colortex.cn

[U30] Py：数据类
来源：http://mc.shxzukj.cn

@dataclass(slots=True)
来源：http://dv.huixinmuqiang.cn

[U31] Py：单测
来源：http://ck.nszjky.cn

python -m pytest -q
来源：http://gg.wgjwhj.cn

[U32] Py：代码格式化
来源：http://ur.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://rr.bookmarksfly.cn

[U33] Py：打包发布
来源：http://hm.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://ao.gzmigu.cn

[U34] Py：判断编码
来源：http://ee.panjiajie.cn

chardet.detect(raw)
来源：http://tc.newstarts.cn

[U35] Py：发送邮件
来源：http://cb.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ny.bookmarksfly.cn

[U36] Py：定时任务
来源：http://rz.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://tu.newstarts.cn

[U37] Py：读写 Excel
来源：http://ud.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dp.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://gi.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://bl.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://mc.huanxung.cn

sys.stdout.isatty()
来源：http://dl.hahajie.cn

[U40] Py：打印到标准错误
来源：http://qj.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://qc.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://nz.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ui.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://nz.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tm.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://jm.gzmigu.cn

namespace App\Http;
来源：http://uy.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://ck.bookmarksfly.cn

declare(strict_types=1);
来源：http://bb.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://bd.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.colortex.cn

[U46] PHP：可空类型
来源：http://rb.asd995.cn

?string $name = null
来源：http://qs.nicolike.cn

[U47] PHP：联合类型
来源：http://rt.haigaiapp.cn

int|string $id
来源：http://zx.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://kt.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://it.asd995.cn

[U49] PHP：只读属性
来源：http://cl.muxihuayi.cn

public readonly string $name
来源：http://wg.asd995.cn

[U50] PHP：构造器属性提升
来源：http://fn.huanxung.cn

public function __construct(private int $id) {}
来源：http://iw.jctech888.com.cn

[U51] PHP：数组解构
来源：http://ms.nicolike.cn

[$a, $b] = $arr;
来源：http://ly.521024.cn

[U52] PHP：箭头函数
来源：http://vg.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://xs.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://dk.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://uk.newstarts.cn

[U54] PHP：空安全调用
来源：http://tr.szxytkj.cn

$obj?->method()
来源：http://ox.shxzskj.cn

[U55] PHP：match 表达式
来源：http://gc.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fu.jctech888.com.cn

[U56] PHP：命名参数
来源：http://kg.hnjuh.cn

f(a: 1, b: 2)
来源：http://sb.nszjky.cn

[U57] PHP：字符串插值
来源：http://yr.newstarts.cn

"值: {$a}"
来源：http://tw.hahajie.cn

[U58] PHP：数组三件套
来源：http://rg.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gs.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ih.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jp.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://wk.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wv.gzmigu.cn

[U61] PHP：正则
来源：http://ch.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bt.gzmigu.cn

[U62] PHP：日期对象
来源：http://nn.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://st.9csxet.cn

[U63] PHP：文件读写
来源：http://wh.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xb.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://es.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://qa.yuntaijiaju.cn

[U65] PHP：会话
来源：http://uj.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jt.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://co.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qb.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://tn.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uh.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://rq.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cz.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://qb.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ju.nicolike.cn

[U70] PHP：PDO 事务
来源：http://pv.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fv.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ii.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://ly.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://vp.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://de.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://nm.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://mo.newstarts.cn

[U74] PHP：读取环境变量
来源：http://jq.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://uu.521024.cn

[U75] PHP：依赖注入
来源：http://lx.huixiangedu.cn

composer require psr/container
来源：http://cy.chemitech.net.cn

[U76] PHP：简单路由
来源：http://bu.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vj.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://tj.yuexingan06.cn

composer require twig/twig
来源：http://iv.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://nk.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://zx.shxzskj.cn

[U79] PHP：静态分析
来源：http://gw.asd995.cn

composer require --dev phpstan/phpstan
来源：http://sg.asd995.cn

[U80] PHP：代码规范修复
来源：http://lh.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vc.muxihuayi.cn

[U81] JS：初始化项目
来源：http://ot.bjjhwx.cn

npm init -y;  npm i express
来源：http://su.huanxung.cn

[U82] JS：package.json 脚本
来源：http://zr.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ah.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://nl.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uo.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://mm.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bo.shxzukj.cn

[U85] JS：可选链
来源：http://vc.bjjhwx.cn

a?.b?.c
来源：http://ge.bookmarksfly.cn

[U86] JS：空值合并
来源：http://pa.huanxung.cn

a ?? b
来源：http://sd.chemitech.net.cn

[U87] JS：解构默认值
来源：http://eg.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://fb.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://sf.szxytkj.cn

{ ...a, ...b }
来源：http://hb.chemitech.net.cn

[U89] JS：数组去重
来源：http://tn.asd995.cn

[...new Set(arr)]
来源：http://ge.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://ri.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://mh.colortex.cn

[U91] JS：对象键值遍历
来源：http://lj.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://te.hnjuh.cn

[U92] JS：深拷贝
来源：http://if.chemitech.net.cn

structuredClone(obj)
来源：http://yc.nicolike.cn

[U93] JS：模板字符串
来源：http://rj.shxzukj.cn

`共 ${n} 条`
来源：http://jw.shxzukj.cn

[U94] JS：箭头函数
来源：http://dv.shxzukj.cn

const double = x => x * 2;
来源：http://tw.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://vj.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://nh.nszjky.cn

[U96] JS：async/await 与异常
来源：http://bj.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cx.asd995.cn

[U97] JS：并发请求
来源：http://rj.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bj.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://se.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://py.chemitech.net.cn

[U99] JS：事件监听
来源：http://iw.521024.cn

el.addEventListener("click", e => {})
来源：http://er.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://as.szxytkj.cn

document.querySelector(".item")
来源：http://dn.szsharing.cn

[U101] JS：classList 操作
来源：http://yi.huanxung.cn

el.classList.toggle("active")
来源：http://bc.nicolike.cn

[U102] JS：本地存储
来源：http://pi.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jt.panjiajie.cn

[U103] JS：定时器
来源：http://uk.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nj.yuexingan06.cn

[U104] JS：防抖
来源：http://aj.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zm.521024.cn

[U105] JS：节流
来源：http://pq.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://va.bjjhwx.cn

[U106] JS：日期格式化
来源：http://hv.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ps.bjjhwx.cn

[U107] JS：数字千分位
来源：http://ar.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yi.shxzukj.cn

[U108] JS：随机整数
来源：http://oh.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ke.shxzukj.cn

[U109] JS：数组分组
来源：http://ri.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://ld.chemitech.net.cn

[U110] JS：数组分块
来源：http://ut.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ud.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://yt.521024.cn

new Map(Object.entries(obj))
来源：http://iz.shxzskj.cn

[U112] JS：字符串补位
来源：http://im.wgjwhj.cn

"7".padStart(3, "0")
来源：http://rt.nszjky.cn

[U113] JS：正则替换全部
来源：http://gx.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://lk.nicolike.cn

[U114] JS：JSON 深比较
来源：http://bf.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ra.521024.cn

[U115] JS：生成 UUID
来源：http://xc.colortex.cn

crypto.randomUUID()
来源：http://ti.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://lv.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://oe.hahajie.cn

[U117] JS：单元测试
来源：http://dg.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://np.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://fj.nicolike.cn

npm i -D vite;  npx vite
来源：http://go.szsharing.cn

[U119] JS：生产构建
来源：http://nj.bjjhwx.cn

npx vite build
来源：http://da.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://wx.asd995.cn

import.meta.env.VITE_API_URL
来源：http://it.szxytkj.cn

================================================================================
来源：http://jy.szxytkj.cn

统计汇总
来源：http://gu.chemitech.net.cn

================================================================================
来源：http://zs.shxzukj.cn

按语言统计（条）：
来源：http://qb.szsharing.cn

Python ......... 252
来源：http://no.shxzukj.cn

PHP ............ 252
来源：http://vx.huanxung.cn

JavaScript ..... 252
来源：http://ws.colortex.cn

TypeScript ..... 212
来源：http://tp.lnxyls.cn

Java ........... 212
来源：http://io.asd995.cn

Go ............. 212
来源：http://qs.shxzukj.cn

Ruby ........... 212
来源：http://jr.nszjky.cn

C# ............. 212
来源：http://yi.huixiangedu.cn

C .............. 30
来源：http://xn.nicolike.cn

C++ ............ 30
来源：http://nv.haigaiapp.cn

SQL ............ 90
来源：http://yb.bjjhwx.cn

Bash ........... 80
来源：http://dj.asd995.cn

Kotlin ......... 15
来源：http://au.chemitech.net.cn

Swift .......... 15
来源：http://rb.hnjuh.cn

Lua ............ 10
来源：http://ng.hahajie.cn

Perl ........... 10
来源：http://rv.gzmigu.cn

Scala .......... 10
来源：http://ov.huanxung.cn

------------------------------------
来源：http://fa.szxytkj.cn

合计 ........... 2106 条
来源：http://kl.bookmarksfly.cn

按章节统计：
来源：http://ll.chemitech.net.cn


<!-- 参考信息 -->