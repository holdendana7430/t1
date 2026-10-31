代发 wailian999

[U05] Py：列表去重且保序
来源：http://vs.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://ey.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://kx.hnjuh.cn

{**a, **b}
来源：http://ey.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://bh.nszjky.cn

{v: k for k, v in d.items()}
来源：http://as.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://ge.hnjuh.cn

[y for x in nested for y in x]
来源：http://ff.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://uy.shxzukj.cn

max(d, key=d.get)
来源：http://ok.lnxyls.cn

[U10] Py：按值排序字典
来源：http://uc.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bv.szsharing.cn

[U11] Py：生成器表达式
来源：http://wt.huixiangedu.cn

(x * 2 for x in arr)
来源：http://bj.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ip.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://dw.asd995.cn

[U13] Py：固定长度队列
来源：http://uq.yuexingan06.cn

deque(maxlen=10)
来源：http://mx.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://bv.asd995.cn

defaultdict(list)
来源：http://pe.hahajie.cn

[U15] Py：高精度计时
来源：http://mf.jianghongdianzi.cn

t = time.perf_counter()
来源：http://br.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://bo.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://es.shxzukj.cn

[U17] Py：初始化日志
来源：http://vk.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://ec.gzmigu.cn

[U18] Py：预编译正则
来源：http://lr.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://nw.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://zx.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qp.521024.cn

[U20] Py：缓存函数结果
来源：http://jt.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://rc.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ke.521024.cn

@contextlib.contextmanager
来源：http://mp.hahajie.cn

[U22] Py：矩阵转置
来源：http://zl.yuexingan06.cn

list(zip(*m))
来源：http://mf.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://rv.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tz.colortex.cn

[U24] Py：路径操作
来源：http://ph.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bi.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://zz.bjjhwx.cn

csv.DictReader(f)
来源：http://hn.asd995.cn

[U26] Py：并发下载
来源：http://hu.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hj.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://xn.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://zl.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://dh.shxzukj.cn

UserId = int
来源：http://dq.asd995.cn

[U29] Py：属性校验
来源：http://at.gzmigu.cn

@property 与 @x.setter 配合
来源：http://le.yuntaijiaju.cn

[U30] Py：数据类
来源：http://ik.shtwfgs.cn

@dataclass(slots=True)
来源：http://dc.yuntaijiaju.cn

[U31] Py：单测
来源：http://sx.jctech888.com.cn

python -m pytest -q
来源：http://zq.shtwfgs.cn

[U32] Py：代码格式化
来源：http://tr.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://gl.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://qw.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://xz.asd995.cn

[U34] Py：判断编码
来源：http://zx.shxzukj.cn

chardet.detect(raw)
来源：http://dh.newstarts.cn

[U35] Py：发送邮件
来源：http://jy.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vt.nszjky.cn

[U36] Py：定时任务
来源：http://by.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ve.szxytkj.cn

[U37] Py：读写 Excel
来源：http://xk.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sp.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://lk.panjiajie.cn

Path(__file__).resolve().parent
来源：http://dc.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://jc.huixiangedu.cn

sys.stdout.isatty()
来源：http://lk.nszjky.cn

[U40] Py：打印到标准错误
来源：http://fa.shxzukj.cn

print("err", file=sys.stderr)
来源：http://tp.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://av.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lg.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://hc.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://op.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://df.szsharing.cn

namespace App\Http;
来源：http://ts.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://tu.haigaiapp.cn

declare(strict_types=1);
来源：http://ku.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://yu.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vf.colortex.cn

[U46] PHP：可空类型
来源：http://cj.shxzukj.cn

?string $name = null
来源：http://wo.huanxung.cn

[U47] PHP：联合类型
来源：http://db.9csxet.cn

int|string $id
来源：http://qi.huanxung.cn

[U48] PHP：纯枚举
来源：http://dk.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zv.shxzukj.cn

[U49] PHP：只读属性
来源：http://nr.newstarts.cn

public readonly string $name
来源：http://du.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://zb.colortex.cn

public function __construct(private int $id) {}
来源：http://zt.9csxet.cn

[U51] PHP：数组解构
来源：http://qc.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ro.panjiajie.cn

