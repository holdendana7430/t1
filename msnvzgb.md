代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://ib.colortex.cn

[T59] Scala：循环
来源：http://ds.521024.cn

for (i <- 1 to 10) println(i)
来源：http://by.bookmarksfly.cn

[T60] Scala：折叠
来源：http://fd.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rn.nszjky.cn

================================================================================
来源：http://oz.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xs.bookmarksfly.cn

================================================================================
来源：http://ad.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://si.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yh.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://qr.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iw.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://ck.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nj.szxytkj.cn

[U04] Py：变量调试打印
来源：http://ar.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pl.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://zp.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://ak.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://rd.jianghongdianzi.cn

{**a, **b}
来源：http://vs.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://lv.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://uj.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://mq.nszjky.cn

[y for x in nested for y in x]
来源：http://qz.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://gu.szsharing.cn

max(d, key=d.get)
来源：http://fp.gzmigu.cn

[U10] Py：按值排序字典
来源：http://sq.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ds.9csxet.cn

[U11] Py：生成器表达式
来源：http://ch.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://gp.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yj.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://oa.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://hu.colortex.cn

deque(maxlen=10)
来源：http://tt.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://jy.jctech888.com.cn

defaultdict(list)
来源：http://fo.wgjwhj.cn

[U15] Py：高精度计时
来源：http://zz.521024.cn

t = time.perf_counter()
来源：http://tk.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://nm.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://st.yuexingan06.cn

[U17] Py：初始化日志
来源：http://py.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://jp.hnjuh.cn

[U18] Py：预编译正则
来源：http://jo.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://tt.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://ip.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ri.521024.cn

[U20] Py：缓存函数结果
来源：http://pd.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://fc.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://ch.shtwfgs.cn

@contextlib.contextmanager
来源：http://yw.hnjuh.cn

[U22] Py：矩阵转置
来源：http://tp.huanxung.cn

list(zip(*m))
来源：http://se.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://da.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pk.szxytkj.cn

[U24] Py：路径操作
来源：http://ug.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ql.521024.cn

[U25] Py：CSV 按字典读
来源：http://hr.huixiangedu.cn

csv.DictReader(f)
来源：http://zz.jctech888.com.cn

[U26] Py：并发下载
来源：http://vp.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cg.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://ut.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://ny.nicolike.cn

[U28] Py：类型别名
来源：http://bx.muxihuayi.cn

UserId = int
来源：http://ll.huixiangedu.cn

[U29] Py：属性校验
来源：http://do.lnxyls.cn

@property 与 @x.setter 配合
来源：http://uc.huanxung.cn

[U30] Py：数据类
来源：http://iy.jctech888.com.cn

@dataclass(slots=True)
来源：http://mp.jctech888.com.cn

[U31] Py：单测
来源：http://xr.9csxet.cn

python -m pytest -q
来源：http://du.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://so.521024.cn

ruff format . && ruff check --fix .
来源：http://uq.huanxung.cn

[U33] Py：打包发布
来源：http://qy.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://ux.bookmarksfly.cn

[U34] Py：判断编码
来源：http://gv.nicolike.cn

chardet.detect(raw)
来源：http://jt.9csxet.cn

[U35] Py：发送邮件
来源：http://rv.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pw.9csxet.cn

[U36] Py：定时任务
来源：http://xi.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://jp.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://ru.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jz.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://jk.panjiajie.cn

Path(__file__).resolve().parent
来源：http://tw.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://ip.wgjwhj.cn

sys.stdout.isatty()
来源：http://gs.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ah.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://uc.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ov.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rj.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://jp.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://up.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://xy.szxytkj.cn

namespace App\Http;
来源：http://dg.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://vq.yuntaijiaju.cn

declare(strict_types=1);
来源：http://bu.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://rg.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qq.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://ts.jianghongdianzi.cn

?string $name = null
来源：http://su.shxzukj.cn

[U47] PHP：联合类型
来源：http://ar.newstarts.cn

int|string $id
来源：http://vc.9csxet.cn

