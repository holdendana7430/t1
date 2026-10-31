代发 wailian999

[U09] Py：字典取最大值的键
来源：http://yl.9csxet.cn

max(d, key=d.get)
来源：http://oi.hnjuh.cn

[U10] Py：按值排序字典
来源：http://oa.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dq.shxzukj.cn

[U11] Py：生成器表达式
来源：http://ij.huixiangedu.cn

(x * 2 for x in arr)
来源：http://up.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://my.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://fi.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://gh.hnjuh.cn

deque(maxlen=10)
来源：http://sh.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://mw.nszjky.cn

defaultdict(list)
来源：http://eg.asd995.cn

[U15] Py：高精度计时
来源：http://cj.hahajie.cn

t = time.perf_counter()
来源：http://fp.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://kh.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jc.shxzukj.cn

[U17] Py：初始化日志
来源：http://gk.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://dv.newstarts.cn

[U18] Py：预编译正则
来源：http://gm.nicolike.cn

pat = re.compile(r"\d+")
来源：http://al.521024.cn

[U19] Py：正则替换带回调
来源：http://ro.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://od.521024.cn

[U20] Py：缓存函数结果
来源：http://sf.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://vg.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://nt.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://rz.hnjuh.cn

[U22] Py：矩阵转置
来源：http://dz.gzmigu.cn

list(zip(*m))
来源：http://oj.newstarts.cn

[U23] Py：分块读取大文件
来源：http://ee.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bz.asd995.cn

[U24] Py：路径操作
来源：http://ar.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gf.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://eb.shxzukj.cn

csv.DictReader(f)
来源：http://tt.nszjky.cn

[U26] Py：并发下载
来源：http://fd.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wy.huanxung.cn

[U27] Py：异步 HTTP
来源：http://ig.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://wt.gzmigu.cn

[U28] Py：类型别名
来源：http://zz.shtwfgs.cn

UserId = int
来源：http://pv.nszjky.cn

[U29] Py：属性校验
来源：http://ii.huanxung.cn

@property 与 @x.setter 配合
来源：http://uj.muxihuayi.cn

[U30] Py：数据类
来源：http://by.bjjhwx.cn

@dataclass(slots=True)
来源：http://te.shxzskj.cn

[U31] Py：单测
来源：http://qc.bookmarksfly.cn

python -m pytest -q
来源：http://au.panjiajie.cn

[U32] Py：代码格式化
来源：http://hh.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://fs.bjjhwx.cn

[U33] Py：打包发布
来源：http://ba.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://xt.newstarts.cn

[U34] Py：判断编码
来源：http://tb.nicolike.cn

chardet.detect(raw)
来源：http://ia.nszjky.cn

[U35] Py：发送邮件
来源：http://fu.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ow.shxzskj.cn

[U36] Py：定时任务
来源：http://aq.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://do.nicolike.cn

[U37] Py：读写 Excel
来源：http://pf.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wk.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://yl.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://eu.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://ei.wgjwhj.cn

sys.stdout.isatty()
来源：http://tk.hahajie.cn

[U40] Py：打印到标准错误
来源：http://zn.hnjuh.cn

print("err", file=sys.stderr)
来源：http://cs.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://op.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xa.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://zy.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fx.521024.cn

[U43] PHP：声明命名空间
来源：http://aj.huanxung.cn

namespace App\Http;
来源：http://fr.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://we.jianghongdianzi.cn

declare(strict_types=1);
来源：http://vz.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://gg.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.nicolike.cn

[U46] PHP：可空类型
来源：http://vy.shxzukj.cn

?string $name = null
来源：http://fn.szxytkj.cn

[U47] PHP：联合类型
来源：http://jn.nszjky.cn

int|string $id
来源：http://gx.panjiajie.cn

[U48] PHP：纯枚举
来源：http://qx.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dr.szxytkj.cn

[U49] PHP：只读属性
来源：http://pb.chemitech.net.cn

public readonly string $name
来源：http://sc.colortex.cn

[U50] PHP：构造器属性提升
来源：http://sg.gzmigu.cn

public function __construct(private int $id) {}
来源：http://fk.chemitech.net.cn

