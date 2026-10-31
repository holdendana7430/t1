代发 wailian999

[T45] Perl：数组遍历
来源：http://ct.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://pz.521024.cn

[T46] Perl：哈希操作
来源：http://og.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lz.shxzskj.cn

[T47] Perl：正则捕获
来源：http://ow.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yi.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://zx.hnjuh.cn

$s =~ s/old/new/g;
来源：http://wp.szxytkj.cn

[T49] Perl：函数
来源：http://xd.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ke.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://vu.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cx.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://xj.szxytkj.cn

[T51] Scala：Hello World
来源：http://ge.bjjhwx.cn

println("Hello")
来源：http://il.wgjwhj.cn

[T52] Scala：变量
来源：http://vm.haigaiapp.cn

val a = 1;  var b = 2
来源：http://cu.szxytkj.cn

[T53] Scala：字符串插值
来源：http://cp.521024.cn

s"值: $b"
来源：http://ek.nicolike.cn

[T54] Scala：集合映射
来源：http://pn.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://yv.colortex.cn

[T55] Scala：集合过滤
来源：http://dd.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hw.hahajie.cn

[T56] Scala：样例类
来源：http://nq.panjiajie.cn

case class User(name: String, age: Int)
来源：http://pq.hahajie.cn

[T57] Scala：模式匹配
来源：http://jo.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qc.gzmigu.cn

[T58] Scala：函数定义
来源：http://rw.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ol.szsharing.cn

[T59] Scala：循环
来源：http://gk.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://hs.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://iy.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qd.szsharing.cn

================================================================================
来源：http://qf.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xq.nicolike.cn

================================================================================
来源：http://fz.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://st.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xv.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://hs.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yu.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://dp.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hg.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://am.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gh.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://tc.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://kc.nicolike.cn

[U06] Py：合并两个字典
来源：http://xi.nszjky.cn

{**a, **b}
来源：http://ud.hnjuh.cn

[U07] Py：反转字典键值
来源：http://jf.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://xb.521024.cn

[U08] Py：展平二维列表
来源：http://ch.asd995.cn

[y for x in nested for y in x]
来源：http://pf.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://bp.bookmarksfly.cn

max(d, key=d.get)
来源：http://cq.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://nj.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hw.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://bm.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://cg.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zx.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://cz.hahajie.cn

[U13] Py：固定长度队列
来源：http://ps.hahajie.cn

deque(maxlen=10)
来源：http://eg.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://fq.shxzskj.cn

defaultdict(list)
来源：http://ma.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://qb.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ak.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://py.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jx.colortex.cn

[U17] Py：初始化日志
来源：http://nb.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ng.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://vf.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://sz.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://dh.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tf.newstarts.cn

[U20] Py：缓存函数结果
来源：http://fm.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://wn.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://iy.huanxung.cn

@contextlib.contextmanager
来源：http://fj.szxytkj.cn

[U22] Py：矩阵转置
来源：http://xq.wgjwhj.cn

list(zip(*m))
来源：http://hl.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://dn.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://od.huanxung.cn

[U24] Py：路径操作
来源：http://wi.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dk.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://kn.shxzukj.cn

csv.DictReader(f)
来源：http://rm.9csxet.cn

[U26] Py：并发下载
来源：http://fs.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xa.9csxet.cn

[U27] Py：异步 HTTP
来源：http://wp.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://jw.szsharing.cn

[U28] Py：类型别名
来源：http://oc.chemitech.net.cn

UserId = int
来源：http://bv.panjiajie.cn

[U29] Py：属性校验
来源：http://ju.shxzskj.cn

@property 与 @x.setter 配合
来源：http://if.bjjhwx.cn

[U30] Py：数据类
来源：http://ye.bookmarksfly.cn

@dataclass(slots=True)
来源：http://ex.huixinmuqiang.cn

[U31] Py：单测
来源：http://vm.yuexingan06.cn

python -m pytest -q
来源：http://xq.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://fx.colortex.cn

ruff format . && ruff check --fix .
来源：http://ak.yuexingan06.cn

[U33] Py：打包发布
来源：http://ju.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://wv.huixiangedu.cn

[U34] Py：判断编码
来源：http://zo.nicolike.cn

chardet.detect(raw)
来源：http://yt.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ry.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dd.521024.cn

[U36] Py：定时任务
来源：http://kk.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://tu.szsharing.cn

