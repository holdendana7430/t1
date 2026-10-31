代发 wailian999

case class User(name: String, age: Int)
来源：http://vp.nicolike.cn

[T57] Scala：模式匹配
来源：http://ye.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pd.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://wa.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xl.wgjwhj.cn

[T59] Scala：循环
来源：http://ys.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://rb.colortex.cn

[T60] Scala：折叠
来源：http://cz.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ze.haigaiapp.cn

================================================================================
来源：http://ng.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vd.newstarts.cn

================================================================================
来源：http://ec.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://ha.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mt.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://sn.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xq.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://nu.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kb.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://pl.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sg.newstarts.cn

[U05] Py：列表去重且保序
来源：http://gd.colortex.cn

list(dict.fromkeys(arr))
来源：http://ku.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://li.huixinmuqiang.cn

{**a, **b}
来源：http://he.lnxyls.cn

[U07] Py：反转字典键值
来源：http://xn.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://cv.shxzukj.cn

[U08] Py：展平二维列表
来源：http://hx.521024.cn

[y for x in nested for y in x]
来源：http://bt.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://on.huanxung.cn

max(d, key=d.get)
来源：http://xw.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://xc.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nt.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://sm.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://sj.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dl.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://vh.nicolike.cn

[U13] Py：固定长度队列
来源：http://ya.hahajie.cn

deque(maxlen=10)
来源：http://wx.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://si.szsharing.cn

defaultdict(list)
来源：http://hj.haigaiapp.cn

[U15] Py：高精度计时
来源：http://zy.huanxung.cn

t = time.perf_counter()
来源：http://th.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://uh.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qw.wgjwhj.cn

[U17] Py：初始化日志
来源：http://fj.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://zi.colortex.cn

[U18] Py：预编译正则
来源：http://cu.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://yz.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://br.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sd.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://vj.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://rc.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://vs.521024.cn

@contextlib.contextmanager
来源：http://by.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://pv.yuntaijiaju.cn

list(zip(*m))
来源：http://ko.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://sj.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mg.shxzukj.cn

[U24] Py：路径操作
来源：http://bb.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fl.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ux.bjjhwx.cn

csv.DictReader(f)
来源：http://cd.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://ek.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gx.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://pz.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qi.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://zd.jctech888.com.cn

UserId = int
来源：http://hn.bookmarksfly.cn

[U29] Py：属性校验
来源：http://eh.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://bs.521024.cn

[U30] Py：数据类
来源：http://ng.hnjuh.cn

@dataclass(slots=True)
来源：http://aw.hnjuh.cn

[U31] Py：单测
来源：http://pi.haigaiapp.cn

python -m pytest -q
来源：http://qv.shtwfgs.cn

[U32] Py：代码格式化
来源：http://ng.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ps.shxzskj.cn

[U33] Py：打包发布
来源：http://gb.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://en.shxzskj.cn

[U34] Py：判断编码
来源：http://pj.jctech888.com.cn

chardet.detect(raw)
来源：http://qs.colortex.cn

[U35] Py：发送邮件
来源：http://ef.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ly.shxzskj.cn

[U36] Py：定时任务
来源：http://gu.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://hn.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://bl.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ok.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://if.asd995.cn

Path(__file__).resolve().parent
来源：http://pn.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://dc.szsharing.cn

sys.stdout.isatty()
来源：http://zf.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://nt.newstarts.cn

print("err", file=sys.stderr)
来源：http://er.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://gh.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pa.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://bu.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://id.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://be.bookmarksfly.cn

namespace App\Http;
来源：http://as.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://yb.lnxyls.cn

declare(strict_types=1);
来源：http://jl.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://nd.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ut.hahajie.cn

[U46] PHP：可空类型
来源：http://fj.yuexingan06.cn

?string $name = null
来源：http://nh.hnjuh.cn

[U47] PHP：联合类型
来源：http://az.huanxung.cn

