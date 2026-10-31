代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ul.panjiajie.cn

[T55] Scala：集合过滤
来源：http://bv.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fy.wgjwhj.cn

[T56] Scala：样例类
来源：http://kx.shxzukj.cn

case class User(name: String, age: Int)
来源：http://hu.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://vq.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iy.haigaiapp.cn

[T58] Scala：函数定义
来源：http://qn.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ri.shtwfgs.cn

[T59] Scala：循环
来源：http://aw.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://yl.muxihuayi.cn

[T60] Scala：折叠
来源：http://mu.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sb.shxzskj.cn

================================================================================
来源：http://vd.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kr.nicolike.cn

================================================================================
来源：http://uy.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://iq.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dj.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://sc.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ip.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://gp.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ml.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://js.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vu.szsharing.cn

[U05] Py：列表去重且保序
来源：http://vz.hahajie.cn

list(dict.fromkeys(arr))
来源：http://lq.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://zl.wgjwhj.cn

{**a, **b}
来源：http://ru.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://cv.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://la.9csxet.cn

[U08] Py：展平二维列表
来源：http://lu.hahajie.cn

[y for x in nested for y in x]
来源：http://dl.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://zj.szsharing.cn

max(d, key=d.get)
来源：http://lw.shxzukj.cn

[U10] Py：按值排序字典
来源：http://zt.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mz.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://nh.bjjhwx.cn

(x * 2 for x in arr)
来源：http://hv.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qt.shxzukj.cn

Counter(arr).most_common(3)
来源：http://so.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ns.hnjuh.cn

deque(maxlen=10)
来源：http://vu.szsharing.cn

[U14] Py：分组收集到列表
来源：http://xu.nszjky.cn

defaultdict(list)
来源：http://sl.colortex.cn

[U15] Py：高精度计时
来源：http://zr.nszjky.cn

t = time.perf_counter()
来源：http://cr.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://du.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ma.nicolike.cn

[U17] Py：初始化日志
来源：http://ke.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://zu.wgjwhj.cn

[U18] Py：预编译正则
来源：http://dx.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://fm.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://jp.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fm.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://kf.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://ym.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://pq.bjjhwx.cn

@contextlib.contextmanager
来源：http://ls.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://vk.wgjwhj.cn

list(zip(*m))
来源：http://jz.colortex.cn

[U23] Py：分块读取大文件
来源：http://ay.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://au.bjjhwx.cn

[U24] Py：路径操作
来源：http://xc.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qk.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://tm.chemitech.net.cn

csv.DictReader(f)
来源：http://cm.shxzukj.cn

[U26] Py：并发下载
来源：http://id.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zb.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://ns.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ok.chemitech.net.cn

[U28] Py：类型别名
来源：http://li.jianghongdianzi.cn

UserId = int
来源：http://bb.haigaiapp.cn

[U29] Py：属性校验
来源：http://np.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ir.hahajie.cn

[U30] Py：数据类
来源：http://bv.newstarts.cn

@dataclass(slots=True)
来源：http://ms.gzmigu.cn

[U31] Py：单测
来源：http://hs.colortex.cn

python -m pytest -q
来源：http://pd.yuexingan06.cn

[U32] Py：代码格式化
来源：http://hr.hahajie.cn

ruff format . && ruff check --fix .
来源：http://rm.wgjwhj.cn

[U33] Py：打包发布
来源：http://nx.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://vo.haigaiapp.cn

[U34] Py：判断编码
来源：http://wt.huixinmuqiang.cn

chardet.detect(raw)
来源：http://di.bjjhwx.cn

[U35] Py：发送邮件
来源：http://yf.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oy.szxytkj.cn

[U36] Py：定时任务
来源：http://pi.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://kp.asd995.cn

[U37] Py：读写 Excel
来源：http://gt.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ro.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://lo.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://vz.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://hk.bjjhwx.cn

sys.stdout.isatty()
来源：http://aq.newstarts.cn

[U40] Py：打印到标准错误
来源：http://sp.shxzskj.cn

print("err", file=sys.stderr)
来源：http://er.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://ce.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oy.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://pe.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oq.9csxet.cn

[U43] PHP：声明命名空间
来源：http://xo.shxzukj.cn

