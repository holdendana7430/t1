代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://si.huixiangedu.cn

[T51] Scala：Hello World
来源：http://fg.chemitech.net.cn

println("Hello")
来源：http://jj.shtwfgs.cn

[T52] Scala：变量
来源：http://tg.newstarts.cn

val a = 1;  var b = 2
来源：http://vl.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://nd.panjiajie.cn

s"值: $b"
来源：http://mw.newstarts.cn

[T54] Scala：集合映射
来源：http://zm.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://dl.gzmigu.cn

[T55] Scala：集合过滤
来源：http://jd.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zx.shtwfgs.cn

[T56] Scala：样例类
来源：http://pw.huanxung.cn

case class User(name: String, age: Int)
来源：http://ns.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://mb.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wm.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://dq.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rk.hnjuh.cn

[T59] Scala：循环
来源：http://wh.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://em.bjjhwx.cn

[T60] Scala：折叠
来源：http://pg.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jc.shxzskj.cn

================================================================================
来源：http://wv.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jo.panjiajie.cn

================================================================================
来源：http://hk.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://mg.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qn.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://xt.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mh.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://cx.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nb.asd995.cn

[U04] Py：变量调试打印
来源：http://dx.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ct.asd995.cn

[U05] Py：列表去重且保序
来源：http://hd.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://bp.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://wd.chemitech.net.cn

{**a, **b}
来源：http://qp.nszjky.cn

[U07] Py：反转字典键值
来源：http://tq.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://er.newstarts.cn

[U08] Py：展平二维列表
来源：http://jn.colortex.cn

[y for x in nested for y in x]
来源：http://rk.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://xr.chemitech.net.cn

max(d, key=d.get)
来源：http://xd.gzmigu.cn

[U10] Py：按值排序字典
来源：http://mq.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ex.521024.cn

[U11] Py：生成器表达式
来源：http://yr.yuexingan06.cn

(x * 2 for x in arr)
来源：http://wg.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gc.nicolike.cn

Counter(arr).most_common(3)
来源：http://cn.asd995.cn

[U13] Py：固定长度队列
来源：http://cz.wgjwhj.cn

deque(maxlen=10)
来源：http://ox.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://mg.huixinmuqiang.cn

defaultdict(list)
来源：http://zl.huanxung.cn

[U15] Py：高精度计时
来源：http://ol.shxzskj.cn

t = time.perf_counter()
来源：http://fy.huanxung.cn

[U16] Py：命令行参数解析
来源：http://sf.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rn.asd995.cn

[U17] Py：初始化日志
来源：http://ix.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://te.gzmigu.cn

[U18] Py：预编译正则
来源：http://ia.521024.cn

pat = re.compile(r"\d+")
来源：http://ir.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://na.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cb.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ww.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://xd.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://gj.lnxyls.cn

@contextlib.contextmanager
来源：http://bn.521024.cn

[U22] Py：矩阵转置
来源：http://lf.nszjky.cn

list(zip(*m))
来源：http://jy.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://dg.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hv.hnjuh.cn

[U24] Py：路径操作
来源：http://uc.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ez.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://bt.nicolike.cn

csv.DictReader(f)
来源：http://st.nicolike.cn

[U26] Py：并发下载
来源：http://ms.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xu.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://oc.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://hd.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://mj.shtwfgs.cn

UserId = int
来源：http://pz.shtwfgs.cn

[U29] Py：属性校验
来源：http://ja.hnjuh.cn

@property 与 @x.setter 配合
来源：http://om.szsharing.cn

[U30] Py：数据类
来源：http://mx.haigaiapp.cn

@dataclass(slots=True)
来源：http://xh.bookmarksfly.cn

[U31] Py：单测
来源：http://cq.521024.cn

python -m pytest -q
来源：http://dw.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://cs.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://uh.nszjky.cn

[U33] Py：打包发布
来源：http://xu.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://pg.hnjuh.cn

[U34] Py：判断编码
来源：http://nx.521024.cn

chardet.detect(raw)
来源：http://ms.521024.cn

[U35] Py：发送邮件
来源：http://cs.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yi.521024.cn

