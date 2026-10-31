代发 wailian999

[T45] Perl：数组遍历
来源：http://xq.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://sz.colortex.cn

[T46] Perl：哈希操作
来源：http://jt.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ug.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://dp.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xk.haigaiapp.cn

[T48] Perl：正则替换
来源：http://hj.521024.cn

$s =~ s/old/new/g;
来源：http://et.newstarts.cn

[T49] Perl：函数
来源：http://oe.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uc.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://gh.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://et.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://tp.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://sy.shxzskj.cn

println("Hello")
来源：http://bt.asd995.cn

[T52] Scala：变量
来源：http://mx.lnxyls.cn

val a = 1;  var b = 2
来源：http://sv.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://gc.szsharing.cn

s"值: $b"
来源：http://it.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://fc.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://mz.szsharing.cn

[T55] Scala：集合过滤
来源：http://zr.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qw.muxihuayi.cn

[T56] Scala：样例类
来源：http://ki.hnjuh.cn

case class User(name: String, age: Int)
来源：http://vj.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://yo.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fg.9csxet.cn

[T58] Scala：函数定义
来源：http://ne.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vz.jianghongdianzi.cn

[T59] Scala：循环
来源：http://iw.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ak.9csxet.cn

[T60] Scala：折叠
来源：http://vj.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ve.lnxyls.cn

================================================================================
来源：http://uk.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ny.panjiajie.cn

================================================================================
来源：http://hq.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://px.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uk.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://rk.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kv.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://zk.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hu.asd995.cn

[U04] Py：变量调试打印
来源：http://aj.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hr.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://fu.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://ml.newstarts.cn

[U06] Py：合并两个字典
来源：http://hk.asd995.cn

{**a, **b}
来源：http://vj.nszjky.cn

[U07] Py：反转字典键值
来源：http://em.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://mn.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://mc.gzmigu.cn

[y for x in nested for y in x]
来源：http://eo.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://qn.huixiangedu.cn

max(d, key=d.get)
来源：http://pt.9csxet.cn

[U10] Py：按值排序字典
来源：http://ra.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://um.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://zk.jctech888.com.cn

(x * 2 for x in arr)
来源：http://zg.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uc.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://ei.colortex.cn

[U13] Py：固定长度队列
来源：http://wf.shtwfgs.cn

deque(maxlen=10)
来源：http://xq.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://sh.haigaiapp.cn

defaultdict(list)
来源：http://ox.panjiajie.cn

[U15] Py：高精度计时
来源：http://qe.lnxyls.cn

t = time.perf_counter()
来源：http://mi.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://mo.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ek.szxytkj.cn

[U17] Py：初始化日志
来源：http://jh.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://zw.huixiangedu.cn

[U18] Py：预编译正则
来源：http://yb.hahajie.cn

pat = re.compile(r"\d+")
来源：http://wk.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://tp.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pk.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://iv.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://tq.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://zv.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ey.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://rx.bookmarksfly.cn

list(zip(*m))
来源：http://sz.asd995.cn

[U23] Py：分块读取大文件
来源：http://uo.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ex.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://wc.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iw.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://dc.shtwfgs.cn

csv.DictReader(f)
来源：http://ol.newstarts.cn

[U26] Py：并发下载
来源：http://qq.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cq.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://jf.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://vf.jctech888.com.cn

[U28] Py：类型别名
来源：http://jo.nszjky.cn

UserId = int
来源：http://zl.colortex.cn

[U29] Py：属性校验
来源：http://oo.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://uy.shxzukj.cn

[U30] Py：数据类
来源：http://da.panjiajie.cn

@dataclass(slots=True)
来源：http://dc.hahajie.cn

[U31] Py：单测
来源：http://ul.hnjuh.cn

python -m pytest -q
来源：http://ok.521024.cn

[U32] Py：代码格式化
来源：http://zi.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://eq.gzmigu.cn

[U33] Py：打包发布
来源：http://al.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ji.jctech888.com.cn

[U34] Py：判断编码
来源：http://is.hahajie.cn

chardet.detect(raw)
来源：http://kt.newstarts.cn

