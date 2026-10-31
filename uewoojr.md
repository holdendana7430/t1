代发 wailian999

[T49] Perl：函数
来源：http://tx.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fm.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://ku.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mb.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://pp.jctech888.com.cn

[T51] Scala：Hello World
来源：http://fr.wgjwhj.cn

println("Hello")
来源：http://vl.bookmarksfly.cn

[T52] Scala：变量
来源：http://gr.gzmigu.cn

val a = 1;  var b = 2
来源：http://jk.colortex.cn

[T53] Scala：字符串插值
来源：http://ei.huixiangedu.cn

s"值: $b"
来源：http://ys.hahajie.cn

[T54] Scala：集合映射
来源：http://rf.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://aw.521024.cn

[T55] Scala：集合过滤
来源：http://fq.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qu.huixiangedu.cn

[T56] Scala：样例类
来源：http://az.shxzukj.cn

case class User(name: String, age: Int)
来源：http://uk.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://xc.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tc.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://ad.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zj.hnjuh.cn

[T59] Scala：循环
来源：http://ub.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://oq.hnjuh.cn

[T60] Scala：折叠
来源：http://af.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ef.nicolike.cn

================================================================================
来源：http://lc.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lq.9csxet.cn

================================================================================
来源：http://qj.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://kk.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ts.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://di.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nm.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://jp.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qb.szxytkj.cn

[U04] Py：变量调试打印
来源：http://pm.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yf.9csxet.cn

[U05] Py：列表去重且保序
来源：http://oa.colortex.cn

list(dict.fromkeys(arr))
来源：http://dr.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://av.lnxyls.cn

{**a, **b}
来源：http://vm.panjiajie.cn

[U07] Py：反转字典键值
来源：http://es.szsharing.cn

{v: k for k, v in d.items()}
来源：http://ed.lnxyls.cn

[U08] Py：展平二维列表
来源：http://or.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://tm.colortex.cn

[U09] Py：字典取最大值的键
来源：http://mz.haigaiapp.cn

max(d, key=d.get)
来源：http://xf.shxzskj.cn

[U10] Py：按值排序字典
来源：http://ao.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aq.521024.cn

[U11] Py：生成器表达式
来源：http://pr.9csxet.cn

(x * 2 for x in arr)
来源：http://xk.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xh.nicolike.cn

Counter(arr).most_common(3)
来源：http://ya.9csxet.cn

[U13] Py：固定长度队列
来源：http://tn.bjjhwx.cn

deque(maxlen=10)
来源：http://lf.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://bg.wgjwhj.cn

defaultdict(list)
来源：http://ba.yuexingan06.cn

[U15] Py：高精度计时
来源：http://iv.huixinmuqiang.cn

t = time.perf_counter()
来源：http://wu.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://sa.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ow.szxytkj.cn

[U17] Py：初始化日志
来源：http://sv.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://gv.haigaiapp.cn

[U18] Py：预编译正则
来源：http://qk.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://ak.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://jt.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mm.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://kw.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ts.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://fo.szsharing.cn

@contextlib.contextmanager
来源：http://pp.hnjuh.cn

[U22] Py：矩阵转置
来源：http://uo.hnjuh.cn

list(zip(*m))
来源：http://bc.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://wt.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qh.shtwfgs.cn

[U24] Py：路径操作
来源：http://dp.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zo.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://bg.chemitech.net.cn

csv.DictReader(f)
来源：http://gq.newstarts.cn

[U26] Py：并发下载
来源：http://ny.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gd.newstarts.cn

[U27] Py：异步 HTTP
来源：http://wj.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://mp.bjjhwx.cn

[U28] Py：类型别名
来源：http://nv.asd995.cn

UserId = int
来源：http://nd.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://uk.asd995.cn

@property 与 @x.setter 配合
来源：http://cd.521024.cn

[U30] Py：数据类
来源：http://uz.gzmigu.cn

@dataclass(slots=True)
来源：http://hp.bookmarksfly.cn

[U31] Py：单测
来源：http://rn.huixinmuqiang.cn

python -m pytest -q
来源：http://ue.haigaiapp.cn

[U32] Py：代码格式化
来源：http://rk.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://he.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://tu.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://iq.panjiajie.cn

[U34] Py：判断编码
来源：http://rf.yuexingan06.cn

chardet.detect(raw)
来源：http://rj.szsharing.cn

