代发 wailian999

[U05] Py：列表去重且保序
来源：http://xg.colortex.cn

list(dict.fromkeys(arr))
来源：http://st.asd995.cn

[U06] Py：合并两个字典
来源：http://dy.asd995.cn

{**a, **b}
来源：http://rn.521024.cn

[U07] Py：反转字典键值
来源：http://nw.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://qy.szsharing.cn

[U08] Py：展平二维列表
来源：http://hf.nszjky.cn

[y for x in nested for y in x]
来源：http://ls.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://ds.9csxet.cn

max(d, key=d.get)
来源：http://el.9csxet.cn

[U10] Py：按值排序字典
来源：http://sd.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uw.shxzskj.cn

[U11] Py：生成器表达式
来源：http://cu.huanxung.cn

(x * 2 for x in arr)
来源：http://hz.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ix.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://xe.nicolike.cn

[U13] Py：固定长度队列
来源：http://be.shxzukj.cn

deque(maxlen=10)
来源：http://kh.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://hn.jianghongdianzi.cn

defaultdict(list)
来源：http://be.colortex.cn

[U15] Py：高精度计时
来源：http://zc.szsharing.cn

t = time.perf_counter()
来源：http://zs.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://qm.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mv.newstarts.cn

[U17] Py：初始化日志
来源：http://tm.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://vy.hnjuh.cn

[U18] Py：预编译正则
来源：http://zn.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://nc.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://oo.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ee.nicolike.cn

[U20] Py：缓存函数结果
来源：http://ny.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://xa.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://zk.szxytkj.cn

@contextlib.contextmanager
来源：http://wc.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://xu.nicolike.cn

list(zip(*m))
来源：http://ag.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://gp.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mw.9csxet.cn

[U24] Py：路径操作
来源：http://oi.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tw.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://gx.huixinmuqiang.cn

csv.DictReader(f)
来源：http://pn.huixiangedu.cn

[U26] Py：并发下载
来源：http://vt.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wf.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://fo.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://ud.9csxet.cn

[U28] Py：类型别名
来源：http://we.colortex.cn

UserId = int
来源：http://nx.lnxyls.cn

[U29] Py：属性校验
来源：http://sx.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://dc.yuexingan06.cn

[U30] Py：数据类
来源：http://mn.colortex.cn

@dataclass(slots=True)
来源：http://df.haigaiapp.cn

[U31] Py：单测
来源：http://kr.jianghongdianzi.cn

python -m pytest -q
来源：http://fd.9csxet.cn

[U32] Py：代码格式化
来源：http://wx.9csxet.cn

ruff format . && ruff check --fix .
来源：http://ws.huixiangedu.cn

[U33] Py：打包发布
来源：http://er.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://yj.nszjky.cn

[U34] Py：判断编码
来源：http://nd.jianghongdianzi.cn

chardet.detect(raw)
来源：http://qj.lnxyls.cn

[U35] Py：发送邮件
来源：http://ty.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wg.szsharing.cn

[U36] Py：定时任务
来源：http://al.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://gw.gzmigu.cn

[U37] Py：读写 Excel
来源：http://pl.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uf.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://zk.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://op.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://qi.bookmarksfly.cn

sys.stdout.isatty()
来源：http://vm.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://lb.shxzskj.cn

print("err", file=sys.stderr)
来源：http://fa.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://xy.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://di.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://pt.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dp.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://qc.jianghongdianzi.cn

namespace App\Http;
来源：http://ww.521024.cn

[U44] PHP：开启严格类型
来源：http://tv.szsharing.cn

declare(strict_types=1);
来源：http://fi.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://jw.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zr.newstarts.cn

[U46] PHP：可空类型
来源：http://pf.muxihuayi.cn

?string $name = null
来源：http://yd.huanxung.cn

[U47] PHP：联合类型
来源：http://ww.chemitech.net.cn

int|string $id
来源：http://mh.9csxet.cn

[U48] PHP：纯枚举
来源：http://ku.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dg.haigaiapp.cn

[U49] PHP：只读属性
来源：http://dp.nszjky.cn

public readonly string $name
来源：http://mn.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://zq.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://tt.colortex.cn