[U35] Py：发送邮件
来源：http://qa.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uv.muxihuayi.cn

[U36] Py：定时任务
来源：http://cz.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://qc.shxzskj.cn

[U37] Py：读写 Excel
来源：http://gq.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rx.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://wv.newstarts.cn

Path(__file__).resolve().parent
来源：http://vx.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://fs.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://al.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://aq.asd995.cn

print("err", file=sys.stderr)
来源：http://gv.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://vc.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cp.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://jb.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xq.hahajie.cn

[U43] PHP：声明命名空间
来源：http://eb.gzmigu.cn

namespace App\Http;
来源：http://mb.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://qf.shxzskj.cn

declare(strict_types=1);
来源：http://tp.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://fo.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sj.jctech888.com.cn

[U46] PHP：可空类型
来源：http://my.huixinmuqiang.cn

?string $name = null
来源：http://rn.chemitech.net.cn

[U47] PHP：联合类型
来源：http://og.shtwfgs.cn

int|string $id
来源：http://mm.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://na.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://us.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://dk.haigaiapp.cn

public readonly string $name
来源：http://zu.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://me.panjiajie.cn

public function __construct(private int $id) {}
来源：http://ci.gzmigu.cn

[U51] PHP：数组解构
来源：http://ei.szsharing.cn

[$a, $b] = $arr;
来源：http://qw.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://us.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://cz.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://bg.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://tl.asd995.cn

[U54] PHP：空安全调用
来源：http://zv.hahajie.cn

$obj?->method()
来源：http://za.szxytkj.cn

[U55] PHP：match 表达式
来源：http://gj.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ay.chemitech.net.cn

[U56] PHP：命名参数
来源：http://xh.lnxyls.cn

f(a: 1, b: 2)
来源：http://di.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://to.huixiangedu.cn

"值: {$a}"
来源：http://yq.colortex.cn

[U58] PHP：数组三件套
来源：http://nb.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ys.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://pm.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oa.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://kr.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hp.nicolike.cn

[U61] PHP：正则
来源：http://gv.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://od.nicolike.cn

[U62] PHP：日期对象
来源：http://ar.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wl.nszjky.cn

[U63] PHP：文件读写
来源：http://rp.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rb.hahajie.cn

[U64] PHP：目录遍历
来源：http://fo.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://vb.szsharing.cn

[U65] PHP：会话
来源：http://oc.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zi.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://gx.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rt.nszjky.cn

[U67] PHP：处理文件上传
来源：http://pm.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dj.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://em.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xj.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://xw.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lm.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://th.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://th.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://cm.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://pi.colortex.cn

[U72] PHP：写错误日志
来源：http://zt.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://pi.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://iv.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://wx.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://qm.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://ws.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://tj.nicolike.cn

composer require psr/container
来源：http://mw.szxytkj.cn

[U76] PHP：简单路由
来源：http://yz.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fk.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://kj.colortex.cn

composer require twig/twig
来源：http://vb.hnjuh.cn

[U78] PHP：单元测试
来源：http://rl.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://zz.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://kv.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://vu.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://fc.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ow.shxzukj.cn

[U81] JS：初始化项目
来源：http://gh.wgjwhj.cn

npm init -y;  npm i express
来源：http://gt.huanxung.cn

[U82] JS：package.json 脚本
来源：http://qd.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tm.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://sa.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gq.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://bl.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kg.nicolike.cn

[U85] JS：可选链
来源：http://ci.yuexingan06.cn

a?.b?.c
来源：http://ft.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://vv.haigaiapp.cn

a ?? b
来源：http://ic.jctech888.com.cn

[U87] JS：解构默认值
来源：http://bj.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://de.shxzukj.cn

[U88] JS：对象展开合并
来源：http://jl.bjjhwx.cn

{ ...a, ...b }
来源：http://au.colortex.cn

[U89] JS：数组去重
来源：http://lo.hnjuh.cn

[...new Set(arr)]
来源：http://ie.gzmigu.cn

[U90] JS：数字数组排序
来源：http://yt.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://ou.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://tk.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fl.hnjuh.cn

