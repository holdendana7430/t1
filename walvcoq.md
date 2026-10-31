代发 wailian999

[T43] Perl：字符串插值
来源：http://cx.gzmigu.cn

"值: $a"
来源：http://uk.colortex.cn

[T44] Perl：条件
来源：http://ma.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://qs.lnxyls.cn

[T45] Perl：数组遍历
来源：http://cq.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://tc.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://wh.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tr.panjiajie.cn

[T47] Perl：正则捕获
来源：http://mo.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zq.lnxyls.cn

[T48] Perl：正则替换
来源：http://jg.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ml.gzmigu.cn

[T49] Perl：函数
来源：http://fk.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zw.newstarts.cn

[T50] Perl：逐行读文件
来源：http://ld.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tr.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://lj.huanxung.cn

[T51] Scala：Hello World
来源：http://fa.shtwfgs.cn

println("Hello")
来源：http://xa.yuntaijiaju.cn

[T52] Scala：变量
来源：http://uf.nszjky.cn

val a = 1;  var b = 2
来源：http://no.nszjky.cn

[T53] Scala：字符串插值
来源：http://tj.shxzukj.cn

s"值: $b"
来源：http://nl.bjjhwx.cn

[T54] Scala：集合映射
来源：http://rd.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://yd.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://tf.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://an.shxzskj.cn

[T56] Scala：样例类
来源：http://bq.szxytkj.cn

case class User(name: String, age: Int)
来源：http://gh.szxytkj.cn

[T57] Scala：模式匹配
来源：http://bz.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xq.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://zz.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fl.newstarts.cn

[T59] Scala：循环
来源：http://mb.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://gj.colortex.cn

[T60] Scala：折叠
来源：http://ny.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lj.nszjky.cn

================================================================================
来源：http://iq.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://al.gzmigu.cn

================================================================================
来源：http://mj.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://ju.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dc.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://wa.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ck.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://bz.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qk.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ip.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zl.szsharing.cn

[U05] Py：列表去重且保序
来源：http://uj.asd995.cn

list(dict.fromkeys(arr))
来源：http://dr.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://vn.nszjky.cn

{**a, **b}
来源：http://ew.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://qd.newstarts.cn

{v: k for k, v in d.items()}
来源：http://kr.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://jz.haigaiapp.cn

[y for x in nested for y in x]
来源：http://hx.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://zf.gzmigu.cn

max(d, key=d.get)
来源：http://vj.gzmigu.cn

[U10] Py：按值排序字典
来源：http://so.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lf.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://tf.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://tz.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qk.hahajie.cn

Counter(arr).most_common(3)
来源：http://sh.gzmigu.cn

[U13] Py：固定长度队列
来源：http://bc.hnjuh.cn

deque(maxlen=10)
来源：http://vq.newstarts.cn

[U14] Py：分组收集到列表
来源：http://ro.9csxet.cn

defaultdict(list)
来源：http://ew.shxzskj.cn

[U15] Py：高精度计时
来源：http://ag.lnxyls.cn

t = time.perf_counter()
来源：http://na.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://rk.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hl.hnjuh.cn

[U17] Py：初始化日志
来源：http://kf.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://xw.shxzskj.cn

[U18] Py：预编译正则
来源：http://rt.huanxung.cn

pat = re.compile(r"\d+")
来源：http://qz.colortex.cn

[U19] Py：正则替换带回调
来源：http://xw.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iz.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://wk.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://md.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://ac.jctech888.com.cn

@contextlib.contextmanager
来源：http://tw.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://gk.hahajie.cn

list(zip(*m))
来源：http://qf.hahajie.cn

[U23] Py：分块读取大文件
来源：http://hu.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xh.colortex.cn

[U24] Py：路径操作
来源：http://qu.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://in.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://zw.jctech888.com.cn

csv.DictReader(f)
来源：http://mr.yuexingan06.cn

[U26] Py：并发下载
来源：http://aq.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pa.hahajie.cn

[U27] Py：异步 HTTP
来源：http://sp.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://rr.szsharing.cn

[U28] Py：类型别名
来源：http://ou.wgjwhj.cn

UserId = int
来源：http://zq.wgjwhj.cn

[U29] Py：属性校验
来源：http://ur.shxzskj.cn

@property 与 @x.setter 配合
来源：http://an.nszjky.cn

