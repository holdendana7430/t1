代发 wailian999

val a = 1;  var b = 2
来源：http://mm.nicolike.cn

[T53] Scala：字符串插值
来源：http://zz.hnjuh.cn

s"值: $b"
来源：http://gk.hahajie.cn

[T54] Scala：集合映射
来源：http://iv.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://di.colortex.cn

[T55] Scala：集合过滤
来源：http://bt.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pa.shxzukj.cn

[T56] Scala：样例类
来源：http://ya.shxzskj.cn

case class User(name: String, age: Int)
来源：http://rp.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://go.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mb.szsharing.cn

[T58] Scala：函数定义
来源：http://vd.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ar.hnjuh.cn

[T59] Scala：循环
来源：http://ir.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://yf.lnxyls.cn

[T60] Scala：折叠
来源：http://em.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dy.hnjuh.cn

================================================================================
来源：http://de.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bu.hahajie.cn

================================================================================
来源：http://uf.colortex.cn

[U01] Py：创建虚拟环境
来源：http://qw.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dz.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://uj.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fq.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://qh.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ra.hnjuh.cn

[U04] Py：变量调试打印
来源：http://zj.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dx.newstarts.cn

[U05] Py：列表去重且保序
来源：http://tx.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://ii.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://hb.gzmigu.cn

{**a, **b}
来源：http://py.newstarts.cn

[U07] Py：反转字典键值
来源：http://lj.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://mz.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://kh.newstarts.cn

[y for x in nested for y in x]
来源：http://hp.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://jf.asd995.cn

max(d, key=d.get)
来源：http://eb.521024.cn

[U10] Py：按值排序字典
来源：http://fq.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hj.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://un.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://tf.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ww.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://xy.hahajie.cn

[U13] Py：固定长度队列
来源：http://om.panjiajie.cn

deque(maxlen=10)
来源：http://vo.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://hm.szxytkj.cn

defaultdict(list)
来源：http://wq.yuexingan06.cn

[U15] Py：高精度计时
来源：http://ir.haigaiapp.cn

t = time.perf_counter()
来源：http://ig.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://pa.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mj.chemitech.net.cn

[U17] Py：初始化日志
来源：http://dv.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://uk.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://kp.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://oy.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://by.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tg.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://sr.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://ol.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://im.wgjwhj.cn

@contextlib.contextmanager
来源：http://va.lnxyls.cn

[U22] Py：矩阵转置
来源：http://lx.yuexingan06.cn

list(zip(*m))
来源：http://ln.newstarts.cn

[U23] Py：分块读取大文件
来源：http://wd.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uz.hahajie.cn

[U24] Py：路径操作
来源：http://qs.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://im.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://fv.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ow.huixiangedu.cn

[U26] Py：并发下载
来源：http://fg.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qv.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://qt.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://nw.huixiangedu.cn

[U28] Py：类型别名
来源：http://pr.yuntaijiaju.cn

UserId = int
来源：http://yi.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://ul.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://qa.muxihuayi.cn

[U30] Py：数据类
来源：http://mp.wgjwhj.cn

@dataclass(slots=True)
来源：http://ym.nicolike.cn

[U31] Py：单测
来源：http://zx.szxytkj.cn

python -m pytest -q
来源：http://vb.huixiangedu.cn

[U32] Py：代码格式化
来源：http://lc.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://if.chemitech.net.cn

[U33] Py：打包发布
来源：http://hg.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ao.szxytkj.cn

[U34] Py：判断编码
来源：http://rw.asd995.cn

chardet.detect(raw)
来源：http://vw.huixiangedu.cn

[U35] Py：发送邮件
来源：http://at.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fz.gzmigu.cn

[U36] Py：定时任务
来源：http://jo.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://ne.nszjky.cn

[U37] Py：读写 Excel
来源：http://al.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rg.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://xp.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://xg.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://nz.bookmarksfly.cn

