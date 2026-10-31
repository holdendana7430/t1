代发 wailian999

[U13] Py：固定长度队列
来源：http://uo.szxytkj.cn

deque(maxlen=10)
来源：http://ck.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://qb.shxzukj.cn

defaultdict(list)
来源：http://ii.shxzskj.cn

[U15] Py：高精度计时
来源：http://rl.haigaiapp.cn

t = time.perf_counter()
来源：http://fq.521024.cn

[U16] Py：命令行参数解析
来源：http://jl.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sw.gzmigu.cn

[U17] Py：初始化日志
来源：http://ik.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://yr.haigaiapp.cn

[U18] Py：预编译正则
来源：http://dm.huanxung.cn

pat = re.compile(r"\d+")
来源：http://de.521024.cn

[U19] Py：正则替换带回调
来源：http://gn.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gv.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://dd.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://um.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://wp.szsharing.cn

@contextlib.contextmanager
来源：http://ss.nszjky.cn

[U22] Py：矩阵转置
来源：http://ai.muxihuayi.cn

list(zip(*m))
来源：http://vh.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://pn.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ks.szxytkj.cn

[U24] Py：路径操作
来源：http://gd.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lx.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://vv.szsharing.cn

csv.DictReader(f)
来源：http://jy.asd995.cn

[U26] Py：并发下载
来源：http://kx.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lk.nszjky.cn

[U27] Py：异步 HTTP
来源：http://me.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://vx.shxzukj.cn

[U28] Py：类型别名
来源：http://rn.shtwfgs.cn

UserId = int
来源：http://ix.colortex.cn

[U29] Py：属性校验
来源：http://hk.lnxyls.cn

@property 与 @x.setter 配合
来源：http://ia.huanxung.cn

[U30] Py：数据类
来源：http://kc.bookmarksfly.cn

@dataclass(slots=True)
来源：http://kq.asd995.cn

[U31] Py：单测
来源：http://te.wgjwhj.cn

python -m pytest -q
来源：http://ea.chemitech.net.cn

[U32] Py：代码格式化
来源：http://qr.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://zp.szsharing.cn

[U33] Py：打包发布
来源：http://by.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://zz.wgjwhj.cn

[U34] Py：判断编码
来源：http://aj.9csxet.cn

chardet.detect(raw)
来源：http://lv.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://rk.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tw.szsharing.cn

[U36] Py：定时任务
来源：http://hy.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://ng.hnjuh.cn

[U37] Py：读写 Excel
来源：http://bj.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gp.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://xu.hnjuh.cn

Path(__file__).resolve().parent
来源：http://vh.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://zg.hnjuh.cn

sys.stdout.isatty()
来源：http://mp.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://zn.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ks.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ah.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rf.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://bq.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oi.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://kk.nicolike.cn

namespace App\Http;
来源：http://oh.521024.cn

[U44] PHP：开启严格类型
来源：http://zz.huixinmuqiang.cn

declare(strict_types=1);
来源：http://td.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://id.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sr.szxytkj.cn

[U46] PHP：可空类型
来源：http://kh.wgjwhj.cn

?string $name = null
来源：http://xe.panjiajie.cn

[U47] PHP：联合类型
来源：http://dc.haigaiapp.cn

int|string $id
来源：http://yi.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://ms.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xc.lnxyls.cn

[U49] PHP：只读属性
来源：http://la.szxytkj.cn

public readonly string $name
来源：http://mr.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://lw.hahajie.cn

public function __construct(private int $id) {}
来源：http://ic.chemitech.net.cn

[U51] PHP：数组解构
来源：http://an.shxzukj.cn

[$a, $b] = $arr;
来源：http://qy.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://nt.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://el.colortex.cn

[U53] PHP：空合并运算符
来源：http://sp.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://mb.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://kk.panjiajie.cn

$obj?->method()
来源：http://mk.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://hm.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gw.wgjwhj.cn

[U56] PHP：命名参数
来源：http://ih.hahajie.cn

f(a: 1, b: 2)
来源：http://fj.9csxet.cn

[U57] PHP：字符串插值
来源：http://vm.panjiajie.cn

