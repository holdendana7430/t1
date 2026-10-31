代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yn.huixinmuqiang.cn

================================================================================
来源：http://nv.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ny.jianghongdianzi.cn

================================================================================
来源：http://yx.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://jb.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ea.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://ps.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oa.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://hh.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hj.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://ct.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qy.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://cu.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://sl.hnjuh.cn

[U06] Py：合并两个字典
来源：http://qt.haigaiapp.cn

{**a, **b}
来源：http://pj.colortex.cn

[U07] Py：反转字典键值
来源：http://sm.asd995.cn

{v: k for k, v in d.items()}
来源：http://mx.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://iw.panjiajie.cn

[y for x in nested for y in x]
来源：http://xk.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://cr.colortex.cn

max(d, key=d.get)
来源：http://kg.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://fb.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tm.lnxyls.cn

[U11] Py：生成器表达式
来源：http://nd.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://xt.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lc.asd995.cn

Counter(arr).most_common(3)
来源：http://lb.asd995.cn

[U13] Py：固定长度队列
来源：http://xt.newstarts.cn

deque(maxlen=10)
来源：http://sp.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://yy.asd995.cn

defaultdict(list)
来源：http://ls.nszjky.cn

[U15] Py：高精度计时
来源：http://sg.huixiangedu.cn

t = time.perf_counter()
来源：http://fk.newstarts.cn

[U16] Py：命令行参数解析
来源：http://cf.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://za.nicolike.cn

[U17] Py：初始化日志
来源：http://bd.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://dv.shxzukj.cn

[U18] Py：预编译正则
来源：http://wj.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://lk.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://dc.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bs.521024.cn

[U20] Py：缓存函数结果
来源：http://ji.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://ei.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://zb.nicolike.cn

@contextlib.contextmanager
来源：http://yj.colortex.cn

[U22] Py：矩阵转置
来源：http://ts.muxihuayi.cn

list(zip(*m))
来源：http://kl.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://pn.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zk.huixiangedu.cn

[U24] Py：路径操作
来源：http://vd.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rg.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://bh.shxzukj.cn

csv.DictReader(f)
来源：http://af.asd995.cn

[U26] Py：并发下载
来源：http://bg.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yi.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://mn.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://pl.shxzskj.cn

[U28] Py：类型别名
来源：http://qy.bjjhwx.cn

UserId = int
来源：http://pf.hahajie.cn

[U29] Py：属性校验
来源：http://uu.nszjky.cn

@property 与 @x.setter 配合
来源：http://rp.bookmarksfly.cn

[U30] Py：数据类
来源：http://gd.shxzskj.cn

@dataclass(slots=True)
来源：http://bv.huanxung.cn

[U31] Py：单测
来源：http://la.shxzskj.cn

python -m pytest -q
来源：http://vg.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://ve.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://ma.gzmigu.cn

[U33] Py：打包发布
来源：http://qv.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://pw.asd995.cn

[U34] Py：判断编码
来源：http://ab.shtwfgs.cn

chardet.detect(raw)
来源：http://ww.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://ue.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sj.lnxyls.cn

[U36] Py：定时任务
来源：http://vc.521024.cn

schedule.every(10).minutes.do(job)
来源：http://an.colortex.cn

[U37] Py：读写 Excel
来源：http://qj.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pd.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://ji.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://lk.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://yf.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://bh.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://bf.szxytkj.cn

print("err", file=sys.stderr)
来源：http://dd.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://xi.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ar.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://qk.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gr.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://em.muxihuayi.cn

namespace App\Http;
来源：http://yb.asd995.cn

[U44] PHP：开启严格类型
来源：http://pi.shxzskj.cn

declare(strict_types=1);
来源：http://fh.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://zx.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uk.wgjwhj.cn

[U46] PHP：可空类型
来源：http://xc.szsharing.cn

?string $name = null
来源：http://rl.gzmigu.cn

[U47] PHP：联合类型
来源：http://rt.nszjky.cn

int|string $id
来源：http://wo.szsharing.cn

[U48] PHP：纯枚举
来源：http://qc.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rq.chemitech.net.cn

[U49] PHP：只读属性
来源：http://rg.jctech888.com.cn

