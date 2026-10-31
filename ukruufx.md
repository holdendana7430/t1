代发 wailian999

[U05] Py：列表去重且保序
来源：http://lh.nszjky.cn

list(dict.fromkeys(arr))
来源：http://cr.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://fj.jctech888.com.cn

{**a, **b}
来源：http://ms.nszjky.cn

[U07] Py：反转字典键值
来源：http://xg.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://yc.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://uz.panjiajie.cn

[y for x in nested for y in x]
来源：http://az.colortex.cn

[U09] Py：字典取最大值的键
来源：http://rz.panjiajie.cn

max(d, key=d.get)
来源：http://wu.colortex.cn

[U10] Py：按值排序字典
来源：http://ez.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eo.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://cr.bjjhwx.cn

(x * 2 for x in arr)
来源：http://wu.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yu.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://io.shxzukj.cn

[U13] Py：固定长度队列
来源：http://xw.newstarts.cn

deque(maxlen=10)
来源：http://ip.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://rm.haigaiapp.cn

defaultdict(list)
来源：http://jt.szxytkj.cn

[U15] Py：高精度计时
来源：http://hx.nszjky.cn

t = time.perf_counter()
来源：http://lv.asd995.cn

[U16] Py：命令行参数解析
来源：http://xu.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nt.shxzskj.cn

[U17] Py：初始化日志
来源：http://dk.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ju.chemitech.net.cn

[U18] Py：预编译正则
来源：http://ar.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://kn.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://sz.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hf.newstarts.cn

[U20] Py：缓存函数结果
来源：http://eo.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://bd.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://bg.huixiangedu.cn

@contextlib.contextmanager
来源：http://cz.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://wo.huanxung.cn

list(zip(*m))
来源：http://et.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ph.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dj.huixiangedu.cn

[U24] Py：路径操作
来源：http://tv.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sm.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://gj.shxzukj.cn

csv.DictReader(f)
来源：http://rg.wgjwhj.cn

[U26] Py：并发下载
来源：http://bx.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dl.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://ab.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://kn.muxihuayi.cn

[U28] Py：类型别名
来源：http://wt.wgjwhj.cn

UserId = int
来源：http://oq.chemitech.net.cn

[U29] Py：属性校验
来源：http://ol.asd995.cn

@property 与 @x.setter 配合
来源：http://qy.asd995.cn

[U30] Py：数据类
来源：http://um.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://fx.jctech888.com.cn

[U31] Py：单测
来源：http://rf.gzmigu.cn

python -m pytest -q
来源：http://hs.huanxung.cn

[U32] Py：代码格式化
来源：http://fs.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://fi.gzmigu.cn

[U33] Py：打包发布
来源：http://al.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://kr.lnxyls.cn

[U34] Py：判断编码
来源：http://sw.haigaiapp.cn

chardet.detect(raw)
来源：http://wb.huixiangedu.cn

[U35] Py：发送邮件
来源：http://uv.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fc.bookmarksfly.cn

[U36] Py：定时任务
来源：http://he.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://pe.szxytkj.cn

[U37] Py：读写 Excel
来源：http://qy.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vh.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://xb.nicolike.cn

Path(__file__).resolve().parent
来源：http://hx.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://dw.nicolike.cn

sys.stdout.isatty()
来源：http://pn.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://gb.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://kn.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://mu.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qm.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://tk.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hh.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://zu.hnjuh.cn

namespace App\Http;
来源：http://rs.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://lu.521024.cn

declare(strict_types=1);
来源：http://xs.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://rn.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ax.jctech888.com.cn

[U46] PHP：可空类型
来源：http://vx.bookmarksfly.cn

?string $name = null
来源：http://qw.haigaiapp.cn

[U47] PHP：联合类型
来源：http://po.jctech888.com.cn

int|string $id
来源：http://tm.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://pb.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dq.chemitech.net.cn

[U49] PHP：只读属性
来源：http://wm.asd995.cn

public readonly string $name
来源：http://sm.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://xp.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://fs.yuexingan06.cn

[U51] PHP：数组解构
来源：http://jy.huixiangedu.cn

[$a, $b] = $arr;
来源：http://os.colortex.cn

