代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://xc.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://jz.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vv.wgjwhj.cn

[T56] Scala：样例类
来源：http://go.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ic.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ka.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jp.yuexingan06.cn

[T58] Scala：函数定义
来源：http://ep.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jw.shtwfgs.cn

[T59] Scala：循环
来源：http://uq.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://ig.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://xm.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sa.nicolike.cn

================================================================================
来源：http://sb.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qj.muxihuayi.cn

================================================================================
来源：http://yw.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://hc.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kd.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://ow.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ma.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://jh.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sc.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://ns.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bz.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ys.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://os.shxzskj.cn

[U06] Py：合并两个字典
来源：http://fb.yuexingan06.cn

{**a, **b}
来源：http://qs.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://wz.nicolike.cn

{v: k for k, v in d.items()}
来源：http://uk.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://oz.asd995.cn

[y for x in nested for y in x]
来源：http://lb.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://ne.lnxyls.cn

max(d, key=d.get)
来源：http://we.9csxet.cn

[U10] Py：按值排序字典
来源：http://ki.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pd.newstarts.cn

[U11] Py：生成器表达式
来源：http://vg.newstarts.cn

(x * 2 for x in arr)
来源：http://ub.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vp.gzmigu.cn

Counter(arr).most_common(3)
来源：http://bq.szsharing.cn

[U13] Py：固定长度队列
来源：http://jj.bjjhwx.cn

deque(maxlen=10)
来源：http://wk.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://fl.szsharing.cn

defaultdict(list)
来源：http://iw.muxihuayi.cn

[U15] Py：高精度计时
来源：http://mt.nicolike.cn

t = time.perf_counter()
来源：http://wm.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ec.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kw.hahajie.cn

[U17] Py：初始化日志
来源：http://an.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://tm.521024.cn

[U18] Py：预编译正则
来源：http://sf.hahajie.cn

pat = re.compile(r"\d+")
来源：http://zz.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://iu.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vb.huanxung.cn

[U20] Py：缓存函数结果
来源：http://tu.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://pt.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://nx.gzmigu.cn

@contextlib.contextmanager
来源：http://uv.521024.cn

[U22] Py：矩阵转置
来源：http://br.muxihuayi.cn

list(zip(*m))
来源：http://ix.521024.cn

[U23] Py：分块读取大文件
来源：http://jy.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://as.lnxyls.cn

[U24] Py：路径操作
来源：http://br.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ye.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://ic.muxihuayi.cn

csv.DictReader(f)
来源：http://ph.shtwfgs.cn

[U26] Py：并发下载
来源：http://vu.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lr.colortex.cn

[U27] Py：异步 HTTP
来源：http://ga.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://mp.shxzskj.cn

[U28] Py：类型别名
来源：http://lo.huixiangedu.cn

UserId = int
来源：http://bf.shtwfgs.cn

[U29] Py：属性校验
来源：http://ke.asd995.cn

@property 与 @x.setter 配合
来源：http://xv.nicolike.cn

[U30] Py：数据类
来源：http://ow.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://un.jctech888.com.cn

[U31] Py：单测
来源：http://ly.yuntaijiaju.cn

python -m pytest -q
来源：http://ta.huanxung.cn

[U32] Py：代码格式化
来源：http://ah.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://dn.szxytkj.cn

[U33] Py：打包发布
来源：http://fb.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://fb.szsharing.cn

[U34] Py：判断编码
来源：http://xg.yuexingan06.cn

chardet.detect(raw)
来源：http://bv.wgjwhj.cn

[U35] Py：发送邮件
来源：http://lb.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yw.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://tx.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://bx.nicolike.cn

[U37] Py：读写 Excel
来源：http://du.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xk.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://sr.szxytkj.cn

Path(__file__).resolve().parent
来源：http://tl.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://sw.bjjhwx.cn

sys.stdout.isatty()
来源：http://mi.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://ci.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://jp.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://or.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fw.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://ba.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://of.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://kr.wgjwhj.cn

