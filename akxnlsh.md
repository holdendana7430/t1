代发 wailian999

[U05] Py：列表去重且保序
来源：http://mb.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://ff.lnxyls.cn

[U06] Py：合并两个字典
来源：http://qp.muxihuayi.cn

{**a, **b}
来源：http://fs.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://lm.nicolike.cn

{v: k for k, v in d.items()}
来源：http://tg.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://mn.colortex.cn

[y for x in nested for y in x]
来源：http://ey.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://ab.colortex.cn

max(d, key=d.get)
来源：http://vj.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://wu.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ij.huanxung.cn

[U11] Py：生成器表达式
来源：http://hu.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://bc.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mm.shxzskj.cn

Counter(arr).most_common(3)
来源：http://dc.newstarts.cn

[U13] Py：固定长度队列
来源：http://pl.asd995.cn

deque(maxlen=10)
来源：http://ba.asd995.cn

[U14] Py：分组收集到列表
来源：http://su.shtwfgs.cn

defaultdict(list)
来源：http://xb.521024.cn

[U15] Py：高精度计时
来源：http://ls.yuntaijiaju.cn

t = time.perf_counter()
来源：http://bb.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://qp.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ly.521024.cn

[U17] Py：初始化日志
来源：http://wv.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://uo.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://jp.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://tb.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://td.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kd.colortex.cn

[U20] Py：缓存函数结果
来源：http://yx.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://sd.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://xl.huanxung.cn

@contextlib.contextmanager
来源：http://le.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://qs.huixinmuqiang.cn

list(zip(*m))
来源：http://jl.newstarts.cn

[U23] Py：分块读取大文件
来源：http://hb.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aw.panjiajie.cn

[U24] Py：路径操作
来源：http://dl.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qg.colortex.cn

[U25] Py：CSV 按字典读
来源：http://lg.szsharing.cn

csv.DictReader(f)
来源：http://vv.hahajie.cn

[U26] Py：并发下载
来源：http://vp.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ru.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://jn.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://es.bjjhwx.cn

[U28] Py：类型别名
来源：http://uz.jianghongdianzi.cn

UserId = int
来源：http://ab.newstarts.cn

[U29] Py：属性校验
来源：http://mg.nszjky.cn

@property 与 @x.setter 配合
来源：http://ct.gzmigu.cn

[U30] Py：数据类
来源：http://lk.jctech888.com.cn

@dataclass(slots=True)
来源：http://gl.jianghongdianzi.cn

[U31] Py：单测
来源：http://to.shxzskj.cn

python -m pytest -q
来源：http://zd.szxytkj.cn

[U32] Py：代码格式化
来源：http://co.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://zu.hnjuh.cn

[U33] Py：打包发布
来源：http://bg.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://mi.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://st.huanxung.cn

chardet.detect(raw)
来源：http://ch.huanxung.cn

[U35] Py：发送邮件
来源：http://qk.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eh.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://vz.521024.cn

schedule.every(10).minutes.do(job)
来源：http://ob.nszjky.cn

[U37] Py：读写 Excel
来源：http://rx.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kb.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://le.nszjky.cn

Path(__file__).resolve().parent
来源：http://ed.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://vg.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://fh.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://zg.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://bd.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://ml.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zb.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://cs.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uh.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://ur.colortex.cn

namespace App\Http;
来源：http://wu.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://ni.9csxet.cn

declare(strict_types=1);
来源：http://eu.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://zd.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cd.wgjwhj.cn

[U46] PHP：可空类型
来源：http://ku.szxytkj.cn

?string $name = null
来源：http://sv.nicolike.cn

[U47] PHP：联合类型
来源：http://mt.newstarts.cn

int|string $id
来源：http://hc.nszjky.cn

[U48] PHP：纯枚举
来源：http://vr.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pe.colortex.cn

[U49] PHP：只读属性
来源：http://kj.szxytkj.cn

public readonly string $name
来源：http://nn.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://nr.hnjuh.cn

public function __construct(private int $id) {}
来源：http://jn.chemitech.net.cn

