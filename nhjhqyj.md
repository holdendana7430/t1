代发 wailian999

[U09] Py：字典取最大值的键
来源：http://iy.hahajie.cn

max(d, key=d.get)
来源：http://sm.gzmigu.cn

[U10] Py：按值排序字典
来源：http://zj.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vn.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://hx.shtwfgs.cn

(x * 2 for x in arr)
来源：http://xi.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iy.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://dm.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://pz.jianghongdianzi.cn

deque(maxlen=10)
来源：http://or.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://ko.yuexingan06.cn

defaultdict(list)
来源：http://lf.lnxyls.cn

[U15] Py：高精度计时
来源：http://ki.wgjwhj.cn

t = time.perf_counter()
来源：http://qs.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://zk.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gh.shxzskj.cn

[U17] Py：初始化日志
来源：http://jz.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ct.szsharing.cn

[U18] Py：预编译正则
来源：http://ts.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://pj.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://uh.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cn.szsharing.cn

[U20] Py：缓存函数结果
来源：http://ca.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://rg.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://qd.bjjhwx.cn

@contextlib.contextmanager
来源：http://ao.shxzskj.cn

[U22] Py：矩阵转置
来源：http://yn.yuexingan06.cn

list(zip(*m))
来源：http://qb.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://zr.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cq.nszjky.cn

[U24] Py：路径操作
来源：http://qo.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yj.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://kx.chemitech.net.cn

csv.DictReader(f)
来源：http://wi.hnjuh.cn

[U26] Py：并发下载
来源：http://yt.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://va.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://yh.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://hw.lnxyls.cn

[U28] Py：类型别名
来源：http://qq.shxzskj.cn

UserId = int
来源：http://mk.jctech888.com.cn

[U29] Py：属性校验
来源：http://co.nicolike.cn

@property 与 @x.setter 配合
来源：http://nj.huixiangedu.cn

[U30] Py：数据类
来源：http://uy.hnjuh.cn

@dataclass(slots=True)
来源：http://um.yuntaijiaju.cn

[U31] Py：单测
来源：http://vr.asd995.cn

python -m pytest -q
来源：http://sd.chemitech.net.cn

[U32] Py：代码格式化
来源：http://wr.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://hp.shxzukj.cn

[U33] Py：打包发布
来源：http://bf.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://cb.yuexingan06.cn

[U34] Py：判断编码
来源：http://xs.newstarts.cn

chardet.detect(raw)
来源：http://xi.nszjky.cn

[U35] Py：发送邮件
来源：http://am.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gh.9csxet.cn

[U36] Py：定时任务
来源：http://ji.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://rl.newstarts.cn

[U37] Py：读写 Excel
来源：http://sc.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://th.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://ow.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://sr.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://pw.hahajie.cn

sys.stdout.isatty()
来源：http://oj.newstarts.cn

[U40] Py：打印到标准错误
来源：http://tc.nszjky.cn

print("err", file=sys.stderr)
来源：http://iz.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ak.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://su.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://bn.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lv.hahajie.cn

[U43] PHP：声明命名空间
来源：http://rf.hnjuh.cn

namespace App\Http;
来源：http://qz.szsharing.cn

[U44] PHP：开启严格类型
来源：http://wv.bjjhwx.cn

declare(strict_types=1);
来源：http://it.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://kz.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ao.szxytkj.cn

[U46] PHP：可空类型
来源：http://wl.colortex.cn

?string $name = null
来源：http://vo.haigaiapp.cn

[U47] PHP：联合类型
来源：http://gk.yuntaijiaju.cn

int|string $id
来源：http://wj.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://ab.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hj.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ut.huixinmuqiang.cn

public readonly string $name
来源：http://ur.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://en.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://xi.newstarts.cn

[U51] PHP：数组解构
来源：http://us.asd995.cn

[$a, $b] = $arr;
来源：http://ur.shxzukj.cn

[U52] PHP：箭头函数
来源：http://ts.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://yv.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://yg.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://au.asd995.cn

[U54] PHP：空安全调用
来源：http://mz.newstarts.cn