[U52] PHP：箭头函数
来源：http://sg.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://df.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://vl.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://wz.huanxung.cn

[U54] PHP：空安全调用
来源：http://di.bookmarksfly.cn

$obj?->method()
来源：http://jq.lnxyls.cn

[U55] PHP：match 表达式
来源：http://vn.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://af.hnjuh.cn

[U56] PHP：命名参数
来源：http://ix.asd995.cn

f(a: 1, b: 2)
来源：http://fa.huanxung.cn

[U57] PHP：字符串插值
来源：http://km.panjiajie.cn

"值: {$a}"
来源：http://qs.9csxet.cn

[U58] PHP：数组三件套
来源：http://cr.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vz.hnjuh.cn

[U59] PHP：自定义排序
来源：http://mz.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eq.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://dp.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cm.colortex.cn

[U61] PHP：正则
来源：http://pf.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ic.shxzukj.cn

[U62] PHP：日期对象
来源：http://un.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ov.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ks.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sl.lnxyls.cn

[U64] PHP：目录遍历
来源：http://lj.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://kn.shxzskj.cn

[U65] PHP：会话
来源：http://qa.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ex.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://xm.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nm.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://sz.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fn.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://or.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fg.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://wf.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://at.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ob.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fp.colortex.cn

[U71] PHP：抛出异常
来源：http://ll.521024.cn

throw new RuntimeException("失败", 500);
来源：http://au.colortex.cn

[U72] PHP：写错误日志
来源：http://ff.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://sd.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://tt.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://cf.huanxung.cn

[U74] PHP：读取环境变量
来源：http://wv.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://js.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://cr.panjiajie.cn

composer require psr/container
来源：http://ju.panjiajie.cn

[U76] PHP：简单路由
来源：http://gx.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xl.nicolike.cn

[U77] PHP：模板渲染
来源：http://cs.asd995.cn

composer require twig/twig
来源：http://nw.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://lt.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://ux.521024.cn

[U79] PHP：静态分析
来源：http://pf.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://oo.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://um.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xz.nszjky.cn

[U81] JS：初始化项目
来源：http://if.huixiangedu.cn

npm init -y;  npm i express
来源：http://vk.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://ty.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fb.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://rf.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xl.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://vf.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pf.jianghongdianzi.cn

[U85] JS：可选链
来源：http://oe.shtwfgs.cn

a?.b?.c
来源：http://hp.gzmigu.cn

[U86] JS：空值合并
来源：http://er.yuexingan06.cn

a ?? b
来源：http://fc.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://uo.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://zz.asd995.cn

[U88] JS：对象展开合并
来源：http://rv.nicolike.cn

{ ...a, ...b }
来源：http://dz.szsharing.cn

[U89] JS：数组去重
来源：http://tt.lnxyls.cn

[...new Set(arr)]
来源：http://ot.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://wl.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://dt.521024.cn

[U91] JS：对象键值遍历
来源：http://cn.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dt.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://ya.shxzukj.cn

structuredClone(obj)
来源：http://xa.gzmigu.cn

[U93] JS：模板字符串
来源：http://rk.huixiangedu.cn

`共 ${n} 条`
来源：http://wr.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://hz.bookmarksfly.cn

const double = x => x * 2;
来源：http://xe.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://jm.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://oj.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://ej.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fh.9csxet.cn

[U97] JS：并发请求
来源：http://ue.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fc.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://xq.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wk.asd995.cn

[U99] JS：事件监听
来源：http://es.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://gl.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://yf.jianghongdianzi.cn

document.querySelector(".item")
来源：http://be.bjjhwx.cn

[U101] JS：classList 操作
来源：http://hp.jctech888.com.cn

el.classList.toggle("active")
来源：http://yo.wgjwhj.cn

[U102] JS：本地存储
来源：http://ju.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kk.yuexingan06.cn

[U103] JS：定时器
来源：http://dc.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ia.szxytkj.cn

[U104] JS：防抖
来源：http://so.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fo.newstarts.cn

[U105] JS：节流
来源：http://fu.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gl.nicolike.cn

[U106] JS：日期格式化
来源：http://kb.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rl.huanxung.cn