[U30] Py：数据类
来源：http://mi.yuexingan06.cn

@dataclass(slots=True)
来源：http://qz.muxihuayi.cn

[U31] Py：单测
来源：http://ch.wgjwhj.cn

python -m pytest -q
来源：http://nw.huixiangedu.cn

[U32] Py：代码格式化
来源：http://wv.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://hu.nicolike.cn

[U33] Py：打包发布
来源：http://zp.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://ie.asd995.cn

[U34] Py：判断编码
来源：http://gp.shtwfgs.cn

chardet.detect(raw)
来源：http://ci.szsharing.cn

[U35] Py：发送邮件
来源：http://ne.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hk.colortex.cn

[U36] Py：定时任务
来源：http://gj.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://yv.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://pa.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mx.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://iv.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://zh.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://sa.jctech888.com.cn

sys.stdout.isatty()
来源：http://ne.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://mb.nicolike.cn

print("err", file=sys.stderr)
来源：http://cn.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://kv.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xl.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://dr.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gz.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://uh.asd995.cn

namespace App\Http;
来源：http://bo.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://mj.haigaiapp.cn

declare(strict_types=1);
来源：http://lc.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://ld.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://su.muxihuayi.cn

[U46] PHP：可空类型
来源：http://va.9csxet.cn

?string $name = null
来源：http://xr.colortex.cn

[U47] PHP：联合类型
来源：http://iz.gzmigu.cn

int|string $id
来源：http://im.hahajie.cn

[U48] PHP：纯枚举
来源：http://gs.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jk.huixiangedu.cn

[U49] PHP：只读属性
来源：http://yd.lnxyls.cn

public readonly string $name
来源：http://fv.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://lo.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://ik.chemitech.net.cn

[U51] PHP：数组解构
来源：http://lu.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ta.szsharing.cn

[U52] PHP：箭头函数
来源：http://ek.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://jf.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://pg.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://tb.nszjky.cn

[U54] PHP：空安全调用
来源：http://am.wgjwhj.cn

$obj?->method()
来源：http://vg.shxzskj.cn

[U55] PHP：match 表达式
来源：http://iq.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://td.colortex.cn

[U56] PHP：命名参数
来源：http://bn.shtwfgs.cn

f(a: 1, b: 2)
来源：http://hs.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://tn.lnxyls.cn

"值: {$a}"
来源：http://ma.nicolike.cn

[U58] PHP：数组三件套
来源：http://fc.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://as.hahajie.cn

[U59] PHP：自定义排序
来源：http://zu.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pl.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://kn.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fw.huixiangedu.cn

[U61] PHP：正则
来源：http://oo.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wg.newstarts.cn

[U62] PHP：日期对象
来源：http://xy.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://au.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://as.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gi.hnjuh.cn

[U64] PHP：目录遍历
来源：http://bc.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://wx.shxzukj.cn

[U65] PHP：会话
来源：http://qg.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hv.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://uo.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tl.huanxung.cn

[U67] PHP：处理文件上传
来源：http://nr.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ux.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://zw.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ux.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://ks.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lv.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://vf.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zj.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://bc.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://ks.gzmigu.cn

[U72] PHP：写错误日志
来源：http://eo.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://wg.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://np.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://vv.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://rf.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://id.lnxyls.cn

[U75] PHP：依赖注入
来源：http://cs.yuexingan06.cn

composer require psr/container
来源：http://uj.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://km.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pa.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://aj.nszjky.cn

composer require twig/twig
来源：http://vj.szsharing.cn

[U78] PHP：单元测试
来源：http://ut.521024.cn

composer require --dev phpunit/phpunit
来源：http://ni.newstarts.cn

[U79] PHP：静态分析
来源：http://zt.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://vq.colortex.cn

[U80] PHP：代码规范修复
来源：http://jj.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jy.asd995.cn

[U81] JS：初始化项目
来源：http://yg.9csxet.cn

npm init -y;  npm i express
来源：http://fl.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://zt.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xx.521024.cn

[U83] JS：ES Module 导入导出
来源：http://ir.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aw.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://ie.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rs.hnjuh.cn

[U85] JS：可选链
来源：http://co.chemitech.net.cn

a?.b?.c
来源：http://rp.hahajie.cn

[U86] JS：空值合并
来源：http://bz.chemitech.net.cn

a ?? b
来源：http://va.gzmigu.cn

