代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://ma.shtwfgs.cn

[T59] Scala：循环
来源：http://xz.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://md.haigaiapp.cn

[T60] Scala：折叠
来源：http://yw.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ik.gzmigu.cn

================================================================================
来源：http://uv.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vg.muxihuayi.cn

================================================================================
来源：http://xk.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://nt.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fa.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://xq.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ob.asd995.cn

[U03] Py：加载 .env 配置
来源：http://su.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yl.huanxung.cn

[U04] Py：变量调试打印
来源：http://gb.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://de.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://dk.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://kn.huanxung.cn

[U06] Py：合并两个字典
来源：http://lb.bookmarksfly.cn

{**a, **b}
来源：http://qk.gzmigu.cn

[U07] Py：反转字典键值
来源：http://je.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://ai.nszjky.cn

[U08] Py：展平二维列表
来源：http://hd.nszjky.cn

[y for x in nested for y in x]
来源：http://le.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://eu.huixiangedu.cn

max(d, key=d.get)
来源：http://no.nszjky.cn

[U10] Py：按值排序字典
来源：http://ht.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mx.huanxung.cn

[U11] Py：生成器表达式
来源：http://fj.gzmigu.cn

(x * 2 for x in arr)
来源：http://tq.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xg.nszjky.cn

Counter(arr).most_common(3)
来源：http://cd.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://az.hahajie.cn

deque(maxlen=10)
来源：http://by.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://ve.colortex.cn

defaultdict(list)
来源：http://cc.szxytkj.cn

[U15] Py：高精度计时
来源：http://ob.huanxung.cn

t = time.perf_counter()
来源：http://ch.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://fg.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://as.hnjuh.cn

[U17] Py：初始化日志
来源：http://hg.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://sh.szxytkj.cn

[U18] Py：预编译正则
来源：http://cn.521024.cn

pat = re.compile(r"\d+")
来源：http://gi.newstarts.cn

[U19] Py：正则替换带回调
来源：http://dl.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pa.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://wr.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://dg.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ir.gzmigu.cn

@contextlib.contextmanager
来源：http://qm.panjiajie.cn

[U22] Py：矩阵转置
来源：http://ly.newstarts.cn

list(zip(*m))
来源：http://oz.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://ik.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zl.asd995.cn

[U24] Py：路径操作
来源：http://um.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iq.colortex.cn

[U25] Py：CSV 按字典读
来源：http://mk.lnxyls.cn

csv.DictReader(f)
来源：http://ua.9csxet.cn

[U26] Py：并发下载
来源：http://eb.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ah.colortex.cn

[U27] Py：异步 HTTP
来源：http://hn.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://bh.gzmigu.cn

[U28] Py：类型别名
来源：http://vc.newstarts.cn

UserId = int
来源：http://hc.yuexingan06.cn

[U29] Py：属性校验
来源：http://kn.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://oq.muxihuayi.cn

[U30] Py：数据类
来源：http://yj.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://yo.chemitech.net.cn

[U31] Py：单测
来源：http://ey.szsharing.cn

python -m pytest -q
来源：http://tj.panjiajie.cn

[U32] Py：代码格式化
来源：http://wz.521024.cn

ruff format . && ruff check --fix .
来源：http://bs.gzmigu.cn

[U33] Py：打包发布
来源：http://gl.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://ek.huanxung.cn

[U34] Py：判断编码
来源：http://kg.yuexingan06.cn

chardet.detect(raw)
来源：http://kg.chemitech.net.cn

[U35] Py：发送邮件
来源：http://dg.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://go.huanxung.cn

[U36] Py：定时任务
来源：http://gb.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://wk.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ii.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ya.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://ao.szsharing.cn

Path(__file__).resolve().parent
来源：http://gw.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://qe.huixiangedu.cn

sys.stdout.isatty()
来源：http://gb.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://yv.szsharing.cn

print("err", file=sys.stderr)
来源：http://ur.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://as.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sq.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://tv.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xk.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://wr.nszjky.cn

namespace App\Http;
来源：http://nr.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://bs.bookmarksfly.cn

declare(strict_types=1);
来源：http://st.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://yb.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hr.shxzskj.cn

[U46] PHP：可空类型
来源：http://ea.shxzukj.cn

