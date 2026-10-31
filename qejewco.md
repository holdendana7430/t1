代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://dk.nszjky.cn

[T59] Scala：循环
来源：http://yj.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://bt.bjjhwx.cn

[T60] Scala：折叠
来源：http://fc.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cm.nszjky.cn

================================================================================
来源：http://ll.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gj.asd995.cn

================================================================================
来源：http://zk.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://lg.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sz.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://hn.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ya.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://yk.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ud.newstarts.cn

[U04] Py：变量调试打印
来源：http://op.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kt.9csxet.cn

[U05] Py：列表去重且保序
来源：http://ke.9csxet.cn

list(dict.fromkeys(arr))
来源：http://zr.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://yu.newstarts.cn

{**a, **b}
来源：http://zp.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://ef.nszjky.cn

{v: k for k, v in d.items()}
来源：http://pj.colortex.cn

[U08] Py：展平二维列表
来源：http://cc.newstarts.cn

[y for x in nested for y in x]
来源：http://ao.521024.cn

[U09] Py：字典取最大值的键
来源：http://hp.szsharing.cn

max(d, key=d.get)
来源：http://zh.521024.cn

[U10] Py：按值排序字典
来源：http://ht.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rb.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://fr.chemitech.net.cn

(x * 2 for x in arr)
来源：http://fv.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://md.newstarts.cn

Counter(arr).most_common(3)
来源：http://wk.huanxung.cn

[U13] Py：固定长度队列
来源：http://tg.szxytkj.cn

deque(maxlen=10)
来源：http://ec.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://ni.yuntaijiaju.cn

defaultdict(list)
来源：http://zh.hnjuh.cn

[U15] Py：高精度计时
来源：http://oh.huixinmuqiang.cn

t = time.perf_counter()
来源：http://xd.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://wl.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dr.asd995.cn

[U17] Py：初始化日志
来源：http://il.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://ng.yuexingan06.cn

[U18] Py：预编译正则
来源：http://ag.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://pn.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://sv.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gl.colortex.cn

[U20] Py：缓存函数结果
来源：http://xh.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://za.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://km.panjiajie.cn

@contextlib.contextmanager
来源：http://ka.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://ud.hahajie.cn

list(zip(*m))
来源：http://pt.huanxung.cn

[U23] Py：分块读取大文件
来源：http://ys.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://um.jctech888.com.cn

[U24] Py：路径操作
来源：http://ml.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rb.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://yp.jctech888.com.cn

csv.DictReader(f)
来源：http://mn.newstarts.cn

[U26] Py：并发下载
来源：http://rk.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://su.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://tm.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://zi.asd995.cn

[U28] Py：类型别名
来源：http://ki.muxihuayi.cn

UserId = int
来源：http://nr.nszjky.cn

[U29] Py：属性校验
来源：http://uc.nicolike.cn

@property 与 @x.setter 配合
来源：http://ae.wgjwhj.cn

[U30] Py：数据类
来源：http://tv.chemitech.net.cn

@dataclass(slots=True)
来源：http://po.jctech888.com.cn

[U31] Py：单测
来源：http://st.shtwfgs.cn

python -m pytest -q
来源：http://ho.bjjhwx.cn

[U32] Py：代码格式化
来源：http://xu.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://qs.bookmarksfly.cn

[U33] Py：打包发布
来源：http://eo.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://rs.shxzskj.cn

[U34] Py：判断编码
来源：http://qr.chemitech.net.cn

chardet.detect(raw)
来源：http://oi.hnjuh.cn

[U35] Py：发送邮件
来源：http://hs.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pr.shxzukj.cn

[U36] Py：定时任务
来源：http://pg.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://pe.521024.cn

[U37] Py：读写 Excel
来源：http://dv.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yg.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://yc.huanxung.cn

Path(__file__).resolve().parent
来源：http://ap.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ac.jctech888.com.cn

sys.stdout.isatty()
来源：http://fn.9csxet.cn

[U40] Py：打印到标准错误
来源：http://pi.9csxet.cn

print("err", file=sys.stderr)
来源：http://sr.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://ps.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vg.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://cu.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fq.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://jq.szsharing.cn

namespace App\Http;
来源：http://wb.9csxet.cn

[U44] PHP：开启严格类型
来源：http://ld.jctech888.com.cn

