代发 wailian999

case class User(name: String, age: Int)
来源：http://xb.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://ks.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fx.nszjky.cn

[T58] Scala：函数定义
来源：http://dz.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wu.jctech888.com.cn

[T59] Scala：循环
来源：http://pw.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://kx.muxihuayi.cn

[T60] Scala：折叠
来源：http://vi.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://da.huixinmuqiang.cn

================================================================================
来源：http://xb.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xs.shtwfgs.cn

================================================================================
来源：http://ms.colortex.cn

[U01] Py：创建虚拟环境
来源：http://kw.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ok.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://sz.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sl.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://op.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tc.szsharing.cn

[U04] Py：变量调试打印
来源：http://zn.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ch.9csxet.cn

[U05] Py：列表去重且保序
来源：http://rb.szsharing.cn

list(dict.fromkeys(arr))
来源：http://cd.hahajie.cn

[U06] Py：合并两个字典
来源：http://lf.hnjuh.cn

{**a, **b}
来源：http://lm.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://ui.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://uw.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://hm.nicolike.cn

[y for x in nested for y in x]
来源：http://jm.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://od.shxzukj.cn

max(d, key=d.get)
来源：http://pl.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://na.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xl.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://jc.newstarts.cn

(x * 2 for x in arr)
来源：http://sn.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bu.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://df.colortex.cn

[U13] Py：固定长度队列
来源：http://pk.yuexingan06.cn

deque(maxlen=10)
来源：http://ku.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://xe.lnxyls.cn

defaultdict(list)
来源：http://sp.yuexingan06.cn

[U15] Py：高精度计时
来源：http://jn.huixiangedu.cn

t = time.perf_counter()
来源：http://ts.asd995.cn

[U16] Py：命令行参数解析
来源：http://sg.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cg.nicolike.cn

[U17] Py：初始化日志
来源：http://to.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://ob.521024.cn

[U18] Py：预编译正则
来源：http://rj.szsharing.cn

pat = re.compile(r"\d+")
来源：http://jl.nszjky.cn

[U19] Py：正则替换带回调
来源：http://iv.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cu.huanxung.cn

[U20] Py：缓存函数结果
来源：http://zg.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://ol.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://dk.shxzskj.cn

@contextlib.contextmanager
来源：http://kl.huanxung.cn

[U22] Py：矩阵转置
来源：http://cp.shtwfgs.cn

list(zip(*m))
来源：http://at.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://uj.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xt.gzmigu.cn

[U24] Py：路径操作
来源：http://kc.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ck.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://wo.colortex.cn

csv.DictReader(f)
来源：http://hy.szsharing.cn

[U26] Py：并发下载
来源：http://vl.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ji.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://pp.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://pk.haigaiapp.cn

[U28] Py：类型别名
来源：http://yj.szsharing.cn

UserId = int
来源：http://hd.bookmarksfly.cn

[U29] Py：属性校验
来源：http://wo.hahajie.cn

@property 与 @x.setter 配合
来源：http://ty.newstarts.cn

[U30] Py：数据类
来源：http://xc.nszjky.cn

@dataclass(slots=True)
来源：http://dv.shxzukj.cn

[U31] Py：单测
来源：http://ff.chemitech.net.cn

python -m pytest -q
来源：http://nf.huanxung.cn

[U32] Py：代码格式化
来源：http://zd.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ja.chemitech.net.cn

[U33] Py：打包发布
来源：http://mo.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://vo.yuexingan06.cn

[U34] Py：判断编码
来源：http://zi.yuexingan06.cn

chardet.detect(raw)
来源：http://tv.newstarts.cn

[U35] Py：发送邮件
来源：http://zi.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ib.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://qq.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://hq.hnjuh.cn

[U37] Py：读写 Excel
来源：http://aa.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dt.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://lm.szsharing.cn

Path(__file__).resolve().parent
来源：http://rs.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://ui.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://oo.9csxet.cn

[U40] Py：打印到标准错误
来源：http://uv.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://yo.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://pk.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gc.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://rc.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://on.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://zl.nicolike.cn

namespace App\Http;
来源：http://wm.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://rd.9csxet.cn

declare(strict_types=1);
来源：http://nk.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://ks.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.szxytkj.cn

