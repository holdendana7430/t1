代发 wailian999

[U13] Py：固定长度队列
来源：http://ib.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ml.nszjky.cn

[U14] Py：分组收集到列表
来源：http://ss.huixinmuqiang.cn

defaultdict(list)
来源：http://tp.wgjwhj.cn

[U15] Py：高精度计时
来源：http://st.hnjuh.cn

t = time.perf_counter()
来源：http://qs.asd995.cn

[U16] Py：命令行参数解析
来源：http://kq.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dx.haigaiapp.cn

[U17] Py：初始化日志
来源：http://kf.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://lr.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://nf.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://lc.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://jz.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vs.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://vf.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://zv.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://yh.haigaiapp.cn

@contextlib.contextmanager
来源：http://tj.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://jm.wgjwhj.cn

list(zip(*m))
来源：http://ji.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://is.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fq.huanxung.cn

[U24] Py：路径操作
来源：http://bc.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ak.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://je.hnjuh.cn

csv.DictReader(f)
来源：http://kw.yuexingan06.cn

[U26] Py：并发下载
来源：http://bt.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tt.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://sx.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://pw.bjjhwx.cn

[U28] Py：类型别名
来源：http://uc.hahajie.cn

UserId = int
来源：http://zx.shtwfgs.cn

[U29] Py：属性校验
来源：http://bl.lnxyls.cn

@property 与 @x.setter 配合
来源：http://ij.gzmigu.cn

[U30] Py：数据类
来源：http://sg.9csxet.cn

@dataclass(slots=True)
来源：http://ic.muxihuayi.cn

[U31] Py：单测
来源：http://fm.shtwfgs.cn

python -m pytest -q
来源：http://tr.newstarts.cn

[U32] Py：代码格式化
来源：http://us.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://lc.hnjuh.cn

[U33] Py：打包发布
来源：http://mj.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://il.hahajie.cn

[U34] Py：判断编码
来源：http://qk.panjiajie.cn

chardet.detect(raw)
来源：http://bt.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://qs.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bx.nicolike.cn

[U36] Py：定时任务
来源：http://yp.521024.cn

schedule.every(10).minutes.do(job)
来源：http://vg.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://jw.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ss.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://xe.hahajie.cn

Path(__file__).resolve().parent
来源：http://fl.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://xl.yuexingan06.cn

sys.stdout.isatty()
来源：http://fq.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://ku.shxzukj.cn

print("err", file=sys.stderr)
来源：http://qk.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://fr.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://de.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ar.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bq.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://hy.muxihuayi.cn

namespace App\Http;
来源：http://ia.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://bz.shxzskj.cn

declare(strict_types=1);
来源：http://un.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://mi.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jr.newstarts.cn

[U46] PHP：可空类型
来源：http://um.nicolike.cn

?string $name = null
来源：http://ok.nszjky.cn

[U47] PHP：联合类型
来源：http://ym.muxihuayi.cn

int|string $id
来源：http://zu.nszjky.cn

[U48] PHP：纯枚举
来源：http://bc.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aw.muxihuayi.cn

[U49] PHP：只读属性
来源：http://ws.huixiangedu.cn

public readonly string $name
来源：http://ic.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://hz.gzmigu.cn

public function __construct(private int $id) {}
来源：http://xz.nicolike.cn

[U51] PHP：数组解构
来源：http://kp.nszjky.cn

[$a, $b] = $arr;
来源：http://ec.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://ld.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://vh.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ib.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://bn.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://wu.panjiajie.cn

$obj?->method()
来源：http://uq.colortex.cn

[U55] PHP：match 表达式
来源：http://be.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ge.newstarts.cn

[U56] PHP：命名参数
来源：http://mv.szsharing.cn

f(a: 1, b: 2)
来源：http://tr.newstarts.cn

[U57] PHP：字符串插值
来源：http://fg.hnjuh.cn

