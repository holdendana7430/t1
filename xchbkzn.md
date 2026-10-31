代发 wailian999

[U03] Py：加载 .env 配置
来源：http://af.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hs.asd995.cn

[U04] Py：变量调试打印
来源：http://ad.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://co.9csxet.cn

[U05] Py：列表去重且保序
来源：http://ui.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://kv.asd995.cn

[U06] Py：合并两个字典
来源：http://ob.9csxet.cn

{**a, **b}
来源：http://mu.szsharing.cn

[U07] Py：反转字典键值
来源：http://he.9csxet.cn

{v: k for k, v in d.items()}
来源：http://uy.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://eq.szxytkj.cn

[y for x in nested for y in x]
来源：http://ta.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://pf.shtwfgs.cn

max(d, key=d.get)
来源：http://ld.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://mp.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ba.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://fi.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://jx.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ts.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://lf.hahajie.cn

[U13] Py：固定长度队列
来源：http://yg.9csxet.cn

deque(maxlen=10)
来源：http://hb.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://yd.shtwfgs.cn

defaultdict(list)
来源：http://ep.shtwfgs.cn

[U15] Py：高精度计时
来源：http://mm.9csxet.cn

t = time.perf_counter()
来源：http://uv.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://ii.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ev.shxzukj.cn

[U17] Py：初始化日志
来源：http://zp.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://xl.521024.cn

[U18] Py：预编译正则
来源：http://sm.nszjky.cn

pat = re.compile(r"\d+")
来源：http://zj.nszjky.cn

[U19] Py：正则替换带回调
来源：http://hk.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qf.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://dl.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://jk.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://sz.nicolike.cn

@contextlib.contextmanager
来源：http://rn.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://qg.muxihuayi.cn

list(zip(*m))
来源：http://ur.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://lx.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ay.nicolike.cn

[U24] Py：路径操作
来源：http://pp.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vf.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://hm.bjjhwx.cn

csv.DictReader(f)
来源：http://yq.bookmarksfly.cn

[U26] Py：并发下载
来源：http://iq.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rj.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://ts.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://je.yuexingan06.cn

[U28] Py：类型别名
来源：http://kd.gzmigu.cn

UserId = int
来源：http://mi.newstarts.cn

[U29] Py：属性校验
来源：http://rr.gzmigu.cn

@property 与 @x.setter 配合
来源：http://fx.huixiangedu.cn

[U30] Py：数据类
来源：http://ix.lnxyls.cn

@dataclass(slots=True)
来源：http://sa.bookmarksfly.cn

[U31] Py：单测
来源：http://rf.szsharing.cn

python -m pytest -q
来源：http://ae.panjiajie.cn

[U32] Py：代码格式化
来源：http://pr.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://lu.lnxyls.cn

[U33] Py：打包发布
来源：http://rh.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://kw.hnjuh.cn

[U34] Py：判断编码
来源：http://qy.shxzukj.cn

chardet.detect(raw)
来源：http://vr.hnjuh.cn

[U35] Py：发送邮件
来源：http://op.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lf.colortex.cn

[U36] Py：定时任务
来源：http://kd.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://wm.lnxyls.cn

[U37] Py：读写 Excel
来源：http://io.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dy.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://gh.shxzskj.cn

Path(__file__).resolve().parent
来源：http://pk.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://tg.bookmarksfly.cn

sys.stdout.isatty()
来源：http://uw.521024.cn

[U40] Py：打印到标准错误
来源：http://bl.shxzukj.cn

print("err", file=sys.stderr)
来源：http://eh.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://jq.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vb.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://yk.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ne.huanxung.cn

[U43] PHP：声明命名空间
来源：http://nl.jianghongdianzi.cn

namespace App\Http;
来源：http://eb.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://cg.huixinmuqiang.cn

declare(strict_types=1);
来源：http://qk.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://db.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://au.gzmigu.cn

[U46] PHP：可空类型
来源：http://uq.asd995.cn

?string $name = null
来源：http://bf.9csxet.cn

