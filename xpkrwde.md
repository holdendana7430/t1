代发 wailian999

[U07] Py：反转字典键值
来源：http://oy.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://su.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://cd.9csxet.cn

[y for x in nested for y in x]
来源：http://xk.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://oo.asd995.cn

max(d, key=d.get)
来源：http://tg.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://cb.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sr.gzmigu.cn

[U11] Py：生成器表达式
来源：http://bt.muxihuayi.cn

(x * 2 for x in arr)
来源：http://ip.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sw.gzmigu.cn

Counter(arr).most_common(3)
来源：http://ok.szxytkj.cn

[U13] Py：固定长度队列
来源：http://uh.colortex.cn

deque(maxlen=10)
来源：http://zy.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://pq.szsharing.cn

defaultdict(list)
来源：http://dy.panjiajie.cn

[U15] Py：高精度计时
来源：http://rk.bookmarksfly.cn

t = time.perf_counter()
来源：http://jd.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://rn.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sk.lnxyls.cn

[U17] Py：初始化日志
来源：http://ma.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://vq.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://rs.9csxet.cn

pat = re.compile(r"\d+")
来源：http://wo.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://uk.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ck.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://wr.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://qs.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://gx.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://ew.shxzskj.cn

[U22] Py：矩阵转置
来源：http://uh.muxihuayi.cn

list(zip(*m))
来源：http://pw.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://ph.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wt.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://tp.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ol.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://dj.asd995.cn

csv.DictReader(f)
来源：http://oj.hahajie.cn

[U26] Py：并发下载
来源：http://ak.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nw.9csxet.cn

[U27] Py：异步 HTTP
来源：http://vk.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://oe.shtwfgs.cn

[U28] Py：类型别名
来源：http://qw.shtwfgs.cn

UserId = int
来源：http://nz.nszjky.cn

[U29] Py：属性校验
来源：http://yd.shxzukj.cn

@property 与 @x.setter 配合
来源：http://vq.wgjwhj.cn

[U30] Py：数据类
来源：http://ml.huanxung.cn

@dataclass(slots=True)
来源：http://gw.huanxung.cn

[U31] Py：单测
来源：http://vv.asd995.cn

python -m pytest -q
来源：http://yu.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://qr.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ta.szsharing.cn

[U33] Py：打包发布
来源：http://vp.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://go.haigaiapp.cn

[U34] Py：判断编码
来源：http://ju.huanxung.cn

chardet.detect(raw)
来源：http://lz.nicolike.cn

[U35] Py：发送邮件
来源：http://xs.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ax.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://in.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://cs.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://wx.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zj.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://qx.lnxyls.cn

Path(__file__).resolve().parent
来源：http://ju.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://cc.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://ja.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://rl.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://xx.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://xs.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gm.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://np.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aq.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://rm.nicolike.cn

namespace App\Http;
来源：http://mh.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://lu.huixiangedu.cn

declare(strict_types=1);
来源：http://bi.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://ki.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://df.gzmigu.cn

[U46] PHP：可空类型
来源：http://ej.asd995.cn

?string $name = null
来源：http://tb.newstarts.cn

[U47] PHP：联合类型
来源：http://hk.newstarts.cn

int|string $id
来源：http://ju.newstarts.cn

[U48] PHP：纯枚举
来源：http://oi.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fi.huixiangedu.cn

[U49] PHP：只读属性
来源：http://oj.huixinmuqiang.cn

public readonly string $name
来源：http://gd.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://aa.szxytkj.cn

public function __construct(private int $id) {}
来源：http://fm.haigaiapp.cn

[U51] PHP：数组解构
来源：http://sk.9csxet.cn

[$a, $b] = $arr;
来源：http://vh.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://pi.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://do.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ue.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://tn.hahajie.cn

[U54] PHP：空安全调用
来源：http://zc.colortex.cn

$obj?->method()
来源：http://qt.shxzskj.cn

