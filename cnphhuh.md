代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lc.jianghongdianzi.cn

================================================================================
来源：http://nm.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pl.chemitech.net.cn

================================================================================
来源：http://mp.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://al.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kp.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://lq.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rj.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://up.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hw.hnjuh.cn

[U04] Py：变量调试打印
来源：http://be.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jd.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://hq.hahajie.cn

list(dict.fromkeys(arr))
来源：http://ps.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://wl.haigaiapp.cn

{**a, **b}
来源：http://wq.huanxung.cn

[U07] Py：反转字典键值
来源：http://ge.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://ha.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://ht.asd995.cn

[y for x in nested for y in x]
来源：http://kg.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://zv.yuexingan06.cn

max(d, key=d.get)
来源：http://um.521024.cn

[U10] Py：按值排序字典
来源：http://dd.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mc.9csxet.cn

[U11] Py：生成器表达式
来源：http://af.nszjky.cn

(x * 2 for x in arr)
来源：http://kp.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xo.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ql.shxzukj.cn

[U13] Py：固定长度队列
来源：http://wj.yuntaijiaju.cn

deque(maxlen=10)
来源：http://qz.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://oh.chemitech.net.cn

defaultdict(list)
来源：http://ju.huixiangedu.cn

[U15] Py：高精度计时
来源：http://jn.colortex.cn

t = time.perf_counter()
来源：http://ge.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://qn.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bc.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ta.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://po.nicolike.cn

[U18] Py：预编译正则
来源：http://fp.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://cd.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://fn.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yv.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://as.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://pa.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://mr.gzmigu.cn

@contextlib.contextmanager
来源：http://dv.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://dy.yuexingan06.cn

list(zip(*m))
来源：http://xa.521024.cn

[U23] Py：分块读取大文件
来源：http://fl.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mk.chemitech.net.cn

[U24] Py：路径操作
来源：http://fo.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ep.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://ou.lnxyls.cn

csv.DictReader(f)
来源：http://di.yuexingan06.cn

[U26] Py：并发下载
来源：http://if.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ur.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ii.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://at.panjiajie.cn

[U28] Py：类型别名
来源：http://yq.wgjwhj.cn

UserId = int
来源：http://am.colortex.cn

[U29] Py：属性校验
来源：http://ue.colortex.cn

@property 与 @x.setter 配合
来源：http://hz.chemitech.net.cn

[U30] Py：数据类
来源：http://le.newstarts.cn

@dataclass(slots=True)
来源：http://ge.bjjhwx.cn

[U31] Py：单测
来源：http://ki.newstarts.cn

python -m pytest -q
来源：http://vu.colortex.cn

[U32] Py：代码格式化
来源：http://rz.521024.cn

ruff format . && ruff check --fix .
来源：http://cl.bookmarksfly.cn

[U33] Py：打包发布
来源：http://do.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://xh.asd995.cn

[U34] Py：判断编码
来源：http://mc.szsharing.cn

chardet.detect(raw)
来源：http://xd.hnjuh.cn

[U35] Py：发送邮件
来源：http://va.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lu.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://oh.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://cb.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://we.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lb.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://qf.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://og.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://jv.nszjky.cn

sys.stdout.isatty()
来源：http://zv.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://vx.newstarts.cn

print("err", file=sys.stderr)
来源：http://ht.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://zo.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hi.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ds.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://om.9csxet.cn

[U43] PHP：声明命名空间
来源：http://qw.huixinmuqiang.cn

namespace App\Http;
来源：http://ya.nszjky.cn

[U44] PHP：开启严格类型
来源：http://lk.yuexingan06.cn

declare(strict_types=1);
来源：http://ec.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://zq.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ne.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://sy.szsharing.cn

?string $name = null
来源：http://ni.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://uw.yuexingan06.cn

int|string $id
来源：http://dg.nicolike.cn

[U48] PHP：纯枚举
来源：http://pr.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xw.huanxung.cn

[U49] PHP：只读属性
来源：http://wp.hahajie.cn

public readonly string $name
来源：http://zl.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ga.newstarts.cn

