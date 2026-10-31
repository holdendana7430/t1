代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qu.lnxyls.cn

================================================================================
来源：http://df.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pm.jianghongdianzi.cn

================================================================================
来源：http://ob.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://lz.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iy.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://yr.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tu.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://dc.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cd.shxzukj.cn

[U04] Py：变量调试打印
来源：http://qr.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tf.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://wa.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://la.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://cb.gzmigu.cn

{**a, **b}
来源：http://jl.colortex.cn

[U07] Py：反转字典键值
来源：http://yk.colortex.cn

{v: k for k, v in d.items()}
来源：http://gh.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://ed.szsharing.cn

[y for x in nested for y in x]
来源：http://cp.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://jp.jctech888.com.cn

max(d, key=d.get)
来源：http://nb.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ea.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lx.gzmigu.cn

[U11] Py：生成器表达式
来源：http://qo.colortex.cn

(x * 2 for x in arr)
来源：http://be.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bq.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://cb.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://db.shxzskj.cn

deque(maxlen=10)
来源：http://ak.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://mi.nszjky.cn

defaultdict(list)
来源：http://bh.gzmigu.cn

[U15] Py：高精度计时
来源：http://qf.newstarts.cn

t = time.perf_counter()
来源：http://eu.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://la.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tk.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://ie.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://tp.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ku.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://we.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://ah.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aj.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://fn.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://qu.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://kp.huanxung.cn

@contextlib.contextmanager
来源：http://lm.lnxyls.cn

[U22] Py：矩阵转置
来源：http://sf.521024.cn

list(zip(*m))
来源：http://km.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://bu.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yb.newstarts.cn

[U24] Py：路径操作
来源：http://gw.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ev.asd995.cn

[U25] Py：CSV 按字典读
来源：http://xz.wgjwhj.cn

csv.DictReader(f)
来源：http://zj.9csxet.cn

[U26] Py：并发下载
来源：http://fs.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qu.nicolike.cn

[U27] Py：异步 HTTP
来源：http://jn.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://hs.szxytkj.cn

[U28] Py：类型别名
来源：http://ub.yuexingan06.cn

UserId = int
来源：http://xg.521024.cn

[U29] Py：属性校验
来源：http://qg.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://tt.szxytkj.cn

[U30] Py：数据类
来源：http://bb.huixiangedu.cn

@dataclass(slots=True)
来源：http://cl.szsharing.cn

[U31] Py：单测
来源：http://wn.shxzukj.cn

python -m pytest -q
来源：http://uc.shtwfgs.cn

[U32] Py：代码格式化
来源：http://op.szsharing.cn

ruff format . && ruff check --fix .
来源：http://dj.chemitech.net.cn

[U33] Py：打包发布
来源：http://sy.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://nv.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://tr.yuexingan06.cn

chardet.detect(raw)
来源：http://bm.huixiangedu.cn

[U35] Py：发送邮件
来源：http://bg.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://um.wgjwhj.cn

[U36] Py：定时任务
来源：http://ib.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ca.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://oo.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tx.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://eu.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://vd.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://ay.wgjwhj.cn

sys.stdout.isatty()
来源：http://rw.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://av.hnjuh.cn

print("err", file=sys.stderr)
来源：http://zm.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://fq.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xw.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ce.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ru.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://jn.hnjuh.cn

namespace App\Http;
来源：http://hr.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://wn.huanxung.cn

declare(strict_types=1);
来源：http://xs.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://nm.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ny.nszjky.cn

[U46] PHP：可空类型
来源：http://bp.colortex.cn

?string $name = null
来源：http://pl.521024.cn

[U47] PHP：联合类型
来源：http://yv.colortex.cn

int|string $id
来源：http://az.lnxyls.cn

[U48] PHP：纯枚举
来源：http://xb.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lr.nicolike.cn

[U49] PHP：只读属性
来源：http://wk.shxzskj.cn

public readonly string $name
来源：http://ba.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://iy.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://ay.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://yc.jctech888.com.cn

