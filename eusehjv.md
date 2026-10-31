代发 wailian999

[U03] Py：加载 .env 配置
来源：http://kw.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gt.gzmigu.cn

[U04] Py：变量调试打印
来源：http://fd.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fw.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://gm.hahajie.cn

list(dict.fromkeys(arr))
来源：http://sn.colortex.cn

[U06] Py：合并两个字典
来源：http://cm.muxihuayi.cn

{**a, **b}
来源：http://rc.szxytkj.cn

[U07] Py：反转字典键值
来源：http://xw.521024.cn

{v: k for k, v in d.items()}
来源：http://dj.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://my.hnjuh.cn

[y for x in nested for y in x]
来源：http://me.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://px.shtwfgs.cn

max(d, key=d.get)
来源：http://ak.shxzukj.cn

[U10] Py：按值排序字典
来源：http://yf.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zd.szsharing.cn

[U11] Py：生成器表达式
来源：http://mg.nszjky.cn

(x * 2 for x in arr)
来源：http://kf.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aw.panjiajie.cn

Counter(arr).most_common(3)
来源：http://iy.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://es.muxihuayi.cn

deque(maxlen=10)
来源：http://jf.nicolike.cn

[U14] Py：分组收集到列表
来源：http://co.colortex.cn

defaultdict(list)
来源：http://qh.hahajie.cn

[U15] Py：高精度计时
来源：http://yu.nicolike.cn

t = time.perf_counter()
来源：http://cy.9csxet.cn

[U16] Py：命令行参数解析
来源：http://pp.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qz.lnxyls.cn

[U17] Py：初始化日志
来源：http://uf.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://sr.shtwfgs.cn

[U18] Py：预编译正则
来源：http://of.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://su.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://rr.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xa.nicolike.cn

[U20] Py：缓存函数结果
来源：http://of.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://yh.521024.cn

[U21] Py：自定义上下文管理器
来源：http://bj.nicolike.cn

@contextlib.contextmanager
来源：http://ge.szxytkj.cn

[U22] Py：矩阵转置
来源：http://qo.hahajie.cn

list(zip(*m))
来源：http://hq.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://he.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ni.shxzskj.cn

[U24] Py：路径操作
来源：http://wn.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ve.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://xn.muxihuayi.cn

csv.DictReader(f)
来源：http://wj.jctech888.com.cn

[U26] Py：并发下载
来源：http://sv.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sx.huanxung.cn

[U27] Py：异步 HTTP
来源：http://du.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://aq.asd995.cn

[U28] Py：类型别名
来源：http://zp.nszjky.cn

UserId = int
来源：http://vf.hahajie.cn

[U29] Py：属性校验
来源：http://on.huanxung.cn

@property 与 @x.setter 配合
来源：http://dp.chemitech.net.cn

[U30] Py：数据类
来源：http://eo.nicolike.cn

@dataclass(slots=True)
来源：http://nr.bookmarksfly.cn

[U31] Py：单测
来源：http://lz.yuexingan06.cn

python -m pytest -q
来源：http://cf.colortex.cn

[U32] Py：代码格式化
来源：http://uo.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://lo.lnxyls.cn

[U33] Py：打包发布
来源：http://vp.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://cz.9csxet.cn

[U34] Py：判断编码
来源：http://mk.lnxyls.cn

chardet.detect(raw)
来源：http://ow.shxzukj.cn

[U35] Py：发送邮件
来源：http://pn.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sr.yuexingan06.cn

[U36] Py：定时任务
来源：http://mv.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://ft.hahajie.cn

[U37] Py：读写 Excel
来源：http://fs.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fc.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://hv.9csxet.cn

Path(__file__).resolve().parent
来源：http://ws.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://by.nszjky.cn

sys.stdout.isatty()
来源：http://xn.521024.cn

[U40] Py：打印到标准错误
来源：http://ho.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://sr.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://ah.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ys.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://bd.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vz.nicolike.cn

[U43] PHP：声明命名空间
来源：http://uy.szxytkj.cn

namespace App\Http;
来源：http://yy.nszjky.cn

[U44] PHP：开启严格类型
来源：http://qe.jianghongdianzi.cn

declare(strict_types=1);
来源：http://eo.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ms.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sm.hnjuh.cn

