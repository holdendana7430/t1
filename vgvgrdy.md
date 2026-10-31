代发 wailian999

case class User(name: String, age: Int)
来源：http://hg.szsharing.cn

[T57] Scala：模式匹配
来源：http://xh.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ns.nicolike.cn

[T58] Scala：函数定义
来源：http://bw.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yh.colortex.cn

[T59] Scala：循环
来源：http://bk.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://ek.huixiangedu.cn

[T60] Scala：折叠
来源：http://rr.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sn.wgjwhj.cn

================================================================================
来源：http://xt.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://us.lnxyls.cn

================================================================================
来源：http://tb.asd995.cn

[U01] Py：创建虚拟环境
来源：http://vx.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nc.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://br.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://go.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://hj.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ei.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://pu.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ip.nszjky.cn

[U05] Py：列表去重且保序
来源：http://rm.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://mu.colortex.cn

[U06] Py：合并两个字典
来源：http://vn.nszjky.cn

{**a, **b}
来源：http://os.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://rf.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://eq.lnxyls.cn

[U08] Py：展平二维列表
来源：http://hj.asd995.cn

[y for x in nested for y in x]
来源：http://pe.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://rx.bookmarksfly.cn

max(d, key=d.get)
来源：http://tv.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://dn.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xn.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://dt.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://oc.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://el.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://xr.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://vy.521024.cn

deque(maxlen=10)
来源：http://va.colortex.cn

[U14] Py：分组收集到列表
来源：http://fn.huanxung.cn

defaultdict(list)
来源：http://xa.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://oo.shxzskj.cn

t = time.perf_counter()
来源：http://vo.szsharing.cn

[U16] Py：命令行参数解析
来源：http://fj.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://no.huanxung.cn

[U17] Py：初始化日志
来源：http://zg.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://lb.huixiangedu.cn

[U18] Py：预编译正则
来源：http://tl.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://km.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://yo.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ki.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://ys.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://ax.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://lq.shtwfgs.cn

@contextlib.contextmanager
来源：http://ui.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://yx.huanxung.cn

list(zip(*m))
来源：http://qb.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://wu.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qb.521024.cn

[U24] Py：路径操作
来源：http://ea.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zn.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://lx.huanxung.cn

csv.DictReader(f)
来源：http://ma.bjjhwx.cn

[U26] Py：并发下载
来源：http://yu.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xa.9csxet.cn

[U27] Py：异步 HTTP
来源：http://ea.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://bn.szsharing.cn

[U28] Py：类型别名
来源：http://ro.huixinmuqiang.cn

UserId = int
来源：http://az.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://kq.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://qv.nszjky.cn

[U30] Py：数据类
来源：http://iu.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ai.szsharing.cn

[U31] Py：单测
来源：http://cj.haigaiapp.cn

python -m pytest -q
来源：http://jy.nszjky.cn

[U32] Py：代码格式化
来源：http://kd.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://sd.521024.cn

[U33] Py：打包发布
来源：http://iu.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://fs.huixiangedu.cn

[U34] Py：判断编码
来源：http://pn.haigaiapp.cn

chardet.detect(raw)
来源：http://ik.huanxung.cn

[U35] Py：发送邮件
来源：http://lq.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gp.bjjhwx.cn

[U36] Py：定时任务
来源：http://yn.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://bg.huanxung.cn

[U37] Py：读写 Excel
来源：http://ek.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hj.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://pf.huanxung.cn

Path(__file__).resolve().parent
来源：http://nw.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://rl.9csxet.cn

sys.stdout.isatty()
来源：http://ix.nszjky.cn

[U40] Py：打印到标准错误
来源：http://fc.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://wv.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://qm.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ln.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://yk.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uu.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://pe.szxytkj.cn

namespace App\Http;
来源：http://bf.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://pz.shxzskj.cn

declare(strict_types=1);
来源：http://bl.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://nh.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://py.jctech888.com.cn

[U46] PHP：可空类型
来源：http://ap.shtwfgs.cn

?string $name = null
来源：http://lp.szxytkj.cn

[U47] PHP：联合类型
来源：http://va.yuntaijiaju.cn

int|string $id
来源：http://qe.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://hh.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ka.hahajie.cn