[U46] PHP：可空类型
来源：http://oc.jianghongdianzi.cn

?string $name = null
来源：http://vx.chemitech.net.cn

[U47] PHP：联合类型
来源：http://lf.newstarts.cn

int|string $id
来源：http://dc.shxzskj.cn

[U48] PHP：纯枚举
来源：http://oc.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vj.huanxung.cn

[U49] PHP：只读属性
来源：http://og.szxytkj.cn

public readonly string $name
来源：http://su.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://rq.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://cb.szsharing.cn

[U51] PHP：数组解构
来源：http://si.jctech888.com.cn

[$a, $b] = $arr;
来源：http://ri.newstarts.cn

[U52] PHP：箭头函数
来源：http://yt.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://ia.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://hz.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://qj.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://ac.9csxet.cn

$obj?->method()
来源：http://fa.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://kv.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wx.9csxet.cn

[U56] PHP：命名参数
来源：http://vg.lnxyls.cn

f(a: 1, b: 2)
来源：http://rc.shxzukj.cn

[U57] PHP：字符串插值
来源：http://gr.panjiajie.cn

"值: {$a}"
来源：http://sw.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://sk.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wm.gzmigu.cn

[U59] PHP：自定义排序
来源：http://yl.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ow.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://jt.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kv.yuntaijiaju.cn

[U61] PHP：正则
来源：http://pp.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uf.shxzukj.cn

[U62] PHP：日期对象
来源：http://dz.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rj.jctech888.com.cn

[U63] PHP：文件读写
来源：http://sh.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xq.asd995.cn

[U64] PHP：目录遍历
来源：http://zf.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://jm.chemitech.net.cn

[U65] PHP：会话
来源：http://yq.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uw.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://xv.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bx.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://xl.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tf.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://sg.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jr.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://yz.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lm.asd995.cn

[U70] PHP：PDO 事务
来源：http://bd.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://am.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://hg.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://no.9csxet.cn

[U72] PHP：写错误日志
来源：http://vh.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://xn.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://yj.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://hw.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://en.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://ia.asd995.cn

[U75] PHP：依赖注入
来源：http://kl.bjjhwx.cn

composer require psr/container
来源：http://lw.jctech888.com.cn

[U76] PHP：简单路由
来源：http://fv.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nt.huanxung.cn

[U77] PHP：模板渲染
来源：http://sy.huanxung.cn

composer require twig/twig
来源：http://yc.nicolike.cn

[U78] PHP：单元测试
来源：http://vm.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://ez.muxihuayi.cn

[U79] PHP：静态分析
来源：http://xb.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://pt.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://wp.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ni.huanxung.cn

[U81] JS：初始化项目
来源：http://ol.asd995.cn

npm init -y;  npm i express
来源：http://er.newstarts.cn

[U82] JS：package.json 脚本
来源：http://gj.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qo.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://wg.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cr.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://ym.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://so.yuexingan06.cn

[U85] JS：可选链
来源：http://dh.521024.cn

a?.b?.c
来源：http://rm.huanxung.cn

[U86] JS：空值合并
来源：http://tr.hnjuh.cn

a ?? b
来源：http://hx.colortex.cn

[U87] JS：解构默认值
来源：http://hq.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://my.521024.cn

[U88] JS：对象展开合并
来源：http://sf.bookmarksfly.cn

{ ...a, ...b }
来源：http://pa.9csxet.cn

[U89] JS：数组去重
来源：http://ix.521024.cn

[...new Set(arr)]
来源：http://ky.newstarts.cn

[U90] JS：数字数组排序
来源：http://jl.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://fs.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://rk.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oa.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://hk.jctech888.com.cn

structuredClone(obj)
来源：http://px.gzmigu.cn

[U93] JS：模板字符串
来源：http://kr.szxytkj.cn

`共 ${n} 条`
来源：http://kr.9csxet.cn

[U94] JS：箭头函数
来源：http://nz.szsharing.cn

const double = x => x * 2;
来源：http://sq.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://ty.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://sk.nicolike.cn

[U96] JS：async/await 与异常
来源：http://de.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zy.colortex.cn

[U97] JS：并发请求
来源：http://fm.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://wn.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ac.chemitech.net.cn

