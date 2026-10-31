代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://mb.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://nu.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://li.asd995.cn

[T56] Scala：样例类
来源：http://mq.colortex.cn

case class User(name: String, age: Int)
来源：http://af.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://av.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sc.muxihuayi.cn

[T58] Scala：函数定义
来源：http://gi.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kh.hnjuh.cn

[T59] Scala：循环
来源：http://or.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://lb.shxzskj.cn

[T60] Scala：折叠
来源：http://nb.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://va.nszjky.cn

================================================================================
来源：http://lg.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lh.huixinmuqiang.cn

================================================================================
来源：http://pa.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://ba.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qj.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://sx.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://do.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://nm.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fm.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://qk.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kv.521024.cn

[U05] Py：列表去重且保序
来源：http://ps.huanxung.cn

list(dict.fromkeys(arr))
来源：http://ua.9csxet.cn

[U06] Py：合并两个字典
来源：http://gc.gzmigu.cn

{**a, **b}
来源：http://ib.shxzukj.cn

[U07] Py：反转字典键值
来源：http://po.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://tb.szxytkj.cn

[U08] Py：展平二维列表
来源：http://hf.bjjhwx.cn

[y for x in nested for y in x]
来源：http://tj.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ul.wgjwhj.cn

max(d, key=d.get)
来源：http://bb.huanxung.cn

[U10] Py：按值排序字典
来源：http://qm.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vk.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://hd.asd995.cn

(x * 2 for x in arr)
来源：http://tu.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kf.shxzukj.cn

Counter(arr).most_common(3)
来源：http://vg.nicolike.cn

[U13] Py：固定长度队列
来源：http://pk.shxzukj.cn

deque(maxlen=10)
来源：http://dy.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://cr.521024.cn

defaultdict(list)
来源：http://ab.bjjhwx.cn

[U15] Py：高精度计时
来源：http://rs.lnxyls.cn

t = time.perf_counter()
来源：http://tz.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://xc.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ea.szxytkj.cn

[U17] Py：初始化日志
来源：http://qe.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://dp.gzmigu.cn

[U18] Py：预编译正则
来源：http://zo.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://kd.521024.cn

[U19] Py：正则替换带回调
来源：http://ti.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ev.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://wm.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://gp.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://mk.asd995.cn

@contextlib.contextmanager
来源：http://dj.gzmigu.cn

[U22] Py：矩阵转置
来源：http://by.yuexingan06.cn

list(zip(*m))
来源：http://xl.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://jm.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lx.wgjwhj.cn

[U24] Py：路径操作
来源：http://kr.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mm.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://as.jctech888.com.cn

csv.DictReader(f)
来源：http://nf.gzmigu.cn

[U26] Py：并发下载
来源：http://ue.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://di.szsharing.cn

[U27] Py：异步 HTTP
来源：http://od.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://te.panjiajie.cn

[U28] Py：类型别名
来源：http://gs.shxzskj.cn

UserId = int
来源：http://pm.nicolike.cn

[U29] Py：属性校验
来源：http://zs.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://kx.shxzukj.cn

[U30] Py：数据类
来源：http://qr.bjjhwx.cn

@dataclass(slots=True)
来源：http://kq.hnjuh.cn

[U31] Py：单测
来源：http://gm.yuntaijiaju.cn

python -m pytest -q
来源：http://bw.haigaiapp.cn

[U32] Py：代码格式化
来源：http://mo.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://hn.shxzskj.cn

[U33] Py：打包发布
来源：http://eo.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://uo.hnjuh.cn

[U34] Py：判断编码
来源：http://kp.521024.cn

chardet.detect(raw)
来源：http://hb.bjjhwx.cn

[U35] Py：发送邮件
来源：http://zm.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bt.9csxet.cn

[U36] Py：定时任务
来源：http://in.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://im.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://iq.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xn.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://dq.nicolike.cn

Path(__file__).resolve().parent
来源：http://tn.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://xy.nicolike.cn

sys.stdout.isatty()
来源：http://vh.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ph.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://kx.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ta.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ym.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://ue.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://au.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://pg.szxytkj.cn

namespace App\Http;
来源：http://mx.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://zt.hnjuh.cn

declare(strict_types=1);
来源：http://kc.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://of.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ir.colortex.cn

