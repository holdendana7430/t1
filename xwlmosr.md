代发 wailian999

[U07] Py：反转字典键值
来源：http://fk.szsharing.cn

{v: k for k, v in d.items()}
来源：http://am.asd995.cn

[U08] Py：展平二维列表
来源：http://rd.nicolike.cn

[y for x in nested for y in x]
来源：http://ed.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://rp.9csxet.cn

max(d, key=d.get)
来源：http://ua.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://ys.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qz.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://tl.hahajie.cn

(x * 2 for x in arr)
来源：http://pb.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ky.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://uo.newstarts.cn

[U13] Py：固定长度队列
来源：http://sy.shxzukj.cn

deque(maxlen=10)
来源：http://bm.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://km.hnjuh.cn

defaultdict(list)
来源：http://ma.asd995.cn

[U15] Py：高精度计时
来源：http://fz.hahajie.cn

t = time.perf_counter()
来源：http://nz.521024.cn

[U16] Py：命令行参数解析
来源：http://ee.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gz.hnjuh.cn

[U17] Py：初始化日志
来源：http://gt.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ek.gzmigu.cn

[U18] Py：预编译正则
来源：http://cy.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://al.9csxet.cn

[U19] Py：正则替换带回调
来源：http://ci.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rb.colortex.cn

[U20] Py：缓存函数结果
来源：http://gd.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://eg.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://fw.gzmigu.cn

@contextlib.contextmanager
来源：http://zt.nicolike.cn

[U22] Py：矩阵转置
来源：http://eg.huixiangedu.cn

list(zip(*m))
来源：http://dw.hahajie.cn

[U23] Py：分块读取大文件
来源：http://np.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jq.panjiajie.cn

[U24] Py：路径操作
来源：http://wm.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ug.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://hv.wgjwhj.cn

csv.DictReader(f)
来源：http://ki.9csxet.cn

[U26] Py：并发下载
来源：http://ix.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xf.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://ff.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://kg.newstarts.cn

[U28] Py：类型别名
来源：http://df.yuntaijiaju.cn

UserId = int
来源：http://gz.521024.cn

[U29] Py：属性校验
来源：http://dr.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://su.lnxyls.cn

[U30] Py：数据类
来源：http://eb.huanxung.cn

@dataclass(slots=True)
来源：http://ku.521024.cn

[U31] Py：单测
来源：http://zj.shxzskj.cn

python -m pytest -q
来源：http://ly.lnxyls.cn

[U32] Py：代码格式化
来源：http://rx.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://dl.lnxyls.cn

[U33] Py：打包发布
来源：http://xz.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://mw.bjjhwx.cn

[U34] Py：判断编码
来源：http://gr.newstarts.cn

chardet.detect(raw)
来源：http://kt.nicolike.cn

[U35] Py：发送邮件
来源：http://wj.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ig.muxihuayi.cn

[U36] Py：定时任务
来源：http://et.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://rv.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://od.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ny.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://aq.hahajie.cn

Path(__file__).resolve().parent
来源：http://gn.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://gs.nicolike.cn

sys.stdout.isatty()
来源：http://wq.nicolike.cn

[U40] Py：打印到标准错误
来源：http://xo.szxytkj.cn

print("err", file=sys.stderr)
来源：http://ik.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://yl.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://up.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://jd.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ty.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://zj.521024.cn

namespace App\Http;
来源：http://zq.huanxung.cn

[U44] PHP：开启严格类型
来源：http://se.hnjuh.cn

declare(strict_types=1);
来源：http://df.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://qy.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ye.wgjwhj.cn

[U46] PHP：可空类型
来源：http://kq.asd995.cn

?string $name = null
来源：http://yp.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://dt.hnjuh.cn

int|string $id
来源：http://ib.hahajie.cn

[U48] PHP：纯枚举
来源：http://wo.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://do.colortex.cn

[U49] PHP：只读属性
来源：http://ox.muxihuayi.cn

public readonly string $name
来源：http://nw.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://an.hahajie.cn

public function __construct(private int $id) {}
来源：http://bq.newstarts.cn

