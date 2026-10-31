代发 wailian999

[T43] Perl：字符串插值
来源：http://dw.lnxyls.cn

"值: $a"
来源：http://mb.hnjuh.cn

[T44] Perl：条件
来源：http://hd.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://yt.nicolike.cn

[T45] Perl：数组遍历
来源：http://bc.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://xl.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://ai.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gz.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://uf.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xp.shtwfgs.cn

[T48] Perl：正则替换
来源：http://cc.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://en.shxzskj.cn

[T49] Perl：函数
来源：http://qr.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kt.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://fj.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rv.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://bi.asd995.cn

[T51] Scala：Hello World
来源：http://sv.asd995.cn

println("Hello")
来源：http://em.panjiajie.cn

[T52] Scala：变量
来源：http://yi.colortex.cn

val a = 1;  var b = 2
来源：http://ys.521024.cn

[T53] Scala：字符串插值
来源：http://qh.yuexingan06.cn

s"值: $b"
来源：http://uz.panjiajie.cn

[T54] Scala：集合映射
来源：http://gt.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ak.nicolike.cn

[T55] Scala：集合过滤
来源：http://df.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bu.gzmigu.cn

[T56] Scala：样例类
来源：http://km.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://bi.panjiajie.cn

[T57] Scala：模式匹配
来源：http://pn.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zn.521024.cn

[T58] Scala：函数定义
来源：http://zo.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://po.szxytkj.cn

[T59] Scala：循环
来源：http://mx.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://vr.wgjwhj.cn

[T60] Scala：折叠
来源：http://ba.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fv.wgjwhj.cn

================================================================================
来源：http://ks.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sb.521024.cn

================================================================================
来源：http://eh.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://jf.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wj.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://yl.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rt.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://fg.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sk.521024.cn

[U04] Py：变量调试打印
来源：http://jn.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pg.huanxung.cn

[U05] Py：列表去重且保序
来源：http://xk.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://qi.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://ps.szsharing.cn

{**a, **b}
来源：http://wt.asd995.cn

[U07] Py：反转字典键值
来源：http://bk.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://cg.hahajie.cn

[U08] Py：展平二维列表
来源：http://ed.muxihuayi.cn

[y for x in nested for y in x]
来源：http://gv.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ny.szsharing.cn

max(d, key=d.get)
来源：http://ar.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://lu.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oq.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://kx.chemitech.net.cn

(x * 2 for x in arr)
来源：http://ft.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bt.asd995.cn

Counter(arr).most_common(3)
来源：http://bb.colortex.cn

[U13] Py：固定长度队列
来源：http://ls.shxzukj.cn

deque(maxlen=10)
来源：http://dd.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ke.colortex.cn

defaultdict(list)
来源：http://es.newstarts.cn

[U15] Py：高精度计时
来源：http://sz.panjiajie.cn

t = time.perf_counter()
来源：http://ov.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://kn.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ks.9csxet.cn

[U17] Py：初始化日志
来源：http://rm.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ep.hnjuh.cn

[U18] Py：预编译正则
来源：http://ya.szsharing.cn

pat = re.compile(r"\d+")
来源：http://mj.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://hg.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ff.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://or.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://or.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://fb.panjiajie.cn

@contextlib.contextmanager
来源：http://ww.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://ne.haigaiapp.cn

list(zip(*m))
来源：http://og.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://fi.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qy.haigaiapp.cn

[U24] Py：路径操作
来源：http://qt.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bo.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://ga.szxytkj.cn

csv.DictReader(f)
来源：http://wv.chemitech.net.cn

[U26] Py：并发下载
来源：http://mf.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gl.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://xi.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://gl.colortex.cn

[U28] Py：类型别名
来源：http://wh.wgjwhj.cn

UserId = int
来源：http://bx.bookmarksfly.cn

[U29] Py：属性校验
来源：http://cj.hnjuh.cn

@property 与 @x.setter 配合
来源：http://yg.huanxung.cn

[U30] Py：数据类
来源：http://qg.chemitech.net.cn

