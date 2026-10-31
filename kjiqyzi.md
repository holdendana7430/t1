代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://sc.hahajie.cn

[T59] Scala：循环
来源：http://ry.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://yw.yuexingan06.cn

[T60] Scala：折叠
来源：http://pk.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yi.gzmigu.cn

================================================================================
来源：http://yv.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sv.jianghongdianzi.cn

================================================================================
来源：http://of.521024.cn

[U01] Py：创建虚拟环境
来源：http://we.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cr.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://bp.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gi.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://qq.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zy.szsharing.cn

[U04] Py：变量调试打印
来源：http://we.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sk.nicolike.cn

[U05] Py：列表去重且保序
来源：http://dz.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://kc.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://po.hahajie.cn

{**a, **b}
来源：http://pv.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://if.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://bi.nszjky.cn

[U08] Py：展平二维列表
来源：http://dy.nszjky.cn

[y for x in nested for y in x]
来源：http://xm.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://by.gzmigu.cn

max(d, key=d.get)
来源：http://oo.szxytkj.cn

[U10] Py：按值排序字典
来源：http://ly.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://md.szsharing.cn

[U11] Py：生成器表达式
来源：http://vi.lnxyls.cn

(x * 2 for x in arr)
来源：http://qy.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eb.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://hq.hnjuh.cn

[U13] Py：固定长度队列
来源：http://fm.wgjwhj.cn

deque(maxlen=10)
来源：http://xd.asd995.cn

[U14] Py：分组收集到列表
来源：http://dw.bookmarksfly.cn

defaultdict(list)
来源：http://pb.chemitech.net.cn

[U15] Py：高精度计时
来源：http://gj.nszjky.cn

t = time.perf_counter()
来源：http://mf.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://op.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oi.wgjwhj.cn

[U17] Py：初始化日志
来源：http://ju.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://bz.shxzskj.cn

[U18] Py：预编译正则
来源：http://mk.nszjky.cn

pat = re.compile(r"\d+")
来源：http://vd.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://hk.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xo.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://bf.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://sx.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://sz.asd995.cn

@contextlib.contextmanager
来源：http://bm.521024.cn

[U22] Py：矩阵转置
来源：http://on.9csxet.cn

list(zip(*m))
来源：http://in.szsharing.cn

[U23] Py：分块读取大文件
来源：http://rq.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qk.521024.cn

[U24] Py：路径操作
来源：http://wn.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ow.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://ky.lnxyls.cn

csv.DictReader(f)
来源：http://qj.newstarts.cn

[U26] Py：并发下载
来源：http://iy.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yp.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://ow.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://bf.gzmigu.cn

[U28] Py：类型别名
来源：http://tt.nicolike.cn

UserId = int
来源：http://wi.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://xx.hahajie.cn

@property 与 @x.setter 配合
来源：http://ol.shxzukj.cn

[U30] Py：数据类
来源：http://wu.panjiajie.cn

@dataclass(slots=True)
来源：http://qm.huanxung.cn

[U31] Py：单测
来源：http://yh.9csxet.cn

python -m pytest -q
来源：http://pn.szxytkj.cn

[U32] Py：代码格式化
来源：http://kd.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://fs.wgjwhj.cn

[U33] Py：打包发布
来源：http://am.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://yl.bjjhwx.cn

[U34] Py：判断编码
来源：http://xm.wgjwhj.cn

chardet.detect(raw)
来源：http://zl.yuexingan06.cn

[U35] Py：发送邮件
来源：http://jo.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pg.hahajie.cn

[U36] Py：定时任务
来源：http://wl.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://np.lnxyls.cn

[U37] Py：读写 Excel
来源：http://hu.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rx.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://nb.hahajie.cn

Path(__file__).resolve().parent
来源：http://cu.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://qv.521024.cn

sys.stdout.isatty()
来源：http://tv.nszjky.cn

[U40] Py：打印到标准错误
来源：http://xi.nszjky.cn

print("err", file=sys.stderr)
来源：http://oi.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://sr.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ra.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://yo.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hr.newstarts.cn

[U43] PHP：声明命名空间
来源：http://zv.asd995.cn

namespace App\Http;
来源：http://gn.nicolike.cn