namespace App\Http;
来源：http://nr.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://oi.colortex.cn

declare(strict_types=1);
来源：http://wd.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://wb.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://py.huanxung.cn

[U46] PHP：可空类型
来源：http://er.newstarts.cn

?string $name = null
来源：http://mx.colortex.cn

[U47] PHP：联合类型
来源：http://dg.jctech888.com.cn

int|string $id
来源：http://gj.asd995.cn

[U48] PHP：纯枚举
来源：http://ec.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dy.huanxung.cn

[U49] PHP：只读属性
来源：http://pg.szsharing.cn

public readonly string $name
来源：http://ix.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://pc.colortex.cn

public function __construct(private int $id) {}
来源：http://gm.chemitech.net.cn

[U51] PHP：数组解构
来源：http://qb.shtwfgs.cn

[$a, $b] = $arr;
来源：http://ft.asd995.cn

[U52] PHP：箭头函数
来源：http://uh.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://py.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://if.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://co.asd995.cn

[U54] PHP：空安全调用
来源：http://kl.shxzukj.cn

$obj?->method()
来源：http://of.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ps.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ug.newstarts.cn

[U56] PHP：命名参数
来源：http://ow.huanxung.cn

f(a: 1, b: 2)
来源：http://bb.gzmigu.cn

[U57] PHP：字符串插值
来源：http://tr.colortex.cn

"值: {$a}"
来源：http://ci.hnjuh.cn

[U58] PHP：数组三件套
来源：http://ee.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://na.gzmigu.cn

[U59] PHP：自定义排序
来源：http://mu.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cb.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://ca.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tf.huixiangedu.cn

[U61] PHP：正则
来源：http://iq.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bc.szsharing.cn

[U62] PHP：日期对象
来源：http://oi.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wm.shxzskj.cn

[U63] PHP：文件读写
来源：http://gt.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://or.nicolike.cn

[U64] PHP：目录遍历
来源：http://qp.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://sr.gzmigu.cn

[U65] PHP：会话
来源：http://pg.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ps.asd995.cn

[U66] PHP：设置 Cookie
来源：http://iv.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nn.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://yx.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dd.newstarts.cn

[U68] PHP：PDO 连接
来源：http://yx.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lf.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://wh.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nk.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://dk.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rv.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://dx.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://dt.nicolike.cn

[U72] PHP：写错误日志
来源：http://dw.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://qy.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://bf.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://tu.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://fm.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ce.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://rr.yuntaijiaju.cn

composer require psr/container
来源：http://yx.hahajie.cn

[U76] PHP：简单路由
来源：http://hn.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://su.asd995.cn

[U77] PHP：模板渲染
来源：http://wb.szxytkj.cn

composer require twig/twig
来源：http://kl.yuexingan06.cn

[U78] PHP：单元测试
来源：http://sc.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://cm.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://ew.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://sh.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://ui.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qq.jctech888.com.cn

[U81] JS：初始化项目
来源：http://gk.szsharing.cn

npm init -y;  npm i express
来源：http://tc.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://mo.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ut.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://vp.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gy.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://nb.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ld.huanxung.cn

[U85] JS：可选链
来源：http://tz.bjjhwx.cn

a?.b?.c
来源：http://jc.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://xz.hahajie.cn

a ?? b
来源：http://lq.yuexingan06.cn

[U87] JS：解构默认值
来源：http://en.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://pd.asd995.cn

[U88] JS：对象展开合并
来源：http://wc.newstarts.cn

{ ...a, ...b }
来源：http://ul.muxihuayi.cn

[U89] JS：数组去重
来源：http://io.chemitech.net.cn

[...new Set(arr)]
来源：http://sk.asd995.cn

[U90] JS：数字数组排序
来源：http://wg.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://ea.hahajie.cn

[U91] JS：对象键值遍历
来源：http://tc.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://au.gzmigu.cn

[U92] JS：深拷贝
来源：http://gj.newstarts.cn

structuredClone(obj)
来源：http://wa.panjiajie.cn

[U93] JS：模板字符串
来源：http://gp.hahajie.cn

`共 ${n} 条`
来源：http://ag.asd995.cn

[U94] JS：箭头函数
来源：http://qm.yuntaijiaju.cn

