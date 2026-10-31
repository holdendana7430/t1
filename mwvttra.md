代发 wailian999

val a = 1;  var b = 2
来源：http://jt.colortex.cn

[T53] Scala：字符串插值
来源：http://sm.9csxet.cn

s"值: $b"
来源：http://kd.9csxet.cn

[T54] Scala：集合映射
来源：http://lp.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ne.asd995.cn

[T55] Scala：集合过滤
来源：http://qr.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fj.9csxet.cn

[T56] Scala：样例类
来源：http://au.panjiajie.cn

case class User(name: String, age: Int)
来源：http://jd.colortex.cn

[T57] Scala：模式匹配
来源：http://fo.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cj.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://pp.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ap.panjiajie.cn

[T59] Scala：循环
来源：http://bf.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://xi.hnjuh.cn

[T60] Scala：折叠
来源：http://gz.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hp.nszjky.cn

================================================================================
来源：http://en.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ga.chemitech.net.cn

================================================================================
来源：http://io.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://rr.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hn.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://dy.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jb.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://mk.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dp.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://ys.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pi.colortex.cn

[U05] Py：列表去重且保序
来源：http://en.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://gm.hahajie.cn

[U06] Py：合并两个字典
来源：http://wt.asd995.cn

{**a, **b}
来源：http://ht.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://vb.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://yb.nicolike.cn

[U08] Py：展平二维列表
来源：http://xr.asd995.cn

[y for x in nested for y in x]
来源：http://qo.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://ke.yuexingan06.cn

max(d, key=d.get)
来源：http://cy.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ge.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uk.huanxung.cn

[U11] Py：生成器表达式
来源：http://vg.shtwfgs.cn

(x * 2 for x in arr)
来源：http://ni.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://el.nszjky.cn

Counter(arr).most_common(3)
来源：http://ds.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://oo.shtwfgs.cn

deque(maxlen=10)
来源：http://hi.newstarts.cn

[U14] Py：分组收集到列表
来源：http://ej.yuntaijiaju.cn

defaultdict(list)
来源：http://lf.szxytkj.cn

[U15] Py：高精度计时
来源：http://dn.hnjuh.cn

t = time.perf_counter()
来源：http://mw.hahajie.cn

[U16] Py：命令行参数解析
来源：http://dx.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pe.9csxet.cn

[U17] Py：初始化日志
来源：http://sp.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://zn.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://ie.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://li.asd995.cn

[U19] Py：正则替换带回调
来源：http://mh.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wh.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://vw.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://bb.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ib.huanxung.cn

@contextlib.contextmanager
来源：http://xr.asd995.cn

[U22] Py：矩阵转置
来源：http://er.gzmigu.cn

list(zip(*m))
来源：http://yr.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ra.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://so.chemitech.net.cn

[U24] Py：路径操作
来源：http://kx.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ks.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://el.yuntaijiaju.cn

csv.DictReader(f)
来源：http://et.bjjhwx.cn

[U26] Py：并发下载
来源：http://jx.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sm.colortex.cn

[U27] Py：异步 HTTP
来源：http://pi.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://um.huanxung.cn

[U28] Py：类型别名
来源：http://te.jianghongdianzi.cn

UserId = int
来源：http://mh.huanxung.cn

[U29] Py：属性校验
来源：http://hg.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://da.hahajie.cn

[U30] Py：数据类
来源：http://cu.lnxyls.cn

@dataclass(slots=True)
来源：http://bv.yuntaijiaju.cn

[U31] Py：单测
来源：http://kr.huixinmuqiang.cn

python -m pytest -q
来源：http://qg.hahajie.cn

[U32] Py：代码格式化
来源：http://vy.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://ud.9csxet.cn

[U33] Py：打包发布
来源：http://jd.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://ur.shtwfgs.cn

[U34] Py：判断编码
来源：http://lq.haigaiapp.cn

chardet.detect(raw)
来源：http://fq.szsharing.cn

[U35] Py：发送邮件
来源：http://ix.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lv.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://bm.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://xd.panjiajie.cn

[U37] Py：读写 Excel
来源：http://at.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://og.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://pr.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://sk.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://iz.newstarts.cn

