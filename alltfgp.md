代发 wailian999

val a = 1;  var b = 2
来源：http://er.lnxyls.cn

[T53] Scala：字符串插值
来源：http://cu.shxzskj.cn

s"值: $b"
来源：http://pv.muxihuayi.cn

[T54] Scala：集合映射
来源：http://hh.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://vb.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://if.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pp.nicolike.cn

[T56] Scala：样例类
来源：http://nf.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://zl.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://th.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sf.asd995.cn

[T58] Scala：函数定义
来源：http://cw.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hl.bjjhwx.cn

[T59] Scala：循环
来源：http://mg.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://kt.colortex.cn

[T60] Scala：折叠
来源：http://ni.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ub.colortex.cn

================================================================================
来源：http://zs.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xu.lnxyls.cn

================================================================================
来源：http://bw.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://cw.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ir.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://aw.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lx.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ku.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cq.huanxung.cn

[U04] Py：变量调试打印
来源：http://eq.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mc.szsharing.cn

[U05] Py：列表去重且保序
来源：http://lo.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://zz.szsharing.cn

[U06] Py：合并两个字典
来源：http://uo.huixinmuqiang.cn

{**a, **b}
来源：http://hd.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://yw.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ul.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://hy.jctech888.com.cn

[y for x in nested for y in x]
来源：http://dp.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ox.521024.cn

max(d, key=d.get)
来源：http://wy.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://wo.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fu.nszjky.cn

[U11] Py：生成器表达式
来源：http://dv.gzmigu.cn

(x * 2 for x in arr)
来源：http://xw.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nn.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://od.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://ih.gzmigu.cn

deque(maxlen=10)
来源：http://rg.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://or.panjiajie.cn

defaultdict(list)
来源：http://zi.jctech888.com.cn

[U15] Py：高精度计时
来源：http://sn.huixinmuqiang.cn

t = time.perf_counter()
来源：http://zb.szsharing.cn

[U16] Py：命令行参数解析
来源：http://rl.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bx.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://cv.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://uf.nszjky.cn

[U18] Py：预编译正则
来源：http://rk.nicolike.cn

pat = re.compile(r"\d+")
来源：http://oa.asd995.cn

[U19] Py：正则替换带回调
来源：http://se.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rm.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ew.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://pb.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://rf.colortex.cn

@contextlib.contextmanager
来源：http://iy.gzmigu.cn

[U22] Py：矩阵转置
来源：http://fy.haigaiapp.cn

list(zip(*m))
来源：http://rf.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://et.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tm.gzmigu.cn

[U24] Py：路径操作
来源：http://xq.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oe.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://kf.newstarts.cn

csv.DictReader(f)
来源：http://yy.wgjwhj.cn

[U26] Py：并发下载
来源：http://rn.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yb.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://sr.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://pg.newstarts.cn

[U28] Py：类型别名
来源：http://cn.jianghongdianzi.cn

UserId = int
来源：http://cp.wgjwhj.cn

[U29] Py：属性校验
来源：http://xj.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://ku.huanxung.cn

[U30] Py：数据类
来源：http://vs.shxzukj.cn

@dataclass(slots=True)
来源：http://vt.colortex.cn

[U31] Py：单测
来源：http://sa.jianghongdianzi.cn

python -m pytest -q
来源：http://mi.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://mg.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://za.colortex.cn

[U33] Py：打包发布
来源：http://mh.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://jc.chemitech.net.cn

[U34] Py：判断编码
来源：http://qi.shtwfgs.cn

chardet.detect(raw)
来源：http://ej.nszjky.cn

[U35] Py：发送邮件
来源：http://yz.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gs.muxihuayi.cn

[U36] Py：定时任务
来源：http://rv.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://qu.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://hs.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lg.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://dn.asd995.cn

Path(__file__).resolve().parent
来源：http://xv.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://kv.panjiajie.cn

sys.stdout.isatty()
来源：http://dl.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://cd.nicolike.cn

print("err", file=sys.stderr)
来源：http://ed.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://zr.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ql.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://kr.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xw.9csxet.cn