public readonly string $name
来源：http://ax.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://cf.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://hl.jctech888.com.cn

[U51] PHP：数组解构
来源：http://vp.lnxyls.cn

[$a, $b] = $arr;
来源：http://wv.9csxet.cn

[U52] PHP：箭头函数
来源：http://bp.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://bm.nszjky.cn

[U53] PHP：空合并运算符
来源：http://kz.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://nk.colortex.cn

[U54] PHP：空安全调用
来源：http://jm.bjjhwx.cn

$obj?->method()
来源：http://ba.colortex.cn

[U55] PHP：match 表达式
来源：http://zq.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zv.haigaiapp.cn

[U56] PHP：命名参数
来源：http://xo.9csxet.cn

f(a: 1, b: 2)
来源：http://qs.gzmigu.cn

[U57] PHP：字符串插值
来源：http://pf.huanxung.cn

"值: {$a}"
来源：http://ji.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://zm.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cg.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://qf.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ox.521024.cn

[U60] PHP：JSON 编解码
来源：http://yf.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pj.huanxung.cn

[U61] PHP：正则
来源：http://fa.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://on.bjjhwx.cn

[U62] PHP：日期对象
来源：http://wy.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ug.szxytkj.cn

[U63] PHP：文件读写
来源：http://mw.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hd.gzmigu.cn

[U64] PHP：目录遍历
来源：http://zp.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://oa.521024.cn

[U65] PHP：会话
来源：http://vd.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bf.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://bk.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fx.asd995.cn

[U67] PHP：处理文件上传
来源：http://wb.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ce.9csxet.cn

[U68] PHP：PDO 连接
来源：http://kw.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://la.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://fk.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qi.asd995.cn

[U70] PHP：PDO 事务
来源：http://qv.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lo.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://hz.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://gu.9csxet.cn

[U72] PHP：写错误日志
来源：http://fh.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://vk.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://pc.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://ta.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://kp.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://er.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://aj.panjiajie.cn

composer require psr/container
来源：http://ge.chemitech.net.cn

[U76] PHP：简单路由
来源：http://nc.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://va.panjiajie.cn

[U77] PHP：模板渲染
来源：http://rr.wgjwhj.cn

composer require twig/twig
来源：http://fy.shxzskj.cn

[U78] PHP：单元测试
来源：http://ok.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://mr.newstarts.cn

[U79] PHP：静态分析
来源：http://bn.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://me.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://du.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nd.muxihuayi.cn

[U81] JS：初始化项目
来源：http://hw.haigaiapp.cn

npm init -y;  npm i express
来源：http://zu.nicolike.cn

[U82] JS：package.json 脚本
来源：http://ps.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ca.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://nz.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sr.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://md.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lb.shxzskj.cn

[U85] JS：可选链
来源：http://vx.bjjhwx.cn

a?.b?.c
来源：http://mm.jctech888.com.cn

[U86] JS：空值合并
来源：http://xs.colortex.cn

a ?? b
来源：http://ep.jctech888.com.cn

[U87] JS：解构默认值
来源：http://vw.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://on.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://gp.jctech888.com.cn

{ ...a, ...b }
来源：http://sn.newstarts.cn

[U89] JS：数组去重
来源：http://lx.szxytkj.cn

[...new Set(arr)]
来源：http://nx.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://tq.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://go.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://ej.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gd.szxytkj.cn

[U92] JS：深拷贝
来源：http://ow.hahajie.cn

structuredClone(obj)
来源：http://nt.shtwfgs.cn

[U93] JS：模板字符串
来源：http://tk.szsharing.cn

`共 ${n} 条`
来源：http://gs.shxzukj.cn

[U94] JS：箭头函数
来源：http://dw.newstarts.cn

const double = x => x * 2;
来源：http://hb.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://fh.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://dv.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://qt.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kr.shxzukj.cn

[U97] JS：并发请求
来源：http://no.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hf.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://tn.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ve.chemitech.net.cn

[U99] JS：事件监听
来源：http://vh.colortex.cn

el.addEventListener("click", e => {})
来源：http://ff.panjiajie.cn

[U100] JS：DOM 查询
来源：http://be.asd995.cn

document.querySelector(".item")
来源：http://mr.colortex.cn