[U47] PHP：联合类型
来源：http://gf.gzmigu.cn

int|string $id
来源：http://uj.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://zo.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oo.shxzskj.cn

[U49] PHP：只读属性
来源：http://sr.jctech888.com.cn

public readonly string $name
来源：http://tk.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://qm.szsharing.cn

public function __construct(private int $id) {}
来源：http://ea.521024.cn

[U51] PHP：数组解构
来源：http://cw.colortex.cn

[$a, $b] = $arr;
来源：http://ud.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://xg.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://it.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://su.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://rd.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://mq.jianghongdianzi.cn

$obj?->method()
来源：http://sy.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://em.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://so.panjiajie.cn

[U56] PHP：命名参数
来源：http://fy.huixiangedu.cn

f(a: 1, b: 2)
来源：http://wy.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ka.yuntaijiaju.cn

"值: {$a}"
来源：http://kz.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ha.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ta.shxzskj.cn

[U59] PHP：自定义排序
来源：http://mb.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ri.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://iw.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wz.szsharing.cn

[U61] PHP：正则
来源：http://xj.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hg.szsharing.cn

[U62] PHP：日期对象
来源：http://kp.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ft.shxzukj.cn

[U63] PHP：文件读写
来源：http://do.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lw.szxytkj.cn

[U64] PHP：目录遍历
来源：http://mr.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://ir.huixiangedu.cn

[U65] PHP：会话
来源：http://qf.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uv.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://ep.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wd.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://gh.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://as.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://oj.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mp.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://ea.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zb.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://vd.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hp.lnxyls.cn

[U71] PHP：抛出异常
来源：http://kp.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://ca.nszjky.cn

[U72] PHP：写错误日志
来源：http://ax.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://lr.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://vp.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://tz.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://mx.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://iv.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://vb.nszjky.cn

composer require psr/container
来源：http://jy.lnxyls.cn

[U76] PHP：简单路由
来源：http://ot.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ju.9csxet.cn

[U77] PHP：模板渲染
来源：http://od.huixiangedu.cn

composer require twig/twig
来源：http://hi.colortex.cn

[U78] PHP：单元测试
来源：http://vv.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://ty.shtwfgs.cn

[U79] PHP：静态分析
来源：http://iq.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://sk.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://fv.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rx.521024.cn

[U81] JS：初始化项目
来源：http://ha.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://sk.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://qt.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ie.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://nu.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ii.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://aw.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vp.huanxung.cn

[U85] JS：可选链
来源：http://en.huixinmuqiang.cn

a?.b?.c
来源：http://dr.hahajie.cn

[U86] JS：空值合并
来源：http://sk.hnjuh.cn

a ?? b
来源：http://pn.newstarts.cn

[U87] JS：解构默认值
来源：http://ti.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://fs.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://cl.nszjky.cn

{ ...a, ...b }
来源：http://fr.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://rj.panjiajie.cn

[...new Set(arr)]
来源：http://gr.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ir.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://bm.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://va.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mn.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://di.panjiajie.cn

structuredClone(obj)
来源：http://qv.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://je.shxzukj.cn

`共 ${n} 条`
来源：http://ae.huanxung.cn

[U94] JS：箭头函数
来源：http://vy.yuexingan06.cn

const double = x => x * 2;
来源：http://ct.hnjuh.cn

[U95] JS：Promise 包装
来源：http://qt.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://cd.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://qp.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yv.asd995.cn

[U97] JS：并发请求
来源：http://oy.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vq.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://mh.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xj.lnxyls.cn

[U99] JS：事件监听
来源：http://hu.nicolike.cn

el.addEventListener("click", e => {})
来源：http://er.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://kp.muxihuayi.cn

document.querySelector(".item")
来源：http://nm.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://lw.shxzukj.cn

el.classList.toggle("active")
来源：http://dt.hahajie.cn

[U102] JS：本地存储
来源：http://il.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ac.shxzukj.cn

[U103] JS：定时器
来源：http://xl.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lu.gzmigu.cn