[U44] PHP：开启严格类型
来源：http://th.huanxung.cn

declare(strict_types=1);
来源：http://nh.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://lt.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ov.gzmigu.cn

[U46] PHP：可空类型
来源：http://dp.asd995.cn

?string $name = null
来源：http://rr.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://ta.nszjky.cn

int|string $id
来源：http://yd.shxzskj.cn

[U48] PHP：纯枚举
来源：http://zd.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wv.shxzskj.cn

[U49] PHP：只读属性
来源：http://yx.szxytkj.cn

public readonly string $name
来源：http://zh.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://jj.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://jn.nszjky.cn

[U51] PHP：数组解构
来源：http://nz.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://eg.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://iv.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://qr.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://dx.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://xd.hnjuh.cn

[U54] PHP：空安全调用
来源：http://dt.lnxyls.cn

$obj?->method()
来源：http://cy.hnjuh.cn

[U55] PHP：match 表达式
来源：http://he.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ne.chemitech.net.cn

[U56] PHP：命名参数
来源：http://ss.521024.cn

f(a: 1, b: 2)
来源：http://bf.colortex.cn

[U57] PHP：字符串插值
来源：http://wz.yuntaijiaju.cn

"值: {$a}"
来源：http://lu.szsharing.cn

[U58] PHP：数组三件套
来源：http://cz.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://si.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://uo.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cs.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://pb.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vt.gzmigu.cn

[U61] PHP：正则
来源：http://fi.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gl.asd995.cn

[U62] PHP：日期对象
来源：http://hx.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ye.lnxyls.cn

[U63] PHP：文件读写
来源：http://mh.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xa.lnxyls.cn

[U64] PHP：目录遍历
来源：http://vj.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://qi.gzmigu.cn

[U65] PHP：会话
来源：http://de.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ll.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://se.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://od.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://rb.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wq.nszjky.cn

[U68] PHP：PDO 连接
来源：http://uo.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cv.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://mu.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bn.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://wf.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://am.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://bz.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://fk.newstarts.cn

[U72] PHP：写错误日志
来源：http://rw.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://vp.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://ls.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://wc.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://fw.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://oy.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://fy.chemitech.net.cn

composer require psr/container
来源：http://zz.hahajie.cn

[U76] PHP：简单路由
来源：http://ew.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yi.asd995.cn

[U77] PHP：模板渲染
来源：http://io.jctech888.com.cn

composer require twig/twig
来源：http://ty.chemitech.net.cn

[U78] PHP：单元测试
来源：http://pv.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://yr.9csxet.cn

[U79] PHP：静态分析
来源：http://kr.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://yv.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://xh.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tf.haigaiapp.cn

[U81] JS：初始化项目
来源：http://ln.szxytkj.cn

npm init -y;  npm i express
来源：http://ea.newstarts.cn

[U82] JS：package.json 脚本
来源：http://uj.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qb.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://cx.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://de.colortex.cn

[U84] JS：CommonJS 写法
来源：http://az.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uz.szxytkj.cn

[U85] JS：可选链
来源：http://tm.bjjhwx.cn

a?.b?.c
来源：http://wf.chemitech.net.cn

[U86] JS：空值合并
来源：http://ef.asd995.cn

a ?? b
来源：http://fi.hnjuh.cn

[U87] JS：解构默认值
来源：http://rg.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://pz.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://dj.asd995.cn

{ ...a, ...b }
来源：http://gb.yuexingan06.cn

[U89] JS：数组去重
来源：http://ut.bjjhwx.cn

[...new Set(arr)]
来源：http://or.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://qm.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://kx.nicolike.cn

[U91] JS：对象键值遍历
来源：http://rk.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://li.chemitech.net.cn

[U92] JS：深拷贝
来源：http://gn.gzmigu.cn

structuredClone(obj)
来源：http://xr.gzmigu.cn

[U93] JS：模板字符串
来源：http://yw.jctech888.com.cn

`共 ${n} 条`
来源：http://de.szsharing.cn

[U94] JS：箭头函数
来源：http://mj.bookmarksfly.cn

const double = x => x * 2;
来源：http://pz.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://jk.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://lr.9csxet.cn