namespace App\Http;
来源：http://aa.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://uf.shxzukj.cn

declare(strict_types=1);
来源：http://fs.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://dz.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gr.9csxet.cn

[U46] PHP：可空类型
来源：http://ti.szsharing.cn

?string $name = null
来源：http://ru.asd995.cn

[U47] PHP：联合类型
来源：http://gg.muxihuayi.cn

int|string $id
来源：http://rl.lnxyls.cn

[U48] PHP：纯枚举
来源：http://kk.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hi.shxzukj.cn

[U49] PHP：只读属性
来源：http://bu.hahajie.cn

public readonly string $name
来源：http://hf.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://zj.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://rp.jctech888.com.cn

[U51] PHP：数组解构
来源：http://ep.wgjwhj.cn

[$a, $b] = $arr;
来源：http://mu.hnjuh.cn

[U52] PHP：箭头函数
来源：http://ix.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://sb.nicolike.cn

[U53] PHP：空合并运算符
来源：http://gt.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ra.521024.cn

[U54] PHP：空安全调用
来源：http://xo.haigaiapp.cn

$obj?->method()
来源：http://ch.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ib.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nz.9csxet.cn

[U56] PHP：命名参数
来源：http://wz.asd995.cn

f(a: 1, b: 2)
来源：http://ys.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://vf.asd995.cn

"值: {$a}"
来源：http://rt.szxytkj.cn

[U58] PHP：数组三件套
来源：http://si.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://el.asd995.cn

[U59] PHP：自定义排序
来源：http://sx.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vv.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://rl.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qd.521024.cn

[U61] PHP：正则
来源：http://ht.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ls.huanxung.cn

[U62] PHP：日期对象
来源：http://zq.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sy.shxzukj.cn

[U63] PHP：文件读写
来源：http://gt.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pr.gzmigu.cn

[U64] PHP：目录遍历
来源：http://tt.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ty.szsharing.cn

[U65] PHP：会话
来源：http://os.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wn.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://qt.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ek.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://wn.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ex.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://bb.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mv.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://gm.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gu.newstarts.cn

[U70] PHP：PDO 事务
来源：http://yr.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vg.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://ou.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://mw.nicolike.cn

[U72] PHP：写错误日志
来源：http://bw.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://rs.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://ac.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://ji.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://te.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://wc.9csxet.cn

[U75] PHP：依赖注入
来源：http://sa.huixiangedu.cn

composer require psr/container
来源：http://gs.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://kw.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ng.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://el.wgjwhj.cn

composer require twig/twig
来源：http://yj.huixiangedu.cn

[U78] PHP：单元测试
来源：http://rv.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://ql.szsharing.cn

[U79] PHP：静态分析
来源：http://xt.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://ly.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://my.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ws.shtwfgs.cn

[U81] JS：初始化项目
来源：http://tr.hnjuh.cn

npm init -y;  npm i express
来源：http://xb.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://hp.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ma.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://yv.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oa.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://es.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zl.huixiangedu.cn

[U85] JS：可选链
来源：http://xb.shxzukj.cn

a?.b?.c
来源：http://qt.hnjuh.cn

[U86] JS：空值合并
来源：http://us.9csxet.cn

a ?? b
来源：http://cn.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ff.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://xn.shxzukj.cn

[U88] JS：对象展开合并
来源：http://oi.yuntaijiaju.cn

{ ...a, ...b }
来源：http://uy.gzmigu.cn

[U89] JS：数组去重
来源：http://ui.lnxyls.cn

[...new Set(arr)]
来源：http://wu.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://cp.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://hw.asd995.cn

[U91] JS：对象键值遍历
来源：http://hm.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ow.jctech888.com.cn

[U92] JS：深拷贝
来源：http://za.nszjky.cn

structuredClone(obj)
来源：http://wz.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://jf.9csxet.cn

`共 ${n} 条`
来源：http://ca.521024.cn

[U94] JS：箭头函数
来源：http://vg.huixinmuqiang.cn

