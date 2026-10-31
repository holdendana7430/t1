代发 wailian999

[T47] Perl：正则捕获
来源：http://qp.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dp.asd995.cn

[T48] Perl：正则替换
来源：http://zc.colortex.cn

$s =~ s/old/new/g;
来源：http://ho.asd995.cn

[T49] Perl：函数
来源：http://tn.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hi.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://jd.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vm.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://br.bjjhwx.cn

[T51] Scala：Hello World
来源：http://at.huixiangedu.cn

println("Hello")
来源：http://vw.wgjwhj.cn

[T52] Scala：变量
来源：http://gt.haigaiapp.cn

val a = 1;  var b = 2
来源：http://op.9csxet.cn

[T53] Scala：字符串插值
来源：http://by.shtwfgs.cn

s"值: $b"
来源：http://tb.gzmigu.cn

[T54] Scala：集合映射
来源：http://qw.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://sb.nszjky.cn

[T55] Scala：集合过滤
来源：http://zn.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lc.bjjhwx.cn

[T56] Scala：样例类
来源：http://kb.lnxyls.cn

case class User(name: String, age: Int)
来源：http://ep.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://yt.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sa.muxihuayi.cn

[T58] Scala：函数定义
来源：http://rz.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://us.shxzskj.cn

[T59] Scala：循环
来源：http://cp.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://sr.shxzukj.cn

[T60] Scala：折叠
来源：http://ti.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://si.shxzukj.cn

================================================================================
来源：http://ss.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wu.shxzskj.cn

================================================================================
来源：http://oe.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://hn.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qg.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://od.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ya.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://ca.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uz.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://qe.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rg.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://xp.nszjky.cn

list(dict.fromkeys(arr))
来源：http://fh.gzmigu.cn

[U06] Py：合并两个字典
来源：http://mv.chemitech.net.cn

{**a, **b}
来源：http://qw.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://wd.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://nz.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://bv.9csxet.cn

[y for x in nested for y in x]
来源：http://gs.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://cv.shxzskj.cn

max(d, key=d.get)
来源：http://aw.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://cg.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ck.shxzskj.cn

[U11] Py：生成器表达式
来源：http://me.hahajie.cn

(x * 2 for x in arr)
来源：http://qx.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sa.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://fa.szsharing.cn

[U13] Py：固定长度队列
来源：http://np.shtwfgs.cn

deque(maxlen=10)
来源：http://tp.521024.cn

[U14] Py：分组收集到列表
来源：http://qg.colortex.cn

defaultdict(list)
来源：http://ui.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://jw.chemitech.net.cn

t = time.perf_counter()
来源：http://en.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://en.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sy.gzmigu.cn

[U17] Py：初始化日志
来源：http://we.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://be.szsharing.cn

[U18] Py：预编译正则
来源：http://eu.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://tp.asd995.cn

[U19] Py：正则替换带回调
来源：http://sa.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ge.asd995.cn

[U20] Py：缓存函数结果
来源：http://pv.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://zp.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://qb.lnxyls.cn

@contextlib.contextmanager
来源：http://zq.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://yk.colortex.cn

list(zip(*m))
来源：http://fj.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://ai.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uh.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://tx.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lf.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://hv.szxytkj.cn

csv.DictReader(f)
来源：http://oq.yuexingan06.cn

[U26] Py：并发下载
来源：http://pl.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mh.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://ls.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://qs.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://tf.lnxyls.cn

UserId = int
来源：http://om.bjjhwx.cn

[U29] Py：属性校验
来源：http://cb.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://kf.shxzukj.cn

[U30] Py：数据类
来源：http://wb.huanxung.cn

@dataclass(slots=True)
来源：http://ek.szsharing.cn

[U31] Py：单测
来源：http://rt.nszjky.cn

python -m pytest -q
来源：http://ta.szxytkj.cn

[U32] Py：代码格式化
来源：http://yi.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://om.szsharing.cn

[U33] Py：打包发布
来源：http://nl.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://dm.shxzukj.cn

[U34] Py：判断编码
来源：http://ew.jianghongdianzi.cn

chardet.detect(raw)
来源：http://yr.chemitech.net.cn

[U35] Py：发送邮件
来源：http://dj.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://av.jctech888.com.cn

