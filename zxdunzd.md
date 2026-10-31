代发 wailian999

[U07] Py：反转字典键值
来源：http://pg.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://lj.asd995.cn

[U08] Py：展平二维列表
来源：http://hc.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://lz.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ki.yuntaijiaju.cn

max(d, key=d.get)
来源：http://hk.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://oa.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ld.szsharing.cn

[U11] Py：生成器表达式
来源：http://tr.nicolike.cn

(x * 2 for x in arr)
来源：http://tl.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cr.nszjky.cn

Counter(arr).most_common(3)
来源：http://fd.asd995.cn

[U13] Py：固定长度队列
来源：http://vq.chemitech.net.cn

deque(maxlen=10)
来源：http://ym.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://xm.muxihuayi.cn

defaultdict(list)
来源：http://vh.shxzukj.cn

[U15] Py：高精度计时
来源：http://in.nicolike.cn

t = time.perf_counter()
来源：http://ul.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://ol.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gv.yuexingan06.cn

[U17] Py：初始化日志
来源：http://bv.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://aj.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://au.colortex.cn

pat = re.compile(r"\d+")
来源：http://zx.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://gu.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jx.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://tz.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://av.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://cs.panjiajie.cn

@contextlib.contextmanager
来源：http://rw.shxzskj.cn

[U22] Py：矩阵转置
来源：http://oj.muxihuayi.cn

list(zip(*m))
来源：http://ey.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://xg.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hn.hnjuh.cn

[U24] Py：路径操作
来源：http://hf.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ja.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://pv.colortex.cn

csv.DictReader(f)
来源：http://sd.9csxet.cn

[U26] Py：并发下载
来源：http://kz.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gu.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://fy.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://iu.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://hw.nszjky.cn

UserId = int
来源：http://yd.chemitech.net.cn

[U29] Py：属性校验
来源：http://be.asd995.cn

@property 与 @x.setter 配合
来源：http://ca.panjiajie.cn

[U30] Py：数据类
来源：http://wh.jctech888.com.cn

@dataclass(slots=True)
来源：http://po.yuntaijiaju.cn

[U31] Py：单测
来源：http://as.chemitech.net.cn

python -m pytest -q
来源：http://le.colortex.cn

[U32] Py：代码格式化
来源：http://bx.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://we.gzmigu.cn

[U33] Py：打包发布
来源：http://gu.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://zf.jctech888.com.cn

[U34] Py：判断编码
来源：http://wp.gzmigu.cn

chardet.detect(raw)
来源：http://mu.szxytkj.cn

[U35] Py：发送邮件
来源：http://dd.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dd.haigaiapp.cn

[U36] Py：定时任务
来源：http://sr.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://gt.newstarts.cn

[U37] Py：读写 Excel
来源：http://ve.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zx.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://ri.colortex.cn

Path(__file__).resolve().parent
来源：http://uq.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://jd.shxzukj.cn

sys.stdout.isatty()
来源：http://hv.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://la.szxytkj.cn

print("err", file=sys.stderr)
来源：http://wb.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ev.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vh.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://je.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tw.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://ig.lnxyls.cn

namespace App\Http;
来源：http://fe.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://mt.jianghongdianzi.cn

declare(strict_types=1);
来源：http://np.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://xh.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jn.huixiangedu.cn

[U46] PHP：可空类型
来源：http://la.hahajie.cn

?string $name = null
来源：http://ye.shxzukj.cn

[U47] PHP：联合类型
来源：http://fe.colortex.cn

int|string $id
来源：http://ld.nszjky.cn

[U48] PHP：纯枚举
来源：http://bu.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.szsharing.cn

[U49] PHP：只读属性
来源：http://jj.lnxyls.cn

public readonly string $name
来源：http://kc.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://rq.panjiajie.cn

public function __construct(private int $id) {}
来源：http://pq.521024.cn

[U51] PHP：数组解构
来源：http://vn.huanxung.cn

[$a, $b] = $arr;
来源：http://hj.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://mn.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://xe.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://gq.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://pg.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://ui.muxihuayi.cn

