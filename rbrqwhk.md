代发 wailian999

[U15] Py：高精度计时
来源：http://mh.lnxyls.cn

t = time.perf_counter()
来源：http://kq.nicolike.cn

[U16] Py：命令行参数解析
来源：http://fw.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gf.hnjuh.cn

[U17] Py：初始化日志
来源：http://il.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://wt.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://yp.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://hu.nszjky.cn

[U19] Py：正则替换带回调
来源：http://kz.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ly.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://lq.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://me.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://ow.shxzskj.cn

@contextlib.contextmanager
来源：http://cu.panjiajie.cn

[U22] Py：矩阵转置
来源：http://xt.colortex.cn

list(zip(*m))
来源：http://gf.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://pg.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dt.huixiangedu.cn

[U24] Py：路径操作
来源：http://qt.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kd.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://kj.shxzskj.cn

csv.DictReader(f)
来源：http://jm.bookmarksfly.cn

[U26] Py：并发下载
来源：http://vk.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ne.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://nl.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://wc.bjjhwx.cn

[U28] Py：类型别名
来源：http://vm.lnxyls.cn

UserId = int
来源：http://fu.yuexingan06.cn

[U29] Py：属性校验
来源：http://mb.asd995.cn

@property 与 @x.setter 配合
来源：http://jc.shtwfgs.cn

[U30] Py：数据类
来源：http://xy.9csxet.cn

@dataclass(slots=True)
来源：http://ev.panjiajie.cn

[U31] Py：单测
来源：http://os.muxihuayi.cn

python -m pytest -q
来源：http://ez.huanxung.cn

[U32] Py：代码格式化
来源：http://xr.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://zz.shxzskj.cn

[U33] Py：打包发布
来源：http://sz.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://hl.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://vm.huixinmuqiang.cn

chardet.detect(raw)
来源：http://lu.shxzukj.cn

[U35] Py：发送邮件
来源：http://yq.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://as.huixiangedu.cn

[U36] Py：定时任务
来源：http://te.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://xn.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://wj.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eu.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://mj.shxzukj.cn

Path(__file__).resolve().parent
来源：http://rp.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://iy.newstarts.cn

sys.stdout.isatty()
来源：http://xq.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://cs.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://we.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://tx.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sd.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://vz.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nd.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://nr.hnjuh.cn

namespace App\Http;
来源：http://gt.9csxet.cn

[U44] PHP：开启严格类型
来源：http://sa.nszjky.cn

declare(strict_types=1);
来源：http://kv.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ic.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sc.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://ne.lnxyls.cn

?string $name = null
来源：http://ud.shtwfgs.cn

[U47] PHP：联合类型
来源：http://lf.wgjwhj.cn

int|string $id
来源：http://gg.colortex.cn

[U48] PHP：纯枚举
来源：http://ly.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://op.bjjhwx.cn

[U49] PHP：只读属性
来源：http://pi.lnxyls.cn

public readonly string $name
来源：http://eg.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://ft.lnxyls.cn

public function __construct(private int $id) {}
来源：http://tg.nicolike.cn

[U51] PHP：数组解构
来源：http://ej.jctech888.com.cn

[$a, $b] = $arr;
来源：http://am.gzmigu.cn

[U52] PHP：箭头函数
来源：http://nd.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://ub.newstarts.cn

[U53] PHP：空合并运算符
来源：http://uu.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://qx.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://tf.bjjhwx.cn

$obj?->method()
来源：http://bz.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://eu.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://we.panjiajie.cn

[U56] PHP：命名参数
来源：http://cw.chemitech.net.cn

f(a: 1, b: 2)
来源：http://lb.521024.cn

[U57] PHP：字符串插值
来源：http://vy.wgjwhj.cn

"值: {$a}"
来源：http://da.shxzskj.cn

[U58] PHP：数组三件套
来源：http://ma.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ze.lnxyls.cn

[U59] PHP：自定义排序
来源：http://va.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ov.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://yf.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ik.bjjhwx.cn