"值: {$a}"
来源：http://gf.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://vt.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xi.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://oy.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bu.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://do.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://da.gzmigu.cn

[U61] PHP：正则
来源：http://cv.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rw.huanxung.cn

[U62] PHP：日期对象
来源：http://om.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kh.haigaiapp.cn

[U63] PHP：文件读写
来源：http://bt.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ds.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://dj.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://un.shxzskj.cn

[U65] PHP：会话
来源：http://nf.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lk.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://ty.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ek.colortex.cn

[U67] PHP：处理文件上传
来源：http://dv.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lu.9csxet.cn

[U68] PHP：PDO 连接
来源：http://zb.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://im.colortex.cn

[U69] PHP：PDO 预处理
来源：http://jj.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hg.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://pu.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aj.panjiajie.cn

[U71] PHP：抛出异常
来源：http://ae.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ee.gzmigu.cn

[U72] PHP：写错误日志
来源：http://qo.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://xb.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://te.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://jy.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://de.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://ir.colortex.cn

[U75] PHP：依赖注入
来源：http://mn.panjiajie.cn

composer require psr/container
来源：http://hc.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://ld.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ji.szsharing.cn

[U77] PHP：模板渲染
来源：http://uy.wgjwhj.cn

composer require twig/twig
来源：http://hn.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://ev.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://pb.muxihuayi.cn

[U79] PHP：静态分析
来源：http://te.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://hu.newstarts.cn

[U80] PHP：代码规范修复
来源：http://zh.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xz.haigaiapp.cn

[U81] JS：初始化项目
来源：http://df.9csxet.cn

npm init -y;  npm i express
来源：http://td.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://cp.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pq.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://fx.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aj.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://cq.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rf.huanxung.cn

[U85] JS：可选链
来源：http://ex.asd995.cn

a?.b?.c
来源：http://oh.nicolike.cn

[U86] JS：空值合并
来源：http://iz.yuexingan06.cn

a ?? b
来源：http://tz.shtwfgs.cn

[U87] JS：解构默认值
来源：http://gy.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://ae.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://dn.jctech888.com.cn

{ ...a, ...b }
来源：http://vb.shxzskj.cn

[U89] JS：数组去重
来源：http://ys.nicolike.cn

[...new Set(arr)]
来源：http://pl.szsharing.cn

[U90] JS：数字数组排序
来源：http://bd.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://ns.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://xa.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lg.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://uq.yuntaijiaju.cn

structuredClone(obj)
来源：http://zs.hahajie.cn

[U93] JS：模板字符串
来源：http://dj.asd995.cn

`共 ${n} 条`
来源：http://aj.huixiangedu.cn

[U94] JS：箭头函数
来源：http://de.asd995.cn

const double = x => x * 2;
来源：http://qh.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://gg.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://wd.huanxung.cn

[U96] JS：async/await 与异常
来源：http://un.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rg.szsharing.cn

[U97] JS：并发请求
来源：http://na.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://la.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://bi.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vi.szxytkj.cn

[U99] JS：事件监听
来源：http://np.nicolike.cn

el.addEventListener("click", e => {})
来源：http://gb.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://qd.shxzukj.cn

document.querySelector(".item")
来源：http://ug.colortex.cn

[U101] JS：classList 操作
来源：http://uo.lnxyls.cn

el.classList.toggle("active")
来源：http://bk.nicolike.cn

[U102] JS：本地存储
来源：http://cp.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://my.yuexingan06.cn

[U103] JS：定时器
来源：http://jf.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cu.jianghongdianzi.cn

[U104] JS：防抖
来源：http://lt.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gs.wgjwhj.cn

[U105] JS：节流
来源：http://az.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dr.nszjky.cn

[U106] JS：日期格式化
来源：http://tx.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bo.shtwfgs.cn

[U107] JS：数字千分位
来源：http://rc.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uv.huixiangedu.cn

[U108] JS：随机整数
来源：http://bp.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bw.wgjwhj.cn

