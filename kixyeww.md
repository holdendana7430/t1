代发 wailian999

[U09] Py：字典取最大值的键
来源：http://qi.hnjuh.cn

max(d, key=d.get)
来源：http://ve.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://iv.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tc.hnjuh.cn

[U11] Py：生成器表达式
来源：http://hc.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ie.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dr.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://gx.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://mq.nszjky.cn

deque(maxlen=10)
来源：http://oi.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://lr.newstarts.cn

defaultdict(list)
来源：http://ii.huanxung.cn

[U15] Py：高精度计时
来源：http://cl.9csxet.cn

t = time.perf_counter()
来源：http://hh.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://rt.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cx.nszjky.cn

[U17] Py：初始化日志
来源：http://en.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://ni.hnjuh.cn

[U18] Py：预编译正则
来源：http://ik.asd995.cn

pat = re.compile(r"\d+")
来源：http://tz.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://jh.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ef.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://cc.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://rp.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ut.asd995.cn

@contextlib.contextmanager
来源：http://fg.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://bh.bjjhwx.cn

list(zip(*m))
来源：http://my.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://og.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zu.gzmigu.cn

[U24] Py：路径操作
来源：http://nh.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zx.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://di.jianghongdianzi.cn

csv.DictReader(f)
来源：http://bj.hahajie.cn

[U26] Py：并发下载
来源：http://mq.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cv.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://av.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://ql.shxzukj.cn

[U28] Py：类型别名
来源：http://yn.521024.cn

UserId = int
来源：http://pd.huanxung.cn

[U29] Py：属性校验
来源：http://fp.asd995.cn

@property 与 @x.setter 配合
来源：http://or.bookmarksfly.cn

[U30] Py：数据类
来源：http://qa.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://xq.shtwfgs.cn

[U31] Py：单测
来源：http://ut.jctech888.com.cn

python -m pytest -q
来源：http://zw.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ez.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://oa.bjjhwx.cn

[U33] Py：打包发布
来源：http://wg.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://wk.asd995.cn

[U34] Py：判断编码
来源：http://so.szxytkj.cn

chardet.detect(raw)
来源：http://wl.szxytkj.cn

[U35] Py：发送邮件
来源：http://ge.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://us.wgjwhj.cn

[U36] Py：定时任务
来源：http://gl.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://uq.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://gw.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hk.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://nv.szsharing.cn

Path(__file__).resolve().parent
来源：http://pw.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://hh.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://ym.521024.cn

[U40] Py：打印到标准错误
来源：http://rr.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://wg.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ov.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zr.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://dk.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mc.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://us.gzmigu.cn

namespace App\Http;
来源：http://ih.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://ui.hnjuh.cn

declare(strict_types=1);
来源：http://xe.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://fq.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://qa.jctech888.com.cn

?string $name = null
来源：http://fl.hahajie.cn

[U47] PHP：联合类型
来源：http://ex.szxytkj.cn

int|string $id
来源：http://qa.asd995.cn

[U48] PHP：纯枚举
来源：http://ar.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pq.nicolike.cn

[U49] PHP：只读属性
来源：http://mv.jctech888.com.cn

public readonly string $name
来源：http://mh.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://pj.asd995.cn

public function __construct(private int $id) {}
来源：http://jf.nicolike.cn

[U51] PHP：数组解构
来源：http://oi.szsharing.cn

[$a, $b] = $arr;
来源：http://fd.shxzukj.cn

[U52] PHP：箭头函数
来源：http://uy.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://vn.szsharing.cn

[U53] PHP：空合并运算符
来源：http://jz.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://xk.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ww.jctech888.com.cn

$obj?->method()
来源：http://uj.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://gs.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ul.bjjhwx.cn

[U56] PHP：命名参数
来源：http://mg.lnxyls.cn

f(a: 1, b: 2)
来源：http://it.nszjky.cn

[U57] PHP：字符串插值
来源：http://ma.521024.cn

"值: {$a}"
来源：http://db.9csxet.cn

[U58] PHP：数组三件套
来源：http://iu.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://on.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://um.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fm.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://tl.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zg.nszjky.cn

[U61] PHP：正则
来源：http://uz.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nb.chemitech.net.cn

[U62] PHP：日期对象
来源：http://sb.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ck.panjiajie.cn

[U63] PHP：文件读写
来源：http://rd.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rr.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://rc.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://wy.colortex.cn

[U65] PHP：会话
来源：http://xk.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eq.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://oo.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gv.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://zr.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ep.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://yc.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gy.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://xr.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nh.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://jv.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rh.hnjuh.cn

[U71] PHP：抛出异常
来源：http://fu.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://uk.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://xo.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://be.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://fm.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://bp.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://vj.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://tu.szsharing.cn

[U75] PHP：依赖注入
来源：http://st.gzmigu.cn

composer require psr/container
来源：http://fs.panjiajie.cn

[U76] PHP：简单路由
来源：http://yf.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fu.shxzukj.cn

[U77] PHP：模板渲染
来源：http://wu.shxzskj.cn

composer require twig/twig
来源：http://rc.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://tf.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://iq.panjiajie.cn

[U79] PHP：静态分析
来源：http://id.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://ia.newstarts.cn

[U80] PHP：代码规范修复
来源：http://th.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pc.hahajie.cn

[U81] JS：初始化项目
来源：http://ma.shtwfgs.cn

npm init -y;  npm i express
来源：http://xb.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://tb.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rl.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://kc.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://je.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://fw.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mc.yuntaijiaju.cn

[U85] JS：可选链
来源：http://au.jctech888.com.cn

a?.b?.c
来源：http://ru.bookmarksfly.cn

[U86] JS：空值合并
来源：http://ii.asd995.cn

a ?? b
来源：http://mr.hahajie.cn