$obj?->method()
来源：http://yr.gzmigu.cn

[U55] PHP：match 表达式
来源：http://jo.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bn.yuexingan06.cn

[U56] PHP：命名参数
来源：http://sl.chemitech.net.cn

f(a: 1, b: 2)
来源：http://zw.colortex.cn

[U57] PHP：字符串插值
来源：http://nd.yuexingan06.cn

"值: {$a}"
来源：http://xc.shxzskj.cn

[U58] PHP：数组三件套
来源：http://hn.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ye.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://gj.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xk.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://df.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kq.jctech888.com.cn

[U61] PHP：正则
来源：http://vi.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://te.lnxyls.cn

[U62] PHP：日期对象
来源：http://bm.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://em.hahajie.cn

[U63] PHP：文件读写
来源：http://ec.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qh.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://kp.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://hc.nszjky.cn

[U65] PHP：会话
来源：http://ms.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yc.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://ye.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ct.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://ms.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bl.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://tw.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://av.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://oa.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.9csxet.cn

[U70] PHP：PDO 事务
来源：http://cw.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ju.hahajie.cn

[U71] PHP：抛出异常
来源：http://bg.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://fj.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://ub.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://oq.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://rv.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://mv.szsharing.cn

[U74] PHP：读取环境变量
来源：http://ha.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://cy.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://py.chemitech.net.cn

composer require psr/container
来源：http://cd.jctech888.com.cn

[U76] PHP：简单路由
来源：http://pd.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ou.shxzukj.cn

[U77] PHP：模板渲染
来源：http://hf.521024.cn

composer require twig/twig
来源：http://cg.haigaiapp.cn

[U78] PHP：单元测试
来源：http://kw.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://ik.szsharing.cn

[U79] PHP：静态分析
来源：http://pr.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://up.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://tr.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tn.lnxyls.cn

[U81] JS：初始化项目
来源：http://xa.hahajie.cn

npm init -y;  npm i express
来源：http://an.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://fj.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vj.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://kl.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iz.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://ej.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vo.colortex.cn

[U85] JS：可选链
来源：http://sw.shxzskj.cn

a?.b?.c
来源：http://qq.wgjwhj.cn

[U86] JS：空值合并
来源：http://mw.colortex.cn

a ?? b
来源：http://xs.jctech888.com.cn

[U87] JS：解构默认值
来源：http://zj.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://bm.nszjky.cn

[U88] JS：对象展开合并
来源：http://et.lnxyls.cn

{ ...a, ...b }
来源：http://vv.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://mu.9csxet.cn

[...new Set(arr)]
来源：http://fy.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://xf.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://wq.huanxung.cn

[U91] JS：对象键值遍历
来源：http://cb.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hx.shxzukj.cn

[U92] JS：深拷贝
来源：http://cw.nicolike.cn

structuredClone(obj)
来源：http://ba.shxzskj.cn

[U93] JS：模板字符串
来源：http://xn.yuntaijiaju.cn

`共 ${n} 条`
来源：http://cj.szxytkj.cn

[U94] JS：箭头函数
来源：http://og.huixinmuqiang.cn

const double = x => x * 2;
来源：http://fg.szsharing.cn

[U95] JS：Promise 包装
来源：http://od.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://bu.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://gu.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lu.9csxet.cn

[U97] JS：并发请求
来源：http://vv.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ht.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://sx.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lj.hahajie.cn

[U99] JS：事件监听
来源：http://au.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://ia.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://mg.521024.cn

document.querySelector(".item")
来源：http://jz.shxzukj.cn

[U101] JS：classList 操作
来源：http://ny.yuexingan06.cn

el.classList.toggle("active")
来源：http://so.shxzukj.cn

[U102] JS：本地存储
来源：http://bc.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ee.yuntaijiaju.cn

[U103] JS：定时器
来源：http://jq.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wi.huixiangedu.cn

[U104] JS：防抖
来源：http://ym.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://da.huanxung.cn

[U105] JS：节流
来源：http://yr.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ia.hnjuh.cn