[U43] PHP：声明命名空间
来源：http://gb.gzmigu.cn

namespace App\Http;
来源：http://zr.szsharing.cn

[U44] PHP：开启严格类型
来源：http://ir.szsharing.cn

declare(strict_types=1);
来源：http://eo.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://es.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nf.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://nb.huanxung.cn

?string $name = null
来源：http://fs.shxzukj.cn

[U47] PHP：联合类型
来源：http://pv.muxihuayi.cn

int|string $id
来源：http://vx.nicolike.cn

[U48] PHP：纯枚举
来源：http://as.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ll.521024.cn

[U49] PHP：只读属性
来源：http://tl.lnxyls.cn

public readonly string $name
来源：http://hx.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://uk.nicolike.cn

public function __construct(private int $id) {}
来源：http://ay.haigaiapp.cn

[U51] PHP：数组解构
来源：http://lo.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ta.nszjky.cn

[U52] PHP：箭头函数
来源：http://zz.521024.cn

$double = fn($x) => $x * 2;
来源：http://ms.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ab.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://jw.gzmigu.cn

[U54] PHP：空安全调用
来源：http://oc.szxytkj.cn

$obj?->method()
来源：http://aw.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://nj.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lg.bjjhwx.cn

[U56] PHP：命名参数
来源：http://uy.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://xr.szsharing.cn

[U57] PHP：字符串插值
来源：http://li.asd995.cn

"值: {$a}"
来源：http://ty.hnjuh.cn

[U58] PHP：数组三件套
来源：http://rc.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cc.asd995.cn

[U59] PHP：自定义排序
来源：http://el.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yk.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://fo.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yx.huixinmuqiang.cn

[U61] PHP：正则
来源：http://sh.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vc.jctech888.com.cn

[U62] PHP：日期对象
来源：http://br.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cp.shxzukj.cn

[U63] PHP：文件读写
来源：http://aa.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gq.szsharing.cn

[U64] PHP：目录遍历
来源：http://fj.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://mw.hahajie.cn

[U65] PHP：会话
来源：http://ud.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ap.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://ll.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jf.hahajie.cn

[U67] PHP：处理文件上传
来源：http://eg.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://te.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://xv.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mo.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://zx.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ju.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://ff.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lg.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://dg.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://oz.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://rr.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://et.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://to.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://cq.newstarts.cn

[U74] PHP：读取环境变量
来源：http://we.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://kn.gzmigu.cn

[U75] PHP：依赖注入
来源：http://fa.muxihuayi.cn

composer require psr/container
来源：http://yp.huanxung.cn

[U76] PHP：简单路由
来源：http://xd.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gh.hahajie.cn

[U77] PHP：模板渲染
来源：http://tt.hahajie.cn

composer require twig/twig
来源：http://uz.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://va.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://rc.asd995.cn

[U79] PHP：静态分析
来源：http://ke.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://yr.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://si.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zh.nicolike.cn

[U81] JS：初始化项目
来源：http://ih.nicolike.cn

npm init -y;  npm i express
来源：http://oj.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://mq.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vl.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://hn.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vc.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://ya.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kj.yuexingan06.cn

[U85] JS：可选链
来源：http://dx.nicolike.cn

a?.b?.c
来源：http://hr.bjjhwx.cn

[U86] JS：空值合并
来源：http://cd.521024.cn

a ?? b
来源：http://aj.asd995.cn

[U87] JS：解构默认值
来源：http://dx.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://py.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://uk.colortex.cn

{ ...a, ...b }
来源：http://hm.haigaiapp.cn

[U89] JS：数组去重
来源：http://ti.yuexingan06.cn

[...new Set(arr)]
来源：http://it.shxzukj.cn

[U90] JS：数字数组排序
来源：http://aj.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://uy.nicolike.cn

[U91] JS：对象键值遍历
来源：http://hn.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bb.nicolike.cn

[U92] JS：深拷贝
来源：http://we.jianghongdianzi.cn

structuredClone(obj)
来源：http://oa.haigaiapp.cn

[U93] JS：模板字符串
来源：http://pc.nicolike.cn

`共 ${n} 条`
来源：http://dy.shtwfgs.cn