?string $name = null
来源：http://tk.nszjky.cn

[U47] PHP：联合类型
来源：http://lh.nicolike.cn

int|string $id
来源：http://dr.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://zo.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yy.wgjwhj.cn

[U49] PHP：只读属性
来源：http://wj.szxytkj.cn

public readonly string $name
来源：http://ma.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://ga.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://rg.yuexingan06.cn

[U51] PHP：数组解构
来源：http://km.shxzukj.cn

[$a, $b] = $arr;
来源：http://gn.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://jc.colortex.cn

$double = fn($x) => $x * 2;
来源：http://ju.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://qg.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://cv.lnxyls.cn

[U54] PHP：空安全调用
来源：http://ds.panjiajie.cn

$obj?->method()
来源：http://uw.newstarts.cn

[U55] PHP：match 表达式
来源：http://oy.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ae.szsharing.cn

[U56] PHP：命名参数
来源：http://mj.521024.cn

f(a: 1, b: 2)
来源：http://pt.shxzskj.cn

[U57] PHP：字符串插值
来源：http://nv.hnjuh.cn

"值: {$a}"
来源：http://vs.9csxet.cn

[U58] PHP：数组三件套
来源：http://jw.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wq.9csxet.cn

[U59] PHP：自定义排序
来源：http://sp.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mo.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://zn.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pd.gzmigu.cn

[U61] PHP：正则
来源：http://rx.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qp.szsharing.cn

[U62] PHP：日期对象
来源：http://ct.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pu.yuexingan06.cn

[U63] PHP：文件读写
来源：http://am.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hx.521024.cn

[U64] PHP：目录遍历
来源：http://qd.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://cs.nszjky.cn

[U65] PHP：会话
来源：http://wh.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yc.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://th.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sw.nszjky.cn

[U67] PHP：处理文件上传
来源：http://xd.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kz.hahajie.cn

[U68] PHP：PDO 连接
来源：http://cy.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qy.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://ev.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ov.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://il.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://io.nicolike.cn

[U71] PHP：抛出异常
来源：http://nn.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://mt.colortex.cn

[U72] PHP：写错误日志
来源：http://rl.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://ys.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://ku.521024.cn

parse_ini_file("config.ini", true)
来源：http://pm.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://jt.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://gf.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://cg.shxzskj.cn

composer require psr/container
来源：http://xd.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://vd.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ua.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://zu.521024.cn

composer require twig/twig
来源：http://wu.shtwfgs.cn

[U78] PHP：单元测试
来源：http://ep.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://uv.colortex.cn

[U79] PHP：静态分析
来源：http://mo.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://ng.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://sv.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.asd995.cn

[U81] JS：初始化项目
来源：http://lg.hahajie.cn

npm init -y;  npm i express
来源：http://dh.nicolike.cn

[U82] JS：package.json 脚本
来源：http://je.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uf.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://wf.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ff.colortex.cn

[U84] JS：CommonJS 写法
来源：http://ug.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dh.jctech888.com.cn

[U85] JS：可选链
来源：http://ok.huixinmuqiang.cn

a?.b?.c
来源：http://rp.bjjhwx.cn

[U86] JS：空值合并
来源：http://dr.huixiangedu.cn

a ?? b
来源：http://pr.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://wn.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://wo.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://qw.hnjuh.cn

{ ...a, ...b }
来源：http://gn.lnxyls.cn

[U89] JS：数组去重
来源：http://ab.9csxet.cn

[...new Set(arr)]
来源：http://zc.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://xr.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://rb.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://qh.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fi.panjiajie.cn

[U92] JS：深拷贝
来源：http://qw.szxytkj.cn

structuredClone(obj)
来源：http://cd.colortex.cn

[U93] JS：模板字符串
来源：http://gl.haigaiapp.cn

`共 ${n} 条`
来源：http://fw.shxzukj.cn

[U94] JS：箭头函数
来源：http://ey.szxytkj.cn

const double = x => x * 2;
来源：http://hm.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://lt.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://vl.hahajie.cn

[U96] JS：async/await 与异常
来源：http://uy.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qu.gzmigu.cn

[U97] JS：并发请求
来源：http://gm.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vm.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://vd.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zt.huanxung.cn

[U99] JS：事件监听
来源：http://zn.521024.cn

