代发 wailian999

[U05] Py：列表去重且保序
来源：http://sa.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://eu.huanxung.cn

[U06] Py：合并两个字典
来源：http://bx.jctech888.com.cn

{**a, **b}
来源：http://pw.hnjuh.cn

[U07] Py：反转字典键值
来源：http://yq.szsharing.cn

{v: k for k, v in d.items()}
来源：http://oa.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://xu.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://nx.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://zh.yuexingan06.cn

max(d, key=d.get)
来源：http://ba.shxzukj.cn

[U10] Py：按值排序字典
来源：http://av.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yx.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://lb.9csxet.cn

(x * 2 for x in arr)
来源：http://cb.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lm.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://ea.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://vc.9csxet.cn

deque(maxlen=10)
来源：http://kt.9csxet.cn

[U14] Py：分组收集到列表
来源：http://oe.yuexingan06.cn

defaultdict(list)
来源：http://sp.521024.cn

[U15] Py：高精度计时
来源：http://yn.shxzskj.cn

t = time.perf_counter()
来源：http://vn.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://vh.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jy.newstarts.cn

[U17] Py：初始化日志
来源：http://qy.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://au.nicolike.cn

[U18] Py：预编译正则
来源：http://ih.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://du.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://ks.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://po.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://jz.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://fb.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://dn.asd995.cn

@contextlib.contextmanager
来源：http://bc.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://rk.yuntaijiaju.cn

list(zip(*m))
来源：http://ct.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://ev.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vy.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://eg.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ub.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ue.hnjuh.cn

csv.DictReader(f)
来源：http://tl.lnxyls.cn

[U26] Py：并发下载
来源：http://nc.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://av.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://hy.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://pq.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://mk.shxzskj.cn

UserId = int
来源：http://ei.muxihuayi.cn

[U29] Py：属性校验
来源：http://sz.gzmigu.cn

@property 与 @x.setter 配合
来源：http://jm.haigaiapp.cn

[U30] Py：数据类
来源：http://ah.bookmarksfly.cn

@dataclass(slots=True)
来源：http://tg.haigaiapp.cn

[U31] Py：单测
来源：http://rc.szxytkj.cn

python -m pytest -q
来源：http://oi.chemitech.net.cn

[U32] Py：代码格式化
来源：http://xe.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://iw.shtwfgs.cn

[U33] Py：打包发布
来源：http://we.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://ve.newstarts.cn

[U34] Py：判断编码
来源：http://lm.huixinmuqiang.cn

chardet.detect(raw)
来源：http://fl.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://dk.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zk.nicolike.cn

[U36] Py：定时任务
来源：http://zu.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://vl.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://dt.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gg.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://hd.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://vg.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://de.asd995.cn

sys.stdout.isatty()
来源：http://cv.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://lh.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://pb.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://wd.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wr.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://er.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://by.colortex.cn

[U43] PHP：声明命名空间
来源：http://lg.gzmigu.cn

namespace App\Http;
来源：http://xs.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://lf.bjjhwx.cn

declare(strict_types=1);
来源：http://wj.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://tc.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qe.nszjky.cn

[U46] PHP：可空类型
来源：http://ml.hnjuh.cn

?string $name = null
来源：http://fl.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://yu.wgjwhj.cn

int|string $id
来源：http://sb.hnjuh.cn

[U48] PHP：纯枚举
来源：http://vr.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sc.hnjuh.cn

[U49] PHP：只读属性
来源：http://ke.jctech888.com.cn

public readonly string $name
来源：http://iz.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://cb.szxytkj.cn

public function __construct(private int $id) {}
来源：http://rg.bjjhwx.cn

[U51] PHP：数组解构
来源：http://yf.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://nq.huanxung.cn

[U52] PHP：箭头函数
来源：http://sg.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://yc.newstarts.cn

[U53] PHP：空合并运算符
来源：http://uz.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://js.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://px.haigaiapp.cn

$obj?->method()
来源：http://zp.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ii.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vt.nicolike.cn

