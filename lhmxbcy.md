代发 wailian999

[T49] Perl：函数
来源：http://ab.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zr.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://wa.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bn.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ju.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://cj.nszjky.cn

println("Hello")
来源：http://pt.hnjuh.cn

[T52] Scala：变量
来源：http://kv.muxihuayi.cn

val a = 1;  var b = 2
来源：http://xg.colortex.cn

[T53] Scala：字符串插值
来源：http://ad.jctech888.com.cn

s"值: $b"
来源：http://dy.huanxung.cn

[T54] Scala：集合映射
来源：http://vu.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://xz.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://zm.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rv.hnjuh.cn

[T56] Scala：样例类
来源：http://he.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://xl.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://ko.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cq.muxihuayi.cn

[T58] Scala：函数定义
来源：http://gy.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ff.chemitech.net.cn

[T59] Scala：循环
来源：http://ee.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://fr.bjjhwx.cn

[T60] Scala：折叠
来源：http://kk.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xz.bookmarksfly.cn

================================================================================
来源：http://we.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gp.haigaiapp.cn

================================================================================
来源：http://ud.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://qy.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qh.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://in.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bl.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://jq.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ek.hahajie.cn

[U04] Py：变量调试打印
来源：http://rn.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zq.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://vc.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://ew.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://sw.asd995.cn

{**a, **b}
来源：http://jd.panjiajie.cn

[U07] Py：反转字典键值
来源：http://hj.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://xi.gzmigu.cn

[U08] Py：展平二维列表
来源：http://qi.shxzukj.cn

[y for x in nested for y in x]
来源：http://ze.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://ol.jianghongdianzi.cn

max(d, key=d.get)
来源：http://kc.nszjky.cn

[U10] Py：按值排序字典
来源：http://jc.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mp.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://bk.nszjky.cn

(x * 2 for x in arr)
来源：http://mf.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zl.szxytkj.cn

Counter(arr).most_common(3)
来源：http://bo.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://hg.hahajie.cn

deque(maxlen=10)
来源：http://rl.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://pd.yuexingan06.cn

defaultdict(list)
来源：http://vx.huanxung.cn

[U15] Py：高精度计时
来源：http://nd.yuntaijiaju.cn

t = time.perf_counter()
来源：http://zb.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://mm.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yc.newstarts.cn

[U17] Py：初始化日志
来源：http://yr.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://fa.chemitech.net.cn

[U18] Py：预编译正则
来源：http://hv.hahajie.cn

pat = re.compile(r"\d+")
来源：http://lh.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://wb.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sr.nicolike.cn

[U20] Py：缓存函数结果
来源：http://to.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://dd.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ok.bjjhwx.cn

@contextlib.contextmanager
来源：http://os.panjiajie.cn

[U22] Py：矩阵转置
来源：http://wr.huanxung.cn

list(zip(*m))
来源：http://nv.colortex.cn

[U23] Py：分块读取大文件
来源：http://pm.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ia.newstarts.cn

[U24] Py：路径操作
来源：http://re.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://et.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ms.nszjky.cn

csv.DictReader(f)
来源：http://ss.yuexingan06.cn

[U26] Py：并发下载
来源：http://wm.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pm.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://ms.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://lm.haigaiapp.cn

[U28] Py：类型别名
来源：http://wf.wgjwhj.cn

UserId = int
来源：http://dy.nszjky.cn

[U29] Py：属性校验
来源：http://tf.shxzskj.cn

@property 与 @x.setter 配合
来源：http://zu.yuntaijiaju.cn

[U30] Py：数据类
来源：http://dk.9csxet.cn

@dataclass(slots=True)
来源：http://so.panjiajie.cn

[U31] Py：单测
来源：http://jt.shxzskj.cn

python -m pytest -q
来源：http://wz.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://hn.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://rb.muxihuayi.cn

[U33] Py：打包发布
来源：http://sy.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://xs.newstarts.cn

[U34] Py：判断编码
来源：http://px.bjjhwx.cn

chardet.detect(raw)
来源：http://kr.wgjwhj.cn

[U35] Py：发送邮件
来源：http://dk.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wv.haigaiapp.cn

[U36] Py：定时任务
来源：http://ek.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ua.nszjky.cn