public function __construct(private int $id) {}
来源：http://hj.shxzskj.cn

[U51] PHP：数组解构
来源：http://xp.asd995.cn

[$a, $b] = $arr;
来源：http://qg.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://ng.asd995.cn

$double = fn($x) => $x * 2;
来源：http://is.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://sq.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://re.asd995.cn

[U54] PHP：空安全调用
来源：http://ta.colortex.cn

$obj?->method()
来源：http://kx.szxytkj.cn

[U55] PHP：match 表达式
来源：http://xn.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jl.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://iw.newstarts.cn

f(a: 1, b: 2)
来源：http://rf.hnjuh.cn

[U57] PHP：字符串插值
来源：http://oa.lnxyls.cn

"值: {$a}"
来源：http://la.asd995.cn

[U58] PHP：数组三件套
来源：http://us.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mg.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://or.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gv.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ro.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vx.yuexingan06.cn

[U61] PHP：正则
来源：http://sd.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tc.yuexingan06.cn

[U62] PHP：日期对象
来源：http://os.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vk.muxihuayi.cn

[U63] PHP：文件读写
来源：http://hy.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ig.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://cz.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://ev.bookmarksfly.cn

[U65] PHP：会话
来源：http://nc.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vy.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://vp.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rz.nicolike.cn

[U67] PHP：处理文件上传
来源：http://be.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pp.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://aa.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pi.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://ez.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://um.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://vq.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jn.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://tv.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://rc.521024.cn

[U72] PHP：写错误日志
来源：http://fm.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://uv.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://gb.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://ml.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://cm.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://ej.gzmigu.cn

[U75] PHP：依赖注入
来源：http://ag.bookmarksfly.cn

composer require psr/container
来源：http://ep.yuexingan06.cn

[U76] PHP：简单路由
来源：http://fv.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sl.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://lc.colortex.cn

composer require twig/twig
来源：http://pw.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ka.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://zn.nicolike.cn

[U79] PHP：静态分析
来源：http://ms.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://bs.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://vs.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jo.shxzskj.cn

[U81] JS：初始化项目
来源：http://jy.gzmigu.cn

npm init -y;  npm i express
来源：http://gq.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://io.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wi.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://se.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bf.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://cf.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kv.szsharing.cn

[U85] JS：可选链
来源：http://jj.wgjwhj.cn

a?.b?.c
来源：http://rt.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://zr.521024.cn

a ?? b
来源：http://qm.colortex.cn

[U87] JS：解构默认值
来源：http://xq.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://fs.hnjuh.cn

[U88] JS：对象展开合并
来源：http://qt.nszjky.cn

{ ...a, ...b }
来源：http://rj.wgjwhj.cn

[U89] JS：数组去重
来源：http://cj.muxihuayi.cn

[...new Set(arr)]
来源：http://hy.szsharing.cn

[U90] JS：数字数组排序
来源：http://yd.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://zp.521024.cn

[U91] JS：对象键值遍历
来源：http://ob.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.shtwfgs.cn

[U92] JS：深拷贝
来源：http://rb.shxzukj.cn

structuredClone(obj)
来源：http://yi.shxzskj.cn

[U93] JS：模板字符串
来源：http://ti.szxytkj.cn

`共 ${n} 条`
来源：http://np.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://kk.huanxung.cn

const double = x => x * 2;
来源：http://yx.colortex.cn

[U95] JS：Promise 包装
来源：http://xp.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://bd.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://no.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lk.shtwfgs.cn

[U97] JS：并发请求
来源：http://tz.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dr.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://po.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dq.yuexingan06.cn

[U99] JS：事件监听
来源：http://oo.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://nt.gzmigu.cn

[U100] JS：DOM 查询
来源：http://mm.muxihuayi.cn

document.querySelector(".item")
来源：http://dc.521024.cn

[U101] JS：classList 操作
来源：http://tz.shtwfgs.cn

el.classList.toggle("active")
来源：http://lt.nicolike.cn

[U102] JS：本地存储
来源：http://rc.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ro.newstarts.cn

