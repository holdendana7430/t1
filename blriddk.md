代发 wailian999

[U05] Py：列表去重且保序
来源：http://xi.colortex.cn

list(dict.fromkeys(arr))
来源：http://if.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://az.nicolike.cn

{**a, **b}
来源：http://kg.nicolike.cn

[U07] Py：反转字典键值
来源：http://fd.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://uy.gzmigu.cn

[U08] Py：展平二维列表
来源：http://wq.shxzskj.cn

[y for x in nested for y in x]
来源：http://lg.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://cj.shxzukj.cn

max(d, key=d.get)
来源：http://pv.asd995.cn

[U10] Py：按值排序字典
来源：http://oq.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yu.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ao.asd995.cn

(x * 2 for x in arr)
来源：http://fi.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hd.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://gg.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://kc.nicolike.cn

deque(maxlen=10)
来源：http://bu.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ds.huanxung.cn

defaultdict(list)
来源：http://br.szxytkj.cn

[U15] Py：高精度计时
来源：http://pv.szxytkj.cn

t = time.perf_counter()
来源：http://vp.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ho.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://he.shxzukj.cn

[U17] Py：初始化日志
来源：http://sd.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://bd.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://so.9csxet.cn

pat = re.compile(r"\d+")
来源：http://fz.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://wk.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eu.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://sy.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://vk.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://mm.hnjuh.cn

@contextlib.contextmanager
来源：http://ls.nicolike.cn

[U22] Py：矩阵转置
来源：http://ym.shxzukj.cn

list(zip(*m))
来源：http://dp.huanxung.cn

[U23] Py：分块读取大文件
来源：http://qw.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://da.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://ja.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zi.colortex.cn

[U25] Py：CSV 按字典读
来源：http://ch.asd995.cn

csv.DictReader(f)
来源：http://au.newstarts.cn

[U26] Py：并发下载
来源：http://uz.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jg.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://tm.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://px.521024.cn

[U28] Py：类型别名
来源：http://oz.yuntaijiaju.cn

UserId = int
来源：http://gn.bjjhwx.cn

[U29] Py：属性校验
来源：http://ke.huanxung.cn

@property 与 @x.setter 配合
来源：http://ux.szsharing.cn

[U30] Py：数据类
来源：http://xw.asd995.cn

@dataclass(slots=True)
来源：http://ax.chemitech.net.cn

[U31] Py：单测
来源：http://hs.shxzskj.cn

python -m pytest -q
来源：http://iy.chemitech.net.cn

[U32] Py：代码格式化
来源：http://ij.nicolike.cn

ruff format . && ruff check --fix .
来源：http://yr.haigaiapp.cn

[U33] Py：打包发布
来源：http://rx.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://kw.bookmarksfly.cn

[U34] Py：判断编码
来源：http://ap.chemitech.net.cn

chardet.detect(raw)
来源：http://qq.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://hg.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dl.shxzskj.cn

[U36] Py：定时任务
来源：http://gw.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://lz.shxzskj.cn

[U37] Py：读写 Excel
来源：http://yj.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gn.521024.cn

[U38] Py：获取脚本所在目录
来源：http://du.colortex.cn

Path(__file__).resolve().parent
来源：http://lb.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://ui.chemitech.net.cn

sys.stdout.isatty()
来源：http://vy.newstarts.cn

[U40] Py：打印到标准错误
来源：http://uq.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://ft.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rw.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://um.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://sk.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ba.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ey.panjiajie.cn

namespace App\Http;
来源：http://ni.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://og.colortex.cn

declare(strict_types=1);
来源：http://pp.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ab.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bs.muxihuayi.cn

[U46] PHP：可空类型
来源：http://qh.bjjhwx.cn

?string $name = null
来源：http://ox.muxihuayi.cn

[U47] PHP：联合类型
来源：http://jl.hnjuh.cn

int|string $id
来源：http://nz.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://zi.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bb.9csxet.cn

[U49] PHP：只读属性
来源：http://gh.hnjuh.cn

public readonly string $name
来源：http://cd.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://dw.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://az.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://qa.9csxet.cn

[$a, $b] = $arr;
来源：http://ut.hnjuh.cn

[U52] PHP：箭头函数
来源：http://sz.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://zf.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://jt.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ib.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://hu.chemitech.net.cn

$obj?->method()
来源：http://ag.nicolike.cn