[U35] Py：发送邮件
来源：http://yy.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oa.haigaiapp.cn

[U36] Py：定时任务
来源：http://eg.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://gb.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://tz.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vr.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://si.szsharing.cn

Path(__file__).resolve().parent
来源：http://sh.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://hr.colortex.cn

sys.stdout.isatty()
来源：http://so.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://cm.hnjuh.cn

print("err", file=sys.stderr)
来源：http://hv.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ih.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ry.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://hm.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bg.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://zb.yuntaijiaju.cn

namespace App\Http;
来源：http://hs.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://mt.gzmigu.cn

declare(strict_types=1);
来源：http://em.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://sd.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.hahajie.cn

[U46] PHP：可空类型
来源：http://ok.bookmarksfly.cn

?string $name = null
来源：http://xz.huixiangedu.cn

[U47] PHP：联合类型
来源：http://hh.jctech888.com.cn

int|string $id
来源：http://zn.szxytkj.cn

[U48] PHP：纯枚举
来源：http://ug.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://on.nszjky.cn

[U49] PHP：只读属性
来源：http://qv.9csxet.cn

public readonly string $name
来源：http://zf.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://uq.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://mg.szsharing.cn

[U51] PHP：数组解构
来源：http://oq.shtwfgs.cn

[$a, $b] = $arr;
来源：http://zh.nicolike.cn

[U52] PHP：箭头函数
来源：http://dc.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://fd.huanxung.cn

[U53] PHP：空合并运算符
来源：http://pq.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://gl.shxzskj.cn

[U54] PHP：空安全调用
来源：http://sv.shxzukj.cn

$obj?->method()
来源：http://hq.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://tr.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cp.huanxung.cn

[U56] PHP：命名参数
来源：http://jl.panjiajie.cn

f(a: 1, b: 2)
来源：http://ty.nszjky.cn

[U57] PHP：字符串插值
来源：http://ov.bjjhwx.cn

"值: {$a}"
来源：http://ra.asd995.cn

[U58] PHP：数组三件套
来源：http://bv.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ss.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://vi.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ze.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://tq.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mv.9csxet.cn

[U61] PHP：正则
来源：http://wp.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qa.asd995.cn

[U62] PHP：日期对象
来源：http://ne.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jz.shxzukj.cn

[U63] PHP：文件读写
来源：http://bz.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rq.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://tv.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://xq.shxzskj.cn

[U65] PHP：会话
来源：http://va.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hk.521024.cn

[U66] PHP：设置 Cookie
来源：http://ax.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ju.szsharing.cn

[U67] PHP：处理文件上传
来源：http://ma.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ru.szsharing.cn

[U68] PHP：PDO 连接
来源：http://hg.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://un.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://rj.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aq.newstarts.cn

[U70] PHP：PDO 事务
来源：http://fc.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://si.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://um.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://at.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://pc.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://tq.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://lm.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://bt.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://ym.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://it.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://vt.jianghongdianzi.cn

composer require psr/container
来源：http://li.szxytkj.cn

[U76] PHP：简单路由
来源：http://rs.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cp.lnxyls.cn

[U77] PHP：模板渲染
来源：http://xf.9csxet.cn

composer require twig/twig
来源：http://kz.hnjuh.cn

[U78] PHP：单元测试
来源：http://ao.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://xo.yuexingan06.cn

[U79] PHP：静态分析
来源：http://wi.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://os.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://gu.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cr.panjiajie.cn

[U81] JS：初始化项目
来源：http://ck.9csxet.cn

npm init -y;  npm i express
来源：http://ik.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://zi.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wn.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://ct.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fj.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://pf.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ja.jianghongdianzi.cn

[U85] JS：可选链
来源：http://vc.yuntaijiaju.cn

a?.b?.c
来源：http://eq.shxzskj.cn

[U86] JS：空值合并
来源：http://sg.bookmarksfly.cn

a ?? b
来源：http://ap.bjjhwx.cn

[U87] JS：解构默认值
来源：http://iq.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://lg.szxytkj.cn

[U88] JS：对象展开合并
来源：http://yb.gzmigu.cn

{ ...a, ...b }
来源：http://ji.huanxung.cn

[U89] JS：数组去重
来源：http://rk.hnjuh.cn