declare(strict_types=1);
来源：http://vl.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://in.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kz.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://vr.newstarts.cn

?string $name = null
来源：http://ax.shxzskj.cn

[U47] PHP：联合类型
来源：http://ni.lnxyls.cn

int|string $id
来源：http://vo.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://eu.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cb.521024.cn

[U49] PHP：只读属性
来源：http://zf.yuexingan06.cn

public readonly string $name
来源：http://hb.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://xo.521024.cn

public function __construct(private int $id) {}
来源：http://wu.jctech888.com.cn

[U51] PHP：数组解构
来源：http://rv.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://lm.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://ax.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://bi.hahajie.cn

[U53] PHP：空合并运算符
来源：http://kc.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://ih.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://mb.muxihuayi.cn

$obj?->method()
来源：http://te.nicolike.cn

[U55] PHP：match 表达式
来源：http://op.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tx.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://mz.szxytkj.cn

f(a: 1, b: 2)
来源：http://sv.asd995.cn

[U57] PHP：字符串插值
来源：http://cv.newstarts.cn

"值: {$a}"
来源：http://rz.lnxyls.cn

[U58] PHP：数组三件套
来源：http://aa.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cf.nicolike.cn

[U59] PHP：自定义排序
来源：http://cl.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://ce.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uc.shxzukj.cn

[U61] PHP：正则
来源：http://be.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vc.colortex.cn

[U62] PHP：日期对象
来源：http://zb.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lw.haigaiapp.cn

[U63] PHP：文件读写
来源：http://xe.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wm.lnxyls.cn

[U64] PHP：目录遍历
来源：http://mn.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://sh.jctech888.com.cn

[U65] PHP：会话
来源：http://da.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fb.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://vh.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ju.nszjky.cn

[U67] PHP：处理文件上传
来源：http://nj.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sk.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ff.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jv.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://hb.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yy.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://lb.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://od.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://nm.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://nz.lnxyls.cn

[U72] PHP：写错误日志
来源：http://wy.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://kd.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://ku.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://rm.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://yf.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://ij.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://ak.asd995.cn

composer require psr/container
来源：http://rg.lnxyls.cn

[U76] PHP：简单路由
来源：http://eu.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sa.szxytkj.cn

[U77] PHP：模板渲染
来源：http://wy.521024.cn

composer require twig/twig
来源：http://xg.chemitech.net.cn

[U78] PHP：单元测试
来源：http://yb.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://dy.newstarts.cn

[U79] PHP：静态分析
来源：http://jt.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://bp.521024.cn

[U80] PHP：代码规范修复
来源：http://ak.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uk.chemitech.net.cn

[U81] JS：初始化项目
来源：http://to.haigaiapp.cn

npm init -y;  npm i express
来源：http://kn.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://rp.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yv.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://fh.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kt.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://rl.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://df.hahajie.cn

[U85] JS：可选链
来源：http://te.colortex.cn

a?.b?.c
来源：http://wm.jctech888.com.cn

[U86] JS：空值合并
来源：http://nh.chemitech.net.cn

a ?? b
来源：http://gp.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://xz.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://ta.szsharing.cn

[U88] JS：对象展开合并
来源：http://pc.bookmarksfly.cn

{ ...a, ...b }
来源：http://ke.colortex.cn

[U89] JS：数组去重
来源：http://zo.shxzskj.cn

[...new Set(arr)]
来源：http://tj.huanxung.cn

[U90] JS：数字数组排序
来源：http://dr.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://tm.szsharing.cn

[U91] JS：对象键值遍历
来源：http://mp.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hr.haigaiapp.cn

[U92] JS：深拷贝
来源：http://hg.521024.cn

structuredClone(obj)
来源：http://jd.wgjwhj.cn

[U93] JS：模板字符串
来源：http://fl.gzmigu.cn

`共 ${n} 条`
来源：http://cq.hahajie.cn

[U94] JS：箭头函数
来源：http://wi.panjiajie.cn

const double = x => x * 2;
来源：http://jt.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://db.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://do.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://iz.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dr.haigaiapp.cn

[U97] JS：并发请求
来源：http://ho.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://re.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nn.chemitech.net.cn

[U99] JS：事件监听
来源：http://om.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://zj.521024.cn