[U55] PHP：match 表达式
来源：http://qo.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qc.shxzukj.cn

[U56] PHP：命名参数
来源：http://kw.lnxyls.cn

f(a: 1, b: 2)
来源：http://kb.nszjky.cn

[U57] PHP：字符串插值
来源：http://oa.wgjwhj.cn

"值: {$a}"
来源：http://bj.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://kp.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://um.521024.cn

[U59] PHP：自定义排序
来源：http://qr.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ow.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://au.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kf.newstarts.cn

[U61] PHP：正则
来源：http://vb.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ev.szxytkj.cn

[U62] PHP：日期对象
来源：http://om.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yu.shxzukj.cn

[U63] PHP：文件读写
来源：http://us.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tp.lnxyls.cn

[U64] PHP：目录遍历
来源：http://yf.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://ue.hahajie.cn

[U65] PHP：会话
来源：http://fv.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://to.colortex.cn

[U66] PHP：设置 Cookie
来源：http://pc.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jv.nicolike.cn

[U67] PHP：处理文件上传
来源：http://ku.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uk.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://pa.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nc.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://zk.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bv.521024.cn

[U70] PHP：PDO 事务
来源：http://do.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ic.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://ze.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://hh.521024.cn

[U72] PHP：写错误日志
来源：http://ff.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://cf.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://xs.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://rx.hahajie.cn

[U74] PHP：读取环境变量
来源：http://tv.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://nk.hahajie.cn

[U75] PHP：依赖注入
来源：http://hr.shxzukj.cn

composer require psr/container
来源：http://en.szsharing.cn

[U76] PHP：简单路由
来源：http://va.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ec.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://xx.hnjuh.cn

composer require twig/twig
来源：http://gp.yuexingan06.cn

[U78] PHP：单元测试
来源：http://xy.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://rx.asd995.cn

[U79] PHP：静态分析
来源：http://ro.asd995.cn

composer require --dev phpstan/phpstan
来源：http://we.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://eh.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cu.hahajie.cn

[U81] JS：初始化项目
来源：http://gq.shxzskj.cn

npm init -y;  npm i express
来源：http://db.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://hm.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fw.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://wh.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lr.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://vc.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pl.huanxung.cn

[U85] JS：可选链
来源：http://rz.hnjuh.cn

a?.b?.c
来源：http://cx.haigaiapp.cn

[U86] JS：空值合并
来源：http://fy.hahajie.cn

a ?? b
来源：http://uf.szxytkj.cn

[U87] JS：解构默认值
来源：http://as.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://ig.9csxet.cn

[U88] JS：对象展开合并
来源：http://tz.bookmarksfly.cn

{ ...a, ...b }
来源：http://zu.nszjky.cn

[U89] JS：数组去重
来源：http://eg.9csxet.cn

[...new Set(arr)]
来源：http://er.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://lj.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://pi.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://gl.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nl.chemitech.net.cn

[U92] JS：深拷贝
来源：http://cl.jctech888.com.cn

structuredClone(obj)
来源：http://cr.szsharing.cn

[U93] JS：模板字符串
来源：http://pt.521024.cn

`共 ${n} 条`
来源：http://vf.gzmigu.cn

[U94] JS：箭头函数
来源：http://xz.panjiajie.cn

const double = x => x * 2;
来源：http://vw.nicolike.cn

[U95] JS：Promise 包装
来源：http://qz.521024.cn

new Promise((resolve, reject) => {})
来源：http://gd.asd995.cn

[U96] JS：async/await 与异常
来源：http://li.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sa.szsharing.cn

[U97] JS：并发请求
来源：http://vp.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bi.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://bz.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://go.shxzskj.cn

[U99] JS：事件监听
来源：http://om.9csxet.cn

el.addEventListener("click", e => {})
来源：http://jh.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://iy.jctech888.com.cn

document.querySelector(".item")
来源：http://bq.shxzukj.cn

[U101] JS：classList 操作
来源：http://kx.bookmarksfly.cn

el.classList.toggle("active")
来源：http://fm.szsharing.cn

[U102] JS：本地存储
来源：http://up.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://en.jianghongdianzi.cn

[U103] JS：定时器
来源：http://vb.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yq.huixinmuqiang.cn

[U104] JS：防抖
来源：http://ku.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cv.panjiajie.cn