[U51] PHP：数组解构
来源：http://jp.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ih.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://st.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://er.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://zl.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://rb.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://sa.nszjky.cn

$obj?->method()
来源：http://vl.shxzukj.cn

[U55] PHP：match 表达式
来源：http://am.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zm.huixiangedu.cn

[U56] PHP：命名参数
来源：http://vr.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://do.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://np.muxihuayi.cn

"值: {$a}"
来源：http://wm.nszjky.cn

[U58] PHP：数组三件套
来源：http://ls.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zg.shxzskj.cn

[U59] PHP：自定义排序
来源：http://bw.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://es.521024.cn

[U60] PHP：JSON 编解码
来源：http://dy.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kj.yuexingan06.cn

[U61] PHP：正则
来源：http://xh.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kw.bjjhwx.cn

[U62] PHP：日期对象
来源：http://fa.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rr.521024.cn

[U63] PHP：文件读写
来源：http://rb.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kz.lnxyls.cn

[U64] PHP：目录遍历
来源：http://jy.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://eb.shxzukj.cn

[U65] PHP：会话
来源：http://wq.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yt.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://lk.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://td.521024.cn

[U67] PHP：处理文件上传
来源：http://bi.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ja.szsharing.cn

[U68] PHP：PDO 连接
来源：http://bn.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wm.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://rh.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://is.nszjky.cn

[U70] PHP：PDO 事务
来源：http://sb.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://as.nszjky.cn

[U71] PHP：抛出异常
来源：http://ob.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://zw.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://lc.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://rr.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://yj.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://zl.colortex.cn

[U74] PHP：读取环境变量
来源：http://fz.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://zs.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://oq.jianghongdianzi.cn

composer require psr/container
来源：http://cc.asd995.cn

[U76] PHP：简单路由
来源：http://sy.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ue.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://fw.huixinmuqiang.cn

composer require twig/twig
来源：http://bt.szsharing.cn

[U78] PHP：单元测试
来源：http://cq.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://xd.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://se.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ny.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://wj.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cb.panjiajie.cn

[U81] JS：初始化项目
来源：http://oj.shtwfgs.cn

npm init -y;  npm i express
来源：http://yl.nszjky.cn

[U82] JS：package.json 脚本
来源：http://zw.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hu.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://qk.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ao.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://zk.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tv.szxytkj.cn

[U85] JS：可选链
来源：http://mm.haigaiapp.cn

a?.b?.c
来源：http://el.nicolike.cn

[U86] JS：空值合并
来源：http://ho.shxzskj.cn

a ?? b
来源：http://pg.shxzukj.cn

[U87] JS：解构默认值
来源：http://bf.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://ze.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://la.jianghongdianzi.cn

{ ...a, ...b }
来源：http://na.panjiajie.cn

[U89] JS：数组去重
来源：http://cr.bjjhwx.cn

[...new Set(arr)]
来源：http://lw.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://gg.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://ws.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://to.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oa.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://nm.bookmarksfly.cn

structuredClone(obj)
来源：http://dr.huixiangedu.cn

[U93] JS：模板字符串
来源：http://jw.szsharing.cn

`共 ${n} 条`
来源：http://lb.huanxung.cn

[U94] JS：箭头函数
来源：http://zk.9csxet.cn

const double = x => x * 2;
来源：http://js.colortex.cn

[U95] JS：Promise 包装
来源：http://nw.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://jh.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://fa.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://im.hnjuh.cn

[U97] JS：并发请求
来源：http://yf.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ur.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://rv.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gs.jctech888.com.cn

[U99] JS：事件监听
来源：http://jg.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://vl.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://et.nicolike.cn

document.querySelector(".item")
来源：http://zd.lnxyls.cn

[U101] JS：classList 操作
来源：http://if.shxzskj.cn

el.classList.toggle("active")
来源：http://vu.shxzukj.cn

[U102] JS：本地存储
来源：http://qn.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ub.szsharing.cn

[U103] JS：定时器
来源：http://ix.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qj.shtwfgs.cn

[U104] JS：防抖
来源：http://sq.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dy.jctech888.com.cn