[$a, $b] = $arr;
来源：http://dx.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://gh.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ed.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://yn.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://ek.colortex.cn

[U54] PHP：空安全调用
来源：http://dy.lnxyls.cn

$obj?->method()
来源：http://yd.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://sr.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hk.huanxung.cn

[U56] PHP：命名参数
来源：http://id.wgjwhj.cn

f(a: 1, b: 2)
来源：http://ze.hahajie.cn

[U57] PHP：字符串插值
来源：http://bs.jctech888.com.cn

"值: {$a}"
来源：http://iz.nicolike.cn

[U58] PHP：数组三件套
来源：http://id.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ti.hnjuh.cn

[U59] PHP：自定义排序
来源：http://lg.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mb.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://jj.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ug.haigaiapp.cn

[U61] PHP：正则
来源：http://zg.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hp.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://ut.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oz.nszjky.cn

[U63] PHP：文件读写
来源：http://ek.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oy.panjiajie.cn

[U64] PHP：目录遍历
来源：http://un.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://cu.hnjuh.cn

[U65] PHP：会话
来源：http://ac.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sy.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://kp.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://un.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://zu.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kb.521024.cn

[U68] PHP：PDO 连接
来源：http://rt.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ja.asd995.cn

[U69] PHP：PDO 预处理
来源：http://ye.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ed.newstarts.cn

[U70] PHP：PDO 事务
来源：http://hi.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tq.shxzskj.cn

[U71] PHP：抛出异常
来源：http://ns.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://tf.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://en.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://ww.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://us.521024.cn

parse_ini_file("config.ini", true)
来源：http://uv.521024.cn

[U74] PHP：读取环境变量
来源：http://wm.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://eo.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://wp.hahajie.cn

composer require psr/container
来源：http://wz.nicolike.cn

[U76] PHP：简单路由
来源：http://ey.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bk.newstarts.cn

[U77] PHP：模板渲染
来源：http://ud.jianghongdianzi.cn

composer require twig/twig
来源：http://ew.bjjhwx.cn

[U78] PHP：单元测试
来源：http://sw.521024.cn

composer require --dev phpunit/phpunit
来源：http://cw.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://vu.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://hy.szsharing.cn

[U80] PHP：代码规范修复
来源：http://ha.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ui.wgjwhj.cn

[U81] JS：初始化项目
来源：http://ks.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://cj.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://gh.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qv.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://nk.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vk.521024.cn

[U84] JS：CommonJS 写法
来源：http://ke.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://za.chemitech.net.cn

[U85] JS：可选链
来源：http://gs.hahajie.cn

a?.b?.c
来源：http://wh.huanxung.cn

[U86] JS：空值合并
来源：http://dz.szxytkj.cn

a ?? b
来源：http://ea.yuexingan06.cn

[U87] JS：解构默认值
来源：http://zh.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://fm.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://tf.shxzskj.cn

{ ...a, ...b }
来源：http://ir.nszjky.cn

[U89] JS：数组去重
来源：http://fl.jianghongdianzi.cn

[...new Set(arr)]
来源：http://pb.newstarts.cn

[U90] JS：数字数组排序
来源：http://fj.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://dg.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://fu.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gp.shxzskj.cn

[U92] JS：深拷贝
来源：http://oh.huixiangedu.cn

structuredClone(obj)
来源：http://dp.wgjwhj.cn

[U93] JS：模板字符串
来源：http://kv.colortex.cn

`共 ${n} 条`
来源：http://qy.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://xz.jianghongdianzi.cn

const double = x => x * 2;
来源：http://ya.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://at.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://uh.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://pi.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cz.9csxet.cn

[U97] JS：并发请求
来源：http://po.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nx.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://xj.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mg.hahajie.cn

[U99] JS：事件监听
来源：http://nv.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://cw.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://oi.yuexingan06.cn

document.querySelector(".item")
来源：http://xz.shxzukj.cn

