代发 wailian999

val a = 1;  var b = 2
来源：http://vx.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://jg.huixinmuqiang.cn

s"值: $b"
来源：http://pb.shtwfgs.cn

[T54] Scala：集合映射
来源：http://ul.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://tj.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://zz.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lw.jctech888.com.cn

[T56] Scala：样例类
来源：http://gi.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ai.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://ct.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lw.shxzskj.cn

[T58] Scala：函数定义
来源：http://sd.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cs.lnxyls.cn

[T59] Scala：循环
来源：http://el.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://kw.huanxung.cn

[T60] Scala：折叠
来源：http://gi.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://de.yuntaijiaju.cn

================================================================================
来源：http://sr.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sd.bjjhwx.cn

================================================================================
来源：http://sy.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://rh.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kv.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://tt.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ay.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://ye.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yv.lnxyls.cn

[U04] Py：变量调试打印
来源：http://sb.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ym.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://sy.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://xi.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://ya.asd995.cn

{**a, **b}
来源：http://hu.nszjky.cn

[U07] Py：反转字典键值
来源：http://lf.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://wz.nicolike.cn

[U08] Py：展平二维列表
来源：http://mw.jctech888.com.cn

[y for x in nested for y in x]
来源：http://dx.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://hv.huixinmuqiang.cn

max(d, key=d.get)
来源：http://sx.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://mj.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://id.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://rq.panjiajie.cn

(x * 2 for x in arr)
来源：http://ep.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gm.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://nj.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://cm.wgjwhj.cn

deque(maxlen=10)
来源：http://bl.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://fe.nicolike.cn

defaultdict(list)
来源：http://pl.muxihuayi.cn

[U15] Py：高精度计时
来源：http://ry.bookmarksfly.cn

t = time.perf_counter()
来源：http://yp.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://qp.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xf.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://hb.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://mi.hahajie.cn

[U18] Py：预编译正则
来源：http://nq.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://ay.521024.cn

[U19] Py：正则替换带回调
来源：http://rh.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uc.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ll.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://jc.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://em.shxzskj.cn

@contextlib.contextmanager
来源：http://vw.gzmigu.cn

[U22] Py：矩阵转置
来源：http://ll.huixiangedu.cn

list(zip(*m))
来源：http://bn.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://ck.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tg.wgjwhj.cn

[U24] Py：路径操作
来源：http://gw.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nm.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://oh.bookmarksfly.cn

csv.DictReader(f)
来源：http://gs.asd995.cn

[U26] Py：并发下载
来源：http://mw.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ea.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://gk.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://nv.muxihuayi.cn

[U28] Py：类型别名
来源：http://tk.gzmigu.cn

UserId = int
来源：http://ho.9csxet.cn

[U29] Py：属性校验
来源：http://fg.9csxet.cn

@property 与 @x.setter 配合
来源：http://rp.yuntaijiaju.cn

[U30] Py：数据类
来源：http://aq.colortex.cn

@dataclass(slots=True)
来源：http://wu.shtwfgs.cn

[U31] Py：单测
来源：http://gy.szsharing.cn

python -m pytest -q
来源：http://ow.szxytkj.cn

[U32] Py：代码格式化
来源：http://sh.nicolike.cn

ruff format . && ruff check --fix .
来源：http://cu.shtwfgs.cn

[U33] Py：打包发布
来源：http://hq.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://qd.chemitech.net.cn

[U34] Py：判断编码
来源：http://xc.shxzskj.cn

chardet.detect(raw)
来源：http://yk.szxytkj.cn

[U35] Py：发送邮件
来源：http://vr.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hl.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ir.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://sr.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://oc.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zs.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://nq.hnjuh.cn

Path(__file__).resolve().parent
来源：http://sv.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://sr.shtwfgs.cn

sys.stdout.isatty()
来源：http://bl.hahajie.cn

[U40] Py：打印到标准错误
来源：http://yq.521024.cn

print("err", file=sys.stderr)
来源：http://cs.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://mq.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fi.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://rc.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tc.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://fk.szsharing.cn