[U49] PHP：只读属性
来源：http://ca.nicolike.cn

public readonly string $name
来源：http://sd.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://uf.shxzskj.cn

public function __construct(private int $id) {}
来源：http://re.nszjky.cn

[U51] PHP：数组解构
来源：http://gc.lnxyls.cn

[$a, $b] = $arr;
来源：http://ny.hnjuh.cn

[U52] PHP：箭头函数
来源：http://uv.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://fi.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://bz.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://sd.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://ex.nicolike.cn

$obj?->method()
来源：http://pm.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://vj.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rq.colortex.cn

[U56] PHP：命名参数
来源：http://iq.nicolike.cn

f(a: 1, b: 2)
来源：http://cc.colortex.cn

[U57] PHP：字符串插值
来源：http://we.huixiangedu.cn

"值: {$a}"
来源：http://yl.newstarts.cn

[U58] PHP：数组三件套
来源：http://mz.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://my.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ty.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ez.asd995.cn

[U60] PHP：JSON 编解码
来源：http://xc.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://us.chemitech.net.cn

[U61] PHP：正则
来源：http://sp.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jf.haigaiapp.cn

[U62] PHP：日期对象
来源：http://gd.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nh.asd995.cn

[U63] PHP：文件读写
来源：http://ou.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xw.hahajie.cn

[U64] PHP：目录遍历
来源：http://rj.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ql.huanxung.cn

[U65] PHP：会话
来源：http://iy.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bn.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://bw.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yr.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://cn.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dm.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://ig.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://du.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://xp.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hl.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://uu.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vh.lnxyls.cn

[U71] PHP：抛出异常
来源：http://nx.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://ui.9csxet.cn

[U72] PHP：写错误日志
来源：http://yn.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://do.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://qx.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://ou.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://lo.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://xo.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://sg.gzmigu.cn

composer require psr/container
来源：http://jd.haigaiapp.cn

[U76] PHP：简单路由
来源：http://zd.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bo.nszjky.cn

[U77] PHP：模板渲染
来源：http://ar.colortex.cn

composer require twig/twig
来源：http://zh.panjiajie.cn

[U78] PHP：单元测试
来源：http://if.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://ag.wgjwhj.cn

[U79] PHP：静态分析
来源：http://cg.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://eg.9csxet.cn

[U80] PHP：代码规范修复
来源：http://qr.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cd.shxzukj.cn

[U81] JS：初始化项目
来源：http://ip.bjjhwx.cn

npm init -y;  npm i express
来源：http://iq.szsharing.cn

[U82] JS：package.json 脚本
来源：http://gi.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dr.521024.cn

[U83] JS：ES Module 导入导出
来源：http://df.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jp.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://sh.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wj.asd995.cn

[U85] JS：可选链
来源：http://xc.lnxyls.cn

a?.b?.c
来源：http://ai.hnjuh.cn

[U86] JS：空值合并
来源：http://ee.asd995.cn

a ?? b
来源：http://sg.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://za.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://ab.hnjuh.cn

[U88] JS：对象展开合并
来源：http://qy.muxihuayi.cn

{ ...a, ...b }
来源：http://fl.asd995.cn

[U89] JS：数组去重
来源：http://ab.lnxyls.cn

[...new Set(arr)]
来源：http://bb.hnjuh.cn

[U90] JS：数字数组排序
来源：http://zu.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://oq.nszjky.cn

[U91] JS：对象键值遍历
来源：http://yd.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fa.hnjuh.cn

[U92] JS：深拷贝
来源：http://ll.huanxung.cn

structuredClone(obj)
来源：http://ft.huanxung.cn

[U93] JS：模板字符串
来源：http://tc.lnxyls.cn

`共 ${n} 条`
来源：http://wl.nicolike.cn

[U94] JS：箭头函数
来源：http://wf.panjiajie.cn

const double = x => x * 2;
来源：http://gc.colortex.cn

[U95] JS：Promise 包装
来源：http://ob.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://lk.szsharing.cn

[U96] JS：async/await 与异常
来源：http://yd.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://em.9csxet.cn

[U97] JS：并发请求
来源：http://gm.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gi.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://se.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yk.shtwfgs.cn

