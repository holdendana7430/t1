代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dg.huanxung.cn

================================================================================
来源：http://wq.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://an.szsharing.cn

================================================================================
来源：http://pn.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://me.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dc.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://cz.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dg.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://ul.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://em.shxzukj.cn

[U04] Py：变量调试打印
来源：http://kz.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xu.colortex.cn

[U05] Py：列表去重且保序
来源：http://da.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://rn.szxytkj.cn

[U06] Py：合并两个字典
来源：http://wi.yuexingan06.cn

{**a, **b}
来源：http://wj.lnxyls.cn

[U07] Py：反转字典键值
来源：http://fv.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://rd.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://ql.bjjhwx.cn

[y for x in nested for y in x]
来源：http://hm.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://xk.szxytkj.cn

max(d, key=d.get)
来源：http://dr.panjiajie.cn

[U10] Py：按值排序字典
来源：http://nj.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uy.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://zs.nicolike.cn

(x * 2 for x in arr)
来源：http://wv.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://st.shxzskj.cn

Counter(arr).most_common(3)
来源：http://nt.colortex.cn

[U13] Py：固定长度队列
来源：http://jo.nicolike.cn

deque(maxlen=10)
来源：http://zs.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://io.hahajie.cn

defaultdict(list)
来源：http://ji.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://oc.wgjwhj.cn

t = time.perf_counter()
来源：http://ex.asd995.cn

[U16] Py：命令行参数解析
来源：http://nh.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://le.9csxet.cn

[U17] Py：初始化日志
来源：http://rz.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://ms.szxytkj.cn

[U18] Py：预编译正则
来源：http://ie.nszjky.cn

pat = re.compile(r"\d+")
来源：http://ra.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://jk.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wf.9csxet.cn

[U20] Py：缓存函数结果
来源：http://hn.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://bj.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://nc.haigaiapp.cn

@contextlib.contextmanager
来源：http://ht.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://uc.bookmarksfly.cn

list(zip(*m))
来源：http://fi.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://di.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ve.hnjuh.cn

[U24] Py：路径操作
来源：http://cb.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zb.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://bp.yuntaijiaju.cn

csv.DictReader(f)
来源：http://yx.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://dq.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rw.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://iu.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://wh.shxzukj.cn

[U28] Py：类型别名
来源：http://ox.shtwfgs.cn

UserId = int
来源：http://bz.nicolike.cn

[U29] Py：属性校验
来源：http://of.hahajie.cn

@property 与 @x.setter 配合
来源：http://dg.nszjky.cn

[U30] Py：数据类
来源：http://th.shtwfgs.cn

@dataclass(slots=True)
来源：http://dc.colortex.cn

[U31] Py：单测
来源：http://aa.panjiajie.cn

python -m pytest -q
来源：http://im.huanxung.cn

[U32] Py：代码格式化
来源：http://av.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://wl.521024.cn

[U33] Py：打包发布
来源：http://ab.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://jt.gzmigu.cn

[U34] Py：判断编码
来源：http://xm.bookmarksfly.cn

chardet.detect(raw)
来源：http://ts.nszjky.cn

[U35] Py：发送邮件
来源：http://ol.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cs.jctech888.com.cn

[U36] Py：定时任务
来源：http://ji.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://wt.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://qd.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tw.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://ma.hnjuh.cn

Path(__file__).resolve().parent
来源：http://gq.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ch.bjjhwx.cn

sys.stdout.isatty()
来源：http://lc.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://zc.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://pf.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://cp.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pc.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://zo.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ea.szsharing.cn

[U43] PHP：声明命名空间
来源：http://pv.hahajie.cn

namespace App\Http;
来源：http://td.newstarts.cn

[U44] PHP：开启严格类型
来源：http://hr.shtwfgs.cn

declare(strict_types=1);
来源：http://kb.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://fa.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ay.nszjky.cn

[U46] PHP：可空类型
来源：http://pl.jctech888.com.cn

?string $name = null
来源：http://cd.chemitech.net.cn

[U47] PHP：联合类型
来源：http://pl.huixinmuqiang.cn

int|string $id
来源：http://dx.lnxyls.cn

[U48] PHP：纯枚举
来源：http://br.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xa.newstarts.cn

