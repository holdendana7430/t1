代发 wailian999

case class User(name: String, age: Int)
来源：http://lw.asd995.cn

[T57] Scala：模式匹配
来源：http://dc.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lj.gzmigu.cn

[T58] Scala：函数定义
来源：http://gf.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ep.bjjhwx.cn

[T59] Scala：循环
来源：http://yd.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://op.newstarts.cn

[T60] Scala：折叠
来源：http://zo.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ae.lnxyls.cn

================================================================================
来源：http://nw.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fn.chemitech.net.cn

================================================================================
来源：http://na.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://ml.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lo.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://wl.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nj.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://iu.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ff.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://md.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://me.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://iz.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://rc.shxzukj.cn

[U06] Py：合并两个字典
来源：http://cx.shxzukj.cn

{**a, **b}
来源：http://gk.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://kr.9csxet.cn

{v: k for k, v in d.items()}
来源：http://zc.szxytkj.cn

[U08] Py：展平二维列表
来源：http://jt.huixiangedu.cn

[y for x in nested for y in x]
来源：http://wg.asd995.cn

[U09] Py：字典取最大值的键
来源：http://mf.muxihuayi.cn

max(d, key=d.get)
来源：http://qd.huanxung.cn

[U10] Py：按值排序字典
来源：http://vq.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yc.521024.cn

[U11] Py：生成器表达式
来源：http://zc.szsharing.cn

(x * 2 for x in arr)
来源：http://fo.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zd.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://aa.hahajie.cn

[U13] Py：固定长度队列
来源：http://zw.wgjwhj.cn

deque(maxlen=10)
来源：http://gt.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://sm.bookmarksfly.cn

defaultdict(list)
来源：http://yh.bjjhwx.cn

[U15] Py：高精度计时
来源：http://oq.szxytkj.cn

t = time.perf_counter()
来源：http://kw.9csxet.cn

[U16] Py：命令行参数解析
来源：http://uc.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ge.shtwfgs.cn

[U17] Py：初始化日志
来源：http://jq.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://sj.colortex.cn

[U18] Py：预编译正则
来源：http://wp.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://az.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://vh.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pw.nicolike.cn

[U20] Py：缓存函数结果
来源：http://cv.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://md.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://yy.jctech888.com.cn

@contextlib.contextmanager
来源：http://wv.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://hs.nicolike.cn

list(zip(*m))
来源：http://rc.9csxet.cn

[U23] Py：分块读取大文件
来源：http://ur.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uy.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://pc.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yr.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://el.newstarts.cn

csv.DictReader(f)
来源：http://cm.bookmarksfly.cn

[U26] Py：并发下载
来源：http://tr.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ng.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://gy.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://hg.nszjky.cn

[U28] Py：类型别名
来源：http://pe.huixinmuqiang.cn

UserId = int
来源：http://kd.shtwfgs.cn

[U29] Py：属性校验
来源：http://ln.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://iy.hahajie.cn

[U30] Py：数据类
来源：http://rh.shxzskj.cn

@dataclass(slots=True)
来源：http://ho.szsharing.cn

[U31] Py：单测
来源：http://eq.wgjwhj.cn

python -m pytest -q
来源：http://da.szsharing.cn

[U32] Py：代码格式化
来源：http://pw.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://yp.szsharing.cn

[U33] Py：打包发布
来源：http://dj.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ca.shxzskj.cn

[U34] Py：判断编码
来源：http://wh.jianghongdianzi.cn

chardet.detect(raw)
来源：http://rt.shtwfgs.cn

[U35] Py：发送邮件
来源：http://rt.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ge.huanxung.cn

[U36] Py：定时任务
来源：http://am.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://tt.szsharing.cn

[U37] Py：读写 Excel
来源：http://vr.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oi.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://yt.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ww.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://vu.huanxung.cn

sys.stdout.isatty()
来源：http://zx.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://qp.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://iw.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://cj.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yt.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://tg.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mo.nszjky.cn

[U43] PHP：声明命名空间
来源：http://dq.bookmarksfly.cn

namespace App\Http;
来源：http://um.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://na.yuexingan06.cn