namespace App\Http;
来源：http://je.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://dy.huixiangedu.cn

declare(strict_types=1);
来源：http://qi.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://rr.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xy.chemitech.net.cn

[U46] PHP：可空类型
来源：http://ph.asd995.cn

?string $name = null
来源：http://mf.hnjuh.cn

[U47] PHP：联合类型
来源：http://si.shxzskj.cn

int|string $id
来源：http://pr.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://wy.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://va.haigaiapp.cn

[U49] PHP：只读属性
来源：http://lr.bookmarksfly.cn

public readonly string $name
来源：http://yy.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://tu.huanxung.cn

public function __construct(private int $id) {}
来源：http://yt.wgjwhj.cn

[U51] PHP：数组解构
来源：http://ib.szxytkj.cn

[$a, $b] = $arr;
来源：http://pw.nicolike.cn

[U52] PHP：箭头函数
来源：http://vp.521024.cn

$double = fn($x) => $x * 2;
来源：http://ou.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://da.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://qt.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://bt.lnxyls.cn

$obj?->method()
来源：http://st.szsharing.cn

[U55] PHP：match 表达式
来源：http://ul.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://du.hnjuh.cn

[U56] PHP：命名参数
来源：http://wm.521024.cn

f(a: 1, b: 2)
来源：http://cr.lnxyls.cn

[U57] PHP：字符串插值
来源：http://ks.hnjuh.cn

"值: {$a}"
来源：http://wd.shxzskj.cn

[U58] PHP：数组三件套
来源：http://zs.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sd.panjiajie.cn

[U59] PHP：自定义排序
来源：http://dj.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yd.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://vp.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lh.szxytkj.cn

[U61] PHP：正则
来源：http://sa.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nj.bjjhwx.cn

[U62] PHP：日期对象
来源：http://dg.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zi.szxytkj.cn

[U63] PHP：文件读写
来源：http://rz.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ii.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://to.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://bn.jianghongdianzi.cn

[U65] PHP：会话
来源：http://dm.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://de.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://eo.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qq.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://km.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ug.newstarts.cn

[U68] PHP：PDO 连接
来源：http://gf.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://da.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://hy.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hr.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://tr.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oa.hahajie.cn

[U71] PHP：抛出异常
来源：http://wx.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://qv.asd995.cn

[U72] PHP：写错误日志
来源：http://uj.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://fp.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://op.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://no.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://xs.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ot.szsharing.cn

[U75] PHP：依赖注入
来源：http://dt.shxzskj.cn

composer require psr/container
来源：http://vb.shtwfgs.cn

[U76] PHP：简单路由
来源：http://wt.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zw.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://jb.muxihuayi.cn

composer require twig/twig
来源：http://qz.muxihuayi.cn

[U78] PHP：单元测试
来源：http://ui.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://hm.wgjwhj.cn

[U79] PHP：静态分析
来源：http://fn.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://kj.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://on.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ry.lnxyls.cn

[U81] JS：初始化项目
来源：http://fv.bjjhwx.cn

npm init -y;  npm i express
来源：http://tp.hahajie.cn

[U82] JS：package.json 脚本
来源：http://lj.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vs.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://tc.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iz.asd995.cn

[U84] JS：CommonJS 写法
来源：http://kj.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vw.chemitech.net.cn

[U85] JS：可选链
来源：http://ji.gzmigu.cn

a?.b?.c
来源：http://hj.gzmigu.cn

[U86] JS：空值合并
来源：http://yw.bjjhwx.cn

a ?? b
来源：http://lc.szsharing.cn

[U87] JS：解构默认值
来源：http://og.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ur.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://hx.colortex.cn

{ ...a, ...b }
来源：http://ju.huanxung.cn

[U89] JS：数组去重
来源：http://gx.521024.cn

[...new Set(arr)]
来源：http://tm.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ji.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://cn.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wy.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ps.yuexingan06.cn

[U92] JS：深拷贝
来源：http://ru.chemitech.net.cn

structuredClone(obj)
来源：http://ef.szxytkj.cn