[U101] JS：classList 操作
来源：http://ah.muxihuayi.cn

el.classList.toggle("active")
来源：http://ey.gzmigu.cn

[U102] JS：本地存储
来源：http://ac.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wi.shtwfgs.cn

[U103] JS：定时器
来源：http://yk.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uw.hahajie.cn

[U104] JS：防抖
来源：http://jf.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hv.jctech888.com.cn

[U105] JS：节流
来源：http://db.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yk.newstarts.cn

[U106] JS：日期格式化
来源：http://ae.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xs.szxytkj.cn

[U107] JS：数字千分位
来源：http://or.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pm.muxihuayi.cn

[U108] JS：随机整数
来源：http://dm.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mm.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://os.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://md.szsharing.cn

[U110] JS：数组分块
来源：http://ef.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lj.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://xl.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://vc.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://wa.haigaiapp.cn

"7".padStart(3, "0")
来源：http://wc.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://to.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://ok.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://vs.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jf.lnxyls.cn

[U115] JS：生成 UUID
来源：http://cf.asd995.cn

crypto.randomUUID()
来源：http://kd.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://gt.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://cs.muxihuayi.cn

[U117] JS：单元测试
来源：http://uq.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://wf.szxytkj.cn

[U118] JS：开发服务器
来源：http://ot.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://ua.jctech888.com.cn

[U119] JS：生产构建
来源：http://tl.shxzukj.cn

npx vite build
来源：http://dq.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://uf.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://vp.bookmarksfly.cn

================================================================================
来源：http://zv.jianghongdianzi.cn

统计汇总
来源：http://tt.muxihuayi.cn

================================================================================
来源：http://ff.huixinmuqiang.cn

按语言统计（条）：
来源：http://oq.shxzukj.cn

Python ......... 252
来源：http://fz.shxzukj.cn

PHP ............ 252
来源：http://op.521024.cn

JavaScript ..... 252
来源：http://aa.yuntaijiaju.cn

TypeScript ..... 212
来源：http://fo.shtwfgs.cn

Java ........... 212
来源：http://ik.huixiangedu.cn

Go ............. 212
来源：http://zf.shtwfgs.cn

Ruby ........... 212
来源：http://uv.nicolike.cn

C# ............. 212
来源：http://zf.shtwfgs.cn

C .............. 30
来源：http://lq.huanxung.cn

C++ ............ 30
来源：http://bp.hahajie.cn

SQL ............ 90
来源：http://qk.shxzukj.cn

Bash ........... 80
来源：http://hs.szsharing.cn

Kotlin ......... 15
来源：http://ix.bjjhwx.cn

Swift .......... 15
来源：http://gn.jctech888.com.cn

Lua ............ 10
来源：http://yc.chemitech.net.cn

Perl ........... 10
来源：http://nl.lnxyls.cn

Scala .......... 10
来源：http://pm.haigaiapp.cn

------------------------------------
来源：http://eu.nicolike.cn

合计 ........... 2106 条
来源：http://or.jctech888.com.cn

按章节统计：
来源：http://wf.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ed.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bz.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ih.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ly.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oz.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bb.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mc.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pe.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yp.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://an.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://po.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jw.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zk.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uq.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zc.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sc.hnjuh.cn

Q SQL 专题                              90
来源：http://vk.szsharing.cn

R Bash 专题                             80
来源：http://nj.shtwfgs.cn

S C / C++ 专题                          60
来源：http://gx.colortex.cn

T 其他语言补充                          60
来源：http://xd.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://wd.lnxyls.cn

------------------------------------
来源：http://df.szxytkj.cn

合计                                  2106 条
来源：http://dv.szsharing.cn

--------------------------------------------------------------------------------
来源：http://vs.shxzukj.cn

使用提醒
来源：http://ql.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://wy.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yc.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kz.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cx.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ei.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ca.521024.cn

—— 文件结束 ——
来源：http://op.huixinmuqiang.cn


<!-- 参考信息 -->