[U36] Py：定时任务
来源：http://ew.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://cl.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://jj.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jt.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://so.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ku.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://zh.yuexingan06.cn

sys.stdout.isatty()
来源：http://ug.hahajie.cn

[U40] Py：打印到标准错误
来源：http://ev.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://we.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://ip.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uu.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://sl.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cg.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://dm.colortex.cn

namespace App\Http;
来源：http://ct.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://lq.hnjuh.cn

declare(strict_types=1);
来源：http://iq.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://jx.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sn.panjiajie.cn

[U46] PHP：可空类型
来源：http://ej.hnjuh.cn

?string $name = null
来源：http://jo.9csxet.cn

[U47] PHP：联合类型
来源：http://qn.521024.cn

int|string $id
来源：http://on.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://me.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dl.jctech888.com.cn

[U49] PHP：只读属性
来源：http://ie.haigaiapp.cn

public readonly string $name
来源：http://fh.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://uq.newstarts.cn

public function __construct(private int $id) {}
来源：http://wq.hnjuh.cn

[U51] PHP：数组解构
来源：http://uo.nicolike.cn

[$a, $b] = $arr;
来源：http://eu.szxytkj.cn

[U52] PHP：箭头函数
来源：http://fc.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://kg.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://or.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://qa.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://jk.muxihuayi.cn

$obj?->method()
来源：http://se.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://oo.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qg.haigaiapp.cn

[U56] PHP：命名参数
来源：http://tc.jctech888.com.cn

f(a: 1, b: 2)
来源：http://yi.asd995.cn

[U57] PHP：字符串插值
来源：http://qn.szsharing.cn

"值: {$a}"
来源：http://vq.lnxyls.cn

[U58] PHP：数组三件套
来源：http://ol.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yl.gzmigu.cn

[U59] PHP：自定义排序
来源：http://xo.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nm.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://fj.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qj.bjjhwx.cn

[U61] PHP：正则
来源：http://lg.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bi.bjjhwx.cn

[U62] PHP：日期对象
来源：http://ob.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xi.hnjuh.cn

[U63] PHP：文件读写
来源：http://qd.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wk.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ef.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://gv.jianghongdianzi.cn

[U65] PHP：会话
来源：http://ky.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bo.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://tl.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kw.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://jk.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uk.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://kb.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bq.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://jt.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rg.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://pk.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kk.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ln.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://oa.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://wy.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://zf.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://sc.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://nb.huanxung.cn

[U74] PHP：读取环境变量
来源：http://eg.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://eg.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://lc.newstarts.cn

composer require psr/container
来源：http://du.haigaiapp.cn

[U76] PHP：简单路由
来源：http://cv.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kk.lnxyls.cn

[U77] PHP：模板渲染
来源：http://qg.shtwfgs.cn

composer require twig/twig
来源：http://yw.521024.cn

[U78] PHP：单元测试
来源：http://mm.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://ax.asd995.cn

[U79] PHP：静态分析
来源：http://mk.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://be.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://gr.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pa.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://uf.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://dl.szsharing.cn

[U82] JS：package.json 脚本
来源：http://du.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ei.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://jz.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ig.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://fv.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pd.colortex.cn

[U85] JS：可选链
来源：http://rg.huixinmuqiang.cn

a?.b?.c
来源：http://zw.szsharing.cn

[U86] JS：空值合并
来源：http://ko.yuntaijiaju.cn

a ?? b
来源：http://sd.chemitech.net.cn

[U87] JS：解构默认值
来源：http://ym.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://ra.nszjky.cn

[U88] JS：对象展开合并
来源：http://kv.szxytkj.cn

{ ...a, ...b }
来源：http://mz.haigaiapp.cn

[U89] JS：数组去重
来源：http://bh.huixinmuqiang.cn

[...new Set(arr)]
来源：http://gk.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://rg.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://de.nicolike.cn

[U91] JS：对象键值遍历
来源：http://oa.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ls.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://wt.shxzukj.cn

structuredClone(obj)
来源：http://sz.hnjuh.cn

[U93] JS：模板字符串
来源：http://mt.yuexingan06.cn