el.addEventListener("click", e => {})
来源：http://yg.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://md.yuexingan06.cn

document.querySelector(".item")
来源：http://uy.nicolike.cn

[U101] JS：classList 操作
来源：http://sj.yuexingan06.cn

el.classList.toggle("active")
来源：http://iw.bjjhwx.cn

[U102] JS：本地存储
来源：http://oz.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ws.shtwfgs.cn

[U103] JS：定时器
来源：http://ed.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wb.lnxyls.cn

[U104] JS：防抖
来源：http://rs.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aq.nicolike.cn

[U105] JS：节流
来源：http://bt.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lg.gzmigu.cn

[U106] JS：日期格式化
来源：http://ux.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hk.nicolike.cn

[U107] JS：数字千分位
来源：http://wf.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jc.huixiangedu.cn

[U108] JS：随机整数
来源：http://ge.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ri.hahajie.cn

[U109] JS：数组分组
来源：http://tp.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://vk.jctech888.com.cn

[U110] JS：数组分块
来源：http://pt.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://si.szxytkj.cn

[U111] JS：对象转 Map
来源：http://sd.nszjky.cn

new Map(Object.entries(obj))
来源：http://dt.521024.cn

[U112] JS：字符串补位
来源：http://gt.521024.cn

"7".padStart(3, "0")
来源：http://hm.szsharing.cn

[U113] JS：正则替换全部
来源：http://jl.asd995.cn

s.replaceAll("a", "b")
来源：http://oy.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://lh.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wk.szsharing.cn

[U115] JS：生成 UUID
来源：http://vp.yuntaijiaju.cn

crypto.randomUUID()
来源：http://fi.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://kc.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://zi.asd995.cn

[U117] JS：单元测试
来源：http://ne.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://io.jctech888.com.cn

[U118] JS：开发服务器
来源：http://ub.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://uq.huixiangedu.cn

[U119] JS：生产构建
来源：http://xn.yuexingan06.cn

npx vite build
来源：http://yu.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://hf.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://hp.asd995.cn

================================================================================
来源：http://td.huanxung.cn

统计汇总
来源：http://qw.shxzskj.cn

================================================================================
来源：http://di.huixiangedu.cn

按语言统计（条）：
来源：http://br.huixiangedu.cn

Python ......... 252
来源：http://zz.shxzukj.cn

PHP ............ 252
来源：http://ng.chemitech.net.cn

JavaScript ..... 252
来源：http://jm.lnxyls.cn

TypeScript ..... 212
来源：http://im.panjiajie.cn

Java ........... 212
来源：http://vf.lnxyls.cn

Go ............. 212
来源：http://ml.bookmarksfly.cn

Ruby ........... 212
来源：http://gf.yuntaijiaju.cn

C# ............. 212
来源：http://rb.chemitech.net.cn

C .............. 30
来源：http://ua.szsharing.cn

C++ ............ 30
来源：http://ts.jctech888.com.cn

SQL ............ 90
来源：http://pq.9csxet.cn

Bash ........... 80
来源：http://ll.9csxet.cn

Kotlin ......... 15
来源：http://nz.nicolike.cn

Swift .......... 15
来源：http://rc.nszjky.cn

Lua ............ 10
来源：http://ic.shtwfgs.cn

Perl ........... 10
来源：http://jw.jctech888.com.cn

Scala .......... 10
来源：http://cl.yuntaijiaju.cn

------------------------------------
来源：http://sx.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://ez.hahajie.cn

按章节统计：
来源：http://fb.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ua.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vf.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bv.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mj.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ja.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xs.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hv.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pt.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jb.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kv.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ji.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ul.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fz.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://di.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qz.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nm.bookmarksfly.cn

Q SQL 专题                              90
来源：http://gw.shtwfgs.cn

R Bash 专题                             80
来源：http://sf.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://mi.huanxung.cn

T 其他语言补充                          60
来源：http://mc.bookmarksfly.cn

U 高频实用片段                         120
来源：http://gc.bjjhwx.cn

------------------------------------
来源：http://do.gzmigu.cn

合计                                  2106 条
来源：http://ak.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://te.asd995.cn

使用提醒
来源：http://hh.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ne.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gi.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mh.nszjky.cn


<!-- 参考信息 -->