[U99] JS：事件监听
来源：http://ot.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://lp.colortex.cn

[U100] JS：DOM 查询
来源：http://sz.9csxet.cn

document.querySelector(".item")
来源：http://rt.wgjwhj.cn

[U101] JS：classList 操作
来源：http://us.9csxet.cn

el.classList.toggle("active")
来源：http://ew.muxihuayi.cn

[U102] JS：本地存储
来源：http://qi.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zj.9csxet.cn

[U103] JS：定时器
来源：http://du.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ar.gzmigu.cn

[U104] JS：防抖
来源：http://pb.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wd.chemitech.net.cn

[U105] JS：节流
来源：http://uk.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://li.wgjwhj.cn

[U106] JS：日期格式化
来源：http://bd.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wo.gzmigu.cn

[U107] JS：数字千分位
来源：http://mb.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ns.asd995.cn

[U108] JS：随机整数
来源：http://xz.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ot.huanxung.cn

[U109] JS：数组分组
来源：http://rs.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://on.shtwfgs.cn

[U110] JS：数组分块
来源：http://yp.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://il.huanxung.cn

[U111] JS：对象转 Map
来源：http://wa.9csxet.cn

new Map(Object.entries(obj))
来源：http://np.colortex.cn

[U112] JS：字符串补位
来源：http://mc.szxytkj.cn

"7".padStart(3, "0")
来源：http://pv.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://zw.huanxung.cn

s.replaceAll("a", "b")
来源：http://pa.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://bu.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ax.nicolike.cn

[U115] JS：生成 UUID
来源：http://hk.haigaiapp.cn

crypto.randomUUID()
来源：http://fz.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://uc.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://ls.wgjwhj.cn

[U117] JS：单元测试
来源：http://xz.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://wz.huanxung.cn

[U118] JS：开发服务器
来源：http://lw.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://aw.hnjuh.cn

[U119] JS：生产构建
来源：http://pq.huixiangedu.cn

npx vite build
来源：http://xs.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://av.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://tp.nicolike.cn

================================================================================
来源：http://ln.hnjuh.cn

统计汇总
来源：http://uo.hnjuh.cn

================================================================================
来源：http://rd.bjjhwx.cn

按语言统计（条）：
来源：http://kz.huixiangedu.cn

Python ......... 252
来源：http://st.521024.cn

PHP ............ 252
来源：http://qz.bookmarksfly.cn

JavaScript ..... 252
来源：http://eu.gzmigu.cn

TypeScript ..... 212
来源：http://ta.shxzskj.cn

Java ........... 212
来源：http://gm.bookmarksfly.cn

Go ............. 212
来源：http://yh.huixinmuqiang.cn

Ruby ........... 212
来源：http://uw.szxytkj.cn

C# ............. 212
来源：http://yy.shxzskj.cn

C .............. 30
来源：http://nf.szxytkj.cn

C++ ............ 30
来源：http://de.nicolike.cn

SQL ............ 90
来源：http://pn.huanxung.cn

Bash ........... 80
来源：http://ey.huixinmuqiang.cn

Kotlin ......... 15
来源：http://sd.yuntaijiaju.cn

Swift .......... 15
来源：http://gq.yuntaijiaju.cn

Lua ............ 10
来源：http://kh.hahajie.cn

Perl ........... 10
来源：http://tk.gzmigu.cn

Scala .......... 10
来源：http://lw.521024.cn

------------------------------------
来源：http://po.szsharing.cn

合计 ........... 2106 条
来源：http://kl.chemitech.net.cn

按章节统计：
来源：http://yy.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mi.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dv.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mq.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uz.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bh.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bb.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yx.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gq.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pu.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tg.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sm.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ep.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jn.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jb.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ek.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vc.panjiajie.cn

Q SQL 专题                              90
来源：http://dj.shxzukj.cn

R Bash 专题                             80
来源：http://xq.yuexingan06.cn

S C / C++ 专题                          60
来源：http://vy.jctech888.com.cn

T 其他语言补充                          60
来源：http://aa.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://er.haigaiapp.cn

------------------------------------
来源：http://cj.panjiajie.cn

合计                                  2106 条
来源：http://cn.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://eq.bjjhwx.cn


<!-- 参考信息 -->