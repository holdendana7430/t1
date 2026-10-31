代发 wailian999

[U11] Py：生成器表达式
来源：http://rl.shxzukj.cn

(x * 2 for x in arr)
来源：http://cs.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gr.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://uo.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://ij.asd995.cn

deque(maxlen=10)
来源：http://co.newstarts.cn

[U14] Py：分组收集到列表
来源：http://da.szxytkj.cn

defaultdict(list)
来源：http://jx.shtwfgs.cn

[U15] Py：高精度计时
来源：http://mc.hnjuh.cn

t = time.perf_counter()
来源：http://qh.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ur.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ly.muxihuayi.cn

[U17] Py：初始化日志
来源：http://fz.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ka.lnxyls.cn

[U18] Py：预编译正则
来源：http://qs.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://qf.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://eg.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rt.hahajie.cn

[U20] Py：缓存函数结果
来源：http://gs.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://bd.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://ne.bjjhwx.cn

@contextlib.contextmanager
来源：http://fu.panjiajie.cn

[U22] Py：矩阵转置
来源：http://fe.521024.cn

list(zip(*m))
来源：http://ht.521024.cn

[U23] Py：分块读取大文件
来源：http://ck.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ef.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://ve.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uh.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://uf.colortex.cn

csv.DictReader(f)
来源：http://ql.szxytkj.cn

[U26] Py：并发下载
来源：http://nx.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lt.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://qj.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ja.colortex.cn

[U28] Py：类型别名
来源：http://rd.gzmigu.cn

UserId = int
来源：http://wb.huanxung.cn

[U29] Py：属性校验
来源：http://gc.shxzskj.cn

@property 与 @x.setter 配合
来源：http://li.gzmigu.cn

[U30] Py：数据类
来源：http://fo.nicolike.cn

@dataclass(slots=True)
来源：http://fo.jctech888.com.cn

[U31] Py：单测
来源：http://tc.yuntaijiaju.cn

python -m pytest -q
来源：http://cs.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://my.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://sk.shxzukj.cn

[U33] Py：打包发布
来源：http://oc.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://cm.lnxyls.cn

[U34] Py：判断编码
来源：http://kn.hnjuh.cn

chardet.detect(raw)
来源：http://do.huixiangedu.cn

[U35] Py：发送邮件
来源：http://re.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kv.muxihuayi.cn

[U36] Py：定时任务
来源：http://qf.521024.cn

schedule.every(10).minutes.do(job)
来源：http://qn.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://wu.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bl.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://ze.lnxyls.cn

Path(__file__).resolve().parent
来源：http://xo.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://vk.szsharing.cn

sys.stdout.isatty()
来源：http://eg.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://zf.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://ca.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://cm.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xg.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://pc.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xn.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://ul.colortex.cn

namespace App\Http;
来源：http://bk.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://xe.asd995.cn

declare(strict_types=1);
来源：http://uq.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://zj.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lw.yuexingan06.cn

[U46] PHP：可空类型
来源：http://zb.521024.cn

?string $name = null
来源：http://rk.hahajie.cn

[U47] PHP：联合类型
来源：http://zc.newstarts.cn

int|string $id
来源：http://ef.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://nn.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zi.wgjwhj.cn

[U49] PHP：只读属性
来源：http://pm.huixinmuqiang.cn

public readonly string $name
来源：http://om.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://hk.gzmigu.cn

public function __construct(private int $id) {}
来源：http://vg.gzmigu.cn

[U51] PHP：数组解构
来源：http://ob.shxzukj.cn

[$a, $b] = $arr;
来源：http://kh.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://ui.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://rb.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://fv.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://yt.lnxyls.cn

[U54] PHP：空安全调用
来源：http://ka.szxytkj.cn

$obj?->method()
来源：http://yj.huanxung.cn

[U55] PHP：match 表达式
来源：http://pp.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fa.jctech888.com.cn

[U56] PHP：命名参数
来源：http://gv.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://ix.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://xk.521024.cn

"值: {$a}"
来源：http://os.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://of.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uc.szxytkj.cn

