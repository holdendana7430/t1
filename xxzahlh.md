代发 wailian999

val a = 1;  var b = 2
来源：http://wa.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://ia.nszjky.cn

s"值: $b"
来源：http://oa.521024.cn

[T54] Scala：集合映射
来源：http://uu.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://lf.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://bh.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yf.huixiangedu.cn

[T56] Scala：样例类
来源：http://gh.panjiajie.cn

case class User(name: String, age: Int)
来源：http://ht.szsharing.cn

[T57] Scala：模式匹配
来源：http://fr.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ww.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://zk.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ho.nszjky.cn

[T59] Scala：循环
来源：http://cj.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://ss.colortex.cn

[T60] Scala：折叠
来源：http://gb.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://so.shtwfgs.cn

================================================================================
来源：http://zb.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ta.shxzukj.cn

================================================================================
来源：http://pg.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://fv.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nc.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://kh.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qp.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://yd.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dg.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://pj.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://ka.nicolike.cn

list(dict.fromkeys(arr))
来源：http://ti.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://kk.521024.cn

{**a, **b}
来源：http://ez.shxzukj.cn

[U07] Py：反转字典键值
来源：http://ty.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://ti.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ww.haigaiapp.cn

[y for x in nested for y in x]
来源：http://wt.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://hx.9csxet.cn

max(d, key=d.get)
来源：http://cu.colortex.cn

[U10] Py：按值排序字典
来源：http://at.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rx.szxytkj.cn

[U11] Py：生成器表达式
来源：http://wu.shxzskj.cn

(x * 2 for x in arr)
来源：http://vs.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://co.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://xy.newstarts.cn

[U13] Py：固定长度队列
来源：http://fx.jianghongdianzi.cn

deque(maxlen=10)
来源：http://uu.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://hk.szsharing.cn

defaultdict(list)
来源：http://fa.521024.cn

[U15] Py：高精度计时
来源：http://kp.huixiangedu.cn

t = time.perf_counter()
来源：http://xe.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://vn.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jb.lnxyls.cn

[U17] Py：初始化日志
来源：http://xu.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://ir.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://oa.newstarts.cn

pat = re.compile(r"\d+")
来源：http://hz.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://qb.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ct.asd995.cn

[U20] Py：缓存函数结果
来源：http://dd.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ha.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://tw.yuexingan06.cn

@contextlib.contextmanager
来源：http://fg.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://mw.hnjuh.cn

list(zip(*m))
来源：http://pb.hahajie.cn

[U23] Py：分块读取大文件
来源：http://cf.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ka.hnjuh.cn

[U24] Py：路径操作
来源：http://qk.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://np.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://vr.bookmarksfly.cn

csv.DictReader(f)
来源：http://tj.szsharing.cn

[U26] Py：并发下载
来源：http://ax.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wk.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://vs.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://yo.nicolike.cn

[U28] Py：类型别名
来源：http://pl.yuntaijiaju.cn

UserId = int
来源：http://ih.newstarts.cn

[U29] Py：属性校验
来源：http://sr.gzmigu.cn

@property 与 @x.setter 配合
来源：http://sy.wgjwhj.cn

[U30] Py：数据类
来源：http://op.nszjky.cn

@dataclass(slots=True)
来源：http://ql.huanxung.cn

[U31] Py：单测
来源：http://eb.newstarts.cn

python -m pytest -q
来源：http://tw.shtwfgs.cn

[U32] Py：代码格式化
来源：http://oc.asd995.cn

ruff format . && ruff check --fix .
来源：http://hb.newstarts.cn

[U33] Py：打包发布
来源：http://lf.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://nf.szsharing.cn

[U34] Py：判断编码
来源：http://fy.szsharing.cn

chardet.detect(raw)
来源：http://hk.huanxung.cn

[U35] Py：发送邮件
来源：http://gc.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bj.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://tf.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://od.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://yy.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yj.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://rn.nszjky.cn

Path(__file__).resolve().parent
来源：http://ah.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://tn.bjjhwx.cn

sys.stdout.isatty()
来源：http://ub.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://ht.nicolike.cn