[U61] PHP：正则
来源：http://ar.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yu.nicolike.cn

[U62] PHP：日期对象
来源：http://at.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pd.chemitech.net.cn

[U63] PHP：文件读写
来源：http://do.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ps.nicolike.cn

[U64] PHP：目录遍历
来源：http://mz.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://gf.haigaiapp.cn

[U65] PHP：会话
来源：http://bg.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uv.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://lu.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sq.521024.cn

[U67] PHP：处理文件上传
来源：http://yw.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ii.huanxung.cn

[U68] PHP：PDO 连接
来源：http://ox.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vt.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://cl.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ck.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://of.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aq.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://az.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ae.hahajie.cn

[U72] PHP：写错误日志
来源：http://xu.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://cp.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://oe.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://jo.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://ob.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://up.szxytkj.cn

[U75] PHP：依赖注入
来源：http://se.newstarts.cn

composer require psr/container
来源：http://bn.hahajie.cn

[U76] PHP：简单路由
来源：http://uf.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fb.9csxet.cn

[U77] PHP：模板渲染
来源：http://ld.bookmarksfly.cn

composer require twig/twig
来源：http://lp.huanxung.cn

[U78] PHP：单元测试
来源：http://du.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://sc.szxytkj.cn

[U79] PHP：静态分析
来源：http://un.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://nx.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://on.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dv.szxytkj.cn

[U81] JS：初始化项目
来源：http://mx.nszjky.cn

npm init -y;  npm i express
来源：http://ux.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://ob.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hv.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://su.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://di.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://tt.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ax.huanxung.cn

[U85] JS：可选链
来源：http://jv.colortex.cn

a?.b?.c
来源：http://nq.chemitech.net.cn

[U86] JS：空值合并
来源：http://mx.shtwfgs.cn

a ?? b
来源：http://tn.shxzukj.cn

[U87] JS：解构默认值
来源：http://cv.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://ik.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://iw.521024.cn

{ ...a, ...b }
来源：http://hx.shtwfgs.cn

[U89] JS：数组去重
来源：http://qi.nszjky.cn

[...new Set(arr)]
来源：http://mf.shxzukj.cn

[U90] JS：数字数组排序
来源：http://cr.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://pd.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://oy.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oz.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://mi.shxzukj.cn

structuredClone(obj)
来源：http://or.bjjhwx.cn

[U93] JS：模板字符串
来源：http://vf.shxzskj.cn

`共 ${n} 条`
来源：http://yh.muxihuayi.cn

[U94] JS：箭头函数
来源：http://nw.muxihuayi.cn

const double = x => x * 2;
来源：http://hb.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://st.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://eh.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://lc.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hq.chemitech.net.cn

[U97] JS：并发请求
来源：http://wi.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eu.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://le.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ep.hahajie.cn

[U99] JS：事件监听
来源：http://kc.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://eo.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://vu.chemitech.net.cn

document.querySelector(".item")
来源：http://pv.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://lb.panjiajie.cn

el.classList.toggle("active")
来源：http://ie.shtwfgs.cn

[U102] JS：本地存储
来源：http://oh.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vg.shxzukj.cn

[U103] JS：定时器
来源：http://qh.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yb.jctech888.com.cn

[U104] JS：防抖
来源：http://ms.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mf.yuntaijiaju.cn

[U105] JS：节流
来源：http://cx.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dh.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://ji.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xt.9csxet.cn

[U107] JS：数字千分位
来源：http://cn.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mk.yuexingan06.cn

[U108] JS：随机整数
来源：http://oe.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ih.shxzskj.cn

[U109] JS：数组分组
来源：http://ht.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://ds.jctech888.com.cn

[U110] JS：数组分块
来源：http://ee.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pe.lnxyls.cn

[U111] JS：对象转 Map
来源：http://gt.colortex.cn

new Map(Object.entries(obj))
来源：http://ew.521024.cn

[U112] JS：字符串补位
来源：http://vo.huanxung.cn

