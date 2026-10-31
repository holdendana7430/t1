代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aq.colortex.cn

================================================================================
来源：http://vo.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wp.huixinmuqiang.cn

================================================================================
来源：http://ds.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://fs.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jw.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://id.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uz.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://hy.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kp.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://ul.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hp.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://dv.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://lc.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ls.lnxyls.cn

{**a, **b}
来源：http://in.nszjky.cn

[U07] Py：反转字典键值
来源：http://ic.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://wo.nicolike.cn

[U08] Py：展平二维列表
来源：http://jm.shxzskj.cn

[y for x in nested for y in x]
来源：http://pz.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://nt.szxytkj.cn

max(d, key=d.get)
来源：http://dz.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://zk.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uw.panjiajie.cn

[U11] Py：生成器表达式
来源：http://ns.asd995.cn

(x * 2 for x in arr)
来源：http://ca.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dn.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://dx.shxzukj.cn

[U13] Py：固定长度队列
来源：http://ac.colortex.cn

deque(maxlen=10)
来源：http://oo.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://rn.jctech888.com.cn

defaultdict(list)
来源：http://pp.colortex.cn

[U15] Py：高精度计时
来源：http://zt.nicolike.cn

t = time.perf_counter()
来源：http://oo.asd995.cn

[U16] Py：命令行参数解析
来源：http://by.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wp.yuexingan06.cn

[U17] Py：初始化日志
来源：http://mu.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://wo.nicolike.cn

[U18] Py：预编译正则
来源：http://ee.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://fb.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://oj.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sq.9csxet.cn

[U20] Py：缓存函数结果
来源：http://pj.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://rv.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://la.asd995.cn

@contextlib.contextmanager
来源：http://mw.panjiajie.cn

[U22] Py：矩阵转置
来源：http://fy.haigaiapp.cn

list(zip(*m))
来源：http://xh.9csxet.cn

[U23] Py：分块读取大文件
来源：http://ky.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yr.chemitech.net.cn

[U24] Py：路径操作
来源：http://su.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gm.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://bc.szsharing.cn

csv.DictReader(f)
来源：http://un.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://it.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://in.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://vt.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://os.haigaiapp.cn

[U28] Py：类型别名
来源：http://hy.szsharing.cn

UserId = int
来源：http://ul.chemitech.net.cn

[U29] Py：属性校验
来源：http://hn.shxzukj.cn

@property 与 @x.setter 配合
来源：http://fc.szxytkj.cn

[U30] Py：数据类
来源：http://pi.gzmigu.cn

@dataclass(slots=True)
来源：http://kj.nszjky.cn

[U31] Py：单测
来源：http://bi.colortex.cn

python -m pytest -q
来源：http://ih.jctech888.com.cn

[U32] Py：代码格式化
来源：http://rr.colortex.cn

ruff format . && ruff check --fix .
来源：http://ws.colortex.cn

[U33] Py：打包发布
来源：http://ch.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://yt.asd995.cn

[U34] Py：判断编码
来源：http://ya.huanxung.cn

chardet.detect(raw)
来源：http://fi.szxytkj.cn

[U35] Py：发送邮件
来源：http://nu.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cm.shxzskj.cn

[U36] Py：定时任务
来源：http://ny.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://tf.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://hk.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ho.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://bt.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://db.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://gx.jctech888.com.cn

sys.stdout.isatty()
来源：http://cp.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://yo.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://yd.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://pg.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oh.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://nz.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ri.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://zk.chemitech.net.cn

namespace App\Http;
来源：http://dm.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://xh.9csxet.cn

declare(strict_types=1);
来源：http://lq.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://ch.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nw.haigaiapp.cn

[U46] PHP：可空类型
来源：http://bd.shxzskj.cn

?string $name = null
来源：http://tp.521024.cn

[U47] PHP：联合类型
来源：http://px.asd995.cn

int|string $id
来源：http://uz.panjiajie.cn

[U48] PHP：纯枚举
来源：http://wu.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://di.panjiajie.cn

[U49] PHP：只读属性
来源：http://ji.huixinmuqiang.cn

