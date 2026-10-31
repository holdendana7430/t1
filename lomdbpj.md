代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://xr.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://ez.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fc.muxihuayi.cn

[T56] Scala：样例类
来源：http://gh.newstarts.cn

case class User(name: String, age: Int)
来源：http://sg.gzmigu.cn

[T57] Scala：模式匹配
来源：http://fw.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bg.haigaiapp.cn

[T58] Scala：函数定义
来源：http://gi.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://md.yuntaijiaju.cn

[T59] Scala：循环
来源：http://hu.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://dz.haigaiapp.cn

[T60] Scala：折叠
来源：http://lg.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vg.wgjwhj.cn

================================================================================
来源：http://vr.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wx.huanxung.cn

================================================================================
来源：http://su.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://vd.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ry.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://tx.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://co.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://xt.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tt.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://dp.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ih.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://ye.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://cy.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://bx.huixiangedu.cn

{**a, **b}
来源：http://oe.szxytkj.cn

[U07] Py：反转字典键值
来源：http://sx.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://dd.nszjky.cn

[U08] Py：展平二维列表
来源：http://yk.newstarts.cn

[y for x in nested for y in x]
来源：http://pv.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://wb.521024.cn

max(d, key=d.get)
来源：http://ou.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://tf.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://if.szsharing.cn

[U11] Py：生成器表达式
来源：http://js.bjjhwx.cn

(x * 2 for x in arr)
来源：http://cp.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://av.hahajie.cn

Counter(arr).most_common(3)
来源：http://ne.colortex.cn

[U13] Py：固定长度队列
来源：http://qi.yuexingan06.cn

deque(maxlen=10)
来源：http://qm.nicolike.cn

[U14] Py：分组收集到列表
来源：http://bf.jianghongdianzi.cn

defaultdict(list)
来源：http://ph.bjjhwx.cn

[U15] Py：高精度计时
来源：http://lx.gzmigu.cn

t = time.perf_counter()
来源：http://wt.hahajie.cn

[U16] Py：命令行参数解析
来源：http://eg.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oj.haigaiapp.cn

[U17] Py：初始化日志
来源：http://ql.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://rq.jctech888.com.cn

[U18] Py：预编译正则
来源：http://lb.9csxet.cn

pat = re.compile(r"\d+")
来源：http://ft.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://lw.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dp.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://no.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://fk.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://vl.szsharing.cn

@contextlib.contextmanager
来源：http://de.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://uw.wgjwhj.cn

list(zip(*m))
来源：http://fc.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://wk.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://me.asd995.cn

[U24] Py：路径操作
来源：http://nd.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pd.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://ke.haigaiapp.cn

csv.DictReader(f)
来源：http://mn.colortex.cn

[U26] Py：并发下载
来源：http://yh.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zv.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://su.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://gk.muxihuayi.cn

[U28] Py：类型别名
来源：http://ed.szsharing.cn

UserId = int
来源：http://qs.huixiangedu.cn

[U29] Py：属性校验
来源：http://vd.huanxung.cn

@property 与 @x.setter 配合
来源：http://em.nicolike.cn

[U30] Py：数据类
来源：http://er.shxzskj.cn

@dataclass(slots=True)
来源：http://uv.huanxung.cn

[U31] Py：单测
来源：http://gu.521024.cn

python -m pytest -q
来源：http://mo.nicolike.cn

[U32] Py：代码格式化
来源：http://gx.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://ac.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://et.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://pz.hahajie.cn

[U34] Py：判断编码
来源：http://xs.wgjwhj.cn

chardet.detect(raw)
来源：http://la.panjiajie.cn

[U35] Py：发送邮件
来源：http://sp.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xp.wgjwhj.cn

[U36] Py：定时任务
来源：http://fe.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://le.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://il.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ul.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://ho.szxytkj.cn

Path(__file__).resolve().parent
来源：http://av.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://it.521024.cn

sys.stdout.isatty()
来源：http://ri.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://cr.shxzskj.cn

print("err", file=sys.stderr)
来源：http://wt.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://gf.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vl.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://ee.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xh.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://hi.szsharing.cn

namespace App\Http;
来源：http://td.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ym.521024.cn