[U103] JS：定时器
来源：http://nx.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fd.shxzukj.cn

[U104] JS：防抖
来源：http://ap.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lo.asd995.cn

[U105] JS：节流
来源：http://ny.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cp.szsharing.cn

[U106] JS：日期格式化
来源：http://eb.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aw.shtwfgs.cn

[U107] JS：数字千分位
来源：http://zk.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ea.shxzukj.cn

[U108] JS：随机整数
来源：http://sf.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ft.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://fr.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ir.szxytkj.cn

[U110] JS：数组分块
来源：http://sw.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ba.gzmigu.cn

[U111] JS：对象转 Map
来源：http://zl.shxzukj.cn

new Map(Object.entries(obj))
来源：http://kn.asd995.cn

[U112] JS：字符串补位
来源：http://sm.hnjuh.cn

"7".padStart(3, "0")
来源：http://jr.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://cy.hnjuh.cn

s.replaceAll("a", "b")
来源：http://ar.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://iy.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kc.9csxet.cn

[U115] JS：生成 UUID
来源：http://go.haigaiapp.cn

crypto.randomUUID()
来源：http://lm.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://qy.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://rw.gzmigu.cn

[U117] JS：单元测试
来源：http://pl.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://tz.wgjwhj.cn

[U118] JS：开发服务器
来源：http://yh.szxytkj.cn

npm i -D vite;  npx vite
来源：http://vo.nszjky.cn

[U119] JS：生产构建
来源：http://qq.hnjuh.cn

npx vite build
来源：http://nh.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://xz.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://tj.szsharing.cn

================================================================================
来源：http://kk.newstarts.cn

统计汇总
来源：http://ym.hahajie.cn

================================================================================
来源：http://el.wgjwhj.cn

按语言统计（条）：
来源：http://kk.huixinmuqiang.cn

Python ......... 252
来源：http://ra.shxzskj.cn

PHP ............ 252
来源：http://xt.9csxet.cn

JavaScript ..... 252
来源：http://cq.chemitech.net.cn

TypeScript ..... 212
来源：http://ax.szsharing.cn

Java ........... 212
来源：http://qo.9csxet.cn

Go ............. 212
来源：http://vg.shxzskj.cn

Ruby ........... 212
来源：http://jd.szxytkj.cn

C# ............. 212
来源：http://rz.nicolike.cn

C .............. 30
来源：http://ep.newstarts.cn

C++ ............ 30
来源：http://ga.9csxet.cn

SQL ............ 90
来源：http://us.hahajie.cn

Bash ........... 80
来源：http://fg.shtwfgs.cn

Kotlin ......... 15
来源：http://ti.colortex.cn

Swift .......... 15
来源：http://ec.jianghongdianzi.cn

Lua ............ 10
来源：http://tl.shtwfgs.cn

Perl ........... 10
来源：http://xc.colortex.cn

Scala .......... 10
来源：http://rg.nszjky.cn

------------------------------------
来源：http://et.bookmarksfly.cn

合计 ........... 2106 条
来源：http://ps.colortex.cn

按章节统计：
来源：http://lz.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zo.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tp.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://un.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oy.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ju.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gf.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fm.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://by.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lv.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dh.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gd.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ci.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ix.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lj.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ac.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lr.nicolike.cn

Q SQL 专题                              90
来源：http://ml.shxzskj.cn

R Bash 专题                             80
来源：http://rd.panjiajie.cn

S C / C++ 专题                          60
来源：http://ie.gzmigu.cn

T 其他语言补充                          60
来源：http://dv.jctech888.com.cn

U 高频实用片段                         120
来源：http://hv.bookmarksfly.cn

------------------------------------
来源：http://mj.newstarts.cn

合计                                  2106 条
来源：http://hr.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://aw.jianghongdianzi.cn

使用提醒
来源：http://kg.asd995.cn

--------------------------------------------------------------------------------
来源：http://we.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iu.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xh.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sw.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xk.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wb.9csxet.cn

—— 文件结束 ——
来源：http://lo.yuntaijiaju.cn


<!-- 参考信息 -->