[U92] JS：深拷贝
来源：http://dn.nicolike.cn

structuredClone(obj)
来源：http://sq.huanxung.cn

[U93] JS：模板字符串
来源：http://qo.szsharing.cn

`共 ${n} 条`
来源：http://dk.colortex.cn

[U94] JS：箭头函数
来源：http://tx.huixiangedu.cn

const double = x => x * 2;
来源：http://mv.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ic.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://yc.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://po.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ra.colortex.cn

[U97] JS：并发请求
来源：http://wq.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qm.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ut.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xo.shxzukj.cn

[U99] JS：事件监听
来源：http://gx.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://la.521024.cn

[U100] JS：DOM 查询
来源：http://dn.gzmigu.cn

document.querySelector(".item")
来源：http://sq.huanxung.cn

[U101] JS：classList 操作
来源：http://ta.szsharing.cn

el.classList.toggle("active")
来源：http://wl.shxzukj.cn

[U102] JS：本地存储
来源：http://qz.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kf.jctech888.com.cn

[U103] JS：定时器
来源：http://kx.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lx.gzmigu.cn

[U104] JS：防抖
来源：http://tq.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.yuexingan06.cn

[U105] JS：节流
来源：http://bo.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wn.yuexingan06.cn

[U106] JS：日期格式化
来源：http://fk.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hm.shxzukj.cn

[U107] JS：数字千分位
来源：http://fk.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cf.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://oe.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://im.nszjky.cn

[U109] JS：数组分组
来源：http://vq.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://or.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://yk.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yi.huanxung.cn

[U111] JS：对象转 Map
来源：http://il.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://ab.wgjwhj.cn

[U112] JS：字符串补位
来源：http://mc.nszjky.cn

"7".padStart(3, "0")
来源：http://xu.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://jx.521024.cn

s.replaceAll("a", "b")
来源：http://tu.asd995.cn

[U114] JS：JSON 深比较
来源：http://hx.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vj.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://rs.panjiajie.cn

crypto.randomUUID()
来源：http://nc.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ea.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://mm.newstarts.cn

[U117] JS：单元测试
来源：http://zy.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://qt.hnjuh.cn

[U118] JS：开发服务器
来源：http://xz.lnxyls.cn

npm i -D vite;  npx vite
来源：http://iq.chemitech.net.cn

[U119] JS：生产构建
来源：http://hy.hahajie.cn

npx vite build
来源：http://ux.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://fr.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://cl.huixinmuqiang.cn

================================================================================
来源：http://pe.huixiangedu.cn

统计汇总
来源：http://vh.newstarts.cn

================================================================================
来源：http://lg.jianghongdianzi.cn

按语言统计（条）：
来源：http://hf.yuexingan06.cn

Python ......... 252
来源：http://ph.szsharing.cn

PHP ............ 252
来源：http://wx.hnjuh.cn

JavaScript ..... 252
来源：http://fi.shxzukj.cn

TypeScript ..... 212
来源：http://jq.panjiajie.cn

Java ........... 212
来源：http://zx.hnjuh.cn

Go ............. 212
来源：http://pm.hahajie.cn

Ruby ........... 212
来源：http://qi.jianghongdianzi.cn

C# ............. 212
来源：http://wt.bjjhwx.cn

C .............. 30
来源：http://iu.szxytkj.cn

C++ ............ 30
来源：http://ts.newstarts.cn

SQL ............ 90
来源：http://xz.yuntaijiaju.cn

Bash ........... 80
来源：http://xq.jianghongdianzi.cn

Kotlin ......... 15
来源：http://vv.lnxyls.cn

Swift .......... 15
来源：http://aj.huixinmuqiang.cn

Lua ............ 10
来源：http://fx.hnjuh.cn

Perl ........... 10
来源：http://ve.shxzskj.cn

Scala .......... 10
来源：http://dl.huixiangedu.cn

------------------------------------
来源：http://lj.nszjky.cn

合计 ........... 2106 条
来源：http://aq.nicolike.cn

按章节统计：
来源：http://on.huixinmuqiang.cn


<!-- 参考信息 -->