int|string $id
来源：http://jy.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://iq.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ci.huanxung.cn

[U49] PHP：只读属性
来源：http://xw.shxzukj.cn

public readonly string $name
来源：http://uf.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://mb.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ko.muxihuayi.cn

[U51] PHP：数组解构
来源：http://fp.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://zu.gzmigu.cn

[U52] PHP：箭头函数
来源：http://dt.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://py.521024.cn

[U53] PHP：空合并运算符
来源：http://na.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://jg.shxzskj.cn

[U54] PHP：空安全调用
来源：http://cp.asd995.cn

$obj?->method()
来源：http://oi.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://va.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kw.shxzukj.cn

[U56] PHP：命名参数
来源：http://fq.chemitech.net.cn

f(a: 1, b: 2)
来源：http://yl.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://vx.newstarts.cn

"值: {$a}"
来源：http://jh.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://me.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ou.hahajie.cn

[U59] PHP：自定义排序
来源：http://wz.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iw.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://hq.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sb.haigaiapp.cn

[U61] PHP：正则
来源：http://wz.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jb.panjiajie.cn

[U62] PHP：日期对象
来源：http://js.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://he.nszjky.cn

[U63] PHP：文件读写
来源：http://ke.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kd.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://qc.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ku.bjjhwx.cn

[U65] PHP：会话
来源：http://fm.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vt.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://jv.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ke.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://ku.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gy.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://vo.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cj.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://ko.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ym.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://gc.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kv.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://wo.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://vp.newstarts.cn

[U72] PHP：写错误日志
来源：http://oh.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://ef.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://he.521024.cn

parse_ini_file("config.ini", true)
来源：http://bx.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://oo.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://yl.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://jv.hnjuh.cn

composer require psr/container
来源：http://ph.hahajie.cn

[U76] PHP：简单路由
来源：http://fi.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sq.gzmigu.cn

[U77] PHP：模板渲染
来源：http://it.yuexingan06.cn

composer require twig/twig
来源：http://hv.lnxyls.cn

[U78] PHP：单元测试
来源：http://cq.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://ij.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://zc.asd995.cn

composer require --dev phpstan/phpstan
来源：http://kt.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://lz.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wr.lnxyls.cn

[U81] JS：初始化项目
来源：http://ie.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://jr.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://br.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nn.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://sw.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sb.521024.cn

[U84] JS：CommonJS 写法
来源：http://ue.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yo.jctech888.com.cn

[U85] JS：可选链
来源：http://zb.jianghongdianzi.cn

a?.b?.c
来源：http://dw.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://ez.haigaiapp.cn

a ?? b
来源：http://ik.hnjuh.cn

[U87] JS：解构默认值
来源：http://dp.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://vf.panjiajie.cn

[U88] JS：对象展开合并
来源：http://pd.nszjky.cn

{ ...a, ...b }
来源：http://sj.newstarts.cn

[U89] JS：数组去重
来源：http://cv.yuntaijiaju.cn

[...new Set(arr)]
来源：http://ky.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://xi.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://wz.colortex.cn

[U91] JS：对象键值遍历
来源：http://kw.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oc.haigaiapp.cn

[U92] JS：深拷贝
来源：http://nf.yuntaijiaju.cn

structuredClone(obj)
来源：http://bm.jctech888.com.cn

[U93] JS：模板字符串
来源：http://kr.newstarts.cn

`共 ${n} 条`
来源：http://jc.chemitech.net.cn

[U94] JS：箭头函数
来源：http://jr.muxihuayi.cn

const double = x => x * 2;
来源：http://au.huanxung.cn

[U95] JS：Promise 包装
来源：http://qa.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://gd.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://xp.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ab.bookmarksfly.cn

[U97] JS：并发请求
来源：http://sl.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ez.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://lx.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gr.jctech888.com.cn

[U99] JS：事件监听
来源：http://se.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://og.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://ra.bookmarksfly.cn