declare(strict_types=1);
来源：http://ct.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://sx.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.hahajie.cn

[U46] PHP：可空类型
来源：http://lu.nicolike.cn

?string $name = null
来源：http://nt.szxytkj.cn

[U47] PHP：联合类型
来源：http://yt.nszjky.cn

int|string $id
来源：http://mb.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://br.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bo.jctech888.com.cn

[U49] PHP：只读属性
来源：http://pn.haigaiapp.cn

public readonly string $name
来源：http://lt.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://nv.9csxet.cn

public function __construct(private int $id) {}
来源：http://kt.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://pn.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ao.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://wh.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://oa.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://tq.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://sy.521024.cn

[U54] PHP：空安全调用
来源：http://lg.hnjuh.cn

$obj?->method()
来源：http://up.colortex.cn

[U55] PHP：match 表达式
来源：http://fq.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zh.lnxyls.cn

[U56] PHP：命名参数
来源：http://zr.shxzukj.cn

f(a: 1, b: 2)
来源：http://kd.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://td.bookmarksfly.cn

"值: {$a}"
来源：http://gw.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://je.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qv.lnxyls.cn

[U59] PHP：自定义排序
来源：http://yc.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nm.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://tj.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xz.shtwfgs.cn

[U61] PHP：正则
来源：http://ro.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kh.haigaiapp.cn

[U62] PHP：日期对象
来源：http://kr.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uw.szxytkj.cn

[U63] PHP：文件读写
来源：http://ni.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xl.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://bt.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://qm.asd995.cn

[U65] PHP：会话
来源：http://ii.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zv.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://ln.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tj.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://vn.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qv.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://pm.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sj.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://jd.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wb.nicolike.cn

[U70] PHP：PDO 事务
来源：http://fw.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ws.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://by.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://dy.521024.cn

[U72] PHP：写错误日志
来源：http://kx.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://dg.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://nj.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://bs.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://ca.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://hk.panjiajie.cn

[U75] PHP：依赖注入
来源：http://dl.shtwfgs.cn

composer require psr/container
来源：http://ly.colortex.cn

[U76] PHP：简单路由
来源：http://ut.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sr.colortex.cn

[U77] PHP：模板渲染
来源：http://hq.panjiajie.cn

composer require twig/twig
来源：http://wz.lnxyls.cn

[U78] PHP：单元测试
来源：http://wr.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://fb.asd995.cn

[U79] PHP：静态分析
来源：http://mp.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://jk.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://un.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jk.9csxet.cn

[U81] JS：初始化项目
来源：http://gu.9csxet.cn

npm init -y;  npm i express
来源：http://sr.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://de.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nv.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://bj.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qp.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://zy.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lm.9csxet.cn

[U85] JS：可选链
来源：http://qu.colortex.cn

a?.b?.c
来源：http://qi.wgjwhj.cn

[U86] JS：空值合并
来源：http://xv.wgjwhj.cn

a ?? b
来源：http://dx.hnjuh.cn

[U87] JS：解构默认值
来源：http://au.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://te.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://xa.jctech888.com.cn

{ ...a, ...b }
来源：http://ol.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://rj.yuexingan06.cn

[...new Set(arr)]
来源：http://lr.nszjky.cn

[U90] JS：数字数组排序
来源：http://er.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://yb.huanxung.cn

[U91] JS：对象键值遍历
来源：http://xj.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ss.huixiangedu.cn

[U92] JS：深拷贝
来源：http://xj.yuexingan06.cn

structuredClone(obj)
来源：http://df.9csxet.cn

[U93] JS：模板字符串
来源：http://ay.asd995.cn

`共 ${n} 条`
来源：http://cr.asd995.cn

[U94] JS：箭头函数
来源：http://of.muxihuayi.cn

const double = x => x * 2;
来源：http://gf.colortex.cn

[U95] JS：Promise 包装
来源：http://nb.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://cv.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://sl.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ly.panjiajie.cn

[U97] JS：并发请求
来源：http://dm.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bk.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://sd.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hu.nszjky.cn

[U99] JS：事件监听
来源：http://bc.nszjky.cn