[U52] PHP：箭头函数
来源：http://xd.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://yk.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://az.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://nv.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://no.muxihuayi.cn

$obj?->method()
来源：http://fy.gzmigu.cn

[U55] PHP：match 表达式
来源：http://fg.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ci.huixiangedu.cn

[U56] PHP：命名参数
来源：http://wi.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://sy.shxzskj.cn

[U57] PHP：字符串插值
来源：http://bs.bookmarksfly.cn

"值: {$a}"
来源：http://bz.szxytkj.cn

[U58] PHP：数组三件套
来源：http://gb.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fk.newstarts.cn

[U59] PHP：自定义排序
来源：http://zn.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dg.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://zk.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ub.bjjhwx.cn

[U61] PHP：正则
来源：http://he.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ct.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://kh.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mh.hnjuh.cn

[U63] PHP：文件读写
来源：http://vz.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nk.asd995.cn

[U64] PHP：目录遍历
来源：http://tw.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://sm.bookmarksfly.cn

[U65] PHP：会话
来源：http://mz.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vh.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://je.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://si.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://ld.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dg.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://zd.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tf.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://ph.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sq.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://st.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yh.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://rv.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://tq.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://wa.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://gj.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://qn.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://rq.hahajie.cn

[U74] PHP：读取环境变量
来源：http://ov.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://wt.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://cx.hnjuh.cn

composer require psr/container
来源：http://dr.lnxyls.cn

[U76] PHP：简单路由
来源：http://tt.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kk.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://fy.jctech888.com.cn

composer require twig/twig
来源：http://dj.lnxyls.cn

[U78] PHP：单元测试
来源：http://rr.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://cu.nicolike.cn

[U79] PHP：静态分析
来源：http://wb.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://mz.colortex.cn

[U80] PHP：代码规范修复
来源：http://ak.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hm.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://lg.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://sf.9csxet.cn

[U82] JS：package.json 脚本
来源：http://zf.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ma.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://mr.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aw.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://og.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zt.jctech888.com.cn

[U85] JS：可选链
来源：http://wq.huixiangedu.cn

a?.b?.c
来源：http://wt.newstarts.cn

[U86] JS：空值合并
来源：http://nx.bjjhwx.cn

a ?? b
来源：http://fi.szxytkj.cn

[U87] JS：解构默认值
来源：http://oh.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://rt.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://cd.hahajie.cn

{ ...a, ...b }
来源：http://ai.bookmarksfly.cn

[U89] JS：数组去重
来源：http://ma.bjjhwx.cn

[...new Set(arr)]
来源：http://cw.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://ta.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://ku.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://jr.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bg.shxzskj.cn

[U92] JS：深拷贝
来源：http://qi.9csxet.cn

structuredClone(obj)
来源：http://yi.muxihuayi.cn

[U93] JS：模板字符串
来源：http://fu.hnjuh.cn

`共 ${n} 条`
来源：http://mf.colortex.cn

[U94] JS：箭头函数
来源：http://yl.asd995.cn

const double = x => x * 2;
来源：http://ax.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://nb.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://gb.newstarts.cn

[U96] JS：async/await 与异常
来源：http://ig.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gw.panjiajie.cn

[U97] JS：并发请求
来源：http://jp.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xy.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://mw.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bh.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://da.hahajie.cn

el.addEventListener("click", e => {})
来源：http://ml.9csxet.cn

[U100] JS：DOM 查询
来源：http://ga.colortex.cn

document.querySelector(".item")
来源：http://gt.yuexingan06.cn

[U101] JS：classList 操作
来源：http://eh.521024.cn

el.classList.toggle("active")
来源：http://qe.521024.cn

[U102] JS：本地存储
来源：http://oe.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://em.szxytkj.cn

[U103] JS：定时器
来源：http://sl.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://es.bookmarksfly.cn

[U104] JS：防抖
来源：http://jk.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yw.jctech888.com.cn

[U105] JS：节流
来源：http://cp.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jr.huixiangedu.cn

[U106] JS：日期格式化
来源：http://kz.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dd.nszjky.cn

[U107] JS：数字千分位
来源：http://ko.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ji.shxzukj.cn