[U37] Py：读写 Excel
来源：http://vo.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wl.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://ve.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://tq.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://dk.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://df.nicolike.cn

[U40] Py：打印到标准错误
来源：http://va.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://ro.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rg.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uk.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://il.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fc.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://aq.nszjky.cn

namespace App\Http;
来源：http://jj.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://jj.chemitech.net.cn

declare(strict_types=1);
来源：http://kd.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://pi.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tt.shtwfgs.cn

[U46] PHP：可空类型
来源：http://ms.szsharing.cn

?string $name = null
来源：http://bs.hnjuh.cn

[U47] PHP：联合类型
来源：http://yj.yuntaijiaju.cn

int|string $id
来源：http://tc.colortex.cn

[U48] PHP：纯枚举
来源：http://ss.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://da.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://ji.bjjhwx.cn

public readonly string $name
来源：http://we.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://ba.shxzskj.cn

public function __construct(private int $id) {}
来源：http://fj.asd995.cn

[U51] PHP：数组解构
来源：http://pd.muxihuayi.cn

[$a, $b] = $arr;
来源：http://jq.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://kw.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://up.newstarts.cn

[U53] PHP：空合并运算符
来源：http://od.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://lf.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://xa.shxzskj.cn

$obj?->method()
来源：http://yb.gzmigu.cn

[U55] PHP：match 表达式
来源：http://ub.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kw.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://xz.szxytkj.cn

f(a: 1, b: 2)
来源：http://wz.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://xt.wgjwhj.cn

"值: {$a}"
来源：http://ek.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://ri.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nh.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://ha.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ve.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://sp.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ei.hahajie.cn

[U61] PHP：正则
来源：http://us.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ux.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://ip.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vo.lnxyls.cn

[U63] PHP：文件读写
来源：http://lf.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hi.asd995.cn

[U64] PHP：目录遍历
来源：http://ah.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://bi.bjjhwx.cn

[U65] PHP：会话
来源：http://zb.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gj.521024.cn

[U66] PHP：设置 Cookie
来源：http://ng.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yv.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://yx.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ja.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://pc.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yu.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://zk.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vd.szsharing.cn

[U70] PHP：PDO 事务
来源：http://pc.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zx.nicolike.cn

[U71] PHP：抛出异常
来源：http://qf.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://kp.521024.cn

[U72] PHP：写错误日志
来源：http://me.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://hd.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://me.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://ho.szsharing.cn

[U74] PHP：读取环境变量
来源：http://bu.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://bw.nicolike.cn

[U75] PHP：依赖注入
来源：http://id.jctech888.com.cn

composer require psr/container
来源：http://lz.chemitech.net.cn

[U76] PHP：简单路由
来源：http://bf.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yr.szsharing.cn

[U77] PHP：模板渲染
来源：http://zi.haigaiapp.cn

composer require twig/twig
来源：http://lg.panjiajie.cn

[U78] PHP：单元测试
来源：http://ku.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://ko.haigaiapp.cn

[U79] PHP：静态分析
来源：http://ml.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://iq.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://fv.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ab.shtwfgs.cn

[U81] JS：初始化项目
来源：http://rp.huanxung.cn

npm init -y;  npm i express
来源：http://vm.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://ff.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://of.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://lo.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://by.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://wr.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rm.hnjuh.cn

[U85] JS：可选链
来源：http://tz.shtwfgs.cn

a?.b?.c
来源：http://az.muxihuayi.cn

[U86] JS：空值合并
来源：http://yi.colortex.cn

a ?? b
来源：http://co.huanxung.cn

[U87] JS：解构默认值
来源：http://gl.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://oc.nicolike.cn

[U88] JS：对象展开合并
来源：http://qs.bookmarksfly.cn

{ ...a, ...b }
来源：http://bf.huixiangedu.cn

[U89] JS：数组去重
来源：http://ve.gzmigu.cn

[...new Set(arr)]
来源：http://va.shxzukj.cn

[U90] JS：数字数组排序
来源：http://wy.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://eb.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://wv.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vw.bjjhwx.cn

[U92] JS：深拷贝
来源：http://ye.bjjhwx.cn

structuredClone(obj)
来源：http://bd.hnjuh.cn

