代发 wailian999

[U07] Py：反转字典键值
来源：http://js.newstarts.cn

{v: k for k, v in d.items()}
来源：http://gl.lnxyls.cn

[U08] Py：展平二维列表
来源：http://vm.shtwfgs.cn

[y for x in nested for y in x]
来源：http://rm.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://dr.lnxyls.cn

max(d, key=d.get)
来源：http://zx.shxzukj.cn

[U10] Py：按值排序字典
来源：http://yr.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gv.gzmigu.cn

[U11] Py：生成器表达式
来源：http://tw.szxytkj.cn

(x * 2 for x in arr)
来源：http://wc.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gg.huanxung.cn

Counter(arr).most_common(3)
来源：http://ad.lnxyls.cn

[U13] Py：固定长度队列
来源：http://ko.nicolike.cn

deque(maxlen=10)
来源：http://lq.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://kg.asd995.cn

defaultdict(list)
来源：http://ue.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://ab.huixinmuqiang.cn

t = time.perf_counter()
来源：http://ci.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://mu.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gg.bjjhwx.cn

[U17] Py：初始化日志
来源：http://lu.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://tw.muxihuayi.cn

[U18] Py：预编译正则
来源：http://bx.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://uw.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://kb.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kf.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://lo.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://rm.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://zh.haigaiapp.cn

@contextlib.contextmanager
来源：http://oh.szsharing.cn

[U22] Py：矩阵转置
来源：http://wb.szsharing.cn

list(zip(*m))
来源：http://ix.nszjky.cn

[U23] Py：分块读取大文件
来源：http://fd.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ci.nszjky.cn

[U24] Py：路径操作
来源：http://gy.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lf.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://kp.asd995.cn

csv.DictReader(f)
来源：http://sk.gzmigu.cn

[U26] Py：并发下载
来源：http://aj.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aa.huanxung.cn

[U27] Py：异步 HTTP
来源：http://og.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://zf.wgjwhj.cn

[U28] Py：类型别名
来源：http://dh.jianghongdianzi.cn

UserId = int
来源：http://xz.nszjky.cn

[U29] Py：属性校验
来源：http://nk.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://tg.huanxung.cn

[U30] Py：数据类
来源：http://iv.haigaiapp.cn

@dataclass(slots=True)
来源：http://kh.yuexingan06.cn

[U31] Py：单测
来源：http://wn.muxihuayi.cn

python -m pytest -q
来源：http://rl.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://ly.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://ek.hnjuh.cn

[U33] Py：打包发布
来源：http://om.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://ml.hahajie.cn

[U34] Py：判断编码
来源：http://oy.wgjwhj.cn

chardet.detect(raw)
来源：http://xu.szsharing.cn

[U35] Py：发送邮件
来源：http://rq.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zg.szsharing.cn

[U36] Py：定时任务
来源：http://kn.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://hh.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://kn.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yx.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://mf.shxzukj.cn

Path(__file__).resolve().parent
来源：http://zd.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://yw.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://cp.asd995.cn

[U40] Py：打印到标准错误
来源：http://ts.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://oi.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://sv.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vl.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://rk.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yp.newstarts.cn

[U43] PHP：声明命名空间
来源：http://dp.panjiajie.cn

namespace App\Http;
来源：http://pi.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://fa.muxihuayi.cn

declare(strict_types=1);
来源：http://bt.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://mp.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fd.chemitech.net.cn

[U46] PHP：可空类型
来源：http://gm.9csxet.cn

?string $name = null
来源：http://zg.yuexingan06.cn

[U47] PHP：联合类型
来源：http://bv.shxzskj.cn

int|string $id
来源：http://ma.hnjuh.cn

[U48] PHP：纯枚举
来源：http://xv.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yi.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://lt.yuntaijiaju.cn

public readonly string $name
来源：http://fb.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://ad.shxzskj.cn

public function __construct(private int $id) {}
来源：http://tu.szsharing.cn

[U51] PHP：数组解构
来源：http://lf.521024.cn

[$a, $b] = $arr;
来源：http://et.huanxung.cn