[U51] PHP：数组解构
来源：http://km.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://yz.hahajie.cn

[U52] PHP：箭头函数
来源：http://bh.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://ap.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://nf.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://wj.521024.cn

[U54] PHP：空安全调用
来源：http://nt.shxzukj.cn

$obj?->method()
来源：http://xu.nicolike.cn

[U55] PHP：match 表达式
来源：http://mw.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dh.521024.cn

[U56] PHP：命名参数
来源：http://fl.szsharing.cn

f(a: 1, b: 2)
来源：http://tg.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://lb.yuexingan06.cn

"值: {$a}"
来源：http://ei.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://pg.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rz.szsharing.cn

[U59] PHP：自定义排序
来源：http://cp.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://op.colortex.cn

[U60] PHP：JSON 编解码
来源：http://zc.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xc.huanxung.cn

[U61] PHP：正则
来源：http://bo.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bb.newstarts.cn

[U62] PHP：日期对象
来源：http://rk.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ym.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://rr.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lg.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://bh.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://fl.szxytkj.cn

[U65] PHP：会话
来源：http://xm.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iw.asd995.cn

[U66] PHP：设置 Cookie
来源：http://bh.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yg.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://zl.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dw.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://zq.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vt.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://ma.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yo.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://wl.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mq.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ld.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://pt.nicolike.cn

[U72] PHP：写错误日志
来源：http://gx.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://fe.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://gm.521024.cn

parse_ini_file("config.ini", true)
来源：http://jo.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://jw.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://ta.huanxung.cn

[U75] PHP：依赖注入
来源：http://gc.asd995.cn

composer require psr/container
来源：http://lw.colortex.cn

[U76] PHP：简单路由
来源：http://nu.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ki.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://vk.huixinmuqiang.cn

composer require twig/twig
来源：http://qe.szsharing.cn

[U78] PHP：单元测试
来源：http://gz.colortex.cn

composer require --dev phpunit/phpunit
来源：http://as.hnjuh.cn

[U79] PHP：静态分析
来源：http://gg.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://rk.colortex.cn

[U80] PHP：代码规范修复
来源：http://mm.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ru.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://fa.9csxet.cn

npm init -y;  npm i express
来源：http://mz.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://ub.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nl.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://qy.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pe.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://ue.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fe.szsharing.cn

[U85] JS：可选链
来源：http://bk.wgjwhj.cn

a?.b?.c
来源：http://bi.shtwfgs.cn

[U86] JS：空值合并
来源：http://lx.huixinmuqiang.cn

a ?? b
来源：http://tn.muxihuayi.cn

[U87] JS：解构默认值
来源：http://gv.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://kj.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://nl.yuntaijiaju.cn

{ ...a, ...b }
来源：http://qq.panjiajie.cn

[U89] JS：数组去重
来源：http://vj.colortex.cn

[...new Set(arr)]
来源：http://we.shxzskj.cn

[U90] JS：数字数组排序
来源：http://ks.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://yi.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://du.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tg.asd995.cn

[U92] JS：深拷贝
来源：http://of.shtwfgs.cn

structuredClone(obj)
来源：http://nz.haigaiapp.cn

[U93] JS：模板字符串
来源：http://lw.nszjky.cn

`共 ${n} 条`
来源：http://sv.gzmigu.cn

[U94] JS：箭头函数
来源：http://nf.asd995.cn

const double = x => x * 2;
来源：http://al.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://bp.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://hk.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://ga.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oj.shxzskj.cn

[U97] JS：并发请求
来源：http://em.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nx.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://mq.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ah.muxihuayi.cn

[U99] JS：事件监听
来源：http://ig.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://nk.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://ny.hahajie.cn

document.querySelector(".item")
来源：http://xt.huanxung.cn

[U101] JS：classList 操作
来源：http://wv.9csxet.cn

el.classList.toggle("active")
来源：http://ff.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://qs.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cq.szsharing.cn

[U103] JS：定时器
来源：http://dj.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ka.huanxung.cn

[U104] JS：防抖
来源：http://tk.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kz.yuntaijiaju.cn

[U105] JS：节流
来源：http://qo.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://me.haigaiapp.cn