[U105] JS：节流
来源：http://uv.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uo.hnjuh.cn

[U106] JS：日期格式化
来源：http://xl.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pc.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://vq.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cu.chemitech.net.cn

[U108] JS：随机整数
来源：http://vu.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zk.szsharing.cn

[U109] JS：数组分组
来源：http://ke.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://vl.chemitech.net.cn

[U110] JS：数组分块
来源：http://zy.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ms.szsharing.cn

[U111] JS：对象转 Map
来源：http://xh.shxzskj.cn

new Map(Object.entries(obj))
来源：http://df.wgjwhj.cn

[U112] JS：字符串补位
来源：http://au.9csxet.cn

"7".padStart(3, "0")
来源：http://az.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://dd.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://dn.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://nr.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://je.colortex.cn

[U115] JS：生成 UUID
来源：http://mp.bjjhwx.cn

crypto.randomUUID()
来源：http://um.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://iq.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://ad.nszjky.cn

[U117] JS：单元测试
来源：http://gl.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://ct.9csxet.cn

[U118] JS：开发服务器
来源：http://zp.szsharing.cn

npm i -D vite;  npx vite
来源：http://ig.jctech888.com.cn

[U119] JS：生产构建
来源：http://hs.wgjwhj.cn

npx vite build
来源：http://cj.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://ut.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://sf.szsharing.cn

================================================================================
来源：http://of.szxytkj.cn

统计汇总
来源：http://dw.shxzukj.cn

================================================================================
来源：http://pc.lnxyls.cn

按语言统计（条）：
来源：http://gi.huanxung.cn

Python ......... 252
来源：http://zl.huixiangedu.cn

PHP ............ 252
来源：http://rs.jianghongdianzi.cn

JavaScript ..... 252
来源：http://yd.szsharing.cn

TypeScript ..... 212
来源：http://cw.yuexingan06.cn

Java ........... 212
来源：http://gz.chemitech.net.cn

Go ............. 212
来源：http://yy.chemitech.net.cn

Ruby ........... 212
来源：http://ii.shtwfgs.cn

C# ............. 212
来源：http://ox.521024.cn

C .............. 30
来源：http://oz.9csxet.cn

C++ ............ 30
来源：http://uz.shxzskj.cn

SQL ............ 90
来源：http://rs.panjiajie.cn

Bash ........... 80
来源：http://bg.hnjuh.cn

Kotlin ......... 15
来源：http://qk.yuntaijiaju.cn

Swift .......... 15
来源：http://vc.shtwfgs.cn

Lua ............ 10
来源：http://ji.colortex.cn

Perl ........... 10
来源：http://sa.gzmigu.cn

Scala .......... 10
来源：http://ci.panjiajie.cn

------------------------------------
来源：http://lf.nszjky.cn

合计 ........... 2106 条
来源：http://vy.bjjhwx.cn

按章节统计：
来源：http://yq.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cn.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rv.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qv.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nd.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aw.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://il.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pj.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gq.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sv.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fd.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nv.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bi.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ck.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://my.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cr.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qq.muxihuayi.cn

Q SQL 专题                              90
来源：http://nk.yuexingan06.cn

R Bash 专题                             80
来源：http://mi.chemitech.net.cn

S C / C++ 专题                          60
来源：http://pu.hahajie.cn

T 其他语言补充                          60
来源：http://el.muxihuayi.cn

U 高频实用片段                         120
来源：http://tt.huanxung.cn

------------------------------------
来源：http://wc.chemitech.net.cn

合计                                  2106 条
来源：http://px.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://uc.chemitech.net.cn

使用提醒
来源：http://pb.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://go.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lv.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ld.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rv.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dj.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wc.huanxung.cn

—— 文件结束 ——
来源：http://zb.newstarts.cn

================================================================================
来源：http://nv.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://nw.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://um.521024.cn

================================================================================
来源：http://ph.newstarts.cn

【收录内容】
来源：http://ev.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nd.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yz.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://fx.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jianghongdianzi.cn

【使用说明】
来源：http://ti.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cm.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ep.bookmarksfly.cn


<!-- 参考信息 -->