[U107] JS：数字千分位
来源：http://yg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ws.colortex.cn

[U108] JS：随机整数
来源：http://lq.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hx.szxytkj.cn

[U109] JS：数组分组
来源：http://fv.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://zs.gzmigu.cn

[U110] JS：数组分块
来源：http://if.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ux.gzmigu.cn

[U111] JS：对象转 Map
来源：http://dg.newstarts.cn

new Map(Object.entries(obj))
来源：http://tp.huixiangedu.cn

[U112] JS：字符串补位
来源：http://ko.bjjhwx.cn

"7".padStart(3, "0")
来源：http://dl.9csxet.cn

[U113] JS：正则替换全部
来源：http://zr.szxytkj.cn

s.replaceAll("a", "b")
来源：http://tq.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://ae.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://up.9csxet.cn

[U115] JS：生成 UUID
来源：http://wb.szxytkj.cn

crypto.randomUUID()
来源：http://eu.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://ev.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://pp.521024.cn

[U117] JS：单元测试
来源：http://wh.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://xy.lnxyls.cn

[U118] JS：开发服务器
来源：http://ge.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://tv.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://bg.szsharing.cn

npx vite build
来源：http://qj.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://ab.521024.cn

import.meta.env.VITE_API_URL
来源：http://lz.hnjuh.cn

================================================================================
来源：http://cb.wgjwhj.cn

统计汇总
来源：http://xy.wgjwhj.cn

================================================================================
来源：http://rp.shxzskj.cn

按语言统计（条）：
来源：http://ff.hnjuh.cn

Python ......... 252
来源：http://du.nszjky.cn

PHP ............ 252
来源：http://ij.521024.cn

JavaScript ..... 252
来源：http://zh.chemitech.net.cn

TypeScript ..... 212
来源：http://so.nszjky.cn

Java ........... 212
来源：http://cu.huixiangedu.cn

Go ............. 212
来源：http://ie.colortex.cn

Ruby ........... 212
来源：http://ty.521024.cn

C# ............. 212
来源：http://lz.nszjky.cn

C .............. 30
来源：http://wo.hahajie.cn

C++ ............ 30
来源：http://hg.shxzskj.cn

SQL ............ 90
来源：http://bw.bjjhwx.cn

Bash ........... 80
来源：http://uk.nszjky.cn

Kotlin ......... 15
来源：http://go.shtwfgs.cn

Swift .......... 15
来源：http://vm.gzmigu.cn

Lua ............ 10
来源：http://bx.yuntaijiaju.cn

Perl ........... 10
来源：http://pg.shxzukj.cn

Scala .......... 10
来源：http://gb.huixiangedu.cn

------------------------------------
来源：http://un.huixiangedu.cn

合计 ........... 2106 条
来源：http://tp.yuntaijiaju.cn

按章节统计：
来源：http://kr.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mb.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vg.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pm.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rd.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bj.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ap.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jh.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zh.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://et.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pa.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fk.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://se.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pp.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sh.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://re.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tp.huixiangedu.cn

Q SQL 专题                              90
来源：http://bu.muxihuayi.cn

R Bash 专题                             80
来源：http://wa.huanxung.cn

S C / C++ 专题                          60
来源：http://ng.panjiajie.cn

T 其他语言补充                          60
来源：http://jr.panjiajie.cn

U 高频实用片段                         120
来源：http://tt.nicolike.cn

------------------------------------
来源：http://xt.muxihuayi.cn

合计                                  2106 条
来源：http://jz.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ls.hnjuh.cn

使用提醒
来源：http://bh.521024.cn

--------------------------------------------------------------------------------
来源：http://jr.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wo.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nw.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ts.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mi.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yw.wgjwhj.cn

—— 文件结束 ——
来源：http://fo.haigaiapp.cn

================================================================================
来源：http://sl.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://ou.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://jd.shxzskj.cn

================================================================================
来源：http://sx.huixinmuqiang.cn

【收录内容】
来源：http://zd.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dg.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ch.hnjuh.cn

SQL · Bash · C · C++
来源：http://xg.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gx.huixiangedu.cn

【使用说明】
来源：http://mc.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bk.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ur.nszjky.cn


<!-- 参考信息 -->