[U87] JS：解构默认值
来源：http://us.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://eo.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://sm.yuexingan06.cn

{ ...a, ...b }
来源：http://bl.huanxung.cn

[U89] JS：数组去重
来源：http://pk.newstarts.cn

[...new Set(arr)]
来源：http://zw.asd995.cn

[U90] JS：数字数组排序
来源：http://mf.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://zg.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://fu.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xl.bjjhwx.cn

[U92] JS：深拷贝
来源：http://ko.szxytkj.cn

structuredClone(obj)
来源：http://lg.shxzukj.cn

[U93] JS：模板字符串
来源：http://wh.newstarts.cn

`共 ${n} 条`
来源：http://sm.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://bi.bjjhwx.cn

const double = x => x * 2;
来源：http://yv.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://rs.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://xe.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://kl.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kp.chemitech.net.cn

[U97] JS：并发请求
来源：http://cm.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ba.521024.cn

[U98] JS：fetch 带 JSON
来源：http://fq.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://em.chemitech.net.cn

[U99] JS：事件监听
来源：http://ts.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://es.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://pp.521024.cn

document.querySelector(".item")
来源：http://cb.muxihuayi.cn

[U101] JS：classList 操作
来源：http://lm.haigaiapp.cn

el.classList.toggle("active")
来源：http://kz.9csxet.cn

[U102] JS：本地存储
来源：http://ow.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oi.hnjuh.cn

[U103] JS：定时器
来源：http://on.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tb.panjiajie.cn

[U104] JS：防抖
来源：http://xv.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pj.panjiajie.cn

[U105] JS：节流
来源：http://jp.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wb.nicolike.cn

[U106] JS：日期格式化
来源：http://rq.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qx.jctech888.com.cn

[U107] JS：数字千分位
来源：http://ru.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kf.gzmigu.cn

[U108] JS：随机整数
来源：http://bo.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nr.yuexingan06.cn

[U109] JS：数组分组
来源：http://dz.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://gk.nicolike.cn

[U110] JS：数组分块
来源：http://qp.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nc.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://gh.asd995.cn

new Map(Object.entries(obj))
来源：http://nz.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://lb.521024.cn

"7".padStart(3, "0")
来源：http://vh.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://fv.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://oi.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://kn.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ua.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://ax.nszjky.cn

crypto.randomUUID()
来源：http://ig.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://es.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://rg.muxihuayi.cn

[U117] JS：单元测试
来源：http://io.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://xf.jctech888.com.cn

[U118] JS：开发服务器
来源：http://kr.shxzskj.cn

npm i -D vite;  npx vite
来源：http://fc.newstarts.cn

[U119] JS：生产构建
来源：http://jr.shxzukj.cn

npx vite build
来源：http://ww.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://hz.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://zd.jctech888.com.cn

================================================================================
来源：http://nq.shxzskj.cn

统计汇总
来源：http://tq.nicolike.cn

================================================================================
来源：http://ej.shtwfgs.cn

按语言统计（条）：
来源：http://yc.shxzukj.cn

Python ......... 252
来源：http://ds.yuexingan06.cn

PHP ............ 252
来源：http://jq.521024.cn

JavaScript ..... 252
来源：http://sl.521024.cn

TypeScript ..... 212
来源：http://pe.bjjhwx.cn

Java ........... 212
来源：http://ii.haigaiapp.cn

Go ............. 212
来源：http://xw.hahajie.cn

Ruby ........... 212
来源：http://ww.hahajie.cn

C# ............. 212
来源：http://xt.huixinmuqiang.cn

C .............. 30
来源：http://bq.szsharing.cn

C++ ............ 30
来源：http://ne.bookmarksfly.cn

SQL ............ 90
来源：http://ox.wgjwhj.cn

Bash ........... 80
来源：http://lf.szxytkj.cn

Kotlin ......... 15
来源：http://zw.szsharing.cn

Swift .......... 15
来源：http://go.9csxet.cn

Lua ............ 10
来源：http://lp.szsharing.cn

Perl ........... 10
来源：http://xa.huixinmuqiang.cn

Scala .......... 10
来源：http://vx.huixinmuqiang.cn

------------------------------------
来源：http://er.muxihuayi.cn

合计 ........... 2106 条
来源：http://ei.szxytkj.cn

按章节统计：
来源：http://bt.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cv.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lu.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zq.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gx.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gl.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://az.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fr.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fw.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ei.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ez.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aq.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ew.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yr.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://df.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uv.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qv.szsharing.cn

Q SQL 专题                              90
来源：http://vs.bjjhwx.cn

R Bash 专题                             80
来源：http://xh.yuexingan06.cn

S C / C++ 专题                          60
来源：http://ld.521024.cn

T 其他语言补充                          60
来源：http://zq.asd995.cn

U 高频实用片段                         120
来源：http://hy.newstarts.cn

------------------------------------
来源：http://ke.nicolike.cn

合计                                  2106 条
来源：http://sv.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://fy.bookmarksfly.cn

使用提醒
来源：http://si.9csxet.cn

--------------------------------------------------------------------------------
来源：http://fm.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ei.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://za.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://me.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ra.shxzskj.cn

—— 文件结束 ——
来源：http://oj.shxzskj.cn

================================================================================
来源：http://id.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://oo.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://tt.huixiangedu.cn

================================================================================
来源：http://xu.jctech888.com.cn

【收录内容】
来源：http://ti.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xg.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vv.shxzskj.cn

SQL · Bash · C · C++
来源：http://sm.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ck.szsharing.cn

【使用说明】
来源：http://nx.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ov.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tn.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uz.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oq.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rn.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uf.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wu.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rm.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wi.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jr.jianghongdianzi.cn


<!-- 参考信息 -->