[U51] PHP：数组解构
来源：http://pe.wgjwhj.cn

[$a, $b] = $arr;
来源：http://gs.hahajie.cn

[U52] PHP：箭头函数
来源：http://lr.colortex.cn

$double = fn($x) => $x * 2;
来源：http://mv.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://ql.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://oz.shxzskj.cn

[U54] PHP：空安全调用
来源：http://fi.nszjky.cn

$obj?->method()
来源：http://oq.asd995.cn

[U55] PHP：match 表达式
来源：http://nm.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gs.huixiangedu.cn

[U56] PHP：命名参数
来源：http://jd.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://mg.colortex.cn

[U57] PHP：字符串插值
来源：http://rr.jctech888.com.cn

"值: {$a}"
来源：http://id.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ke.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://je.newstarts.cn

[U59] PHP：自定义排序
来源：http://ah.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uq.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://oy.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zu.hnjuh.cn

[U61] PHP：正则
来源：http://rv.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wa.shxzukj.cn

[U62] PHP：日期对象
来源：http://ia.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zy.panjiajie.cn

[U63] PHP：文件读写
来源：http://gh.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zy.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://om.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://us.shtwfgs.cn

[U65] PHP：会话
来源：http://bz.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lh.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://rm.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pm.asd995.cn

[U67] PHP：处理文件上传
来源：http://jp.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qg.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://ch.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://em.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://sg.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uy.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://sh.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ty.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ld.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ic.szxytkj.cn

[U72] PHP：写错误日志
来源：http://tu.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://lm.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://qk.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://yj.asd995.cn

[U74] PHP：读取环境变量
来源：http://kg.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://ee.asd995.cn

[U75] PHP：依赖注入
来源：http://jq.521024.cn

composer require psr/container
来源：http://co.huixiangedu.cn

[U76] PHP：简单路由
来源：http://ls.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tl.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://hf.szsharing.cn

composer require twig/twig
来源：http://gw.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://ru.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://ug.colortex.cn

[U79] PHP：静态分析
来源：http://rd.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://de.9csxet.cn

[U80] PHP：代码规范修复
来源：http://jp.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yh.gzmigu.cn

[U81] JS：初始化项目
来源：http://oo.huanxung.cn

npm init -y;  npm i express
来源：http://uu.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://tm.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xq.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://yh.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yy.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://zr.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://im.jianghongdianzi.cn

[U85] JS：可选链
来源：http://ij.wgjwhj.cn

a?.b?.c
来源：http://yh.nszjky.cn

[U86] JS：空值合并
来源：http://wp.bjjhwx.cn

a ?? b
来源：http://fi.yuexingan06.cn

[U87] JS：解构默认值
来源：http://aq.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://ne.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://gk.newstarts.cn

{ ...a, ...b }
来源：http://ie.nszjky.cn

[U89] JS：数组去重
来源：http://sk.yuntaijiaju.cn

[...new Set(arr)]
来源：http://dx.521024.cn

[U90] JS：数字数组排序
来源：http://go.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://ck.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://hk.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ba.lnxyls.cn

[U92] JS：深拷贝
来源：http://pq.hahajie.cn

structuredClone(obj)
来源：http://md.9csxet.cn

[U93] JS：模板字符串
来源：http://or.shxzukj.cn

`共 ${n} 条`
来源：http://im.huanxung.cn

[U94] JS：箭头函数
来源：http://xx.shxzukj.cn

const double = x => x * 2;
来源：http://qo.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://oy.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://cv.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://ht.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bk.gzmigu.cn

[U97] JS：并发请求
来源：http://je.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://wi.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sf.shtwfgs.cn

[U99] JS：事件监听
来源：http://va.huanxung.cn

el.addEventListener("click", e => {})
来源：http://tr.lnxyls.cn

[U100] JS：DOM 查询
来源：http://nr.shxzukj.cn

document.querySelector(".item")
来源：http://pq.yuexingan06.cn

[U101] JS：classList 操作
来源：http://zo.521024.cn

el.classList.toggle("active")
来源：http://jz.haigaiapp.cn

[U102] JS：本地存储
来源：http://uq.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jr.shxzskj.cn