[...new Set(arr)]
来源：http://ob.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://nr.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://tg.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://kx.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ag.haigaiapp.cn

[U92] JS：深拷贝
来源：http://un.jianghongdianzi.cn

structuredClone(obj)
来源：http://dw.9csxet.cn

[U93] JS：模板字符串
来源：http://sw.szsharing.cn

`共 ${n} 条`
来源：http://ys.shtwfgs.cn

[U94] JS：箭头函数
来源：http://ee.yuexingan06.cn

const double = x => x * 2;
来源：http://gc.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://mk.521024.cn

new Promise((resolve, reject) => {})
来源：http://xa.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://hz.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yr.shtwfgs.cn

[U97] JS：并发请求
来源：http://ak.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qz.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://gs.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qk.szxytkj.cn

[U99] JS：事件监听
来源：http://xp.nszjky.cn

el.addEventListener("click", e => {})
来源：http://vu.9csxet.cn

[U100] JS：DOM 查询
来源：http://rz.9csxet.cn

document.querySelector(".item")
来源：http://lx.muxihuayi.cn

[U101] JS：classList 操作
来源：http://jw.muxihuayi.cn

el.classList.toggle("active")
来源：http://ur.9csxet.cn

[U102] JS：本地存储
来源：http://uw.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nq.huanxung.cn

[U103] JS：定时器
来源：http://kx.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hv.shxzskj.cn

[U104] JS：防抖
来源：http://kr.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cs.newstarts.cn

[U105] JS：节流
来源：http://qi.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jj.hahajie.cn

[U106] JS：日期格式化
来源：http://ur.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mh.wgjwhj.cn

[U107] JS：数字千分位
来源：http://ft.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qi.szxytkj.cn

[U108] JS：随机整数
来源：http://gr.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://we.szxytkj.cn

[U109] JS：数组分组
来源：http://rn.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ed.newstarts.cn

[U110] JS：数组分块
来源：http://aw.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xr.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://aa.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://gj.szxytkj.cn

[U112] JS：字符串补位
来源：http://ck.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://tc.9csxet.cn

[U113] JS：正则替换全部
来源：http://ct.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://di.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ny.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vc.9csxet.cn

[U115] JS：生成 UUID
来源：http://hc.muxihuayi.cn

crypto.randomUUID()
来源：http://mv.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ab.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://oy.hnjuh.cn

[U117] JS：单元测试
来源：http://xt.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://pf.yuexingan06.cn

[U118] JS：开发服务器
来源：http://jk.nicolike.cn

npm i -D vite;  npx vite
来源：http://ee.shxzskj.cn

[U119] JS：生产构建
来源：http://ri.nicolike.cn

npx vite build
来源：http://pi.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://fr.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ut.colortex.cn

================================================================================
来源：http://vy.jianghongdianzi.cn

统计汇总
来源：http://wg.hnjuh.cn

================================================================================
来源：http://jv.muxihuayi.cn

按语言统计（条）：
来源：http://bf.huanxung.cn

Python ......... 252
来源：http://am.jctech888.com.cn

PHP ............ 252
来源：http://cg.muxihuayi.cn

JavaScript ..... 252
来源：http://jk.szxytkj.cn

TypeScript ..... 212
来源：http://pl.huanxung.cn

Java ........... 212
来源：http://ya.bjjhwx.cn

Go ............. 212
来源：http://hm.haigaiapp.cn

Ruby ........... 212
来源：http://br.chemitech.net.cn

C# ............. 212
来源：http://og.newstarts.cn

C .............. 30
来源：http://aa.huixiangedu.cn

C++ ............ 30
来源：http://ux.panjiajie.cn

SQL ............ 90
来源：http://wy.9csxet.cn

Bash ........... 80
来源：http://eu.szxytkj.cn

Kotlin ......... 15
来源：http://dx.521024.cn

Swift .......... 15
来源：http://ar.szsharing.cn

Lua ............ 10
来源：http://uk.newstarts.cn

Perl ........... 10
来源：http://hr.nszjky.cn

Scala .......... 10
来源：http://iu.9csxet.cn

------------------------------------
来源：http://ab.huixiangedu.cn

合计 ........... 2106 条
来源：http://kk.nszjky.cn

按章节统计：
来源：http://mb.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nt.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bo.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uf.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lj.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uk.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mr.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nd.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ys.9csxet.cn


<!-- 参考信息 -->