$obj?->method()
来源：http://qw.hnjuh.cn

[U55] PHP：match 表达式
来源：http://hs.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ft.colortex.cn

[U56] PHP：命名参数
来源：http://by.shxzskj.cn

f(a: 1, b: 2)
来源：http://cy.szsharing.cn

[U57] PHP：字符串插值
来源：http://lv.hahajie.cn

"值: {$a}"
来源：http://ji.asd995.cn

[U58] PHP：数组三件套
来源：http://cr.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ll.nszjky.cn

[U59] PHP：自定义排序
来源：http://tz.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xs.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://se.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qr.hnjuh.cn

[U61] PHP：正则
来源：http://sg.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://in.jctech888.com.cn

[U62] PHP：日期对象
来源：http://ko.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fa.lnxyls.cn

[U63] PHP：文件读写
来源：http://rf.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ar.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://om.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://hk.wgjwhj.cn

[U65] PHP：会话
来源：http://gv.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sd.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://xm.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://md.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://pf.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mt.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://jq.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lk.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://my.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://al.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://gu.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ii.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://pe.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://yj.hahajie.cn

[U72] PHP：写错误日志
来源：http://ry.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://ma.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://zx.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://wm.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://gj.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://qt.lnxyls.cn

[U75] PHP：依赖注入
来源：http://hf.hahajie.cn

composer require psr/container
来源：http://be.szxytkj.cn

[U76] PHP：简单路由
来源：http://pq.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mu.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://cg.shxzukj.cn

composer require twig/twig
来源：http://zb.nicolike.cn

[U78] PHP：单元测试
来源：http://hp.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://yt.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://xx.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://qw.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://yd.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mr.hahajie.cn

[U81] JS：初始化项目
来源：http://cr.wgjwhj.cn

npm init -y;  npm i express
来源：http://yp.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://zt.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ey.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://um.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wr.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://qr.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oy.muxihuayi.cn

[U85] JS：可选链
来源：http://ob.hahajie.cn

a?.b?.c
来源：http://nj.asd995.cn

[U86] JS：空值合并
来源：http://pe.hnjuh.cn

a ?? b
来源：http://xr.huixiangedu.cn

[U87] JS：解构默认值
来源：http://mj.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://ef.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://dj.gzmigu.cn

{ ...a, ...b }
来源：http://uf.9csxet.cn

[U89] JS：数组去重
来源：http://jv.bookmarksfly.cn

[...new Set(arr)]
来源：http://ka.huanxung.cn

[U90] JS：数字数组排序
来源：http://oy.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://ay.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://xs.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sr.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://cl.lnxyls.cn

structuredClone(obj)
来源：http://bm.huanxung.cn

[U93] JS：模板字符串
来源：http://yn.shtwfgs.cn

`共 ${n} 条`
来源：http://df.shxzukj.cn

[U94] JS：箭头函数
来源：http://ng.gzmigu.cn

const double = x => x * 2;
来源：http://pl.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://an.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://qx.huanxung.cn

[U96] JS：async/await 与异常
来源：http://vm.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yf.shxzskj.cn

[U97] JS：并发请求
来源：http://xr.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cf.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://nz.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xt.bookmarksfly.cn

[U99] JS：事件监听
来源：http://wz.nicolike.cn

el.addEventListener("click", e => {})
来源：http://qo.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://wz.shxzukj.cn

document.querySelector(".item")
来源：http://iu.hnjuh.cn

[U101] JS：classList 操作
来源：http://vz.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://ju.lnxyls.cn

[U102] JS：本地存储
来源：http://ec.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sg.bjjhwx.cn

[U103] JS：定时器
来源：http://xw.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ls.shxzukj.cn

[U104] JS：防抖
来源：http://mu.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gb.jianghongdianzi.cn

[U105] JS：节流
来源：http://bl.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aj.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://oc.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cb.wgjwhj.cn

[U107] JS：数字千分位
来源：http://ps.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xg.hnjuh.cn

[U108] JS：随机整数
来源：http://mh.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ny.yuexingan06.cn