`共 ${n} 条`
来源：http://uq.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ru.521024.cn

const double = x => x * 2;
来源：http://et.nicolike.cn

[U95] JS：Promise 包装
来源：http://nf.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://dy.huanxung.cn

[U96] JS：async/await 与异常
来源：http://jc.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tr.newstarts.cn

[U97] JS：并发请求
来源：http://xq.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ld.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://dj.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rc.lnxyls.cn

[U99] JS：事件监听
来源：http://pc.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://px.gzmigu.cn

[U100] JS：DOM 查询
来源：http://vr.shtwfgs.cn

document.querySelector(".item")
来源：http://sl.muxihuayi.cn

[U101] JS：classList 操作
来源：http://cy.wgjwhj.cn

el.classList.toggle("active")
来源：http://fq.nszjky.cn

[U102] JS：本地存储
来源：http://in.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rf.asd995.cn

[U103] JS：定时器
来源：http://op.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ka.szxytkj.cn

[U104] JS：防抖
来源：http://jb.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cs.521024.cn

[U105] JS：节流
来源：http://rd.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ja.lnxyls.cn

[U106] JS：日期格式化
来源：http://dr.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hh.hahajie.cn

[U107] JS：数字千分位
来源：http://zc.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uz.newstarts.cn

[U108] JS：随机整数
来源：http://ef.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ot.colortex.cn

[U109] JS：数组分组
来源：http://ye.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://js.gzmigu.cn

[U110] JS：数组分块
来源：http://lp.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sd.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://iu.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ts.huanxung.cn

[U112] JS：字符串补位
来源：http://wq.gzmigu.cn

"7".padStart(3, "0")
来源：http://rk.hnjuh.cn

[U113] JS：正则替换全部
来源：http://vm.lnxyls.cn

s.replaceAll("a", "b")
来源：http://lu.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://im.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lq.521024.cn

[U115] JS：生成 UUID
来源：http://mh.jianghongdianzi.cn

crypto.randomUUID()
来源：http://sx.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://yg.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://dt.hnjuh.cn

[U117] JS：单元测试
来源：http://pk.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://qm.huixiangedu.cn

[U118] JS：开发服务器
来源：http://jx.panjiajie.cn

npm i -D vite;  npx vite
来源：http://wb.shxzskj.cn

[U119] JS：生产构建
来源：http://ba.shtwfgs.cn

npx vite build
来源：http://mj.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://ff.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://vu.hahajie.cn

================================================================================
来源：http://vv.yuexingan06.cn

统计汇总
来源：http://nr.colortex.cn

================================================================================
来源：http://bb.bjjhwx.cn

按语言统计（条）：
来源：http://fg.shxzskj.cn

Python ......... 252
来源：http://pw.bjjhwx.cn

PHP ............ 252
来源：http://ea.muxihuayi.cn

JavaScript ..... 252
来源：http://hs.nszjky.cn

TypeScript ..... 212
来源：http://we.huanxung.cn

Java ........... 212
来源：http://ox.panjiajie.cn

Go ............. 212
来源：http://tz.newstarts.cn

Ruby ........... 212
来源：http://oy.gzmigu.cn

C# ............. 212
来源：http://sp.hnjuh.cn

C .............. 30
来源：http://zx.bookmarksfly.cn

C++ ............ 30
来源：http://fz.hahajie.cn

SQL ............ 90
来源：http://qt.colortex.cn

Bash ........... 80
来源：http://xi.bookmarksfly.cn

Kotlin ......... 15
来源：http://ta.shxzskj.cn

Swift .......... 15
来源：http://oa.bjjhwx.cn

Lua ............ 10
来源：http://em.jianghongdianzi.cn

Perl ........... 10
来源：http://np.panjiajie.cn

Scala .......... 10
来源：http://ib.muxihuayi.cn

------------------------------------
来源：http://yp.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://gv.9csxet.cn

按章节统计：
来源：http://zl.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zw.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zn.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hy.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://os.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ac.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vj.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tf.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nz.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vz.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aq.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ri.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://au.shxzskj.cn


<!-- 参考信息 -->