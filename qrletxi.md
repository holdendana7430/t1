代发 wailian999

[U13] Py：固定长度队列
来源：http://dc.muxihuayi.cn

deque(maxlen=10)
来源：http://yl.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://qd.jctech888.com.cn

defaultdict(list)
来源：http://mm.hahajie.cn

[U15] Py：高精度计时
来源：http://ti.jctech888.com.cn

t = time.perf_counter()
来源：http://qh.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://jr.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rm.muxihuayi.cn

[U17] Py：初始化日志
来源：http://xf.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://zu.wgjwhj.cn

[U18] Py：预编译正则
来源：http://pd.colortex.cn

pat = re.compile(r"\d+")
来源：http://ix.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://kr.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ah.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://xx.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://jm.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://qs.szxytkj.cn

@contextlib.contextmanager
来源：http://ja.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://zz.muxihuayi.cn

list(zip(*m))
来源：http://fk.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://nr.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cj.szsharing.cn

[U24] Py：路径操作
来源：http://hf.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://gz.panjiajie.cn

csv.DictReader(f)
来源：http://rj.chemitech.net.cn

[U26] Py：并发下载
来源：http://kb.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jg.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://ak.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://qd.521024.cn

[U28] Py：类型别名
来源：http://gz.nicolike.cn

UserId = int
来源：http://tg.hahajie.cn

[U29] Py：属性校验
来源：http://vm.hahajie.cn

@property 与 @x.setter 配合
来源：http://qy.shxzukj.cn

[U30] Py：数据类
来源：http://hm.chemitech.net.cn

@dataclass(slots=True)
来源：http://va.wgjwhj.cn

[U31] Py：单测
来源：http://lr.huixinmuqiang.cn

python -m pytest -q
来源：http://ly.szxytkj.cn

[U32] Py：代码格式化
来源：http://ss.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://tu.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://oq.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://se.muxihuayi.cn

[U34] Py：判断编码
来源：http://yb.haigaiapp.cn

chardet.detect(raw)
来源：http://ap.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://zs.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kr.haigaiapp.cn

[U36] Py：定时任务
来源：http://qu.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://wh.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://he.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sa.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://au.521024.cn

Path(__file__).resolve().parent
来源：http://qi.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://bd.wgjwhj.cn

sys.stdout.isatty()
来源：http://vf.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://lr.szxytkj.cn

print("err", file=sys.stderr)
来源：http://rh.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://yw.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cd.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://qw.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zr.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://wm.shxzukj.cn

namespace App\Http;
来源：http://tt.szsharing.cn

[U44] PHP：开启严格类型
来源：http://be.gzmigu.cn

declare(strict_types=1);
来源：http://xq.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://fp.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ay.yuexingan06.cn

[U46] PHP：可空类型
来源：http://ys.shtwfgs.cn

?string $name = null
来源：http://pv.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ll.jctech888.com.cn

int|string $id
来源：http://dw.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://dd.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://la.lnxyls.cn

[U49] PHP：只读属性
来源：http://sm.chemitech.net.cn

public readonly string $name
来源：http://is.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://hu.newstarts.cn

public function __construct(private int $id) {}
来源：http://qi.9csxet.cn

[U51] PHP：数组解构
来源：http://eo.szsharing.cn

[$a, $b] = $arr;
来源：http://kr.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://zq.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://mi.hahajie.cn

[U53] PHP：空合并运算符
来源：http://fi.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://tk.nszjky.cn

[U54] PHP：空安全调用
来源：http://cr.muxihuayi.cn

$obj?->method()
来源：http://gb.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ep.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hu.wgjwhj.cn

[U56] PHP：命名参数
来源：http://xz.colortex.cn

f(a: 1, b: 2)
来源：http://av.newstarts.cn

[U57] PHP：字符串插值
来源：http://an.szxytkj.cn

"值: {$a}"
来源：http://tc.9csxet.cn

[U58] PHP：数组三件套
来源：http://fr.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://co.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://pb.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aq.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://ia.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cd.yuexingan06.cn