[U106] JS：日期格式化
来源：http://sx.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rv.lnxyls.cn

[U107] JS：数字千分位
来源：http://hg.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oh.hahajie.cn

[U108] JS：随机整数
来源：http://ak.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gu.wgjwhj.cn

[U109] JS：数组分组
来源：http://la.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://px.newstarts.cn

[U110] JS：数组分块
来源：http://oh.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sb.huanxung.cn

[U111] JS：对象转 Map
来源：http://by.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://tr.nszjky.cn

[U112] JS：字符串补位
来源：http://lp.yuexingan06.cn

"7".padStart(3, "0")
来源：http://zr.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://kv.panjiajie.cn

s.replaceAll("a", "b")
来源：http://ug.9csxet.cn

[U114] JS：JSON 深比较
来源：http://db.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dj.huanxung.cn

[U115] JS：生成 UUID
来源：http://uq.nszjky.cn

crypto.randomUUID()
来源：http://aq.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://rg.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://qt.lnxyls.cn

[U117] JS：单元测试
来源：http://nw.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://us.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://mu.szxytkj.cn

npm i -D vite;  npx vite
来源：http://bg.hnjuh.cn

[U119] JS：生产构建
来源：http://zg.9csxet.cn

npx vite build
来源：http://xl.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://yj.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://zn.lnxyls.cn

================================================================================
来源：http://il.gzmigu.cn

统计汇总
来源：http://lb.huixinmuqiang.cn

================================================================================
来源：http://ln.jianghongdianzi.cn

按语言统计（条）：
来源：http://mi.nszjky.cn

Python ......... 252
来源：http://su.jctech888.com.cn

PHP ............ 252
来源：http://qj.huixinmuqiang.cn

JavaScript ..... 252
来源：http://ld.haigaiapp.cn

TypeScript ..... 212
来源：http://mb.huixinmuqiang.cn

Java ........... 212
来源：http://un.haigaiapp.cn

Go ............. 212
来源：http://lg.asd995.cn

Ruby ........... 212
来源：http://io.hnjuh.cn

C# ............. 212
来源：http://bi.shxzukj.cn

C .............. 30
来源：http://od.muxihuayi.cn

C++ ............ 30
来源：http://aw.haigaiapp.cn

SQL ............ 90
来源：http://oq.muxihuayi.cn

Bash ........... 80
来源：http://fq.haigaiapp.cn

Kotlin ......... 15
来源：http://cv.lnxyls.cn

Swift .......... 15
来源：http://ug.shtwfgs.cn

Lua ............ 10
来源：http://bc.newstarts.cn

Perl ........... 10
来源：http://fk.huanxung.cn

Scala .......... 10
来源：http://vu.huanxung.cn

------------------------------------
来源：http://gs.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://ch.nicolike.cn

按章节统计：
来源：http://qg.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tf.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mz.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nv.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pb.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ha.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ay.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ip.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zs.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yq.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ry.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vm.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wq.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ys.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cd.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uq.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ld.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://mp.wgjwhj.cn

R Bash 专题                             80
来源：http://ye.shxzukj.cn

S C / C++ 专题                          60
来源：http://kz.bookmarksfly.cn

T 其他语言补充                          60
来源：http://vr.shxzskj.cn

U 高频实用片段                         120
来源：http://td.szxytkj.cn

------------------------------------
来源：http://ti.shtwfgs.cn

合计                                  2106 条
来源：http://bm.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://cp.hahajie.cn

使用提醒
来源：http://cz.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://aj.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://px.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nz.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ar.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hc.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dt.panjiajie.cn

—— 文件结束 ——
来源：http://ci.9csxet.cn

================================================================================
来源：http://yh.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ae.colortex.cn

Common Programming Examples Cheat Book
来源：http://lu.yuntaijiaju.cn

================================================================================
来源：http://rd.jianghongdianzi.cn

【收录内容】
来源：http://yk.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ke.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ne.9csxet.cn

SQL · Bash · C · C++
来源：http://ol.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jg.shxzskj.cn

【使用说明】
来源：http://es.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qq.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gf.hnjuh.cn


<!-- 参考信息 -->