[U49] PHP：只读属性
来源：http://fw.jianghongdianzi.cn

public readonly string $name
来源：http://ni.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://rw.nszjky.cn

public function __construct(private int $id) {}
来源：http://lf.nicolike.cn

[U51] PHP：数组解构
来源：http://sy.nicolike.cn

[$a, $b] = $arr;
来源：http://se.nicolike.cn

[U52] PHP：箭头函数
来源：http://er.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://at.colortex.cn

[U53] PHP：空合并运算符
来源：http://vi.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://mz.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://el.bookmarksfly.cn

$obj?->method()
来源：http://hd.panjiajie.cn

[U55] PHP：match 表达式
来源：http://ch.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uy.shxzukj.cn

[U56] PHP：命名参数
来源：http://ua.shxzskj.cn

f(a: 1, b: 2)
来源：http://ce.hnjuh.cn

[U57] PHP：字符串插值
来源：http://hc.chemitech.net.cn

"值: {$a}"
来源：http://mh.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://iw.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nk.gzmigu.cn

[U59] PHP：自定义排序
来源：http://il.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jr.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://bk.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://by.lnxyls.cn

[U61] PHP：正则
来源：http://mt.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mr.yuexingan06.cn

[U62] PHP：日期对象
来源：http://kq.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dg.521024.cn

[U63] PHP：文件读写
来源：http://rl.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pg.gzmigu.cn

[U64] PHP：目录遍历
来源：http://sk.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://zi.chemitech.net.cn

[U65] PHP：会话
来源：http://ph.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tf.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://tn.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xo.521024.cn

[U67] PHP：处理文件上传
来源：http://md.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vr.hahajie.cn

[U68] PHP：PDO 连接
来源：http://ol.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wu.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://bp.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lq.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://va.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://de.521024.cn

[U71] PHP：抛出异常
来源：http://oo.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://jy.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://hf.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://wi.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://ra.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://bh.nicolike.cn

[U74] PHP：读取环境变量
来源：http://wb.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://no.nszjky.cn

[U75] PHP：依赖注入
来源：http://sf.colortex.cn

composer require psr/container
来源：http://la.nszjky.cn

[U76] PHP：简单路由
来源：http://fi.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pu.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://rc.hahajie.cn

composer require twig/twig
来源：http://zg.gzmigu.cn

[U78] PHP：单元测试
来源：http://gz.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://sc.hahajie.cn

[U79] PHP：静态分析
来源：http://ku.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://kp.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://am.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ca.szxytkj.cn

[U81] JS：初始化项目
来源：http://ql.shxzskj.cn

npm init -y;  npm i express
来源：http://ah.521024.cn

[U82] JS：package.json 脚本
来源：http://cy.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vy.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://gt.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dr.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://po.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bf.shtwfgs.cn

[U85] JS：可选链
来源：http://hc.nszjky.cn

a?.b?.c
来源：http://yy.panjiajie.cn

[U86] JS：空值合并
来源：http://jy.haigaiapp.cn

a ?? b
来源：http://wg.chemitech.net.cn

[U87] JS：解构默认值
来源：http://xv.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://fo.huanxung.cn

[U88] JS：对象展开合并
来源：http://se.bookmarksfly.cn

{ ...a, ...b }
来源：http://sv.lnxyls.cn

[U89] JS：数组去重
来源：http://bq.muxihuayi.cn

[...new Set(arr)]
来源：http://fk.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://ui.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://dr.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://ft.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xs.shxzskj.cn

[U92] JS：深拷贝
来源：http://pl.chemitech.net.cn

structuredClone(obj)
来源：http://yn.chemitech.net.cn

[U93] JS：模板字符串
来源：http://rl.yuexingan06.cn

`共 ${n} 条`
来源：http://dq.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://pq.szsharing.cn

const double = x => x * 2;
来源：http://pd.szsharing.cn

[U95] JS：Promise 包装
来源：http://tu.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://nh.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://ti.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://em.wgjwhj.cn

[U97] JS：并发请求
来源：http://mq.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://du.521024.cn

[U98] JS：fetch 带 JSON
来源：http://bn.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ry.shxzskj.cn

[U99] JS：事件监听
来源：http://dr.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://qt.szsharing.cn

[U100] JS：DOM 查询
来源：http://kk.nszjky.cn