sys.stdout.isatty()
来源：http://fe.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://yw.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://yk.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://hl.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://en.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vt.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pm.521024.cn

[U43] PHP：声明命名空间
来源：http://hj.szsharing.cn

namespace App\Http;
来源：http://yj.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://er.huixinmuqiang.cn

declare(strict_types=1);
来源：http://tw.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://aq.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mf.haigaiapp.cn

[U46] PHP：可空类型
来源：http://hq.panjiajie.cn

?string $name = null
来源：http://uk.gzmigu.cn

[U47] PHP：联合类型
来源：http://ui.shxzukj.cn

int|string $id
来源：http://ku.nszjky.cn

[U48] PHP：纯枚举
来源：http://vf.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zr.521024.cn

[U49] PHP：只读属性
来源：http://wx.yuexingan06.cn

public readonly string $name
来源：http://gh.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://dz.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://tq.jctech888.com.cn

[U51] PHP：数组解构
来源：http://mf.nicolike.cn

[$a, $b] = $arr;
来源：http://md.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ez.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://nz.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://sn.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://gt.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://hl.nszjky.cn

$obj?->method()
来源：http://kq.lnxyls.cn

[U55] PHP：match 表达式
来源：http://xm.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hp.shtwfgs.cn

[U56] PHP：命名参数
来源：http://wi.asd995.cn

f(a: 1, b: 2)
来源：http://ky.hnjuh.cn

[U57] PHP：字符串插值
来源：http://yn.bookmarksfly.cn

"值: {$a}"
来源：http://en.nicolike.cn

[U58] PHP：数组三件套
来源：http://pe.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tf.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://nu.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qb.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://yg.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cb.bookmarksfly.cn

[U61] PHP：正则
来源：http://uh.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vr.huixiangedu.cn

[U62] PHP：日期对象
来源：http://nx.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://va.wgjwhj.cn

[U63] PHP：文件读写
来源：http://hk.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uu.nszjky.cn

[U64] PHP：目录遍历
来源：http://uv.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ud.newstarts.cn

[U65] PHP：会话
来源：http://zs.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hq.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://cb.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nq.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://lg.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kc.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://bt.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ab.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://ic.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qn.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://tq.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xi.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://hq.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://qk.lnxyls.cn

[U72] PHP：写错误日志
来源：http://vp.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://eg.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://vl.asd995.cn

parse_ini_file("config.ini", true)
来源：http://vf.9csxet.cn

[U74] PHP：读取环境变量
来源：http://va.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://oa.huanxung.cn

[U75] PHP：依赖注入
来源：http://pg.gzmigu.cn

composer require psr/container
来源：http://pd.yuexingan06.cn

[U76] PHP：简单路由
来源：http://di.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ve.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://wz.hnjuh.cn

composer require twig/twig
来源：http://jl.huixiangedu.cn

[U78] PHP：单元测试
来源：http://cj.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://im.nicolike.cn

[U79] PHP：静态分析
来源：http://fq.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://pe.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://wf.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ge.asd995.cn

[U81] JS：初始化项目
来源：http://fl.newstarts.cn

npm init -y;  npm i express
来源：http://lf.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://nu.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ej.521024.cn

[U83] JS：ES Module 导入导出
来源：http://vb.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://av.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://si.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jy.lnxyls.cn

[U85] JS：可选链
来源：http://vf.szxytkj.cn

a?.b?.c
来源：http://gl.huanxung.cn

[U86] JS：空值合并
来源：http://ov.jctech888.com.cn

a ?? b
来源：http://cc.shxzskj.cn

[U87] JS：解构默认值
来源：http://tr.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ma.panjiajie.cn

[U88] JS：对象展开合并
来源：http://ld.shxzukj.cn

{ ...a, ...b }
来源：http://ux.wgjwhj.cn

[U89] JS：数组去重
来源：http://uf.muxihuayi.cn

[...new Set(arr)]
来源：http://qm.hahajie.cn

[U90] JS：数字数组排序
来源：http://ud.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://in.newstarts.cn

[U91] JS：对象键值遍历
来源：http://mt.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gi.haigaiapp.cn

[U92] JS：深拷贝
来源：http://xe.szsharing.cn