[U87] JS：解构默认值
来源：http://qf.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://xs.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://tw.9csxet.cn

{ ...a, ...b }
来源：http://wg.521024.cn

[U89] JS：数组去重
来源：http://wa.szxytkj.cn

[...new Set(arr)]
来源：http://jv.szsharing.cn

[U90] JS：数字数组排序
来源：http://ei.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://lp.asd995.cn

[U91] JS：对象键值遍历
来源：http://zl.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hr.haigaiapp.cn

[U92] JS：深拷贝
来源：http://yw.gzmigu.cn

structuredClone(obj)
来源：http://eg.chemitech.net.cn

[U93] JS：模板字符串
来源：http://pv.colortex.cn

`共 ${n} 条`
来源：http://kc.panjiajie.cn

[U94] JS：箭头函数
来源：http://iv.wgjwhj.cn

const double = x => x * 2;
来源：http://tg.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://xy.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://xv.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://zw.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ia.bjjhwx.cn

[U97] JS：并发请求
来源：http://tl.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ox.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://pj.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oa.huixiangedu.cn

[U99] JS：事件监听
来源：http://jt.newstarts.cn

el.addEventListener("click", e => {})
来源：http://qi.asd995.cn

[U100] JS：DOM 查询
来源：http://vj.panjiajie.cn

document.querySelector(".item")
来源：http://la.huixiangedu.cn

[U101] JS：classList 操作
来源：http://ek.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://ct.nicolike.cn

[U102] JS：本地存储
来源：http://ww.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gf.huixinmuqiang.cn

[U103] JS：定时器
来源：http://gi.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ls.shxzskj.cn

[U104] JS：防抖
来源：http://jz.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://me.haigaiapp.cn

[U105] JS：节流
来源：http://xn.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gk.shxzukj.cn

[U106] JS：日期格式化
来源：http://pr.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vt.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://qj.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lw.bjjhwx.cn

[U108] JS：随机整数
来源：http://pl.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://up.asd995.cn

[U109] JS：数组分组
来源：http://qu.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://wc.szsharing.cn

[U110] JS：数组分块
来源：http://oo.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yb.colortex.cn

[U111] JS：对象转 Map
来源：http://we.lnxyls.cn

new Map(Object.entries(obj))
来源：http://pz.shtwfgs.cn

[U112] JS：字符串补位
来源：http://nd.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://ge.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://yq.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://fb.colortex.cn

[U114] JS：JSON 深比较
来源：http://aq.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jd.lnxyls.cn

[U115] JS：生成 UUID
来源：http://ty.jianghongdianzi.cn

crypto.randomUUID()
来源：http://ci.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://jm.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://wn.gzmigu.cn

[U117] JS：单元测试
来源：http://hq.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ve.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://ls.shxzukj.cn

npm i -D vite;  npx vite
来源：http://lk.jctech888.com.cn

[U119] JS：生产构建
来源：http://ti.shtwfgs.cn

npx vite build
来源：http://gh.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://gq.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://to.huanxung.cn

================================================================================
来源：http://yv.bjjhwx.cn

统计汇总
来源：http://np.huixinmuqiang.cn

================================================================================
来源：http://rf.panjiajie.cn

按语言统计（条）：
来源：http://yc.chemitech.net.cn

Python ......... 252
来源：http://wj.9csxet.cn

PHP ............ 252
来源：http://kg.hnjuh.cn

JavaScript ..... 252
来源：http://ew.haigaiapp.cn

TypeScript ..... 212
来源：http://dt.chemitech.net.cn

Java ........... 212
来源：http://ia.wgjwhj.cn

Go ............. 212
来源：http://zf.nicolike.cn

Ruby ........... 212
来源：http://vl.hnjuh.cn

C# ............. 212
来源：http://bj.huanxung.cn

C .............. 30
来源：http://np.nszjky.cn

C++ ............ 30
来源：http://oa.newstarts.cn

SQL ............ 90
来源：http://ls.panjiajie.cn

Bash ........... 80
来源：http://yu.haigaiapp.cn

Kotlin ......... 15
来源：http://yq.jctech888.com.cn

Swift .......... 15
来源：http://lv.hahajie.cn

Lua ............ 10
来源：http://qi.szsharing.cn

Perl ........... 10
来源：http://cy.huixinmuqiang.cn


<!-- 参考信息 -->