public readonly string $name
来源：http://gl.asd995.cn

[U50] PHP：构造器属性提升
来源：http://mg.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://bx.asd995.cn

[U51] PHP：数组解构
来源：http://nj.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://mb.szxytkj.cn

[U52] PHP：箭头函数
来源：http://dx.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://cx.newstarts.cn

[U53] PHP：空合并运算符
来源：http://nl.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://tk.asd995.cn

[U54] PHP：空安全调用
来源：http://na.haigaiapp.cn

$obj?->method()
来源：http://rr.hahajie.cn

[U55] PHP：match 表达式
来源：http://xd.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ns.bjjhwx.cn

[U56] PHP：命名参数
来源：http://ns.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://bg.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://fw.nicolike.cn

"值: {$a}"
来源：http://tq.hnjuh.cn

[U58] PHP：数组三件套
来源：http://sq.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xb.shxzukj.cn

[U59] PHP：自定义排序
来源：http://mm.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://di.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://zi.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ej.newstarts.cn

[U61] PHP：正则
来源：http://qz.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ar.nicolike.cn

[U62] PHP：日期对象
来源：http://bp.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fe.huanxung.cn

[U63] PHP：文件读写
来源：http://gu.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qa.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://ph.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://hf.bookmarksfly.cn

[U65] PHP：会话
来源：http://mh.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yy.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://fk.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yg.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://hx.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uy.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://hn.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qn.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://os.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nz.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://nf.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ej.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://sf.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://wy.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://oe.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://ri.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://gw.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://lh.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://aw.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://wn.gzmigu.cn

[U75] PHP：依赖注入
来源：http://fv.yuntaijiaju.cn

composer require psr/container
来源：http://sp.szsharing.cn

[U76] PHP：简单路由
来源：http://xe.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hf.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://pz.chemitech.net.cn

composer require twig/twig
来源：http://ho.yuexingan06.cn

[U78] PHP：单元测试
来源：http://or.521024.cn

composer require --dev phpunit/phpunit
来源：http://gy.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://tw.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://cf.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://xt.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://op.hnjuh.cn

[U81] JS：初始化项目
来源：http://wg.huanxung.cn

npm init -y;  npm i express
来源：http://ws.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://xj.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ft.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://ah.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qr.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://yy.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gy.nicolike.cn

[U85] JS：可选链
来源：http://zx.szsharing.cn

a?.b?.c
来源：http://ke.bookmarksfly.cn

[U86] JS：空值合并
来源：http://lb.9csxet.cn

a ?? b
来源：http://zg.colortex.cn

[U87] JS：解构默认值
来源：http://sh.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://zw.colortex.cn

[U88] JS：对象展开合并
来源：http://mx.gzmigu.cn

{ ...a, ...b }
来源：http://kb.huanxung.cn

[U89] JS：数组去重
来源：http://lu.nszjky.cn

[...new Set(arr)]
来源：http://pj.nszjky.cn

[U90] JS：数字数组排序
来源：http://fj.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://td.asd995.cn

[U91] JS：对象键值遍历
来源：http://en.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qb.shxzskj.cn

[U92] JS：深拷贝
来源：http://nr.asd995.cn

structuredClone(obj)
来源：http://ru.colortex.cn

[U93] JS：模板字符串
来源：http://sd.huixiangedu.cn

`共 ${n} 条`
来源：http://zx.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://fb.szxytkj.cn

const double = x => x * 2;
来源：http://pr.shxzukj.cn

[U95] JS：Promise 包装
来源：http://rk.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://ek.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://hz.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ai.wgjwhj.cn

[U97] JS：并发请求
来源：http://pt.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ug.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://rd.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ea.chemitech.net.cn

[U99] JS：事件监听
来源：http://uj.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://br.colortex.cn

[U100] JS：DOM 查询
来源：http://ch.521024.cn

document.querySelector(".item")
来源：http://cf.9csxet.cn

[U101] JS：classList 操作
来源：http://am.shtwfgs.cn