[U108] JS：随机整数
来源：http://ow.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gh.shxzukj.cn

[U109] JS：数组分组
来源：http://sm.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://nr.chemitech.net.cn

[U110] JS：数组分块
来源：http://ox.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://se.nszjky.cn

[U111] JS：对象转 Map
来源：http://ap.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://xs.asd995.cn

[U112] JS：字符串补位
来源：http://tv.asd995.cn

"7".padStart(3, "0")
来源：http://sd.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://kc.szsharing.cn

s.replaceAll("a", "b")
来源：http://wc.nszjky.cn

[U114] JS：JSON 深比较
来源：http://lg.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bf.asd995.cn

[U115] JS：生成 UUID
来源：http://tw.yuexingan06.cn

crypto.randomUUID()
来源：http://nu.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://dg.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://dx.haigaiapp.cn

[U117] JS：单元测试
来源：http://vy.521024.cn

npm i -D vitest;  npx vitest
来源：http://iq.panjiajie.cn

[U118] JS：开发服务器
来源：http://yv.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://rv.bookmarksfly.cn

[U119] JS：生产构建
来源：http://av.lnxyls.cn

npx vite build
来源：http://dm.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://qg.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://ct.chemitech.net.cn

================================================================================
来源：http://mf.jctech888.com.cn

统计汇总
来源：http://lv.nszjky.cn

================================================================================
来源：http://ca.yuexingan06.cn

按语言统计（条）：
来源：http://dn.haigaiapp.cn

Python ......... 252
来源：http://mn.wgjwhj.cn

PHP ............ 252
来源：http://ab.shxzskj.cn

JavaScript ..... 252
来源：http://xb.szxytkj.cn

TypeScript ..... 212
来源：http://zl.huixinmuqiang.cn

Java ........... 212
来源：http://er.jianghongdianzi.cn

Go ............. 212
来源：http://el.huixinmuqiang.cn

Ruby ........... 212
来源：http://xv.9csxet.cn

C# ............. 212
来源：http://zy.lnxyls.cn

C .............. 30
来源：http://dw.521024.cn

C++ ............ 30
来源：http://yr.521024.cn

SQL ............ 90
来源：http://rs.hnjuh.cn

Bash ........... 80
来源：http://xk.hnjuh.cn

Kotlin ......... 15
来源：http://gg.yuntaijiaju.cn

Swift .......... 15
来源：http://fj.9csxet.cn

Lua ............ 10
来源：http://ne.szxytkj.cn

Perl ........... 10
来源：http://ue.huanxung.cn

Scala .......... 10
来源：http://qo.jctech888.com.cn

------------------------------------
来源：http://uf.nszjky.cn

合计 ........... 2106 条
来源：http://rs.colortex.cn

按章节统计：
来源：http://ii.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tt.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hf.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rk.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sf.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://on.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zj.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fr.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fg.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gw.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xy.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wd.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bq.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ml.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yk.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hp.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://px.9csxet.cn

Q SQL 专题                              90
来源：http://ey.bookmarksfly.cn

R Bash 专题                             80
来源：http://qk.muxihuayi.cn

S C / C++ 专题                          60
来源：http://nh.shxzskj.cn

T 其他语言补充                          60
来源：http://lp.9csxet.cn

U 高频实用片段                         120
来源：http://rm.bjjhwx.cn

------------------------------------
来源：http://lc.nicolike.cn

合计                                  2106 条
来源：http://vi.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://at.panjiajie.cn

使用提醒
来源：http://vw.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://cp.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hu.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dm.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xf.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xu.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cw.asd995.cn

—— 文件结束 ——
来源：http://vv.haigaiapp.cn

================================================================================
来源：http://oa.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://br.521024.cn

Common Programming Examples Cheat Book
来源：http://zj.szxytkj.cn

================================================================================
来源：http://bu.nicolike.cn

【收录内容】
来源：http://ns.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gr.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wj.hnjuh.cn

SQL · Bash · C · C++
来源：http://lu.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mf.newstarts.cn

【使用说明】
来源：http://hd.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yg.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jf.szxytkj.cn


<!-- 参考信息 -->