[U101] JS：classList 操作
来源：http://nd.szsharing.cn

el.classList.toggle("active")
来源：http://kg.521024.cn

[U102] JS：本地存储
来源：http://ym.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://br.wgjwhj.cn

[U103] JS：定时器
来源：http://na.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xg.newstarts.cn

[U104] JS：防抖
来源：http://cl.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lf.huixinmuqiang.cn

[U105] JS：节流
来源：http://hf.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mn.szxytkj.cn

[U106] JS：日期格式化
来源：http://fn.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vh.muxihuayi.cn

[U107] JS：数字千分位
来源：http://gu.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gj.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://bi.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wo.hahajie.cn

[U109] JS：数组分组
来源：http://gd.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://df.jctech888.com.cn

[U110] JS：数组分块
来源：http://bn.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kz.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ua.panjiajie.cn

new Map(Object.entries(obj))
来源：http://zk.shxzskj.cn

[U112] JS：字符串补位
来源：http://he.asd995.cn

"7".padStart(3, "0")
来源：http://va.gzmigu.cn

[U113] JS：正则替换全部
来源：http://yz.panjiajie.cn

s.replaceAll("a", "b")
来源：http://kf.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://ql.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://am.lnxyls.cn

[U115] JS：生成 UUID
来源：http://wg.nicolike.cn

crypto.randomUUID()
来源：http://xc.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://sr.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://ci.haigaiapp.cn

[U117] JS：单元测试
来源：http://hq.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ij.panjiajie.cn

[U118] JS：开发服务器
来源：http://zk.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://en.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://zx.huixiangedu.cn

npx vite build
来源：http://hd.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://ra.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://es.chemitech.net.cn

================================================================================
来源：http://qp.9csxet.cn

统计汇总
来源：http://vb.nszjky.cn

================================================================================
来源：http://kp.hnjuh.cn

按语言统计（条）：
来源：http://rd.521024.cn

Python ......... 252
来源：http://rf.huixiangedu.cn

PHP ............ 252
来源：http://lq.szxytkj.cn

JavaScript ..... 252
来源：http://ys.muxihuayi.cn

TypeScript ..... 212
来源：http://yz.chemitech.net.cn

Java ........... 212
来源：http://ku.shxzskj.cn

Go ............. 212
来源：http://gc.nszjky.cn

Ruby ........... 212
来源：http://kx.panjiajie.cn

C# ............. 212
来源：http://yb.nszjky.cn

C .............. 30
来源：http://xc.bjjhwx.cn

C++ ............ 30
来源：http://mo.shtwfgs.cn

SQL ............ 90
来源：http://ge.huixiangedu.cn

Bash ........... 80
来源：http://ti.wgjwhj.cn

Kotlin ......... 15
来源：http://iu.newstarts.cn

Swift .......... 15
来源：http://ve.muxihuayi.cn

Lua ............ 10
来源：http://ac.colortex.cn

Perl ........... 10
来源：http://yj.newstarts.cn

Scala .......... 10
来源：http://nx.gzmigu.cn

------------------------------------
来源：http://rt.shxzukj.cn

合计 ........... 2106 条
来源：http://vc.yuntaijiaju.cn

按章节统计：
来源：http://iq.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ya.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ze.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rx.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tv.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wj.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pk.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oy.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ga.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qd.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dj.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sp.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lt.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://he.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wa.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yu.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lb.chemitech.net.cn

Q SQL 专题                              90
来源：http://fj.nszjky.cn

R Bash 专题                             80
来源：http://vo.9csxet.cn

S C / C++ 专题                          60
来源：http://mv.huanxung.cn

T 其他语言补充                          60
来源：http://dg.hahajie.cn

U 高频实用片段                         120
来源：http://zo.jianghongdianzi.cn

------------------------------------
来源：http://hm.szsharing.cn

合计                                  2106 条
来源：http://hh.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://mm.bjjhwx.cn

使用提醒
来源：http://er.huanxung.cn

--------------------------------------------------------------------------------
来源：http://rl.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sp.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vt.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fa.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://av.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vx.gzmigu.cn

—— 文件结束 ——
来源：http://fd.szsharing.cn


<!-- 参考信息 -->