[U61] PHP：正则
来源：http://ek.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yi.haigaiapp.cn

[U62] PHP：日期对象
来源：http://zl.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hl.hahajie.cn

[U63] PHP：文件读写
来源：http://mk.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jv.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ww.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://zo.huixinmuqiang.cn

[U65] PHP：会话
来源：http://gd.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sd.colortex.cn

[U66] PHP：设置 Cookie
来源：http://gv.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ns.asd995.cn

[U67] PHP：处理文件上传
来源：http://ul.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ku.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://jx.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qv.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://cc.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gp.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://hb.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gx.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://em.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://ts.gzmigu.cn

[U72] PHP：写错误日志
来源：http://bs.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ug.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://kp.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://bt.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://gr.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://nq.asd995.cn

[U75] PHP：依赖注入
来源：http://by.yuntaijiaju.cn

composer require psr/container
来源：http://nk.hahajie.cn

[U76] PHP：简单路由
来源：http://dp.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vq.newstarts.cn

[U77] PHP：模板渲染
来源：http://qv.colortex.cn

composer require twig/twig
来源：http://jk.shtwfgs.cn

[U78] PHP：单元测试
来源：http://sl.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://yi.shxzukj.cn

[U79] PHP：静态分析
来源：http://gz.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ak.521024.cn

[U80] PHP：代码规范修复
来源：http://xo.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://to.newstarts.cn

[U81] JS：初始化项目
来源：http://an.shxzukj.cn

npm init -y;  npm i express
来源：http://rx.newstarts.cn

[U82] JS：package.json 脚本
来源：http://lq.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cj.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://np.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rz.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://hp.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ql.nicolike.cn

[U85] JS：可选链
来源：http://sy.lnxyls.cn

a?.b?.c
来源：http://ir.colortex.cn

[U86] JS：空值合并
来源：http://vl.hnjuh.cn

a ?? b
来源：http://jg.szsharing.cn

[U87] JS：解构默认值
来源：http://kh.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://cr.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://jp.bookmarksfly.cn

{ ...a, ...b }
来源：http://jz.chemitech.net.cn

[U89] JS：数组去重
来源：http://tj.chemitech.net.cn

[...new Set(arr)]
来源：http://yc.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://it.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://pu.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://ts.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fm.shxzskj.cn

[U92] JS：深拷贝
来源：http://wf.huixiangedu.cn

structuredClone(obj)
来源：http://rm.newstarts.cn

[U93] JS：模板字符串
来源：http://ay.wgjwhj.cn

`共 ${n} 条`
来源：http://db.nszjky.cn

[U94] JS：箭头函数
来源：http://ku.521024.cn

const double = x => x * 2;
来源：http://jk.shxzskj.cn

[U95] JS：Promise 包装
来源：http://oz.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://tm.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://pe.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sc.shxzskj.cn

[U97] JS：并发请求
来源：http://zb.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ih.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://nd.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://in.hahajie.cn

[U99] JS：事件监听
来源：http://yv.521024.cn

el.addEventListener("click", e => {})
来源：http://ll.shxzukj.cn

[U100] JS：DOM 查询
来源：http://qm.nicolike.cn

document.querySelector(".item")
来源：http://hi.huanxung.cn

[U101] JS：classList 操作
来源：http://xg.gzmigu.cn

el.classList.toggle("active")
来源：http://tw.nszjky.cn

[U102] JS：本地存储
来源：http://jo.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zj.huixiangedu.cn

[U103] JS：定时器
来源：http://ng.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://es.asd995.cn

[U104] JS：防抖
来源：http://ra.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bx.asd995.cn

[U105] JS：节流
来源：http://xu.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gg.huixiangedu.cn

[U106] JS：日期格式化
来源：http://dd.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gw.muxihuayi.cn

[U107] JS：数字千分位
来源：http://jv.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ve.huixiangedu.cn

[U108] JS：随机整数
来源：http://iq.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tb.szsharing.cn

[U109] JS：数组分组
来源：http://ax.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://zl.huanxung.cn

[U110] JS：数组分块
来源：http://by.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mb.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://bh.9csxet.cn