el.classList.toggle("active")
来源：http://xw.huixiangedu.cn

[U102] JS：本地存储
来源：http://qn.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gz.hnjuh.cn

[U103] JS：定时器
来源：http://zd.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ev.shxzukj.cn

[U104] JS：防抖
来源：http://ic.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://da.shtwfgs.cn

[U105] JS：节流
来源：http://nm.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vu.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://lg.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cf.hahajie.cn

[U107] JS：数字千分位
来源：http://fw.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jg.hahajie.cn

[U108] JS：随机整数
来源：http://za.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eo.nicolike.cn

[U109] JS：数组分组
来源：http://do.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://cf.panjiajie.cn

[U110] JS：数组分块
来源：http://by.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gm.newstarts.cn

[U111] JS：对象转 Map
来源：http://ma.shxzskj.cn

new Map(Object.entries(obj))
来源：http://hl.yuexingan06.cn

[U112] JS：字符串补位
来源：http://xd.bjjhwx.cn

"7".padStart(3, "0")
来源：http://tr.521024.cn

[U113] JS：正则替换全部
来源：http://hm.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://aw.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://ph.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cg.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://ox.huixinmuqiang.cn

crypto.randomUUID()
来源：http://aa.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://kz.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://ae.colortex.cn

[U117] JS：单元测试
来源：http://qg.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://ly.521024.cn

[U118] JS：开发服务器
来源：http://ml.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://he.hnjuh.cn

[U119] JS：生产构建
来源：http://xx.asd995.cn

npx vite build
来源：http://yy.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ld.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://lr.gzmigu.cn

================================================================================
来源：http://ng.haigaiapp.cn

统计汇总
来源：http://lm.bookmarksfly.cn

================================================================================
来源：http://tu.jctech888.com.cn

按语言统计（条）：
来源：http://rr.lnxyls.cn

Python ......... 252
来源：http://zv.nszjky.cn

PHP ............ 252
来源：http://tz.shxzukj.cn

JavaScript ..... 252
来源：http://yk.nicolike.cn

TypeScript ..... 212
来源：http://qb.szsharing.cn

Java ........... 212
来源：http://pe.panjiajie.cn

Go ............. 212
来源：http://td.521024.cn

Ruby ........... 212
来源：http://ob.shxzukj.cn

C# ............. 212
来源：http://ko.huixinmuqiang.cn

C .............. 30
来源：http://hz.newstarts.cn

C++ ............ 30
来源：http://nd.asd995.cn

SQL ............ 90
来源：http://zc.newstarts.cn

Bash ........... 80
来源：http://co.hnjuh.cn

Kotlin ......... 15
来源：http://zn.huanxung.cn

Swift .......... 15
来源：http://kp.panjiajie.cn

Lua ............ 10
来源：http://bl.nicolike.cn

Perl ........... 10
来源：http://sc.muxihuayi.cn

Scala .......... 10
来源：http://ht.hnjuh.cn

------------------------------------
来源：http://dn.bjjhwx.cn

合计 ........... 2106 条
来源：http://lx.bjjhwx.cn

按章节统计：
来源：http://vg.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qk.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ml.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://to.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ii.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://je.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sh.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://da.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ky.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pb.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ko.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yj.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wj.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://et.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qe.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://to.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ta.chemitech.net.cn

Q SQL 专题                              90
来源：http://gg.hahajie.cn

R Bash 专题                             80
来源：http://wu.shxzskj.cn

S C / C++ 专题                          60
来源：http://jg.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://co.huanxung.cn

U 高频实用片段                         120
来源：http://ii.9csxet.cn

------------------------------------
来源：http://qd.chemitech.net.cn

合计                                  2106 条
来源：http://ai.asd995.cn

--------------------------------------------------------------------------------
来源：http://go.shxzskj.cn

使用提醒
来源：http://xi.hahajie.cn

--------------------------------------------------------------------------------
来源：http://lg.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ia.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dp.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://as.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xf.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eu.szxytkj.cn

—— 文件结束 ——
来源：http://vl.wgjwhj.cn


<!-- 参考信息 -->