sys.stdout.isatty()
来源：http://sg.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://ll.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://zb.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://eg.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fn.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://jt.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yk.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ub.hnjuh.cn

namespace App\Http;
来源：http://ax.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://cu.521024.cn

declare(strict_types=1);
来源：http://iw.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://sb.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uv.bjjhwx.cn

[U46] PHP：可空类型
来源：http://ax.hnjuh.cn

?string $name = null
来源：http://ug.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ck.shxzskj.cn

int|string $id
来源：http://eu.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://hf.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ga.szxytkj.cn

[U49] PHP：只读属性
来源：http://tt.nicolike.cn

public readonly string $name
来源：http://th.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://av.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://nt.shxzskj.cn

[U51] PHP：数组解构
来源：http://ol.jctech888.com.cn

[$a, $b] = $arr;
来源：http://sx.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://dh.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://md.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ie.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://mw.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://gi.nicolike.cn

$obj?->method()
来源：http://xz.huanxung.cn

[U55] PHP：match 表达式
来源：http://ng.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nq.yuexingan06.cn

[U56] PHP：命名参数
来源：http://ex.shxzukj.cn

f(a: 1, b: 2)
来源：http://cm.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://zk.szsharing.cn

"值: {$a}"
来源：http://db.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ot.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yz.hnjuh.cn

[U59] PHP：自定义排序
来源：http://wz.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vn.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://ku.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uz.shxzskj.cn

[U61] PHP：正则
来源：http://nz.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fa.hnjuh.cn

[U62] PHP：日期对象
来源：http://wy.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://av.521024.cn

[U63] PHP：文件读写
来源：http://qc.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dw.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://kt.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://qm.bookmarksfly.cn

[U65] PHP：会话
来源：http://uk.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hb.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://dr.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://et.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://fh.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xv.nszjky.cn

[U68] PHP：PDO 连接
来源：http://mi.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tc.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://uj.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fe.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://oe.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xe.nicolike.cn

[U71] PHP：抛出异常
来源：http://am.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://mn.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://xe.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://qy.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://kf.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://cv.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ds.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://zy.nicolike.cn

[U75] PHP：依赖注入
来源：http://uq.szxytkj.cn

composer require psr/container
来源：http://qh.colortex.cn

[U76] PHP：简单路由
来源：http://se.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tv.lnxyls.cn

[U77] PHP：模板渲染
来源：http://hl.bjjhwx.cn

composer require twig/twig
来源：http://bc.shxzskj.cn

[U78] PHP：单元测试
来源：http://mk.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ze.asd995.cn

[U79] PHP：静态分析
来源：http://kv.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://iw.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://ir.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mu.lnxyls.cn

[U81] JS：初始化项目
来源：http://ep.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://mb.nicolike.cn

[U82] JS：package.json 脚本
来源：http://tc.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qk.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://gw.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zh.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://hb.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zd.jctech888.com.cn

[U85] JS：可选链
来源：http://hz.colortex.cn

a?.b?.c
来源：http://ic.haigaiapp.cn

[U86] JS：空值合并
来源：http://ia.wgjwhj.cn

a ?? b
来源：http://ia.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://xi.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://ol.hahajie.cn

[U88] JS：对象展开合并
来源：http://so.hnjuh.cn

{ ...a, ...b }
来源：http://sr.bookmarksfly.cn

[U89] JS：数组去重
来源：http://zv.9csxet.cn

[...new Set(arr)]
来源：http://ia.shxzukj.cn

[U90] JS：数字数组排序
来源：http://ts.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://uy.nicolike.cn

[U91] JS：对象键值遍历
来源：http://av.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wg.bjjhwx.cn

[U92] JS：深拷贝
来源：http://cq.wgjwhj.cn

structuredClone(obj)
来源：http://ot.yuexingan06.cn

[U93] JS：模板字符串
来源：http://af.nszjky.cn

`共 ${n} 条`
来源：http://zy.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://ii.newstarts.cn