@dataclass(slots=True)
来源：http://cc.colortex.cn

[U31] Py：单测
来源：http://yb.yuexingan06.cn

python -m pytest -q
来源：http://wt.asd995.cn

[U32] Py：代码格式化
来源：http://ul.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://wn.hahajie.cn

[U33] Py：打包发布
来源：http://fl.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://rd.szsharing.cn

[U34] Py：判断编码
来源：http://ba.bjjhwx.cn

chardet.detect(raw)
来源：http://uy.szsharing.cn

[U35] Py：发送邮件
来源：http://lw.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fy.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://dp.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ix.shxzukj.cn

[U37] Py：读写 Excel
来源：http://oc.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ca.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://nd.shxzukj.cn

Path(__file__).resolve().parent
来源：http://os.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://vq.wgjwhj.cn

sys.stdout.isatty()
来源：http://ry.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://re.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://pt.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://cs.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wz.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://xj.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aa.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://gi.nicolike.cn

namespace App\Http;
来源：http://us.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://rg.huanxung.cn

declare(strict_types=1);
来源：http://vm.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://he.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ie.9csxet.cn

[U46] PHP：可空类型
来源：http://nt.hahajie.cn

?string $name = null
来源：http://hz.lnxyls.cn

[U47] PHP：联合类型
来源：http://mt.nszjky.cn

int|string $id
来源：http://lt.szxytkj.cn

[U48] PHP：纯枚举
来源：http://ta.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xr.bjjhwx.cn

[U49] PHP：只读属性
来源：http://rg.huixiangedu.cn

public readonly string $name
来源：http://tz.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://zm.asd995.cn

public function __construct(private int $id) {}
来源：http://dn.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://js.wgjwhj.cn

[$a, $b] = $arr;
来源：http://rs.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://gf.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://mu.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://ck.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://lm.huanxung.cn

[U54] PHP：空安全调用
来源：http://mi.panjiajie.cn

$obj?->method()
来源：http://xa.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://er.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bb.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://ub.shtwfgs.cn

f(a: 1, b: 2)
来源：http://ps.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://gd.huixiangedu.cn

"值: {$a}"
来源：http://on.shxzskj.cn

[U58] PHP：数组三件套
来源：http://ci.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ws.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://mg.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cp.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://is.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://of.huixinmuqiang.cn

[U61] PHP：正则
来源：http://cy.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ob.jctech888.com.cn

[U62] PHP：日期对象
来源：http://zf.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ff.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://zc.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sd.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://be.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://rb.huixiangedu.cn

[U65] PHP：会话
来源：http://dm.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://er.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://ga.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wj.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://ka.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lk.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://pt.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pr.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://ug.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cx.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://sd.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ht.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://tg.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://lt.colortex.cn

[U72] PHP：写错误日志
来源：http://nf.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://zj.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://uu.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://tq.newstarts.cn

[U74] PHP：读取环境变量
来源：http://ch.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://ap.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://ai.yuntaijiaju.cn

composer require psr/container
来源：http://jn.huanxung.cn

[U76] PHP：简单路由
来源：http://je.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://em.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://it.jianghongdianzi.cn

composer require twig/twig
来源：http://qo.yuexingan06.cn

[U78] PHP：单元测试
来源：http://os.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://rx.9csxet.cn

[U79] PHP：静态分析
来源：http://db.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://an.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://su.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ym.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://pc.chemitech.net.cn

npm init -y;  npm i express
来源：http://dh.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://ou.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tk.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ow.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fz.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://rw.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xh.huixiangedu.cn

[U85] JS：可选链
来源：http://pg.wgjwhj.cn

a?.b?.c
来源：http://lu.521024.cn

[U86] JS：空值合并
来源：http://rz.muxihuayi.cn

a ?? b
来源：http://vn.521024.cn

[U87] JS：解构默认值
来源：http://qn.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://po.lnxyls.cn

[U88] JS：对象展开合并
来源：http://cu.jianghongdianzi.cn

{ ...a, ...b }
来源：http://kj.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://qk.newstarts.cn