declare(strict_types=1);
来源：http://cl.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://gs.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://av.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://zd.shxzskj.cn

?string $name = null
来源：http://zn.panjiajie.cn

[U47] PHP：联合类型
来源：http://kd.jctech888.com.cn

int|string $id
来源：http://wh.colortex.cn

[U48] PHP：纯枚举
来源：http://jd.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ab.huixiangedu.cn

[U49] PHP：只读属性
来源：http://di.521024.cn

public readonly string $name
来源：http://rg.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://al.panjiajie.cn

public function __construct(private int $id) {}
来源：http://rs.muxihuayi.cn

[U51] PHP：数组解构
来源：http://aw.shtwfgs.cn

[$a, $b] = $arr;
来源：http://ru.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://kq.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://ac.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://oo.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://wd.panjiajie.cn

[U54] PHP：空安全调用
来源：http://iv.panjiajie.cn

$obj?->method()
来源：http://wo.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ql.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ia.bjjhwx.cn

[U56] PHP：命名参数
来源：http://nh.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://cv.huanxung.cn

[U57] PHP：字符串插值
来源：http://vp.shxzukj.cn

"值: {$a}"
来源：http://ky.panjiajie.cn

[U58] PHP：数组三件套
来源：http://eh.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aa.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://lv.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nn.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://kw.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zq.colortex.cn

[U61] PHP：正则
来源：http://kz.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wl.shxzskj.cn

[U62] PHP：日期对象
来源：http://lz.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hq.bjjhwx.cn

[U63] PHP：文件读写
来源：http://qt.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eu.nicolike.cn

[U64] PHP：目录遍历
来源：http://ld.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://ge.bookmarksfly.cn

[U65] PHP：会话
来源：http://qh.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bc.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ww.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ki.newstarts.cn

[U67] PHP：处理文件上传
来源：http://sn.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xh.hahajie.cn

[U68] PHP：PDO 连接
来源：http://kb.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wo.colortex.cn

[U69] PHP：PDO 预处理
来源：http://ex.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qt.nicolike.cn

[U70] PHP：PDO 事务
来源：http://aa.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vn.521024.cn

[U71] PHP：抛出异常
来源：http://je.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://so.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://ps.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://al.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://vq.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://gk.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://au.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://ws.newstarts.cn

[U75] PHP：依赖注入
来源：http://sn.hnjuh.cn

composer require psr/container
来源：http://ls.shtwfgs.cn

[U76] PHP：简单路由
来源：http://do.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xh.hahajie.cn

[U77] PHP：模板渲染
来源：http://rj.bjjhwx.cn

composer require twig/twig
来源：http://ao.lnxyls.cn

[U78] PHP：单元测试
来源：http://wh.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://zt.hnjuh.cn

[U79] PHP：静态分析
来源：http://lq.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://yj.9csxet.cn

[U80] PHP：代码规范修复
来源：http://rn.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ia.9csxet.cn

[U81] JS：初始化项目
来源：http://se.nicolike.cn

npm init -y;  npm i express
来源：http://pi.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://de.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xi.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://qq.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://no.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://xh.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jr.gzmigu.cn

[U85] JS：可选链
来源：http://pn.huanxung.cn

a?.b?.c
来源：http://zt.shxzukj.cn

[U86] JS：空值合并
来源：http://uq.gzmigu.cn

a ?? b
来源：http://uc.nszjky.cn

[U87] JS：解构默认值
来源：http://nk.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://hd.newstarts.cn

[U88] JS：对象展开合并
来源：http://zt.9csxet.cn

{ ...a, ...b }
来源：http://ko.muxihuayi.cn

[U89] JS：数组去重
来源：http://ek.lnxyls.cn

[...new Set(arr)]
来源：http://ro.hnjuh.cn

[U90] JS：数字数组排序
来源：http://js.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://xw.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://ph.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xk.jctech888.com.cn

[U92] JS：深拷贝
来源：http://hd.wgjwhj.cn

structuredClone(obj)
来源：http://gu.haigaiapp.cn

[U93] JS：模板字符串
来源：http://rx.9csxet.cn

`共 ${n} 条`
来源：http://vx.shtwfgs.cn

[U94] JS：箭头函数
来源：http://kp.gzmigu.cn