[U55] PHP：match 表达式
来源：http://sz.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mb.newstarts.cn

[U56] PHP：命名参数
来源：http://vt.hahajie.cn

f(a: 1, b: 2)
来源：http://eu.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://cz.lnxyls.cn

"值: {$a}"
来源：http://bu.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://mh.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aj.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://dz.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ti.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://cm.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vh.shxzukj.cn

[U61] PHP：正则
来源：http://zj.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fa.szxytkj.cn

[U62] PHP：日期对象
来源：http://ke.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ww.newstarts.cn

[U63] PHP：文件读写
来源：http://ao.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zs.asd995.cn

[U64] PHP：目录遍历
来源：http://ra.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://fv.521024.cn

[U65] PHP：会话
来源：http://ij.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hf.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://qn.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yd.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://ee.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wn.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://el.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ck.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://pj.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cy.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://ax.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://la.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://vi.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://jr.gzmigu.cn

[U72] PHP：写错误日志
来源：http://xy.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://wt.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://nf.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://vy.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://oc.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://xa.hnjuh.cn

[U75] PHP：依赖注入
来源：http://gm.bookmarksfly.cn

composer require psr/container
来源：http://xi.gzmigu.cn

[U76] PHP：简单路由
来源：http://qy.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ws.panjiajie.cn

[U77] PHP：模板渲染
来源：http://yl.wgjwhj.cn

composer require twig/twig
来源：http://dt.gzmigu.cn

[U78] PHP：单元测试
来源：http://kg.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://pi.lnxyls.cn

[U79] PHP：静态分析
来源：http://ln.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://iu.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://og.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ej.shtwfgs.cn

[U81] JS：初始化项目
来源：http://ui.hnjuh.cn

npm init -y;  npm i express
来源：http://hh.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://xa.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cn.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://mu.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://te.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://ga.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://el.newstarts.cn

[U85] JS：可选链
来源：http://sx.haigaiapp.cn

a?.b?.c
来源：http://zm.jctech888.com.cn

[U86] JS：空值合并
来源：http://rc.nszjky.cn

a ?? b
来源：http://sv.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://xm.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://fg.shxzukj.cn

[U88] JS：对象展开合并
来源：http://jx.colortex.cn

{ ...a, ...b }
来源：http://ye.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://yl.huixinmuqiang.cn

[...new Set(arr)]
来源：http://ds.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://bs.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://ce.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://lk.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cv.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://xz.lnxyls.cn

structuredClone(obj)
来源：http://su.jctech888.com.cn

[U93] JS：模板字符串
来源：http://ha.bookmarksfly.cn

`共 ${n} 条`
来源：http://gj.lnxyls.cn

[U94] JS：箭头函数
来源：http://ik.yuexingan06.cn

const double = x => x * 2;
来源：http://px.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://ka.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://eo.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://ct.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sw.bjjhwx.cn

[U97] JS：并发请求
来源：http://hr.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pb.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://ps.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bm.nicolike.cn

[U99] JS：事件监听
来源：http://mm.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://gn.panjiajie.cn

[U100] JS：DOM 查询
来源：http://mg.lnxyls.cn

document.querySelector(".item")
来源：http://gi.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://vv.gzmigu.cn

el.classList.toggle("active")
来源：http://jp.panjiajie.cn

[U102] JS：本地存储
来源：http://eu.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ml.huixiangedu.cn

[U103] JS：定时器
来源：http://al.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://an.yuntaijiaju.cn

[U104] JS：防抖
来源：http://ih.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sp.szsharing.cn

[U105] JS：节流
来源：http://wv.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ap.hnjuh.cn

[U106] JS：日期格式化
来源：http://ek.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yl.szxytkj.cn

[U107] JS：数字千分位
来源：http://nm.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hk.shtwfgs.cn

[U108] JS：随机整数
来源：http://mr.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ku.shxzukj.cn