[U109] JS：数组分组
来源：http://bt.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://qk.panjiajie.cn

[U110] JS：数组分块
来源：http://gf.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://er.gzmigu.cn

[U111] JS：对象转 Map
来源：http://vd.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://qv.shxzukj.cn

[U112] JS：字符串补位
来源：http://jh.jctech888.com.cn

"7".padStart(3, "0")
来源：http://vs.nicolike.cn

[U113] JS：正则替换全部
来源：http://lp.nicolike.cn

s.replaceAll("a", "b")
来源：http://yj.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://lp.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ei.szsharing.cn

[U115] JS：生成 UUID
来源：http://pq.jianghongdianzi.cn

crypto.randomUUID()
来源：http://ld.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://za.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://nm.asd995.cn

[U117] JS：单元测试
来源：http://ru.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://ir.wgjwhj.cn

[U118] JS：开发服务器
来源：http://ef.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://nn.wgjwhj.cn

[U119] JS：生产构建
来源：http://iz.szsharing.cn

npx vite build
来源：http://bz.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://tv.bookmarksfly.cn

================================================================================
来源：http://un.szsharing.cn

统计汇总
来源：http://jy.bookmarksfly.cn

================================================================================
来源：http://wy.huixinmuqiang.cn

按语言统计（条）：
来源：http://gd.huixinmuqiang.cn

Python ......... 252
来源：http://jz.huanxung.cn

PHP ............ 252
来源：http://tn.lnxyls.cn

JavaScript ..... 252
来源：http://bf.chemitech.net.cn

TypeScript ..... 212
来源：http://ns.huixinmuqiang.cn

Java ........... 212
来源：http://yy.jctech888.com.cn

Go ............. 212
来源：http://al.bookmarksfly.cn

Ruby ........... 212
来源：http://uc.wgjwhj.cn

C# ............. 212
来源：http://pw.szxytkj.cn

C .............. 30
来源：http://kl.9csxet.cn

C++ ............ 30
来源：http://tj.szxytkj.cn

SQL ............ 90
来源：http://pn.muxihuayi.cn

Bash ........... 80
来源：http://qq.huixinmuqiang.cn

Kotlin ......... 15
来源：http://nm.gzmigu.cn

Swift .......... 15
来源：http://ff.chemitech.net.cn

Lua ............ 10
来源：http://lc.szxytkj.cn

Perl ........... 10
来源：http://mc.521024.cn

Scala .......... 10
来源：http://cl.yuntaijiaju.cn

------------------------------------
来源：http://jo.hnjuh.cn

合计 ........... 2106 条
来源：http://kq.shxzukj.cn

按章节统计：
来源：http://qb.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rd.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xw.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sa.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mf.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gz.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yp.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bb.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rt.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vd.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fs.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nj.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://em.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qa.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sn.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ll.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lx.chemitech.net.cn

Q SQL 专题                              90
来源：http://kk.hahajie.cn

R Bash 专题                             80
来源：http://ok.haigaiapp.cn

S C / C++ 专题                          60
来源：http://vy.chemitech.net.cn

T 其他语言补充                          60
来源：http://ku.shtwfgs.cn

U 高频实用片段                         120
来源：http://ql.hahajie.cn

------------------------------------
来源：http://vc.asd995.cn

合计                                  2106 条
来源：http://xw.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://yq.shxzskj.cn

使用提醒
来源：http://qa.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://qk.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pw.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xs.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ec.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lx.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vz.yuexingan06.cn

—— 文件结束 ——
来源：http://cp.lnxyls.cn

================================================================================
来源：http://by.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://mx.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://uq.shxzskj.cn

================================================================================
来源：http://sa.lnxyls.cn

【收录内容】
来源：http://kv.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ma.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xu.panjiajie.cn

SQL · Bash · C · C++
来源：http://ls.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mr.yuexingan06.cn

【使用说明】
来源：http://gu.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ib.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nt.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jy.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lk.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zy.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ju.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kf.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ev.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gk.huixinmuqiang.cn


<!-- 参考信息 -->