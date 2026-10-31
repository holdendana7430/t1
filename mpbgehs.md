代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://pm.yuntaijiaju.cn

[T59] Scala：循环
来源：http://pf.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://vz.haigaiapp.cn

[T60] Scala：折叠
来源：http://hr.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fv.nszjky.cn

================================================================================
来源：http://ux.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kp.asd995.cn

================================================================================
来源：http://mf.521024.cn

[U01] Py：创建虚拟环境
来源：http://uv.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qy.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://tg.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vw.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://fh.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ai.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://tp.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dh.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://en.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ao.asd995.cn

[U06] Py：合并两个字典
来源：http://yp.szsharing.cn

{**a, **b}
来源：http://vv.hahajie.cn

[U07] Py：反转字典键值
来源：http://md.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://sa.huanxung.cn

[U08] Py：展平二维列表
来源：http://wb.panjiajie.cn

[y for x in nested for y in x]
来源：http://bv.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://pc.asd995.cn

max(d, key=d.get)
来源：http://wn.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://fx.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oy.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://gx.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://jr.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vt.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ot.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://iq.hnjuh.cn

deque(maxlen=10)
来源：http://vm.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://xq.jctech888.com.cn

defaultdict(list)
来源：http://uw.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://xi.szsharing.cn

t = time.perf_counter()
来源：http://yu.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://ww.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fe.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://fc.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://zk.lnxyls.cn

[U18] Py：预编译正则
来源：http://la.521024.cn

pat = re.compile(r"\d+")
来源：http://an.szsharing.cn

[U19] Py：正则替换带回调
来源：http://yq.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fc.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ab.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ev.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://ec.shtwfgs.cn

@contextlib.contextmanager
来源：http://zz.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://qb.nicolike.cn

list(zip(*m))
来源：http://wh.colortex.cn

[U23] Py：分块读取大文件
来源：http://hf.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://da.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://cs.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ki.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://pt.szxytkj.cn

csv.DictReader(f)
来源：http://hu.muxihuayi.cn

[U26] Py：并发下载
来源：http://it.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pw.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://rs.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://jt.huixiangedu.cn

[U28] Py：类型别名
来源：http://lw.wgjwhj.cn

UserId = int
来源：http://ng.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://kk.panjiajie.cn

@property 与 @x.setter 配合
来源：http://ks.jianghongdianzi.cn

[U30] Py：数据类
来源：http://qb.hnjuh.cn

@dataclass(slots=True)
来源：http://mu.huanxung.cn

[U31] Py：单测
来源：http://xq.panjiajie.cn

python -m pytest -q
来源：http://lx.9csxet.cn

[U32] Py：代码格式化
来源：http://fg.newstarts.cn

ruff format . && ruff check --fix .
来源：http://oe.szxytkj.cn

[U33] Py：打包发布
来源：http://sh.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://qa.wgjwhj.cn

[U34] Py：判断编码
来源：http://zp.szxytkj.cn

chardet.detect(raw)
来源：http://wz.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://oy.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vm.muxihuayi.cn

[U36] Py：定时任务
来源：http://ys.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://iu.nicolike.cn

[U37] Py：读写 Excel
来源：http://bg.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tg.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://iu.panjiajie.cn

Path(__file__).resolve().parent
来源：http://cj.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://dg.newstarts.cn

sys.stdout.isatty()
来源：http://vx.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://ka.panjiajie.cn

print("err", file=sys.stderr)
来源：http://gb.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://mn.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wb.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://rq.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://br.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://wq.newstarts.cn

namespace App\Http;
来源：http://dv.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://eh.szxytkj.cn

declare(strict_types=1);
来源：http://fb.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://ni.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ek.haigaiapp.cn

[U46] PHP：可空类型
来源：http://xy.yuntaijiaju.cn

?string $name = null
来源：http://dx.muxihuayi.cn

[U47] PHP：联合类型
来源：http://xf.szxytkj.cn

int|string $id
来源：http://mg.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://cr.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vj.shxzukj.cn

[U49] PHP：只读属性
来源：http://no.chemitech.net.cn