const double = x => x * 2;
来源：http://av.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://ax.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://uo.hahajie.cn

[U96] JS：async/await 与异常
来源：http://pq.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://um.jctech888.com.cn

[U97] JS：并发请求
来源：http://xm.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qf.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://wm.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wu.colortex.cn

[U99] JS：事件监听
来源：http://tf.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://qg.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://mc.shxzskj.cn

document.querySelector(".item")
来源：http://nn.521024.cn

[U101] JS：classList 操作
来源：http://xw.nszjky.cn

el.classList.toggle("active")
来源：http://qu.asd995.cn

[U102] JS：本地存储
来源：http://so.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kg.panjiajie.cn

[U103] JS：定时器
来源：http://ln.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gv.colortex.cn

[U104] JS：防抖
来源：http://ai.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.jianghongdianzi.cn

[U105] JS：节流
来源：http://ww.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://or.521024.cn

[U106] JS：日期格式化
来源：http://nz.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wp.haigaiapp.cn

[U107] JS：数字千分位
来源：http://mj.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zj.9csxet.cn

[U108] JS：随机整数
来源：http://ma.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pb.nicolike.cn

[U109] JS：数组分组
来源：http://kh.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://ox.szxytkj.cn

[U110] JS：数组分块
来源：http://mn.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ip.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://qc.lnxyls.cn

new Map(Object.entries(obj))
来源：http://bv.szsharing.cn

[U112] JS：字符串补位
来源：http://bt.hahajie.cn

"7".padStart(3, "0")
来源：http://wl.nszjky.cn

[U113] JS：正则替换全部
来源：http://se.shxzskj.cn

s.replaceAll("a", "b")
来源：http://xb.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://rp.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wb.shxzskj.cn

[U115] JS：生成 UUID
来源：http://gg.bookmarksfly.cn

crypto.randomUUID()
来源：http://ax.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://jy.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://er.bookmarksfly.cn

[U117] JS：单元测试
来源：http://kt.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://mn.hahajie.cn

[U118] JS：开发服务器
来源：http://ox.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://jp.yuexingan06.cn

[U119] JS：生产构建
来源：http://no.gzmigu.cn

npx vite build
来源：http://rr.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ik.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://vq.shtwfgs.cn

================================================================================
来源：http://gq.huanxung.cn

统计汇总
来源：http://ez.szxytkj.cn

================================================================================
来源：http://nj.bookmarksfly.cn

按语言统计（条）：
来源：http://ow.colortex.cn

Python ......... 252
来源：http://pd.huixinmuqiang.cn

PHP ............ 252
来源：http://oe.bookmarksfly.cn

JavaScript ..... 252
来源：http://ya.szsharing.cn

TypeScript ..... 212
来源：http://al.newstarts.cn

Java ........... 212
来源：http://af.muxihuayi.cn

Go ............. 212
来源：http://ft.shtwfgs.cn

Ruby ........... 212
来源：http://cu.huixiangedu.cn

C# ............. 212
来源：http://yn.jctech888.com.cn

C .............. 30
来源：http://ga.szsharing.cn

C++ ............ 30
来源：http://sb.huixinmuqiang.cn

SQL ............ 90
来源：http://fr.lnxyls.cn

Bash ........... 80
来源：http://ll.chemitech.net.cn

Kotlin ......... 15
来源：http://ko.bookmarksfly.cn

Swift .......... 15
来源：http://am.hnjuh.cn

Lua ............ 10
来源：http://dc.newstarts.cn

Perl ........... 10
来源：http://hk.jctech888.com.cn

Scala .......... 10
来源：http://zc.hahajie.cn

------------------------------------
来源：http://ox.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://sh.shxzskj.cn

按章节统计：
来源：http://uj.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gb.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://je.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ht.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xm.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jp.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zn.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dd.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mp.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ms.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gt.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sz.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ie.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fl.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://to.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://um.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oq.colortex.cn

Q SQL 专题                              90
来源：http://po.szsharing.cn

R Bash 专题                             80
来源：http://lq.muxihuayi.cn

S C / C++ 专题                          60
来源：http://bi.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://hl.yuexingan06.cn


<!-- 参考信息 -->