[U36] Py：定时任务
来源：http://xc.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://dm.nszjky.cn

[U37] Py：读写 Excel
来源：http://jq.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ok.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://rj.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://uu.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://sk.hnjuh.cn

sys.stdout.isatty()
来源：http://zt.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://jx.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://ye.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://fw.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hl.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://oo.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ag.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://yg.hnjuh.cn

namespace App\Http;
来源：http://xy.hahajie.cn

[U44] PHP：开启严格类型
来源：http://dz.bjjhwx.cn

declare(strict_types=1);
来源：http://xe.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://om.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hx.gzmigu.cn

[U46] PHP：可空类型
来源：http://vl.yuexingan06.cn

?string $name = null
来源：http://ql.hnjuh.cn

[U47] PHP：联合类型
来源：http://fr.shxzukj.cn

int|string $id
来源：http://ut.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://sl.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pm.huanxung.cn

[U49] PHP：只读属性
来源：http://tb.shxzskj.cn

public readonly string $name
来源：http://ca.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ln.lnxyls.cn

public function __construct(private int $id) {}
来源：http://qh.szsharing.cn

[U51] PHP：数组解构
来源：http://qk.panjiajie.cn

[$a, $b] = $arr;
来源：http://fj.szsharing.cn

[U52] PHP：箭头函数
来源：http://jr.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://lo.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://ga.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://yk.huanxung.cn

[U54] PHP：空安全调用
来源：http://vi.newstarts.cn

$obj?->method()
来源：http://kv.newstarts.cn

[U55] PHP：match 表达式
来源：http://rr.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://be.shxzskj.cn

[U56] PHP：命名参数
来源：http://tp.huanxung.cn

f(a: 1, b: 2)
来源：http://ms.hnjuh.cn

[U57] PHP：字符串插值
来源：http://cm.asd995.cn

"值: {$a}"
来源：http://nr.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://mw.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qq.nszjky.cn

[U59] PHP：自定义排序
来源：http://qv.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eh.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://js.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mc.9csxet.cn

[U61] PHP：正则
来源：http://un.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://za.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://km.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dc.hahajie.cn

[U63] PHP：文件读写
来源：http://hf.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ay.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ua.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://nj.szsharing.cn

[U65] PHP：会话
来源：http://mt.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wo.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://qf.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wh.huanxung.cn

[U67] PHP：处理文件上传
来源：http://jz.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ko.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://cw.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xn.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://vl.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yt.hahajie.cn

[U70] PHP：PDO 事务
来源：http://wp.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gt.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://jy.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://ri.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://ii.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://cz.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://ax.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://ld.nszjky.cn

[U74] PHP：读取环境变量
来源：http://av.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://to.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://je.chemitech.net.cn

composer require psr/container
来源：http://wa.nicolike.cn

[U76] PHP：简单路由
来源：http://jk.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pb.hahajie.cn

[U77] PHP：模板渲染
来源：http://kt.hnjuh.cn

composer require twig/twig
来源：http://fk.gzmigu.cn

[U78] PHP：单元测试
来源：http://tj.asd995.cn

composer require --dev phpunit/phpunit
来源：http://sp.asd995.cn

[U79] PHP：静态分析
来源：http://ga.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://ft.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://qp.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ia.szxytkj.cn

[U81] JS：初始化项目
来源：http://ri.haigaiapp.cn

npm init -y;  npm i express
来源：http://qa.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://us.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bx.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://jq.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wc.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://ba.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ao.jctech888.com.cn

[U85] JS：可选链
来源：http://aw.chemitech.net.cn

a?.b?.c
来源：http://ig.521024.cn

[U86] JS：空值合并
来源：http://nn.huixiangedu.cn

a ?? b
来源：http://nb.newstarts.cn

[U87] JS：解构默认值
来源：http://jm.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://je.nicolike.cn

[U88] JS：对象展开合并
来源：http://lm.huixiangedu.cn

{ ...a, ...b }
来源：http://qr.colortex.cn

[U89] JS：数组去重
来源：http://cd.colortex.cn

[...new Set(arr)]
来源：http://ed.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://he.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ah.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://yd.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://so.yuexingan06.cn