[U105] JS：节流
来源：http://pv.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jw.9csxet.cn

[U106] JS：日期格式化
来源：http://jz.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ib.lnxyls.cn

[U107] JS：数字千分位
来源：http://vu.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://za.yuexingan06.cn

[U108] JS：随机整数
来源：http://nk.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zm.haigaiapp.cn

[U109] JS：数组分组
来源：http://ng.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://ut.521024.cn

[U110] JS：数组分块
来源：http://hd.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ud.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://ik.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://he.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://yv.shxzukj.cn

"7".padStart(3, "0")
来源：http://zd.nszjky.cn

[U113] JS：正则替换全部
来源：http://tl.hahajie.cn

s.replaceAll("a", "b")
来源：http://jh.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://ht.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bi.lnxyls.cn

[U115] JS：生成 UUID
来源：http://uj.chemitech.net.cn

crypto.randomUUID()
来源：http://pd.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://jy.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://jh.szsharing.cn

[U117] JS：单元测试
来源：http://qe.521024.cn

npm i -D vitest;  npx vitest
来源：http://tq.shtwfgs.cn

[U118] JS：开发服务器
来源：http://um.nszjky.cn

npm i -D vite;  npx vite
来源：http://rf.521024.cn

[U119] JS：生产构建
来源：http://fa.huixiangedu.cn

npx vite build
来源：http://hi.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://pe.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://we.shxzskj.cn

================================================================================
来源：http://xj.shxzskj.cn

统计汇总
来源：http://cm.huanxung.cn

================================================================================
来源：http://hg.hahajie.cn

按语言统计（条）：
来源：http://rw.shxzskj.cn

Python ......... 252
来源：http://kd.bjjhwx.cn

PHP ............ 252
来源：http://dh.wgjwhj.cn

JavaScript ..... 252
来源：http://xf.jianghongdianzi.cn

TypeScript ..... 212
来源：http://yo.shxzskj.cn

Java ........... 212
来源：http://hd.shtwfgs.cn

Go ............. 212
来源：http://bm.hnjuh.cn

Ruby ........... 212
来源：http://th.jianghongdianzi.cn

C# ............. 212
来源：http://es.wgjwhj.cn

C .............. 30
来源：http://nk.shxzskj.cn

C++ ............ 30
来源：http://wu.shtwfgs.cn

SQL ............ 90
来源：http://vp.huixiangedu.cn

Bash ........... 80
来源：http://yo.chemitech.net.cn

Kotlin ......... 15
来源：http://hx.hahajie.cn

Swift .......... 15
来源：http://yu.bjjhwx.cn

Lua ............ 10
来源：http://tu.jctech888.com.cn

Perl ........... 10
来源：http://pi.bookmarksfly.cn

Scala .......... 10
来源：http://lv.wgjwhj.cn

------------------------------------
来源：http://cr.jctech888.com.cn

合计 ........... 2106 条
来源：http://or.huanxung.cn

按章节统计：
来源：http://xq.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fb.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://il.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tu.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fm.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iv.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vl.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yu.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nr.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oo.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://et.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yd.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tf.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jm.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mc.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ot.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cl.colortex.cn

Q SQL 专题                              90
来源：http://ko.wgjwhj.cn

R Bash 专题                             80
来源：http://ug.huixiangedu.cn

S C / C++ 专题                          60
来源：http://iy.muxihuayi.cn

T 其他语言补充                          60
来源：http://lr.shxzskj.cn

U 高频实用片段                         120
来源：http://nc.chemitech.net.cn

------------------------------------
来源：http://dx.hnjuh.cn

合计                                  2106 条
来源：http://ve.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://fj.panjiajie.cn

使用提醒
来源：http://md.9csxet.cn

--------------------------------------------------------------------------------
来源：http://kx.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gg.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jj.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rx.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sp.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ov.haigaiapp.cn

—— 文件结束 ——
来源：http://sh.gzmigu.cn

================================================================================
来源：http://ra.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://aw.nicolike.cn

Common Programming Examples Cheat Book
来源：http://la.9csxet.cn

================================================================================
来源：http://dt.yuntaijiaju.cn

【收录内容】
来源：http://ex.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nq.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rl.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://lb.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yc.muxihuayi.cn

【使用说明】
来源：http://sk.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cv.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hi.lnxyls.cn


<!-- 参考信息 -->