[U103] JS：定时器
来源：http://md.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yv.szsharing.cn

[U104] JS：防抖
来源：http://pk.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mj.nszjky.cn

[U105] JS：节流
来源：http://qj.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://af.hnjuh.cn

[U106] JS：日期格式化
来源：http://gn.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ag.muxihuayi.cn

[U107] JS：数字千分位
来源：http://pu.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ca.panjiajie.cn

[U108] JS：随机整数
来源：http://lw.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mn.szxytkj.cn

[U109] JS：数组分组
来源：http://mm.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://tn.szsharing.cn

[U110] JS：数组分块
来源：http://eu.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nk.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://cr.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://dj.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://iz.jctech888.com.cn

"7".padStart(3, "0")
来源：http://oj.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://ev.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://xk.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://wi.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bl.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://zo.yuexingan06.cn

crypto.randomUUID()
来源：http://jg.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://dn.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://fz.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://im.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://nn.nicolike.cn

[U118] JS：开发服务器
来源：http://au.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://xp.lnxyls.cn

[U119] JS：生产构建
来源：http://nk.chemitech.net.cn

npx vite build
来源：http://es.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://kd.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://dh.haigaiapp.cn

================================================================================
来源：http://ty.haigaiapp.cn

统计汇总
来源：http://qp.huanxung.cn

================================================================================
来源：http://up.gzmigu.cn

按语言统计（条）：
来源：http://xo.panjiajie.cn

Python ......... 252
来源：http://zm.panjiajie.cn

PHP ............ 252
来源：http://id.nicolike.cn

JavaScript ..... 252
来源：http://ln.jctech888.com.cn

TypeScript ..... 212
来源：http://hc.huanxung.cn

Java ........... 212
来源：http://mv.hahajie.cn

Go ............. 212
来源：http://ww.huixinmuqiang.cn

Ruby ........... 212
来源：http://wz.lnxyls.cn

C# ............. 212
来源：http://ns.shxzskj.cn

C .............. 30
来源：http://pc.shtwfgs.cn

C++ ............ 30
来源：http://um.nicolike.cn

SQL ............ 90
来源：http://gl.bookmarksfly.cn

Bash ........... 80
来源：http://fg.yuexingan06.cn

Kotlin ......... 15
来源：http://pg.colortex.cn

Swift .......... 15
来源：http://po.shxzskj.cn

Lua ............ 10
来源：http://mx.huixinmuqiang.cn

Perl ........... 10
来源：http://ag.asd995.cn

Scala .......... 10
来源：http://wx.newstarts.cn

------------------------------------
来源：http://ee.newstarts.cn

合计 ........... 2106 条
来源：http://lk.chemitech.net.cn

按章节统计：
来源：http://og.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wk.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kw.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zn.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ze.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xd.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://og.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ep.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cl.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://na.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gw.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qr.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tf.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bg.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qk.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jo.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lb.shxzskj.cn

Q SQL 专题                              90
来源：http://ed.huixinmuqiang.cn

R Bash 专题                             80
来源：http://ct.521024.cn

S C / C++ 专题                          60
来源：http://wq.521024.cn

T 其他语言补充                          60
来源：http://vo.gzmigu.cn

U 高频实用片段                         120
来源：http://hc.hnjuh.cn

------------------------------------
来源：http://qt.shtwfgs.cn

合计                                  2106 条
来源：http://hh.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://lp.huixiangedu.cn

使用提醒
来源：http://cx.521024.cn

--------------------------------------------------------------------------------
来源：http://gb.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vw.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kt.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sj.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uf.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://po.haigaiapp.cn

—— 文件结束 ——
来源：http://qr.colortex.cn

================================================================================
来源：http://kc.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://hm.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://lq.hnjuh.cn

================================================================================
来源：http://ar.asd995.cn

【收录内容】
来源：http://ow.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yo.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vf.muxihuayi.cn

SQL · Bash · C · C++
来源：http://bu.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ns.9csxet.cn

【使用说明】
来源：http://mk.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ly.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yf.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gs.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lb.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uv.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ko.nszjky.cn


<!-- 参考信息 -->