[U59] PHP：自定义排序
来源：http://av.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jm.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://oe.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mg.lnxyls.cn

[U61] PHP：正则
来源：http://qy.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qr.gzmigu.cn

[U62] PHP：日期对象
来源：http://qt.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zm.colortex.cn

[U63] PHP：文件读写
来源：http://cw.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pn.nszjky.cn

[U64] PHP：目录遍历
来源：http://ng.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://or.nicolike.cn

[U65] PHP：会话
来源：http://ey.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ye.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://ya.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dj.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://he.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yw.nszjky.cn

[U68] PHP：PDO 连接
来源：http://au.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mh.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://we.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gs.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://tf.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xj.nszjky.cn

[U71] PHP：抛出异常
来源：http://da.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://xo.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://pp.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://ou.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://pd.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://qh.9csxet.cn

[U74] PHP：读取环境变量
来源：http://rg.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://ts.panjiajie.cn

[U75] PHP：依赖注入
来源：http://uq.szxytkj.cn

composer require psr/container
来源：http://qm.szxytkj.cn

[U76] PHP：简单路由
来源：http://te.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rf.panjiajie.cn

[U77] PHP：模板渲染
来源：http://fd.newstarts.cn

composer require twig/twig
来源：http://cd.hnjuh.cn

[U78] PHP：单元测试
来源：http://mh.asd995.cn

composer require --dev phpunit/phpunit
来源：http://vv.newstarts.cn

[U79] PHP：静态分析
来源：http://ml.asd995.cn

composer require --dev phpstan/phpstan
来源：http://rb.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://ir.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jq.szsharing.cn

[U81] JS：初始化项目
来源：http://za.wgjwhj.cn

npm init -y;  npm i express
来源：http://da.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://kc.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://st.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://it.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cu.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://wx.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hv.colortex.cn

[U85] JS：可选链
来源：http://vx.gzmigu.cn

a?.b?.c
来源：http://dt.lnxyls.cn

[U86] JS：空值合并
来源：http://ce.jianghongdianzi.cn

a ?? b
来源：http://cv.jctech888.com.cn

[U87] JS：解构默认值
来源：http://cm.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://ua.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://df.gzmigu.cn

{ ...a, ...b }
来源：http://hd.nszjky.cn

[U89] JS：数组去重
来源：http://zi.newstarts.cn

[...new Set(arr)]
来源：http://xf.521024.cn

[U90] JS：数字数组排序
来源：http://zb.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://yd.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://fx.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bw.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://so.gzmigu.cn

structuredClone(obj)
来源：http://dh.hnjuh.cn

[U93] JS：模板字符串
来源：http://dc.huixinmuqiang.cn

`共 ${n} 条`
来源：http://sc.521024.cn

[U94] JS：箭头函数
来源：http://tm.yuexingan06.cn

const double = x => x * 2;
来源：http://xj.szsharing.cn

[U95] JS：Promise 包装
来源：http://nw.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://vl.nicolike.cn

[U96] JS：async/await 与异常
来源：http://cc.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lx.panjiajie.cn

[U97] JS：并发请求
来源：http://dp.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uw.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://wv.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vb.9csxet.cn

[U99] JS：事件监听
来源：http://rw.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://mz.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://fs.lnxyls.cn

document.querySelector(".item")
来源：http://rl.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://hz.yuexingan06.cn

el.classList.toggle("active")
来源：http://vf.colortex.cn

[U102] JS：本地存储
来源：http://bd.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kw.gzmigu.cn

[U103] JS：定时器
来源：http://nd.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sc.gzmigu.cn

[U104] JS：防抖
来源：http://dv.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cq.521024.cn

[U105] JS：节流
来源：http://rr.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zc.szsharing.cn

[U106] JS：日期格式化
来源：http://zy.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nw.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://it.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qv.shxzukj.cn

[U108] JS：随机整数
来源：http://hi.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ns.chemitech.net.cn

[U109] JS：数组分组
来源：http://en.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://hb.szsharing.cn