[U96] JS：async/await 与异常
来源：http://ns.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nx.shxzskj.cn

[U97] JS：并发请求
来源：http://cr.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ax.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://va.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hp.521024.cn

[U99] JS：事件监听
来源：http://lj.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://yr.szxytkj.cn

[U100] JS：DOM 查询
来源：http://zw.hnjuh.cn

document.querySelector(".item")
来源：http://co.haigaiapp.cn

[U101] JS：classList 操作
来源：http://ua.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://ck.hnjuh.cn

[U102] JS：本地存储
来源：http://xw.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gy.newstarts.cn

[U103] JS：定时器
来源：http://qt.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fy.huixinmuqiang.cn

[U104] JS：防抖
来源：http://iv.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://id.asd995.cn

[U105] JS：节流
来源：http://bo.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ck.szxytkj.cn

[U106] JS：日期格式化
来源：http://qr.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ay.chemitech.net.cn

[U107] JS：数字千分位
来源：http://oh.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vk.chemitech.net.cn

[U108] JS：随机整数
来源：http://cn.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://id.bjjhwx.cn

[U109] JS：数组分组
来源：http://fl.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://ct.huixiangedu.cn

[U110] JS：数组分块
来源：http://qq.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lo.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://li.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://cx.newstarts.cn

[U112] JS：字符串补位
来源：http://lh.nicolike.cn

"7".padStart(3, "0")
来源：http://xv.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://te.9csxet.cn

s.replaceAll("a", "b")
来源：http://kb.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://bc.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bn.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://rt.chemitech.net.cn

crypto.randomUUID()
来源：http://qi.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://bk.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://hn.shtwfgs.cn

[U117] JS：单元测试
来源：http://ra.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://cv.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://ce.gzmigu.cn

npm i -D vite;  npx vite
来源：http://xx.shxzskj.cn

[U119] JS：生产构建
来源：http://eq.huixiangedu.cn

npx vite build
来源：http://gk.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://sz.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://gz.jctech888.com.cn

================================================================================
来源：http://pr.wgjwhj.cn

统计汇总
来源：http://nt.yuntaijiaju.cn

================================================================================
来源：http://in.yuntaijiaju.cn

按语言统计（条）：
来源：http://og.newstarts.cn

Python ......... 252
来源：http://ea.bjjhwx.cn

PHP ............ 252
来源：http://xk.9csxet.cn

JavaScript ..... 252
来源：http://xt.colortex.cn

TypeScript ..... 212
来源：http://ut.shxzukj.cn

Java ........... 212
来源：http://ei.bookmarksfly.cn

Go ............. 212
来源：http://cg.9csxet.cn

Ruby ........... 212
来源：http://ek.nicolike.cn

C# ............. 212
来源：http://kw.haigaiapp.cn

C .............. 30
来源：http://gi.gzmigu.cn

C++ ............ 30
来源：http://vh.lnxyls.cn

SQL ............ 90
来源：http://vu.gzmigu.cn

Bash ........... 80
来源：http://ho.yuexingan06.cn

Kotlin ......... 15
来源：http://su.jianghongdianzi.cn

Swift .......... 15
来源：http://uv.huixinmuqiang.cn

Lua ............ 10
来源：http://uq.9csxet.cn

Perl ........... 10
来源：http://df.asd995.cn

Scala .......... 10
来源：http://fl.hahajie.cn

------------------------------------
来源：http://it.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://oc.colortex.cn

按章节统计：
来源：http://zs.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ul.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bn.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rn.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cq.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ky.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vj.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zi.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xb.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://by.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ro.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hy.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ss.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nv.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kn.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dz.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pp.521024.cn

Q SQL 专题                              90
来源：http://ja.shtwfgs.cn

R Bash 专题                             80
来源：http://bo.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://nb.521024.cn

T 其他语言补充                          60
来源：http://nj.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://im.bookmarksfly.cn

------------------------------------
来源：http://lv.lnxyls.cn

合计                                  2106 条
来源：http://rm.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://dj.huixinmuqiang.cn

使用提醒
来源：http://oc.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://kh.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vi.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ku.haigaiapp.cn


<!-- 参考信息 -->