document.querySelector(".item")
来源：http://ru.nicolike.cn

[U101] JS：classList 操作
来源：http://nv.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://lb.szsharing.cn

[U102] JS：本地存储
来源：http://mx.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pd.shtwfgs.cn

[U103] JS：定时器
来源：http://jd.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ps.haigaiapp.cn

[U104] JS：防抖
来源：http://yf.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kj.9csxet.cn

[U105] JS：节流
来源：http://lw.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ff.jctech888.com.cn

[U106] JS：日期格式化
来源：http://pb.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mq.huanxung.cn

[U107] JS：数字千分位
来源：http://cy.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://la.9csxet.cn

[U108] JS：随机整数
来源：http://du.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ch.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://wb.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://cl.shxzskj.cn

[U110] JS：数组分块
来源：http://nv.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sm.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://um.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://tc.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://tj.panjiajie.cn

"7".padStart(3, "0")
来源：http://cq.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ug.colortex.cn

s.replaceAll("a", "b")
来源：http://lq.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://uf.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vi.gzmigu.cn

[U115] JS：生成 UUID
来源：http://ac.nszjky.cn

crypto.randomUUID()
来源：http://ei.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://os.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://jo.bookmarksfly.cn

[U117] JS：单元测试
来源：http://ge.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://dw.gzmigu.cn

[U118] JS：开发服务器
来源：http://tv.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://hd.shtwfgs.cn

[U119] JS：生产构建
来源：http://fn.shtwfgs.cn

npx vite build
来源：http://hr.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://xa.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://nn.jctech888.com.cn

================================================================================
来源：http://mg.yuntaijiaju.cn

统计汇总
来源：http://ui.newstarts.cn

================================================================================
来源：http://vc.hahajie.cn

按语言统计（条）：
来源：http://id.chemitech.net.cn

Python ......... 252
来源：http://ro.lnxyls.cn

PHP ............ 252
来源：http://bt.shxzskj.cn

JavaScript ..... 252
来源：http://gt.bookmarksfly.cn

TypeScript ..... 212
来源：http://zx.nicolike.cn

Java ........... 212
来源：http://yv.newstarts.cn

Go ............. 212
来源：http://kt.panjiajie.cn

Ruby ........... 212
来源：http://cx.bookmarksfly.cn

C# ............. 212
来源：http://cr.haigaiapp.cn

C .............. 30
来源：http://wl.huixinmuqiang.cn

C++ ............ 30
来源：http://fl.shxzskj.cn

SQL ............ 90
来源：http://zf.shxzukj.cn

Bash ........... 80
来源：http://xc.szxytkj.cn

Kotlin ......... 15
来源：http://ha.bookmarksfly.cn

Swift .......... 15
来源：http://ec.panjiajie.cn

Lua ............ 10
来源：http://wg.yuntaijiaju.cn

Perl ........... 10
来源：http://zy.muxihuayi.cn

Scala .......... 10
来源：http://sn.huanxung.cn

------------------------------------
来源：http://gw.yuexingan06.cn

合计 ........... 2106 条
来源：http://ve.jianghongdianzi.cn

按章节统计：
来源：http://so.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://op.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dz.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zx.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qd.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rd.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fq.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uf.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ms.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ua.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lr.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://be.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lb.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tb.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oo.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ls.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zm.hahajie.cn

Q SQL 专题                              90
来源：http://fq.yuntaijiaju.cn

R Bash 专题                             80
来源：http://tt.huixiangedu.cn

S C / C++ 专题                          60
来源：http://zl.bjjhwx.cn

T 其他语言补充                          60
来源：http://xj.panjiajie.cn

U 高频实用片段                         120
来源：http://ve.521024.cn

------------------------------------
来源：http://km.huanxung.cn

合计                                  2106 条
来源：http://ha.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://dn.panjiajie.cn


<!-- 参考信息 -->