[U110] JS：数组分块
来源：http://of.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lg.hahajie.cn

[U111] JS：对象转 Map
来源：http://ke.lnxyls.cn

new Map(Object.entries(obj))
来源：http://ap.haigaiapp.cn

[U112] JS：字符串补位
来源：http://cv.shxzskj.cn

"7".padStart(3, "0")
来源：http://hr.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://hw.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://ty.colortex.cn

[U114] JS：JSON 深比较
来源：http://ld.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ww.gzmigu.cn

[U115] JS：生成 UUID
来源：http://an.hnjuh.cn

crypto.randomUUID()
来源：http://mc.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://fw.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://fx.hnjuh.cn

[U117] JS：单元测试
来源：http://yp.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://zk.shxzskj.cn

[U118] JS：开发服务器
来源：http://yn.asd995.cn

npm i -D vite;  npx vite
来源：http://lu.asd995.cn

[U119] JS：生产构建
来源：http://xc.yuntaijiaju.cn

npx vite build
来源：http://ca.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://hg.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://il.bjjhwx.cn

================================================================================
来源：http://rl.huixiangedu.cn

统计汇总
来源：http://li.colortex.cn

================================================================================
来源：http://ft.jctech888.com.cn

按语言统计（条）：
来源：http://ab.yuexingan06.cn

Python ......... 252
来源：http://mc.asd995.cn

PHP ............ 252
来源：http://pw.haigaiapp.cn

JavaScript ..... 252
来源：http://hh.shxzukj.cn

TypeScript ..... 212
来源：http://zl.yuexingan06.cn

Java ........... 212
来源：http://si.haigaiapp.cn

Go ............. 212
来源：http://eq.szsharing.cn

Ruby ........... 212
来源：http://pe.panjiajie.cn

C# ............. 212
来源：http://xz.huixinmuqiang.cn

C .............. 30
来源：http://wh.muxihuayi.cn

C++ ............ 30
来源：http://ds.haigaiapp.cn

SQL ............ 90
来源：http://gy.haigaiapp.cn

Bash ........... 80
来源：http://ob.bookmarksfly.cn

Kotlin ......... 15
来源：http://vq.szxytkj.cn

Swift .......... 15
来源：http://gr.yuntaijiaju.cn

Lua ............ 10
来源：http://el.9csxet.cn

Perl ........... 10
来源：http://hd.shtwfgs.cn

Scala .......... 10
来源：http://sc.newstarts.cn

------------------------------------
来源：http://gj.521024.cn

合计 ........... 2106 条
来源：http://rt.nszjky.cn

按章节统计：
来源：http://io.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ds.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ma.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qs.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nw.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pd.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://px.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zk.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vz.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mu.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hs.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mz.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pn.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ev.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sx.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mp.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mp.shtwfgs.cn

Q SQL 专题                              90
来源：http://gp.shxzukj.cn

R Bash 专题                             80
来源：http://cu.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://mw.nicolike.cn

T 其他语言补充                          60
来源：http://gw.hnjuh.cn

U 高频实用片段                         120
来源：http://uc.panjiajie.cn

------------------------------------
来源：http://hx.jctech888.com.cn

合计                                  2106 条
来源：http://nk.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ia.asd995.cn

使用提醒
来源：http://cd.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://dw.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kp.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zi.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kv.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oa.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yu.asd995.cn

—— 文件结束 ——
来源：http://py.muxihuayi.cn

================================================================================
来源：http://md.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://fp.nszjky.cn

Common Programming Examples Cheat Book
来源：http://nd.asd995.cn

================================================================================
来源：http://am.9csxet.cn

【收录内容】
来源：http://nr.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ks.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jm.panjiajie.cn

SQL · Bash · C · C++
来源：http://ac.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wz.panjiajie.cn

【使用说明】
来源：http://jp.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sl.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xj.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ze.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gm.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fr.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cw.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gz.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ta.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dv.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ry.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xr.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xr.gzmigu.cn

【文件统计】
来源：http://ji.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://re.newstarts.cn


<!-- 参考信息 -->