[U99] JS：事件监听
来源：http://ge.521024.cn

el.addEventListener("click", e => {})
来源：http://zf.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://zr.colortex.cn

document.querySelector(".item")
来源：http://hq.haigaiapp.cn

[U101] JS：classList 操作
来源：http://ph.panjiajie.cn

el.classList.toggle("active")
来源：http://bb.szxytkj.cn

[U102] JS：本地存储
来源：http://ej.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yf.newstarts.cn

[U103] JS：定时器
来源：http://hz.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zr.nicolike.cn

[U104] JS：防抖
来源：http://dt.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cp.nszjky.cn

[U105] JS：节流
来源：http://cb.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pf.asd995.cn

[U106] JS：日期格式化
来源：http://fi.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wm.gzmigu.cn

[U107] JS：数字千分位
来源：http://kc.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ak.bookmarksfly.cn

[U108] JS：随机整数
来源：http://fx.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ju.jctech888.com.cn

[U109] JS：数组分组
来源：http://mk.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://mh.hahajie.cn

[U110] JS：数组分块
来源：http://lq.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gi.521024.cn

[U111] JS：对象转 Map
来源：http://xz.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://hm.yuexingan06.cn

[U112] JS：字符串补位
来源：http://gr.bjjhwx.cn

"7".padStart(3, "0")
来源：http://ea.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://zl.9csxet.cn

s.replaceAll("a", "b")
来源：http://td.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://sd.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sw.panjiajie.cn

[U115] JS：生成 UUID
来源：http://cw.huixiangedu.cn

crypto.randomUUID()
来源：http://la.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://uc.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://rb.panjiajie.cn

[U117] JS：单元测试
来源：http://sv.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://zo.huixiangedu.cn

[U118] JS：开发服务器
来源：http://hk.hahajie.cn

npm i -D vite;  npx vite
来源：http://vx.newstarts.cn

[U119] JS：生产构建
来源：http://dy.yuntaijiaju.cn

npx vite build
来源：http://sl.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://jz.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://js.panjiajie.cn

================================================================================
来源：http://zf.huanxung.cn

统计汇总
来源：http://ls.chemitech.net.cn

================================================================================
来源：http://ui.shxzukj.cn

按语言统计（条）：
来源：http://xj.panjiajie.cn

Python ......... 252
来源：http://ko.asd995.cn

PHP ............ 252
来源：http://jn.jctech888.com.cn

JavaScript ..... 252
来源：http://uz.9csxet.cn

TypeScript ..... 212
来源：http://pv.panjiajie.cn

Java ........... 212
来源：http://vx.nszjky.cn

Go ............. 212
来源：http://zq.haigaiapp.cn

Ruby ........... 212
来源：http://pq.panjiajie.cn

C# ............. 212
来源：http://il.hnjuh.cn

C .............. 30
来源：http://if.huixiangedu.cn

C++ ............ 30
来源：http://yd.szxytkj.cn

SQL ............ 90
来源：http://ip.muxihuayi.cn

Bash ........... 80
来源：http://no.szsharing.cn

Kotlin ......... 15
来源：http://zu.hahajie.cn

Swift .......... 15
来源：http://nf.huixinmuqiang.cn

Lua ............ 10
来源：http://dg.wgjwhj.cn

Perl ........... 10
来源：http://us.szsharing.cn

Scala .......... 10
来源：http://fo.huanxung.cn

------------------------------------
来源：http://fc.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://jz.jctech888.com.cn

按章节统计：
来源：http://xo.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qb.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rn.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lm.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ux.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pv.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://du.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qe.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ar.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hs.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qy.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iu.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xa.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yt.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qi.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cg.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fo.hahajie.cn

Q SQL 专题                              90
来源：http://ma.chemitech.net.cn

R Bash 专题                             80
来源：http://in.wgjwhj.cn

S C / C++ 专题                          60
来源：http://ln.gzmigu.cn

T 其他语言补充                          60
来源：http://rw.lnxyls.cn

U 高频实用片段                         120
来源：http://sj.jianghongdianzi.cn

------------------------------------
来源：http://ut.panjiajie.cn

合计                                  2106 条
来源：http://fm.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ui.bjjhwx.cn


<!-- 参考信息 -->