代发 wailian999

[T49] Perl：函数
来源：http://gq.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ue.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://po.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lw.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://or.muxihuayi.cn

[T51] Scala：Hello World
来源：http://ll.panjiajie.cn

println("Hello")
来源：http://cy.muxihuayi.cn

[T52] Scala：变量
来源：http://wb.hnjuh.cn

val a = 1;  var b = 2
来源：http://es.nicolike.cn

[T53] Scala：字符串插值
来源：http://pz.panjiajie.cn

s"值: $b"
来源：http://gd.haigaiapp.cn

[T54] Scala：集合映射
来源：http://uj.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://qw.hahajie.cn

[T55] Scala：集合过滤
来源：http://ni.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://du.wgjwhj.cn

[T56] Scala：样例类
来源：http://ux.gzmigu.cn

case class User(name: String, age: Int)
来源：http://dp.hahajie.cn

[T57] Scala：模式匹配
来源：http://wu.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lg.colortex.cn

[T58] Scala：函数定义
来源：http://zd.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://et.jianghongdianzi.cn

[T59] Scala：循环
来源：http://de.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://yo.gzmigu.cn

[T60] Scala：折叠
来源：http://bh.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yo.bookmarksfly.cn

================================================================================
来源：http://dz.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fi.szsharing.cn

================================================================================
来源：http://il.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://eg.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xs.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://na.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ti.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://tm.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ce.hahajie.cn

[U04] Py：变量调试打印
来源：http://eg.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zv.521024.cn

[U05] Py：列表去重且保序
来源：http://mr.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://mr.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://hh.muxihuayi.cn

{**a, **b}
来源：http://ww.shxzskj.cn

[U07] Py：反转字典键值
来源：http://gn.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://av.gzmigu.cn

[U08] Py：展平二维列表
来源：http://ul.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://wm.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://dc.hahajie.cn

max(d, key=d.get)
来源：http://hu.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://di.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://az.9csxet.cn

[U11] Py：生成器表达式
来源：http://au.wgjwhj.cn

(x * 2 for x in arr)
来源：http://wc.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ps.9csxet.cn

Counter(arr).most_common(3)
来源：http://an.lnxyls.cn

[U13] Py：固定长度队列
来源：http://ub.hnjuh.cn

deque(maxlen=10)
来源：http://ky.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://io.asd995.cn

defaultdict(list)
来源：http://ba.bjjhwx.cn

[U15] Py：高精度计时
来源：http://uq.jctech888.com.cn

t = time.perf_counter()
来源：http://gg.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://ef.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ei.wgjwhj.cn

[U17] Py：初始化日志
来源：http://am.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://kn.szxytkj.cn

[U18] Py：预编译正则
来源：http://zh.9csxet.cn

pat = re.compile(r"\d+")
来源：http://hw.nszjky.cn

[U19] Py：正则替换带回调
来源：http://za.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kk.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://mz.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://vf.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://pd.newstarts.cn

@contextlib.contextmanager
来源：http://wb.nicolike.cn

[U22] Py：矩阵转置
来源：http://pt.hahajie.cn

list(zip(*m))
来源：http://wt.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://cg.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bb.shxzskj.cn

[U24] Py：路径操作
来源：http://gr.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ot.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://ok.haigaiapp.cn

csv.DictReader(f)
来源：http://wm.hnjuh.cn

[U26] Py：并发下载
来源：http://xh.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ko.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://gh.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://qz.huanxung.cn

[U28] Py：类型别名
来源：http://yb.szsharing.cn

UserId = int
来源：http://po.szsharing.cn

[U29] Py：属性校验
来源：http://zr.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://cq.colortex.cn

[U30] Py：数据类
来源：http://jx.huanxung.cn

@dataclass(slots=True)
来源：http://cq.jianghongdianzi.cn

[U31] Py：单测
来源：http://hw.hahajie.cn

python -m pytest -q
来源：http://it.szsharing.cn

[U32] Py：代码格式化
来源：http://iy.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://pi.panjiajie.cn

[U33] Py：打包发布
来源：http://vb.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://hf.shxzukj.cn

[U34] Py：判断编码
来源：http://ud.szsharing.cn

chardet.detect(raw)
来源：http://dx.9csxet.cn

[U35] Py：发送邮件
来源：http://zq.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wu.jctech888.com.cn