print("err", file=sys.stderr)
来源：http://cu.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://vi.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://aw.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://rx.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bp.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://tx.szsharing.cn

namespace App\Http;
来源：http://iy.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://sd.bookmarksfly.cn

declare(strict_types=1);
来源：http://tx.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://ut.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://un.jctech888.com.cn

[U46] PHP：可空类型
来源：http://ou.huixiangedu.cn

?string $name = null
来源：http://ld.nszjky.cn

[U47] PHP：联合类型
来源：http://xl.szxytkj.cn

int|string $id
来源：http://of.asd995.cn

[U48] PHP：纯枚举
来源：http://jl.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eo.yuexingan06.cn

[U49] PHP：只读属性
来源：http://bw.huixinmuqiang.cn

public readonly string $name
来源：http://jm.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://nl.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://no.jctech888.com.cn

[U51] PHP：数组解构
来源：http://bo.9csxet.cn

[$a, $b] = $arr;
来源：http://bq.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ub.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://pq.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://gk.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://mu.szxytkj.cn

[U54] PHP：空安全调用
来源：http://uv.huixiangedu.cn

$obj?->method()
来源：http://lv.shxzskj.cn

[U55] PHP：match 表达式
来源：http://lo.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mr.wgjwhj.cn

[U56] PHP：命名参数
来源：http://ze.bjjhwx.cn

f(a: 1, b: 2)
来源：http://ab.shxzskj.cn

[U57] PHP：字符串插值
来源：http://on.huixinmuqiang.cn

"值: {$a}"
来源：http://vc.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://no.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ey.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://mn.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://al.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://dv.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mm.haigaiapp.cn

[U61] PHP：正则
来源：http://wd.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lf.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://zl.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hn.chemitech.net.cn

[U63] PHP：文件读写
来源：http://zb.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yp.huanxung.cn

[U64] PHP：目录遍历
来源：http://fq.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://qb.huixiangedu.cn

[U65] PHP：会话
来源：http://bi.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sg.colortex.cn

[U66] PHP：设置 Cookie
来源：http://qt.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wz.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://rr.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://od.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://uo.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gu.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://st.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gx.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://iz.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xa.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://sc.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://jt.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://jq.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ub.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://hm.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://xf.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://wi.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://zh.nicolike.cn

[U75] PHP：依赖注入
来源：http://gc.huanxung.cn

composer require psr/container
来源：http://wx.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://tp.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fb.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://sy.szsharing.cn

composer require twig/twig
来源：http://qi.wgjwhj.cn

[U78] PHP：单元测试
来源：http://dt.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://mv.asd995.cn

[U79] PHP：静态分析
来源：http://dg.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://oo.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://sy.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nn.szsharing.cn

[U81] JS：初始化项目
来源：http://yb.shxzskj.cn

npm init -y;  npm i express
来源：http://py.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://pp.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iz.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://fr.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jb.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://vk.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yg.9csxet.cn

[U85] JS：可选链
来源：http://pa.chemitech.net.cn

a?.b?.c
来源：http://ud.9csxet.cn

[U86] JS：空值合并
来源：http://el.jctech888.com.cn

a ?? b
来源：http://kt.panjiajie.cn

[U87] JS：解构默认值
来源：http://ca.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://lx.521024.cn

[U88] JS：对象展开合并
来源：http://pg.huixiangedu.cn

{ ...a, ...b }
来源：http://qr.nicolike.cn

[U89] JS：数组去重
来源：http://ut.9csxet.cn

[...new Set(arr)]
来源：http://mx.lnxyls.cn

[U90] JS：数字数组排序
来源：http://kc.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://zn.nicolike.cn

[U91] JS：对象键值遍历
来源：http://vy.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cf.521024.cn

[U92] JS：深拷贝
来源：http://pz.nicolike.cn

structuredClone(obj)
来源：http://vb.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ly.szxytkj.cn

`共 ${n} 条`
来源：http://ax.chemitech.net.cn

[U94] JS：箭头函数
来源：http://wv.colortex.cn

const double = x => x * 2;
来源：http://gg.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://yk.colortex.cn

new Promise((resolve, reject) => {})
来源：http://ho.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://li.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://of.shxzskj.cn