[U52] PHP：箭头函数
来源：http://aj.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://ex.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://sv.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://ga.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://dw.nicolike.cn

$obj?->method()
来源：http://th.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://av.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sx.panjiajie.cn

[U56] PHP：命名参数
来源：http://ui.9csxet.cn

f(a: 1, b: 2)
来源：http://ls.521024.cn

[U57] PHP：字符串插值
来源：http://bs.panjiajie.cn

"值: {$a}"
来源：http://oj.colortex.cn

[U58] PHP：数组三件套
来源：http://lr.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gl.szsharing.cn

[U59] PHP：自定义排序
来源：http://cx.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xp.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://ct.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yi.yuexingan06.cn

[U61] PHP：正则
来源：http://ua.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pd.shtwfgs.cn

[U62] PHP：日期对象
来源：http://cp.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pf.hnjuh.cn

[U63] PHP：文件读写
来源：http://go.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oh.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://nr.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://cl.wgjwhj.cn

[U65] PHP：会话
来源：http://fd.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vh.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://px.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hq.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://wj.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sr.colortex.cn

[U68] PHP：PDO 连接
来源：http://tn.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dq.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://yx.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zz.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://et.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mo.shxzukj.cn

[U71] PHP：抛出异常
来源：http://ne.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://zp.hahajie.cn

[U72] PHP：写错误日志
来源：http://or.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://qa.521024.cn

[U73] PHP：读取 ini 配置
来源：http://oq.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://rc.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://rd.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://bu.hahajie.cn

[U75] PHP：依赖注入
来源：http://qz.huanxung.cn

composer require psr/container
来源：http://qi.huixiangedu.cn

[U76] PHP：简单路由
来源：http://ky.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xq.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://oq.hahajie.cn

composer require twig/twig
来源：http://jg.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://cw.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://mj.newstarts.cn

[U79] PHP：静态分析
来源：http://vi.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://sz.asd995.cn

[U80] PHP：代码规范修复
来源：http://bg.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gi.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://fi.newstarts.cn

npm init -y;  npm i express
来源：http://pd.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://hm.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://td.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://ds.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dk.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://uw.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uw.szxytkj.cn

[U85] JS：可选链
来源：http://mr.yuntaijiaju.cn

a?.b?.c
来源：http://rt.9csxet.cn

[U86] JS：空值合并
来源：http://jj.nszjky.cn

a ?? b
来源：http://zp.haigaiapp.cn

[U87] JS：解构默认值
来源：http://la.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://dp.nicolike.cn

[U88] JS：对象展开合并
来源：http://hi.nicolike.cn

{ ...a, ...b }
来源：http://ef.shxzskj.cn

[U89] JS：数组去重
来源：http://gf.szxytkj.cn

[...new Set(arr)]
来源：http://ny.huanxung.cn

[U90] JS：数字数组排序
来源：http://cb.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://xn.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://ip.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jy.nicolike.cn

[U92] JS：深拷贝
来源：http://jr.szsharing.cn

structuredClone(obj)
来源：http://ga.nicolike.cn

[U93] JS：模板字符串
来源：http://zm.bjjhwx.cn

`共 ${n} 条`
来源：http://wr.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://pu.521024.cn

const double = x => x * 2;
来源：http://tr.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://yj.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://hb.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://gm.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gu.jctech888.com.cn

[U97] JS：并发请求
来源：http://em.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qg.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://ya.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mx.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://tv.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://sh.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://ue.shxzskj.cn

document.querySelector(".item")
来源：http://gv.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://tr.nicolike.cn

el.classList.toggle("active")
来源：http://jg.shxzukj.cn

[U102] JS：本地存储
来源：http://ps.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mn.9csxet.cn

[U103] JS：定时器
来源：http://nm.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mc.haigaiapp.cn

[U104] JS：防抖
来源：http://mj.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xj.hnjuh.cn

[U105] JS：节流
来源：http://ph.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sx.shxzskj.cn

[U106] JS：日期格式化
来源：http://di.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lz.gzmigu.cn

[U107] JS：数字千分位
来源：http://ry.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bc.huixiangedu.cn