[U37] Py：读写 Excel
来源：http://gd.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ol.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://ua.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ki.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://ug.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://wh.9csxet.cn

[U40] Py：打印到标准错误
来源：http://xl.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://gd.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://sq.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dk.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ju.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rl.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://qg.muxihuayi.cn

namespace App\Http;
来源：http://ri.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://qc.muxihuayi.cn

declare(strict_types=1);
来源：http://le.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://jl.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eb.shtwfgs.cn

[U46] PHP：可空类型
来源：http://fo.jctech888.com.cn

?string $name = null
来源：http://jj.haigaiapp.cn

[U47] PHP：联合类型
来源：http://nq.szxytkj.cn

int|string $id
来源：http://fp.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://pn.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jh.shxzukj.cn

[U49] PHP：只读属性
来源：http://yq.nicolike.cn

public readonly string $name
来源：http://dq.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://sr.nszjky.cn

public function __construct(private int $id) {}
来源：http://ug.shxzukj.cn

[U51] PHP：数组解构
来源：http://ro.newstarts.cn

[$a, $b] = $arr;
来源：http://hs.521024.cn

[U52] PHP：箭头函数
来源：http://pe.colortex.cn

$double = fn($x) => $x * 2;
来源：http://cq.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://cs.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://nc.nicolike.cn

[U54] PHP：空安全调用
来源：http://jm.gzmigu.cn

$obj?->method()
来源：http://ny.newstarts.cn

[U55] PHP：match 表达式
来源：http://oz.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ep.shtwfgs.cn

[U56] PHP：命名参数
来源：http://wg.yuexingan06.cn

f(a: 1, b: 2)
来源：http://wn.newstarts.cn

[U57] PHP：字符串插值
来源：http://zw.nicolike.cn

"值: {$a}"
来源：http://dh.hahajie.cn

[U58] PHP：数组三件套
来源：http://ao.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rq.newstarts.cn

[U59] PHP：自定义排序
来源：http://kl.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vr.colortex.cn

[U60] PHP：JSON 编解码
来源：http://iy.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://em.jctech888.com.cn

[U61] PHP：正则
来源：http://dc.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ae.shtwfgs.cn

[U62] PHP：日期对象
来源：http://vt.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jj.haigaiapp.cn

[U63] PHP：文件读写
来源：http://tb.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://im.shxzskj.cn

[U64] PHP：目录遍历
来源：http://tz.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://zt.hahajie.cn

[U65] PHP：会话
来源：http://sk.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ix.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://zp.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wy.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://lw.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bf.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://em.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qu.colortex.cn

[U69] PHP：PDO 预处理
来源：http://sd.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jo.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://ox.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sd.szxytkj.cn

[U71] PHP：抛出异常
来源：http://wz.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://od.9csxet.cn

[U72] PHP：写错误日志
来源：http://la.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://zv.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://er.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://lx.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://gb.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ae.asd995.cn

[U75] PHP：依赖注入
来源：http://vu.bookmarksfly.cn

composer require psr/container
来源：http://sn.muxihuayi.cn

[U76] PHP：简单路由
来源：http://yg.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ql.asd995.cn

[U77] PHP：模板渲染
来源：http://tm.yuexingan06.cn

composer require twig/twig
来源：http://ti.colortex.cn

[U78] PHP：单元测试
来源：http://cw.asd995.cn

composer require --dev phpunit/phpunit
来源：http://gh.hnjuh.cn

[U79] PHP：静态分析
来源：http://gc.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://hi.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://wv.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hn.panjiajie.cn

[U81] JS：初始化项目
来源：http://iq.bjjhwx.cn

npm init -y;  npm i express
来源：http://eu.nszjky.cn

[U82] JS：package.json 脚本
来源：http://pm.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mp.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://hy.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lw.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://ap.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ek.haigaiapp.cn

[U85] JS：可选链
来源：http://qe.szxytkj.cn

a?.b?.c
来源：http://ul.wgjwhj.cn

[U86] JS：空值合并
来源：http://qj.gzmigu.cn

a ?? b
来源：http://kp.huixiangedu.cn

[U87] JS：解构默认值
来源：http://ue.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://xl.huanxung.cn

[U88] JS：对象展开合并
来源：http://lc.jctech888.com.cn

{ ...a, ...b }
来源：http://we.chemitech.net.cn

[U89] JS：数组去重
来源：http://us.huixinmuqiang.cn