el.addEventListener("click", e => {})
来源：http://pm.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://ki.huanxung.cn

document.querySelector(".item")
来源：http://eo.shxzukj.cn

[U101] JS：classList 操作
来源：http://jx.nicolike.cn

el.classList.toggle("active")
来源：http://ff.colortex.cn

[U102] JS：本地存储
来源：http://rz.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oi.nicolike.cn

[U103] JS：定时器
来源：http://pj.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://je.szxytkj.cn

[U104] JS：防抖
来源：http://qu.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zz.shxzukj.cn

[U105] JS：节流
来源：http://gn.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qm.lnxyls.cn

[U106] JS：日期格式化
来源：http://mj.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uq.szsharing.cn

[U107] JS：数字千分位
来源：http://zq.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qc.shtwfgs.cn

[U108] JS：随机整数
来源：http://zm.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fr.wgjwhj.cn

[U109] JS：数组分组
来源：http://ij.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ch.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://nj.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zk.colortex.cn

[U111] JS：对象转 Map
来源：http://rm.shxzukj.cn

new Map(Object.entries(obj))
来源：http://gi.hahajie.cn

[U112] JS：字符串补位
来源：http://aq.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://du.panjiajie.cn

[U113] JS：正则替换全部
来源：http://os.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://yq.nicolike.cn

[U114] JS：JSON 深比较
来源：http://xb.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dp.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://wl.bookmarksfly.cn

crypto.randomUUID()
来源：http://go.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://fm.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://nc.hahajie.cn

[U117] JS：单元测试
来源：http://gm.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://qt.nszjky.cn

[U118] JS：开发服务器
来源：http://ww.newstarts.cn

npm i -D vite;  npx vite
来源：http://wn.bjjhwx.cn

[U119] JS：生产构建
来源：http://al.szxytkj.cn

npx vite build
来源：http://rc.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://xs.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://iv.jctech888.com.cn

================================================================================
来源：http://pl.shxzskj.cn

统计汇总
来源：http://id.chemitech.net.cn

================================================================================
来源：http://id.szxytkj.cn

按语言统计（条）：
来源：http://wv.huixiangedu.cn

Python ......... 252
来源：http://ws.lnxyls.cn

PHP ............ 252
来源：http://ik.muxihuayi.cn

JavaScript ..... 252
来源：http://du.jianghongdianzi.cn

TypeScript ..... 212
来源：http://xc.521024.cn

Java ........... 212
来源：http://zl.jctech888.com.cn

Go ............. 212
来源：http://vh.haigaiapp.cn

Ruby ........... 212
来源：http://zm.jctech888.com.cn

C# ............. 212
来源：http://xp.bjjhwx.cn

C .............. 30
来源：http://ga.huixinmuqiang.cn

C++ ............ 30
来源：http://ir.nicolike.cn

SQL ............ 90
来源：http://km.yuexingan06.cn

Bash ........... 80
来源：http://zp.wgjwhj.cn

Kotlin ......... 15
来源：http://da.huanxung.cn

Swift .......... 15
来源：http://nm.jianghongdianzi.cn

Lua ............ 10
来源：http://ew.hnjuh.cn

Perl ........... 10
来源：http://wb.panjiajie.cn

Scala .......... 10
来源：http://sm.jianghongdianzi.cn

------------------------------------
来源：http://ii.shtwfgs.cn

合计 ........... 2106 条
来源：http://cr.yuntaijiaju.cn

按章节统计：
来源：http://jh.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zz.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vq.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uj.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zi.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jq.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://he.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://np.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dp.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yg.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pt.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hd.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vs.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uu.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wt.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dj.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ad.huanxung.cn

Q SQL 专题                              90
来源：http://za.hnjuh.cn

R Bash 专题                             80
来源：http://ny.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://xx.nicolike.cn

T 其他语言补充                          60
来源：http://xt.9csxet.cn

U 高频实用片段                         120
来源：http://jw.muxihuayi.cn

------------------------------------
来源：http://ox.hahajie.cn

合计                                  2106 条
来源：http://ao.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://kr.hahajie.cn


<!-- 参考信息 -->