[U51] PHP：数组解构
来源：http://gq.asd995.cn

[$a, $b] = $arr;
来源：http://nw.gzmigu.cn

[U52] PHP：箭头函数
来源：http://oo.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://vi.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://it.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://ra.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://hm.9csxet.cn

$obj?->method()
来源：http://fv.hnjuh.cn

[U55] PHP：match 表达式
来源：http://xt.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zl.shtwfgs.cn

[U56] PHP：命名参数
来源：http://ot.shtwfgs.cn

f(a: 1, b: 2)
来源：http://ze.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://js.gzmigu.cn

"值: {$a}"
来源：http://eu.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://xa.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ne.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://mj.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gc.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://iq.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bi.wgjwhj.cn

[U61] PHP：正则
来源：http://cx.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zu.newstarts.cn

[U62] PHP：日期对象
来源：http://os.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ti.huixiangedu.cn

[U63] PHP：文件读写
来源：http://ao.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rh.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://jr.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://an.lnxyls.cn

[U65] PHP：会话
来源：http://ug.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ty.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://ir.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mq.9csxet.cn

[U67] PHP：处理文件上传
来源：http://ky.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zh.9csxet.cn

[U68] PHP：PDO 连接
来源：http://nl.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fv.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://bw.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kf.nszjky.cn

[U70] PHP：PDO 事务
来源：http://ur.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fr.gzmigu.cn

[U71] PHP：抛出异常
来源：http://iu.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://xe.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://ki.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://nv.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://sy.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://dj.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://sj.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://wq.asd995.cn

[U75] PHP：依赖注入
来源：http://gi.huanxung.cn

composer require psr/container
来源：http://yd.nicolike.cn

[U76] PHP：简单路由
来源：http://sf.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pr.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://kf.lnxyls.cn

composer require twig/twig
来源：http://ku.szsharing.cn

[U78] PHP：单元测试
来源：http://zu.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://nc.asd995.cn

[U79] PHP：静态分析
来源：http://tv.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://zi.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://wq.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xj.shxzukj.cn

[U81] JS：初始化项目
来源：http://hv.szsharing.cn

npm init -y;  npm i express
来源：http://yo.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://ub.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ok.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://sx.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ss.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://ht.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lv.shtwfgs.cn

[U85] JS：可选链
来源：http://px.colortex.cn

a?.b?.c
来源：http://cd.huanxung.cn

[U86] JS：空值合并
来源：http://je.hnjuh.cn

a ?? b
来源：http://eh.huixiangedu.cn

[U87] JS：解构默认值
来源：http://cp.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://nq.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://rc.panjiajie.cn

{ ...a, ...b }
来源：http://hd.newstarts.cn

[U89] JS：数组去重
来源：http://sr.muxihuayi.cn

[...new Set(arr)]
来源：http://td.szsharing.cn

[U90] JS：数字数组排序
来源：http://us.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://ru.9csxet.cn

[U91] JS：对象键值遍历
来源：http://ao.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ys.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://vc.lnxyls.cn

structuredClone(obj)
来源：http://rk.haigaiapp.cn

[U93] JS：模板字符串
来源：http://vb.521024.cn

`共 ${n} 条`
来源：http://qa.wgjwhj.cn

[U94] JS：箭头函数
来源：http://co.shtwfgs.cn

const double = x => x * 2;
来源：http://qt.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://pw.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://up.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://tx.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nf.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://gk.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mg.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://rj.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wt.nszjky.cn

[U99] JS：事件监听
来源：http://rz.asd995.cn

el.addEventListener("click", e => {})
来源：http://pv.panjiajie.cn

[U100] JS：DOM 查询
来源：http://fu.yuexingan06.cn

document.querySelector(".item")
来源：http://yj.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://ly.gzmigu.cn

el.classList.toggle("active")
来源：http://it.huixiangedu.cn

[U102] JS：本地存储
来源：http://uz.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wu.bjjhwx.cn

[U103] JS：定时器
来源：http://oi.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yh.muxihuayi.cn

[U104] JS：防抖
来源：http://gi.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dz.bookmarksfly.cn

[U105] JS：节流
来源：http://kz.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ui.lnxyls.cn