public readonly string $name
来源：http://we.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://tx.colortex.cn

public function __construct(private int $id) {}
来源：http://yb.9csxet.cn

[U51] PHP：数组解构
来源：http://nu.huanxung.cn

[$a, $b] = $arr;
来源：http://ek.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ac.colortex.cn

$double = fn($x) => $x * 2;
来源：http://tm.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://tz.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://qu.9csxet.cn

[U54] PHP：空安全调用
来源：http://aq.9csxet.cn

$obj?->method()
来源：http://br.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://jy.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pv.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://ov.huanxung.cn

f(a: 1, b: 2)
来源：http://bj.newstarts.cn

[U57] PHP：字符串插值
来源：http://oq.shxzskj.cn

"值: {$a}"
来源：http://ne.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://mz.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sn.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://nj.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ro.521024.cn

[U60] PHP：JSON 编解码
来源：http://xc.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ar.chemitech.net.cn

[U61] PHP：正则
来源：http://ae.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ir.panjiajie.cn

[U62] PHP：日期对象
来源：http://wj.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tr.szsharing.cn

[U63] PHP：文件读写
来源：http://ix.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pv.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://rq.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://gu.shxzukj.cn

[U65] PHP：会话
来源：http://jo.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hx.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://xd.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://in.huanxung.cn

[U67] PHP：处理文件上传
来源：http://uj.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cx.nicolike.cn

[U68] PHP：PDO 连接
来源：http://gj.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ye.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://vq.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cd.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://jr.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ob.521024.cn

[U71] PHP：抛出异常
来源：http://tj.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://xo.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://qr.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://eq.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://kd.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://kc.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://mo.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://rw.gzmigu.cn

[U75] PHP：依赖注入
来源：http://ug.nszjky.cn

composer require psr/container
来源：http://xk.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://xa.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://va.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://vm.muxihuayi.cn

composer require twig/twig
来源：http://br.wgjwhj.cn

[U78] PHP：单元测试
来源：http://bl.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://mc.nszjky.cn

[U79] PHP：静态分析
来源：http://bd.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://xc.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://pf.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://au.jctech888.com.cn

[U81] JS：初始化项目
来源：http://qb.bookmarksfly.cn

npm init -y;  npm i express
来源：http://oh.hahajie.cn

[U82] JS：package.json 脚本
来源：http://vp.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oh.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://tt.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ze.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://vy.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ay.muxihuayi.cn

[U85] JS：可选链
来源：http://pj.yuexingan06.cn

a?.b?.c
来源：http://ul.yuexingan06.cn

[U86] JS：空值合并
来源：http://qo.lnxyls.cn

a ?? b
来源：http://ol.hahajie.cn

[U87] JS：解构默认值
来源：http://ni.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://dz.hahajie.cn

[U88] JS：对象展开合并
来源：http://ml.jianghongdianzi.cn

{ ...a, ...b }
来源：http://tk.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://zv.huixiangedu.cn

[...new Set(arr)]
来源：http://io.newstarts.cn

[U90] JS：数字数组排序
来源：http://uh.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://sh.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://gu.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dp.muxihuayi.cn

[U92] JS：深拷贝
来源：http://jy.newstarts.cn

structuredClone(obj)
来源：http://te.panjiajie.cn

[U93] JS：模板字符串
来源：http://lg.muxihuayi.cn

`共 ${n} 条`
来源：http://sk.panjiajie.cn

[U94] JS：箭头函数
来源：http://zw.wgjwhj.cn

const double = x => x * 2;
来源：http://vv.asd995.cn

[U95] JS：Promise 包装
来源：http://vo.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://nb.colortex.cn

[U96] JS：async/await 与异常
来源：http://ww.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lk.asd995.cn

[U97] JS：并发请求
来源：http://ox.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://za.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://qb.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nq.chemitech.net.cn

[U99] JS：事件监听
来源：http://wc.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://zh.shxzukj.cn

[U100] JS：DOM 查询
来源：http://gh.hahajie.cn

document.querySelector(".item")
来源：http://xs.chemitech.net.cn