[U109] JS：数组分组
来源：http://py.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://ze.yuexingan06.cn

[U110] JS：数组分块
来源：http://bd.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://si.9csxet.cn

[U111] JS：对象转 Map
来源：http://rd.gzmigu.cn

new Map(Object.entries(obj))
来源：http://bk.muxihuayi.cn

[U112] JS：字符串补位
来源：http://hp.hahajie.cn

"7".padStart(3, "0")
来源：http://xl.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://mn.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://yo.hahajie.cn

[U114] JS：JSON 深比较
来源：http://ok.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://an.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://he.newstarts.cn

crypto.randomUUID()
来源：http://er.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tg.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://ug.szsharing.cn

[U117] JS：单元测试
来源：http://le.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://lr.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://lh.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://of.shtwfgs.cn

[U119] JS：生产构建
来源：http://xe.haigaiapp.cn

npx vite build
来源：http://oj.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://xe.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://jl.colortex.cn

================================================================================
来源：http://yv.hnjuh.cn

统计汇总
来源：http://lk.panjiajie.cn

================================================================================
来源：http://fy.colortex.cn

按语言统计（条）：
来源：http://gj.gzmigu.cn

Python ......... 252
来源：http://hi.chemitech.net.cn

PHP ............ 252
来源：http://du.bjjhwx.cn

JavaScript ..... 252
来源：http://hw.muxihuayi.cn

TypeScript ..... 212
来源：http://yy.shtwfgs.cn

Java ........... 212
来源：http://jt.bjjhwx.cn

Go ............. 212
来源：http://vo.hnjuh.cn

Ruby ........... 212
来源：http://ir.wgjwhj.cn

C# ............. 212
来源：http://jw.haigaiapp.cn

C .............. 30
来源：http://iz.haigaiapp.cn

C++ ............ 30
来源：http://yf.haigaiapp.cn

SQL ............ 90
来源：http://el.shxzskj.cn

Bash ........... 80
来源：http://vc.newstarts.cn

Kotlin ......... 15
来源：http://he.chemitech.net.cn

Swift .......... 15
来源：http://ne.wgjwhj.cn

Lua ............ 10
来源：http://vj.szsharing.cn

Perl ........... 10
来源：http://qj.asd995.cn

Scala .......... 10
来源：http://el.gzmigu.cn

------------------------------------
来源：http://xf.nszjky.cn

合计 ........... 2106 条
来源：http://jz.jctech888.com.cn

按章节统计：
来源：http://wp.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://su.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nr.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wv.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ar.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://to.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sv.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jy.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rf.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wu.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yz.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hw.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qv.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gm.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bd.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ls.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://re.9csxet.cn

Q SQL 专题                              90
来源：http://uf.huixiangedu.cn

R Bash 专题                             80
来源：http://si.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://qf.colortex.cn

T 其他语言补充                          60
来源：http://vc.shxzukj.cn

U 高频实用片段                         120
来源：http://ak.shxzukj.cn

------------------------------------
来源：http://vv.szxytkj.cn

合计                                  2106 条
来源：http://xi.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://mh.hnjuh.cn

使用提醒
来源：http://nz.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ac.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mp.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xs.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pq.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pj.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bk.szsharing.cn

—— 文件结束 ——
来源：http://eh.huanxung.cn

================================================================================
来源：http://jf.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://lk.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://so.shxzukj.cn

================================================================================
来源：http://fi.9csxet.cn

【收录内容】
来源：http://um.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rl.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xa.shtwfgs.cn

SQL · Bash · C · C++
来源：http://av.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cw.szxytkj.cn

【使用说明】
来源：http://ka.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nu.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fn.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mi.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sf.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ry.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tk.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lh.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bj.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oo.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bg.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xp.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uu.nicolike.cn

【文件统计】
来源：http://ch.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mq.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://xa.521024.cn

目  录
来源：http://bc.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://im.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uf.hnjuh.cn


<!-- 参考信息 -->