"值: {$a}"
来源：http://ob.shxzskj.cn

[U58] PHP：数组三件套
来源：http://lo.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jy.521024.cn

[U59] PHP：自定义排序
来源：http://vg.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tb.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://pe.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mg.chemitech.net.cn

[U61] PHP：正则
来源：http://in.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eu.panjiajie.cn

[U62] PHP：日期对象
来源：http://ly.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ik.szxytkj.cn

[U63] PHP：文件读写
来源：http://mw.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sq.shxzskj.cn

[U64] PHP：目录遍历
来源：http://fc.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://xl.newstarts.cn

[U65] PHP：会话
来源：http://hm.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jl.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://em.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wc.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://bs.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rz.9csxet.cn

[U68] PHP：PDO 连接
来源：http://pg.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hb.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://as.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qs.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ov.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ff.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://rm.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://bf.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://ca.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://ym.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://mf.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://pn.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://fz.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://je.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://uv.yuntaijiaju.cn

composer require psr/container
来源：http://qx.szsharing.cn

[U76] PHP：简单路由
来源：http://ws.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mo.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://wm.yuntaijiaju.cn

composer require twig/twig
来源：http://xl.panjiajie.cn

[U78] PHP：单元测试
来源：http://so.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://yr.hahajie.cn

[U79] PHP：静态分析
来源：http://sz.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://kn.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://lg.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qh.hnjuh.cn

[U81] JS：初始化项目
来源：http://wr.lnxyls.cn

npm init -y;  npm i express
来源：http://xy.521024.cn

[U82] JS：package.json 脚本
来源：http://fz.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xz.521024.cn

[U83] JS：ES Module 导入导出
来源：http://si.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ya.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://wf.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rj.shtwfgs.cn

[U85] JS：可选链
来源：http://du.szxytkj.cn

a?.b?.c
来源：http://bm.lnxyls.cn

[U86] JS：空值合并
来源：http://ta.hnjuh.cn

a ?? b
来源：http://uf.9csxet.cn

[U87] JS：解构默认值
来源：http://mh.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://ng.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://ju.shxzukj.cn

{ ...a, ...b }
来源：http://al.yuexingan06.cn

[U89] JS：数组去重
来源：http://wc.hnjuh.cn

[...new Set(arr)]
来源：http://jk.szsharing.cn

[U90] JS：数字数组排序
来源：http://ic.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://tn.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://vc.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zi.lnxyls.cn

[U92] JS：深拷贝
来源：http://er.hahajie.cn

structuredClone(obj)
来源：http://dh.shtwfgs.cn

[U93] JS：模板字符串
来源：http://kr.nszjky.cn

`共 ${n} 条`
来源：http://ca.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://om.nicolike.cn

const double = x => x * 2;
来源：http://gl.lnxyls.cn

[U95] JS：Promise 包装
来源：http://pm.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://sm.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://pe.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rm.haigaiapp.cn

[U97] JS：并发请求
来源：http://dz.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qf.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://wx.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ew.shxzukj.cn

[U99] JS：事件监听
来源：http://wf.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://md.newstarts.cn

[U100] JS：DOM 查询
来源：http://os.521024.cn

document.querySelector(".item")
来源：http://hq.panjiajie.cn

[U101] JS：classList 操作
来源：http://sa.yuexingan06.cn

el.classList.toggle("active")
来源：http://ak.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://cy.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gb.bookmarksfly.cn

[U103] JS：定时器
来源：http://tr.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vp.gzmigu.cn

[U104] JS：防抖
来源：http://iv.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kc.jctech888.com.cn

[U105] JS：节流
来源：http://xb.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://he.haigaiapp.cn

[U106] JS：日期格式化
来源：http://el.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kp.gzmigu.cn

[U107] JS：数字千分位
来源：http://pc.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hp.bjjhwx.cn

[U108] JS：随机整数
来源：http://yh.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pq.szxytkj.cn

[U109] JS：数组分组
来源：http://ht.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://pt.hahajie.cn

[U110] JS：数组分块
来源：http://qb.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://di.nicolike.cn