const double = x => x * 2;
来源：http://pk.nicolike.cn

[U95] JS：Promise 包装
来源：http://zy.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://el.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://lh.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pn.szxytkj.cn

[U97] JS：并发请求
来源：http://ws.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bd.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://zu.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uf.gzmigu.cn

[U99] JS：事件监听
来源：http://xc.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://gy.newstarts.cn

[U100] JS：DOM 查询
来源：http://dx.szsharing.cn

document.querySelector(".item")
来源：http://vh.muxihuayi.cn

[U101] JS：classList 操作
来源：http://tf.newstarts.cn

el.classList.toggle("active")
来源：http://zf.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://po.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xd.9csxet.cn

[U103] JS：定时器
来源：http://ka.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wr.shxzskj.cn

[U104] JS：防抖
来源：http://ug.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zg.gzmigu.cn

[U105] JS：节流
来源：http://vr.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://li.yuexingan06.cn

[U106] JS：日期格式化
来源：http://fz.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gj.lnxyls.cn

[U107] JS：数字千分位
来源：http://ol.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jb.nicolike.cn

[U108] JS：随机整数
来源：http://bu.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ig.nicolike.cn

[U109] JS：数组分组
来源：http://dk.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://vm.bookmarksfly.cn

[U110] JS：数组分块
来源：http://lj.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pw.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ut.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://pa.nszjky.cn

[U112] JS：字符串补位
来源：http://mt.szxytkj.cn

"7".padStart(3, "0")
来源：http://pe.hahajie.cn

[U113] JS：正则替换全部
来源：http://eo.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://uz.9csxet.cn

[U114] JS：JSON 深比较
来源：http://nj.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sc.panjiajie.cn

[U115] JS：生成 UUID
来源：http://bt.huanxung.cn

crypto.randomUUID()
来源：http://oo.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://yh.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://cl.panjiajie.cn

[U117] JS：单元测试
来源：http://ym.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://ez.lnxyls.cn

[U118] JS：开发服务器
来源：http://bi.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://za.521024.cn

[U119] JS：生产构建
来源：http://kc.jianghongdianzi.cn

npx vite build
来源：http://ob.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://pc.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://fv.wgjwhj.cn

================================================================================
来源：http://gy.colortex.cn

统计汇总
来源：http://qu.hahajie.cn

================================================================================
来源：http://yu.jctech888.com.cn

按语言统计（条）：
来源：http://qh.asd995.cn

Python ......... 252
来源：http://ib.bjjhwx.cn

PHP ............ 252
来源：http://qc.wgjwhj.cn

JavaScript ..... 252
来源：http://bo.nszjky.cn

TypeScript ..... 212
来源：http://rt.9csxet.cn

Java ........... 212
来源：http://pt.yuntaijiaju.cn

Go ............. 212
来源：http://st.9csxet.cn

Ruby ........... 212
来源：http://gg.shtwfgs.cn

C# ............. 212
来源：http://sw.shxzskj.cn

C .............. 30
来源：http://gy.yuntaijiaju.cn

C++ ............ 30
来源：http://sl.bjjhwx.cn

SQL ............ 90
来源：http://dh.yuntaijiaju.cn

Bash ........... 80
来源：http://nx.huixiangedu.cn

Kotlin ......... 15
来源：http://an.bjjhwx.cn

Swift .......... 15
来源：http://vp.hnjuh.cn

Lua ............ 10
来源：http://kd.chemitech.net.cn

Perl ........... 10
来源：http://ah.haigaiapp.cn

Scala .......... 10
来源：http://mt.szsharing.cn

------------------------------------
来源：http://sl.shxzskj.cn

合计 ........... 2106 条
来源：http://sr.jctech888.com.cn

按章节统计：
来源：http://tn.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tl.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xj.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://og.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sd.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ua.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://al.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zr.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oq.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://si.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ap.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sf.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://st.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fj.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jj.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yw.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xz.521024.cn

Q SQL 专题                              90
来源：http://cl.shtwfgs.cn

R Bash 专题                             80
来源：http://bi.hahajie.cn

S C / C++ 专题                          60
来源：http://et.colortex.cn

T 其他语言补充                          60
来源：http://fb.nicolike.cn


<!-- 参考信息 -->