[U94] JS：箭头函数
来源：http://sk.nszjky.cn

const double = x => x * 2;
来源：http://gq.gzmigu.cn

[U95] JS：Promise 包装
来源：http://ap.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://ci.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://np.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fb.shxzukj.cn

[U97] JS：并发请求
来源：http://no.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://my.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://vy.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uv.chemitech.net.cn

[U99] JS：事件监听
来源：http://wo.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://yt.szsharing.cn

[U100] JS：DOM 查询
来源：http://pu.asd995.cn

document.querySelector(".item")
来源：http://wi.wgjwhj.cn

[U101] JS：classList 操作
来源：http://mv.huixiangedu.cn

el.classList.toggle("active")
来源：http://vn.hahajie.cn

[U102] JS：本地存储
来源：http://cn.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cm.9csxet.cn

[U103] JS：定时器
来源：http://uq.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gt.shxzskj.cn

[U104] JS：防抖
来源：http://ut.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ry.bjjhwx.cn

[U105] JS：节流
来源：http://zt.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xr.muxihuayi.cn

[U106] JS：日期格式化
来源：http://hu.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iy.colortex.cn

[U107] JS：数字千分位
来源：http://pl.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mo.chemitech.net.cn

[U108] JS：随机整数
来源：http://iv.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fm.huixiangedu.cn

[U109] JS：数组分组
来源：http://ep.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://mt.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ft.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ug.szxytkj.cn

[U111] JS：对象转 Map
来源：http://fp.nszjky.cn

new Map(Object.entries(obj))
来源：http://gx.panjiajie.cn

[U112] JS：字符串补位
来源：http://ib.hnjuh.cn

"7".padStart(3, "0")
来源：http://dp.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://wb.lnxyls.cn

s.replaceAll("a", "b")
来源：http://jv.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://wa.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sn.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://fg.szxytkj.cn

crypto.randomUUID()
来源：http://br.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://yt.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://en.bjjhwx.cn

[U117] JS：单元测试
来源：http://th.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://gi.newstarts.cn

[U118] JS：开发服务器
来源：http://bw.shxzukj.cn

npm i -D vite;  npx vite
来源：http://fc.bjjhwx.cn

[U119] JS：生产构建
来源：http://so.shtwfgs.cn

npx vite build
来源：http://bt.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://hj.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://ds.nicolike.cn

================================================================================
来源：http://nt.shxzukj.cn

统计汇总
来源：http://kw.muxihuayi.cn

================================================================================
来源：http://dr.haigaiapp.cn

按语言统计（条）：
来源：http://gi.haigaiapp.cn

Python ......... 252
来源：http://oy.haigaiapp.cn

PHP ............ 252
来源：http://tu.yuexingan06.cn

JavaScript ..... 252
来源：http://cv.huixiangedu.cn

TypeScript ..... 212
来源：http://kb.colortex.cn

Java ........... 212
来源：http://lf.huixiangedu.cn

Go ............. 212
来源：http://rm.shxzskj.cn

Ruby ........... 212
来源：http://rm.muxihuayi.cn

C# ............. 212
来源：http://jm.szsharing.cn

C .............. 30
来源：http://cp.9csxet.cn

C++ ............ 30
来源：http://mk.hnjuh.cn

SQL ............ 90
来源：http://so.nszjky.cn

Bash ........... 80
来源：http://uk.bjjhwx.cn

Kotlin ......... 15
来源：http://rw.jianghongdianzi.cn

Swift .......... 15
来源：http://ms.newstarts.cn

Lua ............ 10
来源：http://vf.hahajie.cn

Perl ........... 10
来源：http://sp.yuexingan06.cn

Scala .......... 10
来源：http://qu.jctech888.com.cn

------------------------------------
来源：http://hv.huanxung.cn

合计 ........... 2106 条
来源：http://dh.521024.cn

按章节统计：
来源：http://xc.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yg.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qx.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vo.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iy.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sf.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dv.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://im.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kg.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://es.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gl.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xb.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cr.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zr.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dm.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xh.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kp.newstarts.cn


<!-- 参考信息 -->