[U108] JS：随机整数
来源：http://rb.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jh.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://cn.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://av.haigaiapp.cn

[U110] JS：数组分块
来源：http://hs.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dg.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://fp.nicolike.cn

new Map(Object.entries(obj))
来源：http://mt.shtwfgs.cn

[U112] JS：字符串补位
来源：http://yf.chemitech.net.cn

"7".padStart(3, "0")
来源：http://kw.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://vl.asd995.cn

s.replaceAll("a", "b")
来源：http://me.nicolike.cn

[U114] JS：JSON 深比较
来源：http://lp.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ad.hnjuh.cn

[U115] JS：生成 UUID
来源：http://vc.jctech888.com.cn

crypto.randomUUID()
来源：http://zr.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://nc.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://hv.colortex.cn

[U117] JS：单元测试
来源：http://my.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://yi.haigaiapp.cn

[U118] JS：开发服务器
来源：http://it.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://su.newstarts.cn

[U119] JS：生产构建
来源：http://xy.colortex.cn

npx vite build
来源：http://ek.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://fd.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://yn.asd995.cn

================================================================================
来源：http://yk.szsharing.cn

统计汇总
来源：http://zr.gzmigu.cn

================================================================================
来源：http://ou.colortex.cn

按语言统计（条）：
来源：http://wd.wgjwhj.cn

Python ......... 252
来源：http://qr.lnxyls.cn

PHP ............ 252
来源：http://xz.wgjwhj.cn

JavaScript ..... 252
来源：http://zt.yuexingan06.cn

TypeScript ..... 212
来源：http://ng.yuexingan06.cn

Java ........... 212
来源：http://tk.nicolike.cn

Go ............. 212
来源：http://xh.haigaiapp.cn

Ruby ........... 212
来源：http://yf.newstarts.cn

C# ............. 212
来源：http://fy.bjjhwx.cn

C .............. 30
来源：http://hh.shxzskj.cn

C++ ............ 30
来源：http://wl.shxzukj.cn

SQL ............ 90
来源：http://el.jianghongdianzi.cn

Bash ........... 80
来源：http://yr.muxihuayi.cn

Kotlin ......... 15
来源：http://za.huixinmuqiang.cn

Swift .......... 15
来源：http://to.huixiangedu.cn

Lua ............ 10
来源：http://fq.jctech888.com.cn

Perl ........... 10
来源：http://oe.haigaiapp.cn

Scala .......... 10
来源：http://tj.hahajie.cn

------------------------------------
来源：http://bt.wgjwhj.cn

合计 ........... 2106 条
来源：http://za.szsharing.cn

按章节统计：
来源：http://cb.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mq.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ri.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dt.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cb.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://us.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rm.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://al.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bt.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cu.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nq.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ak.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xm.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kv.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hr.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://er.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hx.lnxyls.cn

Q SQL 专题                              90
来源：http://ec.lnxyls.cn

R Bash 专题                             80
来源：http://nl.szsharing.cn

S C / C++ 专题                          60
来源：http://wa.9csxet.cn

T 其他语言补充                          60
来源：http://uw.hahajie.cn

U 高频实用片段                         120
来源：http://el.wgjwhj.cn

------------------------------------
来源：http://gq.bookmarksfly.cn

合计                                  2106 条
来源：http://ko.asd995.cn

--------------------------------------------------------------------------------
来源：http://of.huixiangedu.cn

使用提醒
来源：http://cw.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://aq.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xc.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cf.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://au.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iv.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://md.asd995.cn

—— 文件结束 ——
来源：http://uf.asd995.cn

================================================================================
来源：http://ah.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://ge.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://rp.muxihuayi.cn

================================================================================
来源：http://aq.wgjwhj.cn

【收录内容】
来源：http://pq.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gq.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://is.bjjhwx.cn

SQL · Bash · C · C++
来源：http://ug.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xf.asd995.cn

【使用说明】
来源：http://iq.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oy.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tm.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ql.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ql.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kv.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qc.haigaiapp.cn


<!-- 参考信息 -->