const double = x => x * 2;
来源：http://im.huanxung.cn

[U95] JS：Promise 包装
来源：http://wc.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://pv.asd995.cn

[U96] JS：async/await 与异常
来源：http://jd.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ky.gzmigu.cn

[U97] JS：并发请求
来源：http://se.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hc.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://hr.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xi.lnxyls.cn

[U99] JS：事件监听
来源：http://aa.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://dr.asd995.cn

[U100] JS：DOM 查询
来源：http://br.nszjky.cn

document.querySelector(".item")
来源：http://bx.asd995.cn

[U101] JS：classList 操作
来源：http://tl.hahajie.cn

el.classList.toggle("active")
来源：http://mg.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://gt.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://il.huixinmuqiang.cn

[U103] JS：定时器
来源：http://zk.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wy.panjiajie.cn

[U104] JS：防抖
来源：http://gq.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://je.asd995.cn

[U105] JS：节流
来源：http://su.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sy.bjjhwx.cn

[U106] JS：日期格式化
来源：http://ak.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://js.shxzskj.cn

[U107] JS：数字千分位
来源：http://ze.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://in.szsharing.cn

[U108] JS：随机整数
来源：http://eq.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eg.huanxung.cn

[U109] JS：数组分组
来源：http://al.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://bq.jctech888.com.cn

[U110] JS：数组分块
来源：http://tq.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ix.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://xb.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://et.muxihuayi.cn

[U112] JS：字符串补位
来源：http://nq.colortex.cn

"7".padStart(3, "0")
来源：http://lb.szxytkj.cn

[U113] JS：正则替换全部
来源：http://ur.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://wm.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://za.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zo.newstarts.cn

[U115] JS：生成 UUID
来源：http://bi.huixinmuqiang.cn

crypto.randomUUID()
来源：http://vz.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://bn.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://my.gzmigu.cn

[U117] JS：单元测试
来源：http://te.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://da.gzmigu.cn

[U118] JS：开发服务器
来源：http://nn.huanxung.cn

npm i -D vite;  npx vite
来源：http://qt.asd995.cn

[U119] JS：生产构建
来源：http://oj.bookmarksfly.cn

npx vite build
来源：http://rt.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://mj.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://ko.panjiajie.cn

================================================================================
来源：http://sw.asd995.cn

统计汇总
来源：http://pt.asd995.cn

================================================================================
来源：http://vo.hahajie.cn

按语言统计（条）：
来源：http://aq.asd995.cn

Python ......... 252
来源：http://vf.hahajie.cn

PHP ............ 252
来源：http://cq.huixinmuqiang.cn

JavaScript ..... 252
来源：http://lo.lnxyls.cn

TypeScript ..... 212
来源：http://ys.hahajie.cn

Java ........... 212
来源：http://mp.huanxung.cn

Go ............. 212
来源：http://kq.colortex.cn

Ruby ........... 212
来源：http://qe.szxytkj.cn

C# ............. 212
来源：http://kb.shxzskj.cn

C .............. 30
来源：http://ld.szxytkj.cn

C++ ............ 30
来源：http://ne.shtwfgs.cn

SQL ............ 90
来源：http://be.chemitech.net.cn

Bash ........... 80
来源：http://uu.newstarts.cn

Kotlin ......... 15
来源：http://ne.9csxet.cn

Swift .......... 15
来源：http://jk.yuexingan06.cn

Lua ............ 10
来源：http://lh.colortex.cn

Perl ........... 10
来源：http://nm.huanxung.cn

Scala .......... 10
来源：http://fa.huanxung.cn

------------------------------------
来源：http://kf.9csxet.cn

合计 ........... 2106 条
来源：http://bf.hnjuh.cn

按章节统计：
来源：http://ml.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mk.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ce.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dz.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://po.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mm.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eo.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jg.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ee.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uq.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oi.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lh.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ta.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bd.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ox.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hk.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jb.szsharing.cn


<!-- 参考信息 -->