[U111] JS：对象转 Map
来源：http://ud.nicolike.cn

new Map(Object.entries(obj))
来源：http://np.521024.cn

[U112] JS：字符串补位
来源：http://hk.newstarts.cn

"7".padStart(3, "0")
来源：http://rj.huanxung.cn

[U113] JS：正则替换全部
来源：http://dz.521024.cn

s.replaceAll("a", "b")
来源：http://li.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://qn.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vc.huanxung.cn

[U115] JS：生成 UUID
来源：http://gz.colortex.cn

crypto.randomUUID()
来源：http://vo.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://fg.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://po.9csxet.cn

[U117] JS：单元测试
来源：http://ya.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://nf.9csxet.cn

[U118] JS：开发服务器
来源：http://ta.lnxyls.cn

npm i -D vite;  npx vite
来源：http://hf.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://wf.shxzskj.cn

npx vite build
来源：http://la.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://iz.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://pu.jianghongdianzi.cn

================================================================================
来源：http://jt.jctech888.com.cn

统计汇总
来源：http://lg.521024.cn

================================================================================
来源：http://bz.shxzskj.cn

按语言统计（条）：
来源：http://ww.szxytkj.cn

Python ......... 252
来源：http://zd.gzmigu.cn

PHP ............ 252
来源：http://vt.panjiajie.cn

JavaScript ..... 252
来源：http://an.newstarts.cn

TypeScript ..... 212
来源：http://nu.yuexingan06.cn

Java ........... 212
来源：http://fo.shxzukj.cn

Go ............. 212
来源：http://qf.bjjhwx.cn

Ruby ........... 212
来源：http://af.chemitech.net.cn

C# ............. 212
来源：http://ue.jctech888.com.cn

C .............. 30
来源：http://up.nicolike.cn

C++ ............ 30
来源：http://md.yuntaijiaju.cn

SQL ............ 90
来源：http://he.521024.cn

Bash ........... 80
来源：http://sw.yuexingan06.cn

Kotlin ......... 15
来源：http://hz.shtwfgs.cn

Swift .......... 15
来源：http://rz.huanxung.cn

Lua ............ 10
来源：http://yw.jianghongdianzi.cn

Perl ........... 10
来源：http://ru.shxzukj.cn

Scala .......... 10
来源：http://xf.yuntaijiaju.cn

------------------------------------
来源：http://pr.bookmarksfly.cn

合计 ........... 2106 条
来源：http://es.colortex.cn

按章节统计：
来源：http://da.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dd.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tq.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zo.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tf.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qp.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rn.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bh.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cs.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cg.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iy.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hd.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cx.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uh.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bg.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ot.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cm.521024.cn

Q SQL 专题                              90
来源：http://dr.asd995.cn

R Bash 专题                             80
来源：http://fp.shxzukj.cn

S C / C++ 专题                          60
来源：http://xv.panjiajie.cn

T 其他语言补充                          60
来源：http://zp.haigaiapp.cn

U 高频实用片段                         120
来源：http://xf.asd995.cn

------------------------------------
来源：http://on.lnxyls.cn

合计                                  2106 条
来源：http://ji.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://lz.newstarts.cn

使用提醒
来源：http://zs.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://kq.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://th.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bh.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rr.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kb.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://le.newstarts.cn

—— 文件结束 ——
来源：http://en.jianghongdianzi.cn

================================================================================
来源：http://ve.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://uk.colortex.cn

Common Programming Examples Cheat Book
来源：http://pu.huixinmuqiang.cn

================================================================================
来源：http://jp.nszjky.cn

【收录内容】
来源：http://yp.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sp.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bl.panjiajie.cn

SQL · Bash · C · C++
来源：http://ch.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gu.gzmigu.cn

【使用说明】
来源：http://im.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sf.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jx.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yg.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sn.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gi.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://km.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kg.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://at.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fa.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jl.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://os.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://op.colortex.cn

【文件统计】
来源：http://eo.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gc.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://yp.haigaiapp.cn

目  录
来源：http://rb.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://qv.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ai.muxihuayi.cn


<!-- 参考信息 -->