[U56] PHP：命名参数
来源：http://kz.shxzskj.cn

f(a: 1, b: 2)
来源：http://io.panjiajie.cn

[U57] PHP：字符串插值
来源：http://fo.hnjuh.cn

"值: {$a}"
来源：http://wx.asd995.cn

[U58] PHP：数组三件套
来源：http://hm.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cy.hahajie.cn

[U59] PHP：自定义排序
来源：http://dq.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lr.521024.cn

[U60] PHP：JSON 编解码
来源：http://sn.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pv.bjjhwx.cn

[U61] PHP：正则
来源：http://mj.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cl.szxytkj.cn

[U62] PHP：日期对象
来源：http://ka.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iv.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://co.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gu.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://yp.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://vt.hahajie.cn

[U65] PHP：会话
来源：http://oe.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tj.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://dh.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://is.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://qc.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bz.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://iq.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ze.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://ce.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zt.szsharing.cn

[U70] PHP：PDO 事务
来源：http://yx.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://al.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://ar.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://yf.nszjky.cn

[U72] PHP：写错误日志
来源：http://kh.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://np.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://ya.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://iq.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ru.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://qf.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://aa.hnjuh.cn

composer require psr/container
来源：http://yn.hahajie.cn

[U76] PHP：简单路由
来源：http://zm.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wy.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://wj.yuntaijiaju.cn

composer require twig/twig
来源：http://mk.newstarts.cn

[U78] PHP：单元测试
来源：http://sm.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://ab.huixiangedu.cn

[U79] PHP：静态分析
来源：http://bd.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://tn.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://bm.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lo.wgjwhj.cn

[U81] JS：初始化项目
来源：http://uo.haigaiapp.cn

npm init -y;  npm i express
来源：http://xa.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://vf.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://un.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://sd.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fs.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://fo.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ug.wgjwhj.cn

[U85] JS：可选链
来源：http://hn.panjiajie.cn

a?.b?.c
来源：http://ie.chemitech.net.cn

[U86] JS：空值合并
来源：http://kx.nszjky.cn

a ?? b
来源：http://bo.newstarts.cn

[U87] JS：解构默认值
来源：http://ai.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://zb.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://sn.521024.cn

{ ...a, ...b }
来源：http://pk.szsharing.cn

[U89] JS：数组去重
来源：http://nf.newstarts.cn

[...new Set(arr)]
来源：http://hi.szsharing.cn

[U90] JS：数字数组排序
来源：http://hk.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://dq.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://xq.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oc.panjiajie.cn

[U92] JS：深拷贝
来源：http://gg.yuntaijiaju.cn

structuredClone(obj)
来源：http://fw.panjiajie.cn

[U93] JS：模板字符串
来源：http://af.gzmigu.cn

`共 ${n} 条`
来源：http://gh.shtwfgs.cn

[U94] JS：箭头函数
来源：http://tm.yuexingan06.cn

const double = x => x * 2;
来源：http://ga.asd995.cn

[U95] JS：Promise 包装
来源：http://kp.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://fi.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://uu.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fu.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://uj.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sl.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://bs.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ni.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://xx.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://ne.shxzukj.cn

[U100] JS：DOM 查询
来源：http://ge.yuexingan06.cn

document.querySelector(".item")
来源：http://ob.panjiajie.cn

[U101] JS：classList 操作
来源：http://zi.asd995.cn

el.classList.toggle("active")
来源：http://ve.shtwfgs.cn

[U102] JS：本地存储
来源：http://ap.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fm.shtwfgs.cn

[U103] JS：定时器
来源：http://pk.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ah.chemitech.net.cn

[U104] JS：防抖
来源：http://nj.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lm.9csxet.cn

[U105] JS：节流
来源：http://si.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cw.chemitech.net.cn

[U106] JS：日期格式化
来源：http://mb.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qo.yuexingan06.cn

[U107] JS：数字千分位
来源：http://bu.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://je.wgjwhj.cn

[U108] JS：随机整数
来源：http://ai.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cl.shxzskj.cn