"7".padStart(3, "0")
来源：http://xy.gzmigu.cn

[U113] JS：正则替换全部
来源：http://pd.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://oh.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://lw.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vn.shxzskj.cn

[U115] JS：生成 UUID
来源：http://zr.shtwfgs.cn

crypto.randomUUID()
来源：http://dn.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ug.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://mi.jctech888.com.cn

[U117] JS：单元测试
来源：http://tg.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://vy.yuexingan06.cn

[U118] JS：开发服务器
来源：http://vi.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://wn.nicolike.cn

[U119] JS：生产构建
来源：http://iw.szsharing.cn

npx vite build
来源：http://jc.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://fy.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://fd.9csxet.cn

================================================================================
来源：http://wm.hnjuh.cn

统计汇总
来源：http://wo.521024.cn

================================================================================
来源：http://bk.haigaiapp.cn

按语言统计（条）：
来源：http://ro.nicolike.cn

Python ......... 252
来源：http://oi.shtwfgs.cn

PHP ............ 252
来源：http://zn.bookmarksfly.cn

JavaScript ..... 252
来源：http://vb.newstarts.cn

TypeScript ..... 212
来源：http://sz.jianghongdianzi.cn

Java ........... 212
来源：http://an.huixiangedu.cn

Go ............. 212
来源：http://tl.hahajie.cn

Ruby ........... 212
来源：http://eh.shtwfgs.cn

C# ............. 212
来源：http://hj.muxihuayi.cn

C .............. 30
来源：http://vy.huixinmuqiang.cn

C++ ............ 30
来源：http://wd.gzmigu.cn

SQL ............ 90
来源：http://ib.huanxung.cn

Bash ........... 80
来源：http://nk.lnxyls.cn

Kotlin ......... 15
来源：http://ta.yuexingan06.cn

Swift .......... 15
来源：http://cm.szxytkj.cn

Lua ............ 10
来源：http://qo.hnjuh.cn

Perl ........... 10
来源：http://ul.bookmarksfly.cn

Scala .......... 10
来源：http://sh.jctech888.com.cn

------------------------------------
来源：http://gj.huixiangedu.cn

合计 ........... 2106 条
来源：http://qe.chemitech.net.cn

按章节统计：
来源：http://kj.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ys.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kc.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vi.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pf.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dh.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ln.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sz.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wl.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rp.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pb.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dj.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wp.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lf.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kt.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pq.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qf.huanxung.cn

Q SQL 专题                              90
来源：http://pu.wgjwhj.cn

R Bash 专题                             80
来源：http://wp.muxihuayi.cn

S C / C++ 专题                          60
来源：http://kt.shtwfgs.cn

T 其他语言补充                          60
来源：http://zj.hnjuh.cn

U 高频实用片段                         120
来源：http://vz.bookmarksfly.cn

------------------------------------
来源：http://aa.hahajie.cn

合计                                  2106 条
来源：http://ya.asd995.cn

--------------------------------------------------------------------------------
来源：http://nb.szsharing.cn

使用提醒
来源：http://kb.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://qu.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sl.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cc.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sw.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wb.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://af.huanxung.cn

—— 文件结束 ——
来源：http://yb.bjjhwx.cn

================================================================================
来源：http://mq.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ak.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://jp.newstarts.cn

================================================================================
来源：http://qf.nicolike.cn

【收录内容】
来源：http://ha.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://he.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://py.jctech888.com.cn

SQL · Bash · C · C++
来源：http://yr.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://np.huixinmuqiang.cn

【使用说明】
来源：http://ui.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ty.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lb.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xd.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ss.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fz.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://re.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nq.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pk.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tk.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wn.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pm.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uy.9csxet.cn

【文件统计】
来源：http://jm.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zj.asd995.cn

--------------------------------------------------------------------------------
来源：http://ds.lnxyls.cn

目  录
来源：http://wd.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://wa.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dy.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://os.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ez.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mn.hahajie.cn


<!-- 参考信息 -->