[U46] PHP：可空类型
来源：http://bq.9csxet.cn

?string $name = null
来源：http://rb.huixiangedu.cn

[U47] PHP：联合类型
来源：http://tl.bjjhwx.cn

int|string $id
来源：http://uh.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://ak.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ku.hnjuh.cn

[U49] PHP：只读属性
来源：http://kq.huixinmuqiang.cn

public readonly string $name
来源：http://rx.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://az.nszjky.cn

public function __construct(private int $id) {}
来源：http://wx.panjiajie.cn

[U51] PHP：数组解构
来源：http://jp.jctech888.com.cn

[$a, $b] = $arr;
来源：http://ex.asd995.cn

[U52] PHP：箭头函数
来源：http://ym.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://hy.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ng.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://vx.huanxung.cn

[U54] PHP：空安全调用
来源：http://ex.jianghongdianzi.cn

$obj?->method()
来源：http://jq.nicolike.cn

[U55] PHP：match 表达式
来源：http://rk.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kq.colortex.cn

[U56] PHP：命名参数
来源：http://xn.shxzskj.cn

f(a: 1, b: 2)
来源：http://ev.shxzskj.cn

[U57] PHP：字符串插值
来源：http://qv.colortex.cn

"值: {$a}"
来源：http://ey.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ty.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wg.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://yp.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://at.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://dy.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cy.jctech888.com.cn

[U61] PHP：正则
来源：http://iz.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rl.huanxung.cn

[U62] PHP：日期对象
来源：http://fh.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bu.szsharing.cn

[U63] PHP：文件读写
来源：http://oo.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nr.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://gi.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://fv.521024.cn

[U65] PHP：会话
来源：http://ei.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mw.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://pz.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dg.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://wg.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://da.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://qy.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ny.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://qx.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hh.asd995.cn

[U70] PHP：PDO 事务
来源：http://bu.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ex.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://uh.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://bc.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://ih.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://pz.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://dk.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://ks.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://lj.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://nq.shxzukj.cn

[U75] PHP：依赖注入
来源：http://hf.hahajie.cn

composer require psr/container
来源：http://ym.szsharing.cn

[U76] PHP：简单路由
来源：http://px.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://op.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://jg.shxzukj.cn

composer require twig/twig
来源：http://wq.gzmigu.cn

[U78] PHP：单元测试
来源：http://in.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://hh.huanxung.cn

[U79] PHP：静态分析
来源：http://jm.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ie.asd995.cn

[U80] PHP：代码规范修复
来源：http://fn.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wy.shtwfgs.cn

[U81] JS：初始化项目
来源：http://ou.haigaiapp.cn

npm init -y;  npm i express
来源：http://tf.szsharing.cn

[U82] JS：package.json 脚本
来源：http://os.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hy.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://pr.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uv.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://bv.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gq.szsharing.cn

[U85] JS：可选链
来源：http://bz.yuntaijiaju.cn

a?.b?.c
来源：http://yw.szxytkj.cn

[U86] JS：空值合并
来源：http://th.huanxung.cn

a ?? b
来源：http://ae.chemitech.net.cn

[U87] JS：解构默认值
来源：http://gv.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://xv.lnxyls.cn

[U88] JS：对象展开合并
来源：http://fc.haigaiapp.cn

{ ...a, ...b }
来源：http://am.szsharing.cn

[U89] JS：数组去重
来源：http://dh.jctech888.com.cn

[...new Set(arr)]
来源：http://xn.hnjuh.cn

[U90] JS：数字数组排序
来源：http://mc.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://cp.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://ts.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oe.shtwfgs.cn

[U92] JS：深拷贝
来源：http://zl.lnxyls.cn

structuredClone(obj)
来源：http://tn.shxzskj.cn

[U93] JS：模板字符串
来源：http://ya.szsharing.cn

`共 ${n} 条`
来源：http://jj.chemitech.net.cn

[U94] JS：箭头函数
来源：http://cj.hahajie.cn

const double = x => x * 2;
来源：http://hs.nicolike.cn

[U95] JS：Promise 包装
来源：http://ef.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://gh.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://kk.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dk.bookmarksfly.cn