[U97] JS：并发请求
来源：http://ry.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ci.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://ij.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vo.nicolike.cn

[U99] JS：事件监听
来源：http://pv.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://nr.nicolike.cn

[U100] JS：DOM 查询
来源：http://li.haigaiapp.cn

document.querySelector(".item")
来源：http://gb.shtwfgs.cn

[U101] JS：classList 操作
来源：http://fr.shtwfgs.cn

el.classList.toggle("active")
来源：http://co.huanxung.cn

[U102] JS：本地存储
来源：http://na.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ek.jianghongdianzi.cn

[U103] JS：定时器
来源：http://xn.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xb.huixiangedu.cn

[U104] JS：防抖
来源：http://mn.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://td.nicolike.cn

[U105] JS：节流
来源：http://qi.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hn.huanxung.cn

[U106] JS：日期格式化
来源：http://ma.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sz.haigaiapp.cn

[U107] JS：数字千分位
来源：http://wf.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jd.huanxung.cn

[U108] JS：随机整数
来源：http://yv.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qb.bookmarksfly.cn

[U109] JS：数组分组
来源：http://xa.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://yp.huanxung.cn

[U110] JS：数组分块
来源：http://qq.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bj.shxzukj.cn

[U111] JS：对象转 Map
来源：http://al.szxytkj.cn

new Map(Object.entries(obj))
来源：http://pa.colortex.cn

[U112] JS：字符串补位
来源：http://fx.hnjuh.cn

"7".padStart(3, "0")
来源：http://px.gzmigu.cn

[U113] JS：正则替换全部
来源：http://ev.panjiajie.cn

s.replaceAll("a", "b")
来源：http://fo.huanxung.cn

[U114] JS：JSON 深比较
来源：http://ni.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aw.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://tg.9csxet.cn

crypto.randomUUID()
来源：http://rl.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://wj.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://rd.colortex.cn

[U117] JS：单元测试
来源：http://rc.521024.cn

npm i -D vitest;  npx vitest
来源：http://pk.colortex.cn

[U118] JS：开发服务器
来源：http://vr.hnjuh.cn

npm i -D vite;  npx vite
来源：http://kp.shxzukj.cn

[U119] JS：生产构建
来源：http://zz.bjjhwx.cn

npx vite build
来源：http://sc.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://pb.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://jk.wgjwhj.cn

================================================================================
来源：http://ni.521024.cn

统计汇总
来源：http://lo.yuntaijiaju.cn

================================================================================
来源：http://ds.nszjky.cn

按语言统计（条）：
来源：http://jg.bjjhwx.cn

Python ......... 252
来源：http://by.hnjuh.cn

PHP ............ 252
来源：http://lw.nicolike.cn

JavaScript ..... 252
来源：http://ih.colortex.cn

TypeScript ..... 212
来源：http://pd.asd995.cn

Java ........... 212
来源：http://vq.lnxyls.cn

Go ............. 212
来源：http://dr.nszjky.cn

Ruby ........... 212
来源：http://se.521024.cn

C# ............. 212
来源：http://nq.521024.cn

C .............. 30
来源：http://jo.jianghongdianzi.cn

C++ ............ 30
来源：http://kh.shxzukj.cn

SQL ............ 90
来源：http://pn.lnxyls.cn

Bash ........... 80
来源：http://pf.yuexingan06.cn

Kotlin ......... 15
来源：http://bc.haigaiapp.cn

Swift .......... 15
来源：http://es.huixinmuqiang.cn

Lua ............ 10
来源：http://wo.hnjuh.cn

Perl ........... 10
来源：http://xn.haigaiapp.cn

Scala .......... 10
来源：http://wg.nszjky.cn

------------------------------------
来源：http://id.bookmarksfly.cn

合计 ........... 2106 条
来源：http://hy.jianghongdianzi.cn

按章节统计：
来源：http://vi.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yy.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ms.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://il.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zm.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fy.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xt.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dg.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zx.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://us.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sj.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ax.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nv.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://et.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pq.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uk.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fj.huixiangedu.cn


<!-- 参考信息 -->