const double = x => x * 2;
来源：http://do.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://fs.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://eb.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://cs.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yu.hahajie.cn

[U97] JS：并发请求
来源：http://la.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://fb.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wc.shxzskj.cn

[U99] JS：事件监听
来源：http://tz.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://pr.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://ly.yuexingan06.cn

document.querySelector(".item")
来源：http://ab.gzmigu.cn

[U101] JS：classList 操作
来源：http://gz.huanxung.cn

el.classList.toggle("active")
来源：http://ad.haigaiapp.cn

[U102] JS：本地存储
来源：http://eg.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zn.nszjky.cn

[U103] JS：定时器
来源：http://qa.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mm.shxzukj.cn

[U104] JS：防抖
来源：http://xz.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ex.szsharing.cn

[U105] JS：节流
来源：http://zh.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://it.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://zu.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rx.colortex.cn

[U107] JS：数字千分位
来源：http://rb.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ey.szxytkj.cn

[U108] JS：随机整数
来源：http://in.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nx.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://qj.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://tz.jctech888.com.cn

[U110] JS：数组分块
来源：http://mq.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rq.shxzukj.cn

[U111] JS：对象转 Map
来源：http://op.szsharing.cn

new Map(Object.entries(obj))
来源：http://xp.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://pg.nicolike.cn

"7".padStart(3, "0")
来源：http://in.shxzukj.cn

[U113] JS：正则替换全部
来源：http://zw.panjiajie.cn

s.replaceAll("a", "b")
来源：http://jm.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://mg.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zl.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://mw.muxihuayi.cn

crypto.randomUUID()
来源：http://rg.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://er.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://aj.huixiangedu.cn

[U117] JS：单元测试
来源：http://so.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://tt.hahajie.cn

[U118] JS：开发服务器
来源：http://cy.hnjuh.cn

npm i -D vite;  npx vite
来源：http://ah.szsharing.cn

[U119] JS：生产构建
来源：http://an.hahajie.cn

npx vite build
来源：http://ry.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://vw.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://aw.huixiangedu.cn

================================================================================
来源：http://ob.asd995.cn

统计汇总
来源：http://tc.szxytkj.cn

================================================================================
来源：http://pl.shxzukj.cn

按语言统计（条）：
来源：http://oq.yuntaijiaju.cn

Python ......... 252
来源：http://ei.bjjhwx.cn

PHP ............ 252
来源：http://al.huanxung.cn

JavaScript ..... 252
来源：http://el.lnxyls.cn

TypeScript ..... 212
来源：http://ie.wgjwhj.cn

Java ........... 212
来源：http://ss.huixiangedu.cn

Go ............. 212
来源：http://mj.521024.cn

Ruby ........... 212
来源：http://su.hnjuh.cn

C# ............. 212
来源：http://lf.asd995.cn

C .............. 30
来源：http://gn.521024.cn

C++ ............ 30
来源：http://nk.huixinmuqiang.cn

SQL ............ 90
来源：http://wr.huixiangedu.cn

Bash ........... 80
来源：http://na.bjjhwx.cn

Kotlin ......... 15
来源：http://qj.szxytkj.cn

Swift .......... 15
来源：http://oi.haigaiapp.cn

Lua ............ 10
来源：http://pf.lnxyls.cn

Perl ........... 10
来源：http://ma.jianghongdianzi.cn

Scala .......... 10
来源：http://ly.wgjwhj.cn

------------------------------------
来源：http://nd.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://lx.huixiangedu.cn

按章节统计：
来源：http://cw.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ki.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qu.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pe.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ba.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wt.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qw.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://az.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nf.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lu.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nt.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xz.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://km.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pb.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://al.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lw.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rl.9csxet.cn

Q SQL 专题                              90
来源：http://op.chemitech.net.cn

R Bash 专题                             80
来源：http://ap.chemitech.net.cn

S C / C++ 专题                          60
来源：http://pe.lnxyls.cn

T 其他语言补充                          60
来源：http://vo.szsharing.cn


<!-- 参考信息 -->