[U97] JS：并发请求
来源：http://zx.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://da.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://dy.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rw.huanxung.cn

[U99] JS：事件监听
来源：http://oi.newstarts.cn

el.addEventListener("click", e => {})
来源：http://mg.hahajie.cn

[U100] JS：DOM 查询
来源：http://ej.hahajie.cn

document.querySelector(".item")
来源：http://sn.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://cq.hnjuh.cn

el.classList.toggle("active")
来源：http://oj.shxzukj.cn

[U102] JS：本地存储
来源：http://mz.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://um.nicolike.cn

[U103] JS：定时器
来源：http://jh.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zr.jianghongdianzi.cn

[U104] JS：防抖
来源：http://cz.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dc.huanxung.cn

[U105] JS：节流
来源：http://ts.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bf.shxzukj.cn

[U106] JS：日期格式化
来源：http://zg.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ta.panjiajie.cn

[U107] JS：数字千分位
来源：http://sh.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://af.panjiajie.cn

[U108] JS：随机整数
来源：http://zy.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hv.hnjuh.cn

[U109] JS：数组分组
来源：http://ot.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://ea.yuexingan06.cn

[U110] JS：数组分块
来源：http://yb.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cz.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://lk.panjiajie.cn

new Map(Object.entries(obj))
来源：http://cy.haigaiapp.cn

[U112] JS：字符串补位
来源：http://mv.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://oc.hahajie.cn

[U113] JS：正则替换全部
来源：http://rn.asd995.cn

s.replaceAll("a", "b")
来源：http://rr.hahajie.cn

[U114] JS：JSON 深比较
来源：http://az.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qe.panjiajie.cn

[U115] JS：生成 UUID
来源：http://os.huixinmuqiang.cn

crypto.randomUUID()
来源：http://hx.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://wb.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://ys.bookmarksfly.cn

[U117] JS：单元测试
来源：http://vd.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://ce.gzmigu.cn

[U118] JS：开发服务器
来源：http://gl.colortex.cn

npm i -D vite;  npx vite
来源：http://xk.muxihuayi.cn

[U119] JS：生产构建
来源：http://ha.haigaiapp.cn

npx vite build
来源：http://yi.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://vs.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ka.9csxet.cn

================================================================================
来源：http://lh.yuntaijiaju.cn

统计汇总
来源：http://pf.hahajie.cn

================================================================================
来源：http://jk.gzmigu.cn

按语言统计（条）：
来源：http://ug.panjiajie.cn

Python ......... 252
来源：http://th.yuntaijiaju.cn

PHP ............ 252
来源：http://mb.nicolike.cn

JavaScript ..... 252
来源：http://kc.panjiajie.cn

TypeScript ..... 212
来源：http://nk.hahajie.cn

Java ........... 212
来源：http://zv.hahajie.cn

Go ............. 212
来源：http://cs.shxzukj.cn

Ruby ........... 212
来源：http://ga.huanxung.cn

C# ............. 212
来源：http://qv.huixinmuqiang.cn

C .............. 30
来源：http://dd.lnxyls.cn

C++ ............ 30
来源：http://un.nszjky.cn

SQL ............ 90
来源：http://bd.newstarts.cn

Bash ........... 80
来源：http://dz.yuntaijiaju.cn

Kotlin ......... 15
来源：http://zn.huixiangedu.cn

Swift .......... 15
来源：http://sa.hahajie.cn

Lua ............ 10
来源：http://qi.bookmarksfly.cn

Perl ........... 10
来源：http://xs.panjiajie.cn

Scala .......... 10
来源：http://hz.nicolike.cn

------------------------------------
来源：http://mj.shxzskj.cn

合计 ........... 2106 条
来源：http://ww.asd995.cn

按章节统计：
来源：http://st.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mx.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jn.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ba.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ng.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bo.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jh.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pw.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wb.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zw.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://at.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ee.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ld.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://go.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xq.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oj.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tb.bjjhwx.cn

Q SQL 专题                              90
来源：http://tu.newstarts.cn

R Bash 专题                             80
来源：http://gt.chemitech.net.cn

S C / C++ 专题                          60
来源：http://ex.bjjhwx.cn

T 其他语言补充                          60
来源：http://sz.chemitech.net.cn


<!-- 参考信息 -->