[U92] JS：深拷贝
来源：http://ey.lnxyls.cn

structuredClone(obj)
来源：http://jx.chemitech.net.cn

[U93] JS：模板字符串
来源：http://tk.nicolike.cn

`共 ${n} 条`
来源：http://md.bjjhwx.cn

[U94] JS：箭头函数
来源：http://lb.shxzukj.cn

const double = x => x * 2;
来源：http://wo.nszjky.cn

[U95] JS：Promise 包装
来源：http://xy.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://lw.huanxung.cn

[U96] JS：async/await 与异常
来源：http://ow.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dj.shxzukj.cn

[U97] JS：并发请求
来源：http://zj.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qw.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://rx.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gl.wgjwhj.cn

[U99] JS：事件监听
来源：http://rk.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://up.shxzskj.cn

[U100] JS：DOM 查询
来源：http://th.shxzskj.cn

document.querySelector(".item")
来源：http://bf.shxzukj.cn

[U101] JS：classList 操作
来源：http://zx.muxihuayi.cn

el.classList.toggle("active")
来源：http://qs.haigaiapp.cn

[U102] JS：本地存储
来源：http://kz.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ij.521024.cn

[U103] JS：定时器
来源：http://ln.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uc.bookmarksfly.cn

[U104] JS：防抖
来源：http://vw.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ax.shxzukj.cn

[U105] JS：节流
来源：http://gj.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://op.wgjwhj.cn

[U106] JS：日期格式化
来源：http://cv.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gz.lnxyls.cn

[U107] JS：数字千分位
来源：http://yi.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qv.muxihuayi.cn

[U108] JS：随机整数
来源：http://zl.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gh.lnxyls.cn

[U109] JS：数组分组
来源：http://pj.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://we.gzmigu.cn

[U110] JS：数组分块
来源：http://iq.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ew.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://ml.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://ql.9csxet.cn

[U112] JS：字符串补位
来源：http://we.haigaiapp.cn

"7".padStart(3, "0")
来源：http://op.panjiajie.cn

[U113] JS：正则替换全部
来源：http://ss.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://ts.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://yj.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hu.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://vq.nicolike.cn

crypto.randomUUID()
来源：http://wo.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://nq.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://no.nicolike.cn

[U117] JS：单元测试
来源：http://uk.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://oa.szxytkj.cn

[U118] JS：开发服务器
来源：http://ll.panjiajie.cn

npm i -D vite;  npx vite
来源：http://kf.521024.cn

[U119] JS：生产构建
来源：http://pj.huixinmuqiang.cn

npx vite build
来源：http://zm.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://jx.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://xc.huanxung.cn

================================================================================
来源：http://ts.nicolike.cn

统计汇总
来源：http://gr.hahajie.cn

================================================================================
来源：http://fd.hahajie.cn

按语言统计（条）：
来源：http://sb.shtwfgs.cn

Python ......... 252
来源：http://mc.huixiangedu.cn

PHP ............ 252
来源：http://fp.lnxyls.cn

JavaScript ..... 252
来源：http://by.newstarts.cn

TypeScript ..... 212
来源：http://af.panjiajie.cn

Java ........... 212
来源：http://ax.9csxet.cn

Go ............. 212
来源：http://dx.haigaiapp.cn

Ruby ........... 212
来源：http://fx.huanxung.cn

C# ............. 212
来源：http://yq.hahajie.cn

C .............. 30
来源：http://kr.bjjhwx.cn

C++ ............ 30
来源：http://ml.wgjwhj.cn

SQL ............ 90
来源：http://zm.szsharing.cn

Bash ........... 80
来源：http://hh.panjiajie.cn

Kotlin ......... 15
来源：http://cx.9csxet.cn

Swift .......... 15
来源：http://kp.jctech888.com.cn

Lua ............ 10
来源：http://xh.yuntaijiaju.cn

Perl ........... 10
来源：http://dw.huixinmuqiang.cn

Scala .......... 10
来源：http://rv.yuexingan06.cn

------------------------------------
来源：http://mj.bookmarksfly.cn

合计 ........... 2106 条
来源：http://rb.huanxung.cn

按章节统计：
来源：http://rb.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fw.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lc.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qa.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lv.newstarts.cn


<!-- 参考信息 -->