[...new Set(arr)]
来源：http://gn.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://br.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://kj.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://eq.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cv.yuexingan06.cn

[U92] JS：深拷贝
来源：http://yy.bookmarksfly.cn

structuredClone(obj)
来源：http://hk.jctech888.com.cn

[U93] JS：模板字符串
来源：http://qn.haigaiapp.cn

`共 ${n} 条`
来源：http://vu.lnxyls.cn

[U94] JS：箭头函数
来源：http://oj.hnjuh.cn

const double = x => x * 2;
来源：http://jj.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ot.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://ek.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://tc.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aw.nicolike.cn

[U97] JS：并发请求
来源：http://wz.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://es.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://fk.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kb.huixiangedu.cn

[U99] JS：事件监听
来源：http://qf.szsharing.cn

el.addEventListener("click", e => {})
来源：http://ke.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://ru.asd995.cn

document.querySelector(".item")
来源：http://uo.bjjhwx.cn

[U101] JS：classList 操作
来源：http://bw.newstarts.cn

el.classList.toggle("active")
来源：http://hm.haigaiapp.cn

[U102] JS：本地存储
来源：http://ss.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://un.newstarts.cn

[U103] JS：定时器
来源：http://oc.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kp.huanxung.cn

[U104] JS：防抖
来源：http://ou.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dd.colortex.cn

[U105] JS：节流
来源：http://qe.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ne.nicolike.cn

[U106] JS：日期格式化
来源：http://ds.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pc.nszjky.cn

[U107] JS：数字千分位
来源：http://mv.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zr.huixiangedu.cn

[U108] JS：随机整数
来源：http://sk.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ay.bookmarksfly.cn

[U109] JS：数组分组
来源：http://rv.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://he.huixiangedu.cn

[U110] JS：数组分块
来源：http://ns.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uf.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://fk.nicolike.cn

new Map(Object.entries(obj))
来源：http://cf.shxzukj.cn

[U112] JS：字符串补位
来源：http://fs.hnjuh.cn

"7".padStart(3, "0")
来源：http://pf.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://as.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://jr.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://oc.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aw.lnxyls.cn

[U115] JS：生成 UUID
来源：http://mi.bookmarksfly.cn

crypto.randomUUID()
来源：http://kq.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://zc.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://wi.asd995.cn

[U117] JS：单元测试
来源：http://ai.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://ix.gzmigu.cn

[U118] JS：开发服务器
来源：http://az.lnxyls.cn

npm i -D vite;  npx vite
来源：http://hq.szsharing.cn

[U119] JS：生产构建
来源：http://se.jctech888.com.cn

npx vite build
来源：http://sk.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://rq.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://ma.bookmarksfly.cn

================================================================================
来源：http://pd.lnxyls.cn

统计汇总
来源：http://ab.panjiajie.cn

================================================================================
来源：http://nu.9csxet.cn

按语言统计（条）：
来源：http://rg.521024.cn

Python ......... 252
来源：http://aw.newstarts.cn

PHP ............ 252
来源：http://xo.panjiajie.cn

JavaScript ..... 252
来源：http://gf.chemitech.net.cn

TypeScript ..... 212
来源：http://we.nszjky.cn

Java ........... 212
来源：http://ls.newstarts.cn

Go ............. 212
来源：http://ub.huixiangedu.cn

Ruby ........... 212
来源：http://fp.jctech888.com.cn

C# ............. 212
来源：http://kd.shxzukj.cn

C .............. 30
来源：http://cz.yuntaijiaju.cn

C++ ............ 30
来源：http://ke.shxzukj.cn

SQL ............ 90
来源：http://zf.hnjuh.cn

Bash ........... 80
来源：http://bs.asd995.cn

Kotlin ......... 15
来源：http://ti.huanxung.cn

Swift .......... 15
来源：http://rx.wgjwhj.cn

Lua ............ 10
来源：http://ni.muxihuayi.cn

Perl ........... 10
来源：http://gs.newstarts.cn


<!-- 参考信息 -->