[U106] JS：日期格式化
来源：http://wf.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ik.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://xz.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://om.asd995.cn

[U108] JS：随机整数
来源：http://fa.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vj.9csxet.cn

[U109] JS：数组分组
来源：http://mn.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://wd.shxzskj.cn

[U110] JS：数组分块
来源：http://ht.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xs.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://gy.lnxyls.cn

new Map(Object.entries(obj))
来源：http://rb.huixiangedu.cn

[U112] JS：字符串补位
来源：http://zs.colortex.cn

"7".padStart(3, "0")
来源：http://it.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://gb.gzmigu.cn

s.replaceAll("a", "b")
来源：http://zn.521024.cn

[U114] JS：JSON 深比较
来源：http://nh.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://in.huanxung.cn

[U115] JS：生成 UUID
来源：http://ev.asd995.cn

crypto.randomUUID()
来源：http://py.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://vd.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://el.yuexingan06.cn

[U117] JS：单元测试
来源：http://tf.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://gn.lnxyls.cn

[U118] JS：开发服务器
来源：http://sr.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://ey.nszjky.cn

[U119] JS：生产构建
来源：http://mo.huixinmuqiang.cn

npx vite build
来源：http://od.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://jj.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://th.newstarts.cn

================================================================================
来源：http://fx.yuexingan06.cn

统计汇总
来源：http://wf.panjiajie.cn

================================================================================
来源：http://kk.chemitech.net.cn

按语言统计（条）：
来源：http://bq.shxzukj.cn

Python ......... 252
来源：http://zt.panjiajie.cn

PHP ............ 252
来源：http://tx.szsharing.cn

JavaScript ..... 252
来源：http://jp.gzmigu.cn

TypeScript ..... 212
来源：http://vx.haigaiapp.cn

Java ........... 212
来源：http://sg.wgjwhj.cn

Go ............. 212
来源：http://pt.huixiangedu.cn

Ruby ........... 212
来源：http://rs.haigaiapp.cn

C# ............. 212
来源：http://jr.szsharing.cn

C .............. 30
来源：http://lk.wgjwhj.cn

C++ ............ 30
来源：http://zo.shxzskj.cn

SQL ............ 90
来源：http://qj.newstarts.cn

Bash ........... 80
来源：http://ge.yuexingan06.cn

Kotlin ......... 15
来源：http://ak.9csxet.cn

Swift .......... 15
来源：http://nd.yuexingan06.cn

Lua ............ 10
来源：http://wq.yuntaijiaju.cn

Perl ........... 10
来源：http://nr.chemitech.net.cn

Scala .......... 10
来源：http://pd.colortex.cn

------------------------------------
来源：http://zu.shxzskj.cn

合计 ........... 2106 条
来源：http://rv.haigaiapp.cn

按章节统计：
来源：http://kv.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mq.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fl.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zz.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bm.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xx.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ej.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hm.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jo.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pe.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dw.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ja.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qu.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ta.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ty.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://un.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tc.newstarts.cn

Q SQL 专题                              90
来源：http://ss.chemitech.net.cn

R Bash 专题                             80
来源：http://uy.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://yn.panjiajie.cn

T 其他语言补充                          60
来源：http://pn.haigaiapp.cn

U 高频实用片段                         120
来源：http://nv.lnxyls.cn

------------------------------------
来源：http://fo.huanxung.cn

合计                                  2106 条
来源：http://rj.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://jw.jianghongdianzi.cn

使用提醒
来源：http://ep.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://hh.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://if.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bg.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ga.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ym.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ke.shxzukj.cn

—— 文件结束 ——
来源：http://so.szxytkj.cn

================================================================================
来源：http://jt.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://ww.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://wo.panjiajie.cn

================================================================================
来源：http://ee.yuexingan06.cn

【收录内容】
来源：http://mf.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rk.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xf.asd995.cn

SQL · Bash · C · C++
来源：http://tl.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ip.haigaiapp.cn

【使用说明】
来源：http://jp.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jm.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ey.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uy.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pk.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ba.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ob.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cy.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hh.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ro.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eu.jctech888.com.cn


<!-- 参考信息 -->