document.querySelector(".item")
来源：http://ps.lnxyls.cn

[U101] JS：classList 操作
来源：http://ur.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://dd.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://kb.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ui.panjiajie.cn

[U103] JS：定时器
来源：http://gl.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hj.muxihuayi.cn

[U104] JS：防抖
来源：http://ze.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.huanxung.cn

[U105] JS：节流
来源：http://fw.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hb.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://ao.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wo.nszjky.cn

[U107] JS：数字千分位
来源：http://ys.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xf.panjiajie.cn

[U108] JS：随机整数
来源：http://nv.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yo.lnxyls.cn

[U109] JS：数组分组
来源：http://hs.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://ow.jctech888.com.cn

[U110] JS：数组分块
来源：http://yb.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ad.newstarts.cn

[U111] JS：对象转 Map
来源：http://kw.gzmigu.cn

new Map(Object.entries(obj))
来源：http://eo.colortex.cn

[U112] JS：字符串补位
来源：http://tp.lnxyls.cn

"7".padStart(3, "0")
来源：http://xx.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://sq.gzmigu.cn

s.replaceAll("a", "b")
来源：http://yi.newstarts.cn

[U114] JS：JSON 深比较
来源：http://ak.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ff.9csxet.cn

[U115] JS：生成 UUID
来源：http://ab.szsharing.cn

crypto.randomUUID()
来源：http://qi.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://za.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://pr.shtwfgs.cn

[U117] JS：单元测试
来源：http://mx.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://tb.asd995.cn

[U118] JS：开发服务器
来源：http://rj.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://on.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://gt.shtwfgs.cn

npx vite build
来源：http://fl.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://nt.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://dj.jctech888.com.cn

================================================================================
来源：http://sj.shtwfgs.cn

统计汇总
来源：http://du.huixinmuqiang.cn

================================================================================
来源：http://jw.bjjhwx.cn

按语言统计（条）：
来源：http://df.asd995.cn

Python ......... 252
来源：http://zg.hnjuh.cn

PHP ............ 252
来源：http://gl.lnxyls.cn

JavaScript ..... 252
来源：http://wc.yuexingan06.cn

TypeScript ..... 212
来源：http://ur.jianghongdianzi.cn

Java ........... 212
来源：http://iu.szxytkj.cn

Go ............. 212
来源：http://nr.panjiajie.cn

Ruby ........... 212
来源：http://da.jianghongdianzi.cn

C# ............. 212
来源：http://jq.haigaiapp.cn

C .............. 30
来源：http://eh.bookmarksfly.cn

C++ ............ 30
来源：http://gf.shxzukj.cn

SQL ............ 90
来源：http://on.gzmigu.cn

Bash ........... 80
来源：http://uu.wgjwhj.cn

Kotlin ......... 15
来源：http://wp.newstarts.cn

Swift .......... 15
来源：http://np.nicolike.cn

Lua ............ 10
来源：http://re.hahajie.cn

Perl ........... 10
来源：http://hx.nszjky.cn

Scala .......... 10
来源：http://am.panjiajie.cn

------------------------------------
来源：http://nu.521024.cn

合计 ........... 2106 条
来源：http://hj.huixinmuqiang.cn

按章节统计：
来源：http://cu.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://di.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ao.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://te.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ql.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fr.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fj.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rr.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ld.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oe.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vg.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://by.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tr.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rl.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kp.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zv.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lb.chemitech.net.cn

Q SQL 专题                              90
来源：http://pr.bookmarksfly.cn

R Bash 专题                             80
来源：http://ua.yuexingan06.cn

S C / C++ 专题                          60
来源：http://dz.gzmigu.cn

T 其他语言补充                          60
来源：http://hz.shxzskj.cn

U 高频实用片段                         120
来源：http://oz.hnjuh.cn

------------------------------------
来源：http://ma.nicolike.cn

合计                                  2106 条
来源：http://rg.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://wx.szsharing.cn

使用提醒
来源：http://cf.newstarts.cn

--------------------------------------------------------------------------------
来源：http://tz.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ey.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mk.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pp.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dl.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://an.lnxyls.cn

—— 文件结束 ——
来源：http://oe.huixinmuqiang.cn


<!-- 参考信息 -->