[U100] JS：DOM 查询
来源：http://hq.yuntaijiaju.cn

document.querySelector(".item")
来源：http://au.gzmigu.cn

[U101] JS：classList 操作
来源：http://zy.haigaiapp.cn

el.classList.toggle("active")
来源：http://zn.shtwfgs.cn

[U102] JS：本地存储
来源：http://yx.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gb.shtwfgs.cn

[U103] JS：定时器
来源：http://ih.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fz.asd995.cn

[U104] JS：防抖
来源：http://aj.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vo.lnxyls.cn

[U105] JS：节流
来源：http://ss.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tw.shtwfgs.cn

[U106] JS：日期格式化
来源：http://jh.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qq.huixiangedu.cn

[U107] JS：数字千分位
来源：http://il.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dr.nszjky.cn

[U108] JS：随机整数
来源：http://lw.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://no.bookmarksfly.cn

[U109] JS：数组分组
来源：http://ml.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://jw.asd995.cn

[U110] JS：数组分块
来源：http://uw.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mh.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://rt.colortex.cn

new Map(Object.entries(obj))
来源：http://ws.nszjky.cn

[U112] JS：字符串补位
来源：http://lj.shxzukj.cn

"7".padStart(3, "0")
来源：http://ha.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://wg.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://xh.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://ni.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jr.newstarts.cn

[U115] JS：生成 UUID
来源：http://wl.haigaiapp.cn

crypto.randomUUID()
来源：http://es.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://ke.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://ln.hnjuh.cn

[U117] JS：单元测试
来源：http://yg.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://rj.huanxung.cn

[U118] JS：开发服务器
来源：http://jh.asd995.cn

npm i -D vite;  npx vite
来源：http://rf.haigaiapp.cn

[U119] JS：生产构建
来源：http://ny.asd995.cn

npx vite build
来源：http://in.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://am.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://sr.shtwfgs.cn

================================================================================
来源：http://gu.9csxet.cn

统计汇总
来源：http://dj.huixinmuqiang.cn

================================================================================
来源：http://we.yuexingan06.cn

按语言统计（条）：
来源：http://yu.bjjhwx.cn

Python ......... 252
来源：http://kj.shxzukj.cn

PHP ............ 252
来源：http://gb.jianghongdianzi.cn

JavaScript ..... 252
来源：http://cj.huanxung.cn

TypeScript ..... 212
来源：http://zj.shtwfgs.cn

Java ........... 212
来源：http://qr.bjjhwx.cn

Go ............. 212
来源：http://vq.bjjhwx.cn

Ruby ........... 212
来源：http://ch.huixiangedu.cn

C# ............. 212
来源：http://xv.huixiangedu.cn

C .............. 30
来源：http://wz.gzmigu.cn

C++ ............ 30
来源：http://rx.jctech888.com.cn

SQL ............ 90
来源：http://qy.shtwfgs.cn

Bash ........... 80
来源：http://wt.szsharing.cn

Kotlin ......... 15
来源：http://gm.shxzskj.cn

Swift .......... 15
来源：http://rg.shxzukj.cn

Lua ............ 10
来源：http://tb.haigaiapp.cn

Perl ........... 10
来源：http://rg.hahajie.cn

Scala .......... 10
来源：http://ut.huixinmuqiang.cn

------------------------------------
来源：http://tu.hahajie.cn

合计 ........... 2106 条
来源：http://ji.huanxung.cn

按章节统计：
来源：http://mi.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yv.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kr.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dt.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yq.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://az.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yz.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ps.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ds.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gs.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ng.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jo.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ti.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jf.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jb.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jp.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tj.shxzskj.cn

Q SQL 专题                              90
来源：http://cd.hahajie.cn

R Bash 专题                             80
来源：http://fz.nszjky.cn

S C / C++ 专题                          60
来源：http://db.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://ej.nicolike.cn

U 高频实用片段                         120
来源：http://mm.jctech888.com.cn

------------------------------------
来源：http://pq.haigaiapp.cn

合计                                  2106 条
来源：http://ge.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://lw.colortex.cn

使用提醒
来源：http://hl.521024.cn

--------------------------------------------------------------------------------
来源：http://fp.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qd.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mi.hnjuh.cn


<!-- 参考信息 -->