structuredClone(obj)
来源：http://tl.jctech888.com.cn

[U93] JS：模板字符串
来源：http://ot.shxzskj.cn

`共 ${n} 条`
来源：http://ch.521024.cn

[U94] JS：箭头函数
来源：http://em.colortex.cn

const double = x => x * 2;
来源：http://hs.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://iv.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://kb.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://rj.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sq.nszjky.cn

[U97] JS：并发请求
来源：http://tv.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vp.521024.cn

[U98] JS：fetch 带 JSON
来源：http://jp.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wb.shtwfgs.cn

[U99] JS：事件监听
来源：http://jq.nicolike.cn

el.addEventListener("click", e => {})
来源：http://bm.huanxung.cn

[U100] JS：DOM 查询
来源：http://bz.jianghongdianzi.cn

document.querySelector(".item")
来源：http://oy.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://uq.chemitech.net.cn

el.classList.toggle("active")
来源：http://jg.wgjwhj.cn

[U102] JS：本地存储
来源：http://yq.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sj.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ot.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nb.yuexingan06.cn

[U104] JS：防抖
来源：http://rg.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ol.haigaiapp.cn

[U105] JS：节流
来源：http://it.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fk.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://ef.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ch.asd995.cn

[U107] JS：数字千分位
来源：http://af.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yh.nicolike.cn

[U108] JS：随机整数
来源：http://um.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lt.nszjky.cn

[U109] JS：数组分组
来源：http://rr.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://dj.nszjky.cn

[U110] JS：数组分块
来源：http://wk.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bw.gzmigu.cn

[U111] JS：对象转 Map
来源：http://vr.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://bv.shxzskj.cn

[U112] JS：字符串补位
来源：http://hv.yuexingan06.cn

"7".padStart(3, "0")
来源：http://jx.gzmigu.cn

[U113] JS：正则替换全部
来源：http://un.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://kx.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://ir.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vd.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://hd.shxzskj.cn

crypto.randomUUID()
来源：http://pu.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ky.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://il.chemitech.net.cn

[U117] JS：单元测试
来源：http://he.colortex.cn

npm i -D vitest;  npx vitest
来源：http://ah.hnjuh.cn

[U118] JS：开发服务器
来源：http://ez.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://nx.colortex.cn

[U119] JS：生产构建
来源：http://to.newstarts.cn

npx vite build
来源：http://nl.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://vr.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://rz.asd995.cn

================================================================================
来源：http://bp.haigaiapp.cn

统计汇总
来源：http://ib.9csxet.cn

================================================================================
来源：http://rk.huanxung.cn

按语言统计（条）：
来源：http://vj.yuntaijiaju.cn

Python ......... 252
来源：http://rl.hahajie.cn

PHP ............ 252
来源：http://tz.yuexingan06.cn

JavaScript ..... 252
来源：http://wk.521024.cn

TypeScript ..... 212
来源：http://xe.gzmigu.cn

Java ........... 212
来源：http://xc.muxihuayi.cn

Go ............. 212
来源：http://ts.szsharing.cn

Ruby ........... 212
来源：http://zs.gzmigu.cn

C# ............. 212
来源：http://kn.yuexingan06.cn

C .............. 30
来源：http://lp.muxihuayi.cn

C++ ............ 30
来源：http://uw.yuntaijiaju.cn

SQL ............ 90
来源：http://aa.bjjhwx.cn

Bash ........... 80
来源：http://of.shxzukj.cn

Kotlin ......... 15
来源：http://eq.muxihuayi.cn

Swift .......... 15
来源：http://bf.asd995.cn

Lua ............ 10
来源：http://kd.asd995.cn

Perl ........... 10
来源：http://ry.muxihuayi.cn

Scala .......... 10
来源：http://jx.chemitech.net.cn

------------------------------------
来源：http://jm.521024.cn

合计 ........... 2106 条
来源：http://dm.newstarts.cn

按章节统计：
来源：http://sw.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wu.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rl.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ng.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zy.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cv.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://as.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ee.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hf.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ox.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hq.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kh.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tr.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vh.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fh.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jn.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://st.huixinmuqiang.cn


<!-- 参考信息 -->