[U93] JS：模板字符串
来源：http://km.nicolike.cn

`共 ${n} 条`
来源：http://op.shxzskj.cn

[U94] JS：箭头函数
来源：http://gs.muxihuayi.cn

const double = x => x * 2;
来源：http://kh.lnxyls.cn

[U95] JS：Promise 包装
来源：http://sm.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://ia.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://fy.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ur.wgjwhj.cn

[U97] JS：并发请求
来源：http://my.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://os.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://ik.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wq.jctech888.com.cn

[U99] JS：事件监听
来源：http://rp.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://vy.panjiajie.cn

[U100] JS：DOM 查询
来源：http://jo.colortex.cn

document.querySelector(".item")
来源：http://ld.szsharing.cn

[U101] JS：classList 操作
来源：http://di.hahajie.cn

el.classList.toggle("active")
来源：http://yc.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://bb.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://if.jianghongdianzi.cn

[U103] JS：定时器
来源：http://le.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://in.9csxet.cn

[U104] JS：防抖
来源：http://lv.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ks.yuntaijiaju.cn

[U105] JS：节流
来源：http://dd.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rv.gzmigu.cn

[U106] JS：日期格式化
来源：http://mc.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qu.hnjuh.cn

[U107] JS：数字千分位
来源：http://jv.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iv.yuexingan06.cn

[U108] JS：随机整数
来源：http://sk.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ky.nszjky.cn

[U109] JS：数组分组
来源：http://sd.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://gp.9csxet.cn

[U110] JS：数组分块
来源：http://qs.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gq.lnxyls.cn

[U111] JS：对象转 Map
来源：http://pv.huanxung.cn

new Map(Object.entries(obj))
来源：http://uh.9csxet.cn

[U112] JS：字符串补位
来源：http://rc.colortex.cn

"7".padStart(3, "0")
来源：http://xk.newstarts.cn

[U113] JS：正则替换全部
来源：http://jl.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://gl.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://po.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pe.huanxung.cn

[U115] JS：生成 UUID
来源：http://cc.chemitech.net.cn

crypto.randomUUID()
来源：http://sn.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ss.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://rs.gzmigu.cn

[U117] JS：单元测试
来源：http://uq.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://dc.521024.cn

[U118] JS：开发服务器
来源：http://ra.hahajie.cn

npm i -D vite;  npx vite
来源：http://py.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://pd.shtwfgs.cn

npx vite build
来源：http://nt.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://dy.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://le.jianghongdianzi.cn

================================================================================
来源：http://sv.haigaiapp.cn

统计汇总
来源：http://ni.panjiajie.cn

================================================================================
来源：http://jd.newstarts.cn

按语言统计（条）：
来源：http://xx.bookmarksfly.cn

Python ......... 252
来源：http://fj.shxzskj.cn

PHP ............ 252
来源：http://bh.gzmigu.cn

JavaScript ..... 252
来源：http://ji.jianghongdianzi.cn

TypeScript ..... 212
来源：http://nw.lnxyls.cn

Java ........... 212
来源：http://yh.jctech888.com.cn

Go ............. 212
来源：http://yv.huixiangedu.cn

Ruby ........... 212
来源：http://ae.chemitech.net.cn

C# ............. 212
来源：http://uo.bjjhwx.cn

C .............. 30
来源：http://cf.muxihuayi.cn

C++ ............ 30
来源：http://ua.huixiangedu.cn

SQL ............ 90
来源：http://pn.hnjuh.cn

Bash ........... 80
来源：http://zc.nicolike.cn

Kotlin ......... 15
来源：http://iy.huixiangedu.cn

Swift .......... 15
来源：http://cz.9csxet.cn

Lua ............ 10
来源：http://fd.9csxet.cn

Perl ........... 10
来源：http://vy.bookmarksfly.cn

Scala .......... 10
来源：http://lt.colortex.cn

------------------------------------
来源：http://ek.shxzukj.cn

合计 ........... 2106 条
来源：http://yc.gzmigu.cn

按章节统计：
来源：http://jo.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lj.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ew.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bn.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lx.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bb.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ft.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tb.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cp.huixiangedu.cn


<!-- 参考信息 -->