[U106] JS：日期格式化
来源：http://it.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jt.shxzukj.cn

[U107] JS：数字千分位
来源：http://he.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xk.521024.cn

[U108] JS：随机整数
来源：http://ni.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ve.hnjuh.cn

[U109] JS：数组分组
来源：http://kg.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://xb.shtwfgs.cn

[U110] JS：数组分块
来源：http://gh.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yr.szxytkj.cn

[U111] JS：对象转 Map
来源：http://ip.colortex.cn

new Map(Object.entries(obj))
来源：http://zq.chemitech.net.cn

[U112] JS：字符串补位
来源：http://ya.muxihuayi.cn

"7".padStart(3, "0")
来源：http://yq.9csxet.cn

[U113] JS：正则替换全部
来源：http://uy.huanxung.cn

s.replaceAll("a", "b")
来源：http://ij.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://ay.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nn.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://ym.gzmigu.cn

crypto.randomUUID()
来源：http://yd.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://ty.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://zn.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://gg.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://ea.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://am.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://aw.colortex.cn

[U119] JS：生产构建
来源：http://jj.panjiajie.cn

npx vite build
来源：http://ra.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://zu.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://vk.muxihuayi.cn

================================================================================
来源：http://tw.newstarts.cn

统计汇总
来源：http://ma.lnxyls.cn

================================================================================
来源：http://ug.yuexingan06.cn

按语言统计（条）：
来源：http://wl.jianghongdianzi.cn

Python ......... 252
来源：http://ic.shtwfgs.cn

PHP ............ 252
来源：http://vq.huanxung.cn

JavaScript ..... 252
来源：http://oy.jianghongdianzi.cn

TypeScript ..... 212
来源：http://hm.asd995.cn

Java ........... 212
来源：http://ew.haigaiapp.cn

Go ............. 212
来源：http://xi.yuexingan06.cn

Ruby ........... 212
来源：http://xq.521024.cn

C# ............. 212
来源：http://lb.shxzskj.cn

C .............. 30
来源：http://wc.521024.cn

C++ ............ 30
来源：http://kj.nszjky.cn

SQL ............ 90
来源：http://oz.panjiajie.cn

Bash ........... 80
来源：http://ua.9csxet.cn

Kotlin ......... 15
来源：http://gq.chemitech.net.cn

Swift .......... 15
来源：http://si.newstarts.cn

Lua ............ 10
来源：http://kg.haigaiapp.cn

Perl ........... 10
来源：http://we.nszjky.cn

Scala .......... 10
来源：http://ky.newstarts.cn

------------------------------------
来源：http://vw.szsharing.cn

合计 ........... 2106 条
来源：http://wa.yuntaijiaju.cn

按章节统计：
来源：http://ad.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lc.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ly.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zd.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oi.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jt.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ww.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ju.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zb.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wf.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sk.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ub.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uw.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ue.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fl.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jq.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://du.lnxyls.cn

Q SQL 专题                              90
来源：http://uk.asd995.cn

R Bash 专题                             80
来源：http://et.wgjwhj.cn

S C / C++ 专题                          60
来源：http://co.9csxet.cn

T 其他语言补充                          60
来源：http://kt.huanxung.cn

U 高频实用片段                         120
来源：http://vk.huixinmuqiang.cn

------------------------------------
来源：http://fx.9csxet.cn

合计                                  2106 条
来源：http://bs.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://um.yuntaijiaju.cn

使用提醒
来源：http://rd.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://cm.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fb.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tj.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ff.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ps.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hj.gzmigu.cn

—— 文件结束 ——
来源：http://xe.szsharing.cn

================================================================================
来源：http://bi.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://gk.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://gl.hahajie.cn

================================================================================
来源：http://wk.szsharing.cn

【收录内容】
来源：http://wz.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sh.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qf.colortex.cn

SQL · Bash · C · C++
来源：http://po.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ck.hahajie.cn

【使用说明】
来源：http://ns.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://db.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nw.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://at.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qz.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fa.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zd.chemitech.net.cn


<!-- 参考信息 -->