[U109] JS：数组分组
来源：http://oc.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://tk.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://bl.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://in.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ad.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://pi.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://tx.newstarts.cn

"7".padStart(3, "0")
来源：http://mt.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://vy.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://zf.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://qo.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qy.lnxyls.cn

[U115] JS：生成 UUID
来源：http://it.asd995.cn

crypto.randomUUID()
来源：http://so.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://sa.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://ow.szsharing.cn

[U117] JS：单元测试
来源：http://eg.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ch.colortex.cn

[U118] JS：开发服务器
来源：http://ow.shxzukj.cn

npm i -D vite;  npx vite
来源：http://kb.szxytkj.cn

[U119] JS：生产构建
来源：http://ec.hnjuh.cn

npx vite build
来源：http://wi.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://zj.colortex.cn

import.meta.env.VITE_API_URL
来源：http://to.huixiangedu.cn

================================================================================
来源：http://mp.nszjky.cn

统计汇总
来源：http://cm.shtwfgs.cn

================================================================================
来源：http://um.szxytkj.cn

按语言统计（条）：
来源：http://op.hnjuh.cn

Python ......... 252
来源：http://ov.bjjhwx.cn

PHP ............ 252
来源：http://rz.gzmigu.cn

JavaScript ..... 252
来源：http://ti.asd995.cn

TypeScript ..... 212
来源：http://ko.colortex.cn

Java ........... 212
来源：http://db.shxzukj.cn

Go ............. 212
来源：http://vk.muxihuayi.cn

Ruby ........... 212
来源：http://zz.huixiangedu.cn

C# ............. 212
来源：http://rv.newstarts.cn

C .............. 30
来源：http://hu.panjiajie.cn

C++ ............ 30
来源：http://mm.yuntaijiaju.cn

SQL ............ 90
来源：http://qz.nicolike.cn

Bash ........... 80
来源：http://va.521024.cn

Kotlin ......... 15
来源：http://sx.asd995.cn

Swift .......... 15
来源：http://zv.shxzukj.cn

Lua ............ 10
来源：http://lf.szxytkj.cn

Perl ........... 10
来源：http://yv.jctech888.com.cn

Scala .......... 10
来源：http://xd.yuntaijiaju.cn

------------------------------------
来源：http://rx.huanxung.cn

合计 ........... 2106 条
来源：http://dj.gzmigu.cn

按章节统计：
来源：http://ix.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ip.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zy.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://en.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ou.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ba.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hn.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bn.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ot.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bb.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ie.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tf.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mc.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ao.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fo.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zw.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jy.nicolike.cn

Q SQL 专题                              90
来源：http://sv.colortex.cn

R Bash 专题                             80
来源：http://kd.asd995.cn

S C / C++ 专题                          60
来源：http://xx.hahajie.cn

T 其他语言补充                          60
来源：http://wg.szsharing.cn

U 高频实用片段                         120
来源：http://sm.hahajie.cn

------------------------------------
来源：http://xn.shxzskj.cn

合计                                  2106 条
来源：http://bg.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://fp.bjjhwx.cn

使用提醒
来源：http://gr.colortex.cn

--------------------------------------------------------------------------------
来源：http://ig.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qt.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bw.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xq.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qi.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ls.lnxyls.cn

—— 文件结束 ——
来源：http://fy.jianghongdianzi.cn

================================================================================
来源：http://kz.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://wv.nszjky.cn

Common Programming Examples Cheat Book
来源：http://xx.bookmarksfly.cn

================================================================================
来源：http://nw.yuntaijiaju.cn

【收录内容】
来源：http://nw.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jf.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ar.jctech888.com.cn

SQL · Bash · C · C++
来源：http://al.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gu.hahajie.cn

【使用说明】
来源：http://lp.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ux.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hm.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pw.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rl.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kr.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ig.muxihuayi.cn


<!-- 参考信息 -->