[U101] JS：classList 操作
来源：http://fj.huixiangedu.cn

el.classList.toggle("active")
来源：http://po.hahajie.cn

[U102] JS：本地存储
来源：http://vk.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://at.hahajie.cn

[U103] JS：定时器
来源：http://ru.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gm.bjjhwx.cn

[U104] JS：防抖
来源：http://my.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ur.nicolike.cn

[U105] JS：节流
来源：http://ah.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sf.jctech888.com.cn

[U106] JS：日期格式化
来源：http://gw.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kn.wgjwhj.cn

[U107] JS：数字千分位
来源：http://vg.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ex.chemitech.net.cn

[U108] JS：随机整数
来源：http://ys.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tk.panjiajie.cn

[U109] JS：数组分组
来源：http://jx.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://cl.szsharing.cn

[U110] JS：数组分块
来源：http://hb.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://co.9csxet.cn

[U111] JS：对象转 Map
来源：http://ex.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://mx.gzmigu.cn

[U112] JS：字符串补位
来源：http://pv.521024.cn

"7".padStart(3, "0")
来源：http://nl.lnxyls.cn

[U113] JS：正则替换全部
来源：http://if.hnjuh.cn

s.replaceAll("a", "b")
来源：http://yb.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://bp.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ch.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://hj.nicolike.cn

crypto.randomUUID()
来源：http://hs.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://bo.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://wo.lnxyls.cn

[U117] JS：单元测试
来源：http://kn.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://oz.hahajie.cn

[U118] JS：开发服务器
来源：http://mb.521024.cn

npm i -D vite;  npx vite
来源：http://wq.9csxet.cn

[U119] JS：生产构建
来源：http://nk.hnjuh.cn

npx vite build
来源：http://if.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://yc.521024.cn

import.meta.env.VITE_API_URL
来源：http://gd.huanxung.cn

================================================================================
来源：http://tc.huanxung.cn

统计汇总
来源：http://yv.yuntaijiaju.cn

================================================================================
来源：http://bj.bjjhwx.cn

按语言统计（条）：
来源：http://pj.szsharing.cn

Python ......... 252
来源：http://cb.szxytkj.cn

PHP ............ 252
来源：http://mq.jctech888.com.cn

JavaScript ..... 252
来源：http://fs.lnxyls.cn

TypeScript ..... 212
来源：http://za.shtwfgs.cn

Java ........... 212
来源：http://ig.huixiangedu.cn

Go ............. 212
来源：http://nv.colortex.cn

Ruby ........... 212
来源：http://ux.yuexingan06.cn

C# ............. 212
来源：http://vi.muxihuayi.cn

C .............. 30
来源：http://bd.szsharing.cn

C++ ............ 30
来源：http://gx.lnxyls.cn

SQL ............ 90
来源：http://nv.shxzskj.cn

Bash ........... 80
来源：http://os.hahajie.cn

Kotlin ......... 15
来源：http://iw.colortex.cn

Swift .......... 15
来源：http://qp.521024.cn

Lua ............ 10
来源：http://vk.bjjhwx.cn

Perl ........... 10
来源：http://mb.hahajie.cn

Scala .......... 10
来源：http://cg.shxzukj.cn

------------------------------------
来源：http://sg.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://et.newstarts.cn

按章节统计：
来源：http://rx.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oi.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wu.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qj.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nr.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ku.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gk.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ni.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ru.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wo.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bp.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bt.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kx.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mu.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xm.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qs.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zm.lnxyls.cn

Q SQL 专题                              90
来源：http://ux.bookmarksfly.cn

R Bash 专题                             80
来源：http://qs.asd995.cn

S C / C++ 专题                          60
来源：http://lw.huanxung.cn

T 其他语言补充                          60
来源：http://cw.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://ae.huixinmuqiang.cn

------------------------------------
来源：http://jy.gzmigu.cn

合计                                  2106 条
来源：http://nw.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kk.nszjky.cn

使用提醒
来源：http://kv.hahajie.cn

--------------------------------------------------------------------------------
来源：http://rd.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zs.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nd.shxzukj.cn


<!-- 参考信息 -->