[U93] JS：模板字符串
来源：http://wn.yuntaijiaju.cn

`共 ${n} 条`
来源：http://ya.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://ij.521024.cn

const double = x => x * 2;
来源：http://bm.hahajie.cn

[U95] JS：Promise 包装
来源：http://sf.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://fq.asd995.cn

[U96] JS：async/await 与异常
来源：http://ei.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zh.hnjuh.cn

[U97] JS：并发请求
来源：http://ua.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jj.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://ap.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rp.szxytkj.cn

[U99] JS：事件监听
来源：http://wc.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://ro.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://hz.szxytkj.cn

document.querySelector(".item")
来源：http://cz.szxytkj.cn

[U101] JS：classList 操作
来源：http://fq.gzmigu.cn

el.classList.toggle("active")
来源：http://rf.asd995.cn

[U102] JS：本地存储
来源：http://zl.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.bjjhwx.cn

[U103] JS：定时器
来源：http://bi.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fx.yuexingan06.cn

[U104] JS：防抖
来源：http://cs.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pl.9csxet.cn

[U105] JS：节流
来源：http://jv.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ve.haigaiapp.cn

[U106] JS：日期格式化
来源：http://ce.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sm.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ph.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iu.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://jr.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ac.shtwfgs.cn

[U109] JS：数组分组
来源：http://eu.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://zr.bjjhwx.cn

[U110] JS：数组分块
来源：http://od.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dy.asd995.cn

[U111] JS：对象转 Map
来源：http://cn.nicolike.cn

new Map(Object.entries(obj))
来源：http://go.9csxet.cn

[U112] JS：字符串补位
来源：http://rk.huixiangedu.cn

"7".padStart(3, "0")
来源：http://tf.szxytkj.cn

[U113] JS：正则替换全部
来源：http://fj.huanxung.cn

s.replaceAll("a", "b")
来源：http://nx.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://zl.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://to.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://qd.521024.cn

crypto.randomUUID()
来源：http://cu.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://wu.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://eo.bookmarksfly.cn

[U117] JS：单元测试
来源：http://wb.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://tb.hnjuh.cn

[U118] JS：开发服务器
来源：http://gy.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://fj.szsharing.cn

[U119] JS：生产构建
来源：http://lj.bookmarksfly.cn

npx vite build
来源：http://hs.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://si.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://sa.asd995.cn

================================================================================
来源：http://bk.hahajie.cn

统计汇总
来源：http://um.szsharing.cn

================================================================================
来源：http://dd.hnjuh.cn

按语言统计（条）：
来源：http://vg.hahajie.cn

Python ......... 252
来源：http://nt.hnjuh.cn

PHP ............ 252
来源：http://ef.colortex.cn

JavaScript ..... 252
来源：http://ao.shtwfgs.cn

TypeScript ..... 212
来源：http://wt.hnjuh.cn

Java ........... 212
来源：http://sw.huanxung.cn

Go ............. 212
来源：http://jz.9csxet.cn

Ruby ........... 212
来源：http://yk.nicolike.cn

C# ............. 212
来源：http://df.gzmigu.cn

C .............. 30
来源：http://xh.huixiangedu.cn

C++ ............ 30
来源：http://qj.yuntaijiaju.cn

SQL ............ 90
来源：http://dw.newstarts.cn

Bash ........... 80
来源：http://zt.wgjwhj.cn

Kotlin ......... 15
来源：http://br.lnxyls.cn

Swift .......... 15
来源：http://eg.huixiangedu.cn

Lua ............ 10
来源：http://qu.asd995.cn

Perl ........... 10
来源：http://xd.szxytkj.cn

Scala .......... 10
来源：http://kq.hahajie.cn

------------------------------------
来源：http://ho.hnjuh.cn

合计 ........... 2106 条
来源：http://zj.wgjwhj.cn

按章节统计：
来源：http://ua.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tq.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qo.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://if.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cn.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pt.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wl.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vr.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bg.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sf.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zs.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bg.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pm.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sx.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pg.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ks.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ey.muxihuayi.cn


<!-- 参考信息 -->