[U36] Py：定时任务
来源：http://cc.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://tu.lnxyls.cn

[U37] Py：读写 Excel
来源：http://wf.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ir.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://tj.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://oa.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://dk.nszjky.cn

sys.stdout.isatty()
来源：http://od.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://os.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://mj.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://hm.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rb.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://mm.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kn.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://lz.wgjwhj.cn

namespace App\Http;
来源：http://ee.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://zb.muxihuayi.cn

declare(strict_types=1);
来源：http://ne.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://sd.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dt.muxihuayi.cn

[U46] PHP：可空类型
来源：http://qy.hahajie.cn

?string $name = null
来源：http://rs.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://wj.hahajie.cn

int|string $id
来源：http://ne.panjiajie.cn

[U48] PHP：纯枚举
来源：http://zi.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qx.hahajie.cn

[U49] PHP：只读属性
来源：http://fd.huixiangedu.cn

public readonly string $name
来源：http://kn.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://ts.szxytkj.cn

public function __construct(private int $id) {}
来源：http://qi.huixiangedu.cn

[U51] PHP：数组解构
来源：http://nr.hahajie.cn

[$a, $b] = $arr;
来源：http://ko.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://pk.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://oj.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://el.521024.cn

$v = $a ?? $b ?? "default";
来源：http://on.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://gx.huanxung.cn

$obj?->method()
来源：http://of.521024.cn

[U55] PHP：match 表达式
来源：http://io.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xb.newstarts.cn

[U56] PHP：命名参数
来源：http://pg.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://lq.shxzskj.cn

[U57] PHP：字符串插值
来源：http://km.gzmigu.cn

"值: {$a}"
来源：http://ya.shxzukj.cn

[U58] PHP：数组三件套
来源：http://li.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tu.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://us.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://my.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://ns.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dl.huixiangedu.cn

[U61] PHP：正则
来源：http://oa.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wp.lnxyls.cn

[U62] PHP：日期对象
来源：http://ry.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ar.shxzukj.cn

[U63] PHP：文件读写
来源：http://mw.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yx.szxytkj.cn

[U64] PHP：目录遍历
来源：http://zr.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://hg.colortex.cn

[U65] PHP：会话
来源：http://ha.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nr.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://cy.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://he.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://yq.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bs.newstarts.cn

[U68] PHP：PDO 连接
来源：http://wy.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bp.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://td.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kb.nszjky.cn

[U70] PHP：PDO 事务
来源：http://oq.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://af.lnxyls.cn

[U71] PHP：抛出异常
来源：http://qc.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://ts.nszjky.cn

[U72] PHP：写错误日志
来源：http://fx.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://la.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://in.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://ks.huanxung.cn

[U74] PHP：读取环境变量
来源：http://hv.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://zf.nicolike.cn

[U75] PHP：依赖注入
来源：http://at.hnjuh.cn

composer require psr/container
来源：http://ow.newstarts.cn

[U76] PHP：简单路由
来源：http://xa.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ix.shxzukj.cn

[U77] PHP：模板渲染
来源：http://xp.huixiangedu.cn

composer require twig/twig
来源：http://ie.szxytkj.cn

[U78] PHP：单元测试
来源：http://cl.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://bm.colortex.cn

[U79] PHP：静态分析
来源：http://wr.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://it.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://nw.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kf.hahajie.cn

[U81] JS：初始化项目
来源：http://md.bjjhwx.cn

npm init -y;  npm i express
来源：http://pn.nicolike.cn

[U82] JS：package.json 脚本
来源：http://pl.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rf.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://wh.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qz.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://wv.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bj.nicolike.cn

[U85] JS：可选链
来源：http://qs.szsharing.cn

a?.b?.c
来源：http://ug.shxzukj.cn

[U86] JS：空值合并
来源：http://dl.huixinmuqiang.cn

a ?? b
来源：http://eh.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://lm.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://fs.asd995.cn

[U88] JS：对象展开合并
来源：http://bd.huixiangedu.cn

{ ...a, ...b }
来源：http://xj.gzmigu.cn

[U89] JS：数组去重
来源：http://sx.yuntaijiaju.cn

[...new Set(arr)]
来源：http://uy.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://da.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://ca.521024.cn

[U91] JS：对象键值遍历
来源：http://rh.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://im.yuexingan06.cn