new Map(Object.entries(obj))
来源：http://ia.hahajie.cn

[U112] JS：字符串补位
来源：http://sg.szxytkj.cn

"7".padStart(3, "0")
来源：http://yt.shxzukj.cn

[U113] JS：正则替换全部
来源：http://zt.shxzskj.cn

s.replaceAll("a", "b")
来源：http://cg.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://gk.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ei.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ju.huixiangedu.cn

crypto.randomUUID()
来源：http://ti.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ka.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://zk.shxzskj.cn

[U117] JS：单元测试
来源：http://ss.colortex.cn

npm i -D vitest;  npx vitest
来源：http://sa.jctech888.com.cn

[U118] JS：开发服务器
来源：http://lr.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://hf.newstarts.cn

[U119] JS：生产构建
来源：http://tz.muxihuayi.cn

npx vite build
来源：http://mm.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://yx.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://oe.shtwfgs.cn

================================================================================
来源：http://en.huanxung.cn

统计汇总
来源：http://sn.wgjwhj.cn

================================================================================
来源：http://nr.shxzskj.cn

按语言统计（条）：
来源：http://qn.jctech888.com.cn

Python ......... 252
来源：http://re.chemitech.net.cn

PHP ............ 252
来源：http://mb.shxzskj.cn

JavaScript ..... 252
来源：http://vq.chemitech.net.cn

TypeScript ..... 212
来源：http://jg.haigaiapp.cn

Java ........... 212
来源：http://vk.jctech888.com.cn

Go ............. 212
来源：http://xt.521024.cn

Ruby ........... 212
来源：http://it.szsharing.cn

C# ............. 212
来源：http://nd.9csxet.cn

C .............. 30
来源：http://ph.gzmigu.cn

C++ ............ 30
来源：http://tp.asd995.cn

SQL ............ 90
来源：http://wb.szsharing.cn

Bash ........... 80
来源：http://fl.panjiajie.cn

Kotlin ......... 15
来源：http://ua.asd995.cn

Swift .......... 15
来源：http://ap.asd995.cn

Lua ............ 10
来源：http://ur.newstarts.cn

Perl ........... 10
来源：http://at.colortex.cn

Scala .......... 10
来源：http://op.hnjuh.cn

------------------------------------
来源：http://cz.panjiajie.cn

合计 ........... 2106 条
来源：http://hu.shtwfgs.cn

按章节统计：
来源：http://cj.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sr.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sh.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tc.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rs.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pt.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ou.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fz.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gg.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ex.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fl.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hf.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cs.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rr.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://di.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ci.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qi.shtwfgs.cn

Q SQL 专题                              90
来源：http://ed.lnxyls.cn

R Bash 专题                             80
来源：http://fl.szxytkj.cn

S C / C++ 专题                          60
来源：http://zf.wgjwhj.cn

T 其他语言补充                          60
来源：http://bn.szsharing.cn

U 高频实用片段                         120
来源：http://sf.hnjuh.cn

------------------------------------
来源：http://mu.hahajie.cn

合计                                  2106 条
来源：http://dm.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://bb.wgjwhj.cn

使用提醒
来源：http://ld.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ci.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kd.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ek.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://we.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mq.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ap.nicolike.cn

—— 文件结束 ——
来源：http://zg.huanxung.cn

================================================================================
来源：http://bf.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://cs.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://ee.colortex.cn

================================================================================
来源：http://cw.huixinmuqiang.cn

【收录内容】
来源：http://ra.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tz.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://id.nszjky.cn

SQL · Bash · C · C++
来源：http://sh.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lf.newstarts.cn

【使用说明】
来源：http://yy.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qt.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zb.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nl.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ai.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dh.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qx.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qd.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://le.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vz.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yz.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mr.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wk.lnxyls.cn

【文件统计】
来源：http://om.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mf.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://wd.huixinmuqiang.cn

目  录
来源：http://wr.colortex.cn

--------------------------------------------------------------------------------
来源：http://lb.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nj.shtwfgs.cn


<!-- 参考信息 -->