[U48] PHP：纯枚举
来源：http://dk.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vt.nszjky.cn

[U49] PHP：只读属性
来源：http://al.wgjwhj.cn

public readonly string $name
来源：http://ks.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ll.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://rp.szsharing.cn

[U51] PHP：数组解构
来源：http://oo.colortex.cn

[$a, $b] = $arr;
来源：http://qm.szsharing.cn

[U52] PHP：箭头函数
来源：http://qp.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://eo.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://fi.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://kv.asd995.cn

[U54] PHP：空安全调用
来源：http://zv.shtwfgs.cn

$obj?->method()
来源：http://to.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://vz.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pi.bjjhwx.cn

[U56] PHP：命名参数
来源：http://lp.521024.cn

f(a: 1, b: 2)
来源：http://gl.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://ej.lnxyls.cn

"值: {$a}"
来源：http://et.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://tk.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pt.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://wz.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zh.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://xr.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ru.nicolike.cn

[U61] PHP：正则
来源：http://ep.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rt.szxytkj.cn

[U62] PHP：日期对象
来源：http://zo.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jc.newstarts.cn

[U63] PHP：文件读写
来源：http://ns.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sa.asd995.cn

[U64] PHP：目录遍历
来源：http://yn.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://ax.hnjuh.cn

[U65] PHP：会话
来源：http://mq.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sc.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://bw.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nh.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://qu.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vx.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://vb.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fm.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://wx.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ql.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://xg.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qz.newstarts.cn

[U71] PHP：抛出异常
来源：http://bb.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://kj.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://bw.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ci.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://rw.asd995.cn

parse_ini_file("config.ini", true)
来源：http://st.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://jo.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://ja.newstarts.cn

[U75] PHP：依赖注入
来源：http://yr.yuntaijiaju.cn

composer require psr/container
来源：http://ql.huixiangedu.cn

[U76] PHP：简单路由
来源：http://yg.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ok.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://me.jctech888.com.cn

composer require twig/twig
来源：http://tr.newstarts.cn

[U78] PHP：单元测试
来源：http://nf.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://mh.chemitech.net.cn

[U79] PHP：静态分析
来源：http://gs.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://xh.huanxung.cn

[U80] PHP：代码规范修复
来源：http://kf.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://re.shtwfgs.cn

[U81] JS：初始化项目
来源：http://db.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://nz.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://ma.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jm.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://vw.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rk.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://kn.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dd.521024.cn

[U85] JS：可选链
来源：http://nn.chemitech.net.cn

a?.b?.c
来源：http://nw.shxzskj.cn

[U86] JS：空值合并
来源：http://xc.shtwfgs.cn

a ?? b
来源：http://mh.shtwfgs.cn

[U87] JS：解构默认值
来源：http://tq.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://iq.newstarts.cn

[U88] JS：对象展开合并
来源：http://cd.szxytkj.cn

{ ...a, ...b }
来源：http://gv.gzmigu.cn

[U89] JS：数组去重
来源：http://ux.jianghongdianzi.cn

[...new Set(arr)]
来源：http://wh.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://fl.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://yh.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://dr.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ae.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ay.colortex.cn

structuredClone(obj)
来源：http://jd.newstarts.cn

[U93] JS：模板字符串
来源：http://mc.gzmigu.cn

`共 ${n} 条`
来源：http://qd.shxzskj.cn

[U94] JS：箭头函数
来源：http://dq.jctech888.com.cn

const double = x => x * 2;
来源：http://wj.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://rb.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://os.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://na.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kf.colortex.cn

[U97] JS：并发请求
来源：http://km.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vd.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://bv.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uz.jctech888.com.cn

[U99] JS：事件监听
来源：http://hn.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://fs.hnjuh.cn

[U100] JS：DOM 查询
来源：http://zn.jctech888.com.cn

document.querySelector(".item")
来源：http://ok.huanxung.cn

[U101] JS：classList 操作
来源：http://yb.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://po.asd995.cn

[U102] JS：本地存储
来源：http://zm.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ry.huanxung.cn