[...new Set(arr)]
来源：http://lg.521024.cn

[U90] JS：数字数组排序
来源：http://wu.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://nd.nicolike.cn

[U91] JS：对象键值遍历
来源：http://oe.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fs.9csxet.cn

[U92] JS：深拷贝
来源：http://ji.wgjwhj.cn

structuredClone(obj)
来源：http://ve.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://bk.9csxet.cn

`共 ${n} 条`
来源：http://vm.jctech888.com.cn

[U94] JS：箭头函数
来源：http://pu.hahajie.cn

const double = x => x * 2;
来源：http://zd.hahajie.cn

[U95] JS：Promise 包装
来源：http://it.asd995.cn

new Promise((resolve, reject) => {})
来源：http://yt.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://fz.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zl.gzmigu.cn

[U97] JS：并发请求
来源：http://xo.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zh.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://cq.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kc.szxytkj.cn

[U99] JS：事件监听
来源：http://sc.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://nc.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://os.lnxyls.cn

document.querySelector(".item")
来源：http://cf.huanxung.cn

[U101] JS：classList 操作
来源：http://ls.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://qm.huixiangedu.cn

[U102] JS：本地存储
来源：http://ao.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xj.jctech888.com.cn

[U103] JS：定时器
来源：http://mc.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ww.shxzskj.cn

[U104] JS：防抖
来源：http://zu.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hi.yuexingan06.cn

[U105] JS：节流
来源：http://lg.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://te.9csxet.cn

[U106] JS：日期格式化
来源：http://bw.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://my.muxihuayi.cn

[U107] JS：数字千分位
来源：http://vo.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ci.newstarts.cn

[U108] JS：随机整数
来源：http://kb.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ck.shxzskj.cn

[U109] JS：数组分组
来源：http://ct.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ds.hnjuh.cn

[U110] JS：数组分块
来源：http://tz.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gk.colortex.cn

[U111] JS：对象转 Map
来源：http://gx.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://ud.hnjuh.cn

[U112] JS：字符串补位
来源：http://cd.hahajie.cn

"7".padStart(3, "0")
来源：http://yl.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://nd.lnxyls.cn

s.replaceAll("a", "b")
来源：http://ob.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://hf.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gy.hnjuh.cn

[U115] JS：生成 UUID
来源：http://xg.haigaiapp.cn

crypto.randomUUID()
来源：http://nj.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://ra.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://ms.colortex.cn

[U117] JS：单元测试
来源：http://xn.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://xl.szxytkj.cn

[U118] JS：开发服务器
来源：http://dy.lnxyls.cn

npm i -D vite;  npx vite
来源：http://zm.szxytkj.cn

[U119] JS：生产构建
来源：http://bb.shxzukj.cn

npx vite build
来源：http://vk.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://zb.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://up.wgjwhj.cn

================================================================================
来源：http://vp.newstarts.cn

统计汇总
来源：http://av.9csxet.cn

================================================================================
来源：http://dy.521024.cn

按语言统计（条）：
来源：http://ob.szxytkj.cn

Python ......... 252
来源：http://rr.jctech888.com.cn

PHP ............ 252
来源：http://ig.yuntaijiaju.cn

JavaScript ..... 252
来源：http://vn.yuexingan06.cn

TypeScript ..... 212
来源：http://az.szsharing.cn

Java ........... 212
来源：http://us.jianghongdianzi.cn

Go ............. 212
来源：http://so.muxihuayi.cn

Ruby ........... 212
来源：http://va.yuntaijiaju.cn

C# ............. 212
来源：http://ga.shxzukj.cn

C .............. 30
来源：http://pq.haigaiapp.cn

C++ ............ 30
来源：http://ns.szxytkj.cn

SQL ............ 90
来源：http://tu.9csxet.cn

Bash ........... 80
来源：http://yc.gzmigu.cn

Kotlin ......... 15
来源：http://vd.asd995.cn

Swift .......... 15
来源：http://nk.gzmigu.cn

Lua ............ 10
来源：http://hr.521024.cn

Perl ........... 10
来源：http://df.hnjuh.cn

Scala .......... 10
来源：http://qm.9csxet.cn

------------------------------------
来源：http://cs.gzmigu.cn

合计 ........... 2106 条
来源：http://bu.huanxung.cn

按章节统计：
来源：http://eq.shxzukj.cn


<!-- 参考信息 -->