[U92] JS：深拷贝
来源：http://cn.hahajie.cn

structuredClone(obj)
来源：http://pv.lnxyls.cn

[U93] JS：模板字符串
来源：http://bs.huixinmuqiang.cn

`共 ${n} 条`
来源：http://gq.nicolike.cn

[U94] JS：箭头函数
来源：http://vu.hahajie.cn

const double = x => x * 2;
来源：http://as.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://vw.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://tm.szsharing.cn

[U96] JS：async/await 与异常
来源：http://yb.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ck.huixiangedu.cn

[U97] JS：并发请求
来源：http://ys.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tw.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://qx.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kh.jctech888.com.cn

[U99] JS：事件监听
来源：http://ht.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://dw.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://cl.newstarts.cn

document.querySelector(".item")
来源：http://mz.asd995.cn

[U101] JS：classList 操作
来源：http://om.shxzskj.cn

el.classList.toggle("active")
来源：http://uy.hnjuh.cn

[U102] JS：本地存储
来源：http://cp.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qx.521024.cn

[U103] JS：定时器
来源：http://mi.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nz.bjjhwx.cn

[U104] JS：防抖
来源：http://pw.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fd.newstarts.cn

[U105] JS：节流
来源：http://qc.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lf.colortex.cn

[U106] JS：日期格式化
来源：http://wq.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dw.newstarts.cn

[U107] JS：数字千分位
来源：http://gz.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dq.szxytkj.cn

[U108] JS：随机整数
来源：http://la.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jt.shxzskj.cn

[U109] JS：数组分组
来源：http://ni.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://wl.jctech888.com.cn

[U110] JS：数组分块
来源：http://bb.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rw.hahajie.cn

[U111] JS：对象转 Map
来源：http://cy.hnjuh.cn

new Map(Object.entries(obj))
来源：http://pr.chemitech.net.cn

[U112] JS：字符串补位
来源：http://pi.shxzukj.cn

"7".padStart(3, "0")
来源：http://mv.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://ne.hahajie.cn

s.replaceAll("a", "b")
来源：http://ho.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://mb.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://la.asd995.cn

[U115] JS：生成 UUID
来源：http://iz.jctech888.com.cn

crypto.randomUUID()
来源：http://up.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://cz.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://dl.huanxung.cn

[U117] JS：单元测试
来源：http://oi.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ee.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://yu.521024.cn

npm i -D vite;  npx vite
来源：http://uk.bjjhwx.cn

[U119] JS：生产构建
来源：http://kq.wgjwhj.cn

npx vite build
来源：http://df.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://tr.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://re.shtwfgs.cn

================================================================================
来源：http://xr.szsharing.cn

统计汇总
来源：http://xm.szxytkj.cn

================================================================================
来源：http://ci.muxihuayi.cn

按语言统计（条）：
来源：http://zs.muxihuayi.cn

Python ......... 252
来源：http://qc.shtwfgs.cn

PHP ............ 252
来源：http://mr.huixinmuqiang.cn

JavaScript ..... 252
来源：http://bk.chemitech.net.cn

TypeScript ..... 212
来源：http://vc.huanxung.cn

Java ........... 212
来源：http://ad.newstarts.cn

Go ............. 212
来源：http://rc.huanxung.cn

Ruby ........... 212
来源：http://mg.newstarts.cn

C# ............. 212
来源：http://ng.huixinmuqiang.cn

C .............. 30
来源：http://lu.bookmarksfly.cn

C++ ............ 30
来源：http://tz.yuexingan06.cn

SQL ............ 90
来源：http://dp.wgjwhj.cn

Bash ........... 80
来源：http://ux.bookmarksfly.cn

Kotlin ......... 15
来源：http://vl.yuntaijiaju.cn

Swift .......... 15
来源：http://vl.szxytkj.cn

Lua ............ 10
来源：http://sv.yuntaijiaju.cn

Perl ........... 10
来源：http://wv.panjiajie.cn

Scala .......... 10
来源：http://wp.huixiangedu.cn

------------------------------------
来源：http://rh.asd995.cn

合计 ........... 2106 条
来源：http://ov.shxzukj.cn

按章节统计：
来源：http://kc.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dy.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zq.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oi.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kl.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hb.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sy.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dh.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ct.gzmigu.cn


<!-- 参考信息 -->