[U103] JS：定时器
来源：http://la.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gt.huixinmuqiang.cn

[U104] JS：防抖
来源：http://ml.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lr.yuntaijiaju.cn

[U105] JS：节流
来源：http://lr.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bl.gzmigu.cn

[U106] JS：日期格式化
来源：http://cj.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xn.colortex.cn

[U107] JS：数字千分位
来源：http://mh.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ev.wgjwhj.cn

[U108] JS：随机整数
来源：http://bl.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://co.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://rr.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://hb.hnjuh.cn

[U110] JS：数组分块
来源：http://th.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uu.szsharing.cn

[U111] JS：对象转 Map
来源：http://bj.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://ka.szxytkj.cn

[U112] JS：字符串补位
来源：http://ei.shtwfgs.cn

"7".padStart(3, "0")
来源：http://uv.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://kv.9csxet.cn

s.replaceAll("a", "b")
来源：http://sc.9csxet.cn

[U114] JS：JSON 深比较
来源：http://hm.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ma.shxzskj.cn

[U115] JS：生成 UUID
来源：http://kl.szsharing.cn

crypto.randomUUID()
来源：http://rh.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://oh.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://pr.yuexingan06.cn

[U117] JS：单元测试
来源：http://se.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://oj.yuexingan06.cn

[U118] JS：开发服务器
来源：http://tb.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://pc.shxzskj.cn

[U119] JS：生产构建
来源：http://vr.9csxet.cn

npx vite build
来源：http://ac.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ux.asd995.cn

import.meta.env.VITE_API_URL
来源：http://yp.haigaiapp.cn

================================================================================
来源：http://xy.yuntaijiaju.cn

统计汇总
来源：http://mz.huixinmuqiang.cn

================================================================================
来源：http://wn.haigaiapp.cn

按语言统计（条）：
来源：http://oy.nicolike.cn

Python ......... 252
来源：http://qo.shxzukj.cn

PHP ............ 252
来源：http://px.muxihuayi.cn

JavaScript ..... 252
来源：http://lc.chemitech.net.cn

TypeScript ..... 212
来源：http://ce.nicolike.cn

Java ........... 212
来源：http://qf.asd995.cn

Go ............. 212
来源：http://ll.colortex.cn

Ruby ........... 212
来源：http://to.wgjwhj.cn

C# ............. 212
来源：http://vs.nicolike.cn

C .............. 30
来源：http://op.hahajie.cn

C++ ............ 30
来源：http://cr.hahajie.cn

SQL ............ 90
来源：http://hl.nicolike.cn

Bash ........... 80
来源：http://ig.yuntaijiaju.cn

Kotlin ......... 15
来源：http://bn.colortex.cn

Swift .......... 15
来源：http://dk.lnxyls.cn

Lua ............ 10
来源：http://vf.shxzukj.cn

Perl ........... 10
来源：http://vd.gzmigu.cn

Scala .......... 10
来源：http://bx.newstarts.cn

------------------------------------
来源：http://uq.yuexingan06.cn

合计 ........... 2106 条
来源：http://gj.muxihuayi.cn

按章节统计：
来源：http://hu.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oy.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lh.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eh.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gi.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://it.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tt.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ec.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jl.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rm.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dd.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pq.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hf.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ej.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zc.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bm.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cg.haigaiapp.cn

Q SQL 专题                              90
来源：http://hq.bookmarksfly.cn

R Bash 专题                             80
来源：http://fj.muxihuayi.cn

S C / C++ 专题                          60
来源：http://jy.szsharing.cn

T 其他语言补充                          60
来源：http://qu.wgjwhj.cn

U 高频实用片段                         120
来源：http://qo.szxytkj.cn

------------------------------------
来源：http://we.jctech888.com.cn

合计                                  2106 条
来源：http://mg.newstarts.cn

--------------------------------------------------------------------------------
来源：http://og.chemitech.net.cn

使用提醒
来源：http://ai.newstarts.cn

--------------------------------------------------------------------------------
来源：http://vz.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://at.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ko.hahajie.cn


<!-- 参考信息 -->