[U104] JS：防抖
来源：http://qk.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://et.wgjwhj.cn

[U105] JS：节流
来源：http://ds.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hl.hahajie.cn

[U106] JS：日期格式化
来源：http://wt.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://os.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://st.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gf.nszjky.cn

[U108] JS：随机整数
来源：http://fx.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uv.gzmigu.cn

[U109] JS：数组分组
来源：http://bz.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://ze.gzmigu.cn

[U110] JS：数组分块
来源：http://gv.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sw.szxytkj.cn

[U111] JS：对象转 Map
来源：http://cy.shxzukj.cn

new Map(Object.entries(obj))
来源：http://gk.szsharing.cn

[U112] JS：字符串补位
来源：http://ln.hahajie.cn

"7".padStart(3, "0")
来源：http://ld.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://ka.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://rw.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://ry.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hr.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ap.yuexingan06.cn

crypto.randomUUID()
来源：http://dj.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://mk.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://kz.hnjuh.cn

[U117] JS：单元测试
来源：http://pz.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://cq.shxzskj.cn

[U118] JS：开发服务器
来源：http://rd.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://lq.nszjky.cn

[U119] JS：生产构建
来源：http://jr.huixinmuqiang.cn

npx vite build
来源：http://vw.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://sk.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://ob.9csxet.cn

================================================================================
来源：http://te.shxzukj.cn

统计汇总
来源：http://ss.hnjuh.cn

================================================================================
来源：http://sn.hahajie.cn

按语言统计（条）：
来源：http://sh.bookmarksfly.cn

Python ......... 252
来源：http://go.huanxung.cn

PHP ............ 252
来源：http://ua.chemitech.net.cn

JavaScript ..... 252
来源：http://pk.shxzukj.cn

TypeScript ..... 212
来源：http://vt.nicolike.cn

Java ........... 212
来源：http://tl.shtwfgs.cn

Go ............. 212
来源：http://jm.panjiajie.cn

Ruby ........... 212
来源：http://vw.szsharing.cn

C# ............. 212
来源：http://wq.jianghongdianzi.cn

C .............. 30
来源：http://vu.shtwfgs.cn

C++ ............ 30
来源：http://hy.huanxung.cn

SQL ............ 90
来源：http://do.newstarts.cn

Bash ........... 80
来源：http://md.shxzskj.cn

Kotlin ......... 15
来源：http://mb.lnxyls.cn

Swift .......... 15
来源：http://rl.shtwfgs.cn

Lua ............ 10
来源：http://lf.muxihuayi.cn

Perl ........... 10
来源：http://yy.newstarts.cn

Scala .......... 10
来源：http://mk.huixinmuqiang.cn

------------------------------------
来源：http://ee.9csxet.cn

合计 ........... 2106 条
来源：http://lu.haigaiapp.cn

按章节统计：
来源：http://qe.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wo.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hc.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://le.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ur.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dc.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jw.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sd.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rg.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pd.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ea.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dy.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uq.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hb.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dz.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ds.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xk.hnjuh.cn

Q SQL 专题                              90
来源：http://yx.jianghongdianzi.cn

R Bash 专题                             80
来源：http://lx.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://vy.9csxet.cn

T 其他语言补充                          60
来源：http://ng.lnxyls.cn

U 高频实用片段                         120
来源：http://jj.lnxyls.cn

------------------------------------
来源：http://hm.jianghongdianzi.cn

合计                                  2106 条
来源：http://rk.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://va.bookmarksfly.cn

使用提醒
来源：http://mh.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://va.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://om.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ga.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ih.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gq.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tc.szxytkj.cn

—— 文件结束 ——
来源：http://vi.nszjky.cn

================================================================================
来源：http://kg.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://gy.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://ax.szxytkj.cn

================================================================================
来源：http://hf.bjjhwx.cn

【收录内容】
来源：http://qk.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://va.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jc.panjiajie.cn

SQL · Bash · C · C++
来源：http://xq.huanxung.cn


<!-- 参考信息 -->