[U109] JS：数组分组
来源：http://rl.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://fw.bjjhwx.cn

[U110] JS：数组分块
来源：http://sn.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dn.gzmigu.cn

[U111] JS：对象转 Map
来源：http://ie.colortex.cn

new Map(Object.entries(obj))
来源：http://qc.chemitech.net.cn

[U112] JS：字符串补位
来源：http://wh.szxytkj.cn

"7".padStart(3, "0")
来源：http://gd.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ds.shxzskj.cn

s.replaceAll("a", "b")
来源：http://zz.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://fc.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rq.nszjky.cn

[U115] JS：生成 UUID
来源：http://gj.jctech888.com.cn

crypto.randomUUID()
来源：http://sg.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://cv.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://zn.nszjky.cn

[U117] JS：单元测试
来源：http://dc.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://wy.wgjwhj.cn

[U118] JS：开发服务器
来源：http://dz.gzmigu.cn

npm i -D vite;  npx vite
来源：http://pn.hahajie.cn

[U119] JS：生产构建
来源：http://sv.asd995.cn

npx vite build
来源：http://dt.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://vc.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://an.panjiajie.cn

================================================================================
来源：http://wy.9csxet.cn

统计汇总
来源：http://ek.huixiangedu.cn

================================================================================
来源：http://oa.hahajie.cn

按语言统计（条）：
来源：http://us.huanxung.cn

Python ......... 252
来源：http://dr.asd995.cn

PHP ............ 252
来源：http://js.hnjuh.cn

JavaScript ..... 252
来源：http://tk.shxzskj.cn

TypeScript ..... 212
来源：http://hp.nicolike.cn

Java ........... 212
来源：http://ss.huanxung.cn

Go ............. 212
来源：http://nf.colortex.cn

Ruby ........... 212
来源：http://ak.asd995.cn

C# ............. 212
来源：http://pu.jctech888.com.cn

C .............. 30
来源：http://sb.huixiangedu.cn

C++ ............ 30
来源：http://gl.521024.cn

SQL ............ 90
来源：http://la.panjiajie.cn

Bash ........... 80
来源：http://zk.hnjuh.cn

Kotlin ......... 15
来源：http://yv.hahajie.cn

Swift .......... 15
来源：http://uy.colortex.cn

Lua ............ 10
来源：http://su.wgjwhj.cn

Perl ........... 10
来源：http://dx.asd995.cn

Scala .......... 10
来源：http://ap.yuntaijiaju.cn

------------------------------------
来源：http://nk.nicolike.cn

合计 ........... 2106 条
来源：http://gp.hahajie.cn

按章节统计：
来源：http://pm.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://es.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ag.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jo.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oz.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hh.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qt.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tu.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ve.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://up.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ds.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jl.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wa.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uq.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tc.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://at.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eh.9csxet.cn

Q SQL 专题                              90
来源：http://uk.asd995.cn

R Bash 专题                             80
来源：http://ck.newstarts.cn

S C / C++ 专题                          60
来源：http://db.huixiangedu.cn

T 其他语言补充                          60
来源：http://yf.huixiangedu.cn

U 高频实用片段                         120
来源：http://cz.wgjwhj.cn

------------------------------------
来源：http://tg.bjjhwx.cn

合计                                  2106 条
来源：http://lo.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://uh.huanxung.cn

使用提醒
来源：http://il.nszjky.cn

--------------------------------------------------------------------------------
来源：http://em.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ig.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ny.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rf.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jt.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ts.nszjky.cn

—— 文件结束 ——
来源：http://sy.shxzskj.cn

================================================================================
来源：http://sr.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://rl.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://kj.shxzskj.cn

================================================================================
来源：http://ys.jctech888.com.cn

【收录内容】
来源：http://ji.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xa.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ty.newstarts.cn

SQL · Bash · C · C++
来源：http://wx.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sw.9csxet.cn

【使用说明】
来源：http://id.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ru.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cq.gzmigu.cn


<!-- 参考信息 -->