[U46] PHP：可空类型
来源：http://ii.521024.cn

?string $name = null
来源：http://jc.colortex.cn

[U47] PHP：联合类型
来源：http://oc.szsharing.cn

int|string $id
来源：http://px.hnjuh.cn

[U48] PHP：纯枚举
来源：http://up.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ze.szxytkj.cn

[U49] PHP：只读属性
来源：http://sx.wgjwhj.cn

public readonly string $name
来源：http://hm.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://jr.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://qr.asd995.cn

[U51] PHP：数组解构
来源：http://no.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://hc.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://xp.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://tj.asd995.cn

[U53] PHP：空合并运算符
来源：http://ks.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://fa.newstarts.cn

[U54] PHP：空安全调用
来源：http://ld.shxzukj.cn

$obj?->method()
来源：http://fe.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://vs.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ug.colortex.cn

[U56] PHP：命名参数
来源：http://wq.panjiajie.cn

f(a: 1, b: 2)
来源：http://de.hnjuh.cn

[U57] PHP：字符串插值
来源：http://qg.wgjwhj.cn

"值: {$a}"
来源：http://jd.hnjuh.cn

[U58] PHP：数组三件套
来源：http://pf.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://on.newstarts.cn

[U59] PHP：自定义排序
来源：http://hx.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mh.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://jx.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ya.wgjwhj.cn

[U61] PHP：正则
来源：http://bm.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://si.9csxet.cn

[U62] PHP：日期对象
来源：http://gk.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nj.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://ok.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fm.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://mg.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://xi.lnxyls.cn

[U65] PHP：会话
来源：http://dn.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kx.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://gn.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dn.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://vz.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hh.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://pj.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yr.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://yz.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rk.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ew.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nb.hahajie.cn

[U71] PHP：抛出异常
来源：http://fh.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://pi.panjiajie.cn

[U72] PHP：写错误日志
来源：http://mf.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ws.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://rg.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://jh.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://ev.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://ks.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://jp.yuntaijiaju.cn

composer require psr/container
来源：http://lw.shxzukj.cn

[U76] PHP：简单路由
来源：http://dl.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ky.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://rw.asd995.cn

composer require twig/twig
来源：http://os.shxzskj.cn

[U78] PHP：单元测试
来源：http://qh.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://vx.szsharing.cn

[U79] PHP：静态分析
来源：http://zn.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://ji.colortex.cn

[U80] PHP：代码规范修复
来源：http://ao.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ua.hahajie.cn

[U81] JS：初始化项目
来源：http://wc.wgjwhj.cn

npm init -y;  npm i express
来源：http://ga.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://dx.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qw.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://pi.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yw.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://ij.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rl.haigaiapp.cn

[U85] JS：可选链
来源：http://ps.huixiangedu.cn

a?.b?.c
来源：http://ro.haigaiapp.cn

[U86] JS：空值合并
来源：http://cm.wgjwhj.cn

a ?? b
来源：http://bp.hnjuh.cn

[U87] JS：解构默认值
来源：http://ue.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://zg.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://zl.hahajie.cn

{ ...a, ...b }
来源：http://yf.panjiajie.cn

[U89] JS：数组去重
来源：http://jb.szsharing.cn

[...new Set(arr)]
来源：http://rq.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://xd.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://ij.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://hj.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ii.szsharing.cn

[U92] JS：深拷贝
来源：http://do.yuntaijiaju.cn

structuredClone(obj)
来源：http://pi.haigaiapp.cn

[U93] JS：模板字符串
来源：http://fz.lnxyls.cn

`共 ${n} 条`
来源：http://mg.hnjuh.cn

[U94] JS：箭头函数
来源：http://pd.huixiangedu.cn

const double = x => x * 2;
来源：http://ie.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://qv.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://bd.nicolike.cn

[U96] JS：async/await 与异常
来源：http://ou.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cz.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://cn.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vm.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://kz.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nb.lnxyls.cn

[U99] JS：事件监听
来源：http://su.huanxung.cn

el.addEventListener("click", e => {})
来源：http://at.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://cm.chemitech.net.cn

document.querySelector(".item")
来源：http://an.shxzskj.cn

[U101] JS：classList 操作
来源：http://nd.asd995.cn

el.classList.toggle("active")
来源：http://ex.panjiajie.cn

[U102] JS：本地存储
来源：http://hb.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rt.huanxung.cn

[U103] JS：定时器
来源：http://go.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kz.newstarts.cn

[U104] JS：防抖
来源：http://mi.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pv.szxytkj.cn

[U105] JS：节流
来源：http://pz.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jb.521024.cn

[U106] JS：日期格式化
来源：http://oh.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gw.huanxung.cn

[U107] JS：数字千分位
来源：http://uh.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xm.gzmigu.cn

[U108] JS：随机整数
来源：http://mw.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qt.shtwfgs.cn

[U109] JS：数组分组
来源：http://ti.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://tc.huixiangedu.cn

[U110] JS：数组分块
来源：http://xn.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://st.colortex.cn

[U111] JS：对象转 Map
来源：http://zm.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://qr.jctech888.com.cn

[U112] JS：字符串补位
来源：http://sy.szxytkj.cn

"7".padStart(3, "0")
来源：http://ru.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://wy.lnxyls.cn

s.replaceAll("a", "b")
来源：http://jc.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://ye.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vy.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://cz.yuntaijiaju.cn

crypto.randomUUID()
来源：http://km.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://oa.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://du.nszjky.cn

[U117] JS：单元测试
来源：http://xh.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://jl.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://cg.huanxung.cn

npm i -D vite;  npx vite
来源：http://nf.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://rf.szsharing.cn

npx vite build
来源：http://vp.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://ap.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://pe.shxzskj.cn

================================================================================
来源：http://hn.huixiangedu.cn

统计汇总
来源：http://nv.haigaiapp.cn

================================================================================
来源：http://oy.szsharing.cn

按语言统计（条）：
来源：http://dz.jianghongdianzi.cn

Python ......... 252
来源：http://gx.hahajie.cn

PHP ............ 252
来源：http://oy.shxzukj.cn

JavaScript ..... 252
来源：http://pt.shtwfgs.cn

TypeScript ..... 212
来源：http://hx.nszjky.cn

Java ........... 212
来源：http://yu.yuexingan06.cn

Go ............. 212
来源：http://pv.521024.cn

Ruby ........... 212
来源：http://we.wgjwhj.cn

C# ............. 212
来源：http://nf.yuntaijiaju.cn

C .............. 30
来源：http://la.panjiajie.cn

C++ ............ 30
来源：http://tm.huixiangedu.cn

SQL ............ 90
来源：http://so.bookmarksfly.cn

Bash ........... 80
来源：http://ao.yuexingan06.cn

Kotlin ......... 15
来源：http://vi.huanxung.cn

Swift .......... 15
来源：http://af.shtwfgs.cn

Lua ............ 10
来源：http://il.9csxet.cn

Perl ........... 10
来源：http://yy.huixinmuqiang.cn

Scala .......... 10
来源：http://tq.huanxung.cn

------------------------------------
来源：http://xu.jctech888.com.cn

合计 ........... 2106 条
来源：http://dw.colortex.cn

按章节统计：
来源：http://qr.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://la.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ev.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jb.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mr.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eu.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://at.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ta.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ru.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://us.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ix.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tg.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ad.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sp.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bp.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zi.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wx.521024.cn

Q SQL 专题                              90
来源：http://jz.jianghongdianzi.cn

R Bash 专题                             80
来源：http://xh.jctech888.com.cn

S C / C++ 专题                          60
来源：http://es.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://vv.haigaiapp.cn

U 高频实用片段                         120
来源：http://nj.521024.cn

------------------------------------
来源：http://qp.bjjhwx.cn

合计                                  2106 条
来源：http://zz.asd995.cn

--------------------------------------------------------------------------------
来源：http://ch.wgjwhj.cn

使用提醒
来源：http://lk.colortex.cn

--------------------------------------------------------------------------------
来源：http://nd.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tu.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ax.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://po.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://do.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zl.huixiangedu.cn

—— 文件结束 ——
来源：http://wh.shxzskj.cn

================================================================================
来源：http://pt.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ea.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://ca.bjjhwx.cn

================================================================================
来源：http://wo.lnxyls.cn

【收录内容】
来源：http://xv.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ku.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xk.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://xo.jctech888.com.cn


<!-- 参考信息 -->