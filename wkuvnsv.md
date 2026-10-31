代发 wailian999

[U07] Py：反转字典键值
来源：http://qk.szsharing.cn

{v: k for k, v in d.items()}
来源：http://kf.asd995.cn

[U08] Py：展平二维列表
来源：http://qx.wgjwhj.cn

[y for x in nested for y in x]
来源：http://zp.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://lt.gzmigu.cn

max(d, key=d.get)
来源：http://vw.newstarts.cn

[U10] Py：按值排序字典
来源：http://tz.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zp.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://bx.gzmigu.cn

(x * 2 for x in arr)
来源：http://vz.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://so.521024.cn

Counter(arr).most_common(3)
来源：http://vm.newstarts.cn

[U13] Py：固定长度队列
来源：http://kd.panjiajie.cn

deque(maxlen=10)
来源：http://gu.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://bd.wgjwhj.cn

defaultdict(list)
来源：http://uu.colortex.cn

[U15] Py：高精度计时
来源：http://sy.hahajie.cn

t = time.perf_counter()
来源：http://pd.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://tp.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mo.9csxet.cn

[U17] Py：初始化日志
来源：http://qw.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://hl.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://oy.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://ph.nicolike.cn

[U19] Py：正则替换带回调
来源：http://bs.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ky.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://ft.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://zu.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://xx.szxytkj.cn

@contextlib.contextmanager
来源：http://wn.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://al.bjjhwx.cn

list(zip(*m))
来源：http://tj.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://lw.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pe.szxytkj.cn

[U24] Py：路径操作
来源：http://yu.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dn.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://td.asd995.cn

csv.DictReader(f)
来源：http://nj.chemitech.net.cn

[U26] Py：并发下载
来源：http://kg.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://la.newstarts.cn

[U27] Py：异步 HTTP
来源：http://an.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://xi.hahajie.cn

[U28] Py：类型别名
来源：http://cg.huanxung.cn

UserId = int
来源：http://ea.9csxet.cn

[U29] Py：属性校验
来源：http://zd.huanxung.cn

@property 与 @x.setter 配合
来源：http://lj.521024.cn

[U30] Py：数据类
来源：http://jf.wgjwhj.cn

@dataclass(slots=True)
来源：http://vy.szsharing.cn

[U31] Py：单测
来源：http://qh.huixinmuqiang.cn

python -m pytest -q
来源：http://th.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://rp.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://yc.nszjky.cn

[U33] Py：打包发布
来源：http://ci.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://rb.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://kf.gzmigu.cn

chardet.detect(raw)
来源：http://hs.shxzukj.cn

[U35] Py：发送邮件
来源：http://lz.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xz.shxzskj.cn

[U36] Py：定时任务
来源：http://mu.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://eq.9csxet.cn

[U37] Py：读写 Excel
来源：http://wp.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ww.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://dw.nszjky.cn

Path(__file__).resolve().parent
来源：http://la.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://dw.newstarts.cn

sys.stdout.isatty()
来源：http://sm.szsharing.cn

[U40] Py：打印到标准错误
来源：http://ay.shxzskj.cn

print("err", file=sys.stderr)
来源：http://sv.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://tw.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ep.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://ph.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hx.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://kj.wgjwhj.cn

namespace App\Http;
来源：http://hn.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://qy.shtwfgs.cn

declare(strict_types=1);
来源：http://ru.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://gz.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rk.colortex.cn

[U46] PHP：可空类型
来源：http://xj.521024.cn

?string $name = null
来源：http://wz.haigaiapp.cn

[U47] PHP：联合类型
来源：http://si.chemitech.net.cn

int|string $id
来源：http://sr.shxzskj.cn

[U48] PHP：纯枚举
来源：http://ft.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ue.wgjwhj.cn

[U49] PHP：只读属性
来源：http://hy.nszjky.cn

public readonly string $name
来源：http://je.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://ae.nicolike.cn

public function __construct(private int $id) {}
来源：http://ez.szxytkj.cn

[U51] PHP：数组解构
来源：http://yt.szsharing.cn

[$a, $b] = $arr;
来源：http://qf.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://pm.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://la.asd995.cn

[U53] PHP：空合并运算符
来源：http://px.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://ld.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://vz.9csxet.cn

$obj?->method()
来源：http://lp.nicolike.cn

[U55] PHP：match 表达式
来源：http://rp.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jv.huanxung.cn

[U56] PHP：命名参数
来源：http://mh.szsharing.cn

f(a: 1, b: 2)
来源：http://ca.asd995.cn

[U57] PHP：字符串插值
来源：http://le.yuexingan06.cn

"值: {$a}"
来源：http://pu.newstarts.cn

[U58] PHP：数组三件套
来源：http://ev.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xz.huanxung.cn

[U59] PHP：自定义排序
来源：http://dy.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bd.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://kc.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://is.huanxung.cn

[U61] PHP：正则
来源：http://gc.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fr.haigaiapp.cn

[U62] PHP：日期对象
来源：http://dw.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yq.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://ll.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rz.panjiajie.cn

[U64] PHP：目录遍历
来源：http://ys.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://ce.9csxet.cn

[U65] PHP：会话
来源：http://cy.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qb.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://bp.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ko.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://ed.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jx.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://re.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://az.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://vn.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://of.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://wa.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xe.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://if.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ns.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://vy.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ad.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://of.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://sw.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://rm.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://aw.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://ys.asd995.cn

composer require psr/container
来源：http://cj.muxihuayi.cn

[U76] PHP：简单路由
来源：http://jb.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wa.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://uv.521024.cn

composer require twig/twig
来源：http://wb.yuexingan06.cn

[U78] PHP：单元测试
来源：http://si.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://hl.gzmigu.cn

[U79] PHP：静态分析
来源：http://uj.521024.cn

composer require --dev phpstan/phpstan
来源：http://ul.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://bh.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xx.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://zf.jctech888.com.cn

npm init -y;  npm i express
来源：http://ml.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://ll.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://us.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://iu.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qf.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://io.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rt.jianghongdianzi.cn

[U85] JS：可选链
来源：http://nx.muxihuayi.cn

a?.b?.c
来源：http://on.szxytkj.cn

[U86] JS：空值合并
来源：http://hv.hahajie.cn

a ?? b
来源：http://mc.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ub.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://mh.gzmigu.cn

[U88] JS：对象展开合并
来源：http://zu.shxzukj.cn

{ ...a, ...b }
来源：http://rt.shxzukj.cn

[U89] JS：数组去重
来源：http://zl.shtwfgs.cn

[...new Set(arr)]
来源：http://xw.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://pv.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://yj.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://di.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jy.wgjwhj.cn

[U92] JS：深拷贝
来源：http://bs.huixinmuqiang.cn

structuredClone(obj)
来源：http://wj.newstarts.cn

[U93] JS：模板字符串
来源：http://ti.szxytkj.cn

`共 ${n} 条`
来源：http://xw.nicolike.cn

[U94] JS：箭头函数
来源：http://fj.jianghongdianzi.cn

const double = x => x * 2;
来源：http://kr.521024.cn

[U95] JS：Promise 包装
来源：http://ob.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://qn.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://pc.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ko.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://lk.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ko.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cp.asd995.cn

[U99] JS：事件监听
来源：http://sd.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://dc.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://jf.jctech888.com.cn

document.querySelector(".item")
来源：http://lu.yuexingan06.cn

[U101] JS：classList 操作
来源：http://gz.521024.cn

el.classList.toggle("active")
来源：http://lz.newstarts.cn

[U102] JS：本地存储
来源：http://rt.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fr.hnjuh.cn

[U103] JS：定时器
来源：http://ek.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tl.huixinmuqiang.cn

[U104] JS：防抖
来源：http://lx.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bp.bjjhwx.cn

[U105] JS：节流
来源：http://bw.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kv.wgjwhj.cn

[U106] JS：日期格式化
来源：http://ok.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ss.huanxung.cn

[U107] JS：数字千分位
来源：http://by.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rx.bjjhwx.cn

[U108] JS：随机整数
来源：http://ba.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://su.bookmarksfly.cn

[U109] JS：数组分组
来源：http://uh.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://ov.colortex.cn

[U110] JS：数组分块
来源：http://dm.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bt.hnjuh.cn

[U111] JS：对象转 Map
来源：http://eh.9csxet.cn

new Map(Object.entries(obj))
来源：http://di.haigaiapp.cn

[U112] JS：字符串补位
来源：http://he.9csxet.cn

"7".padStart(3, "0")
来源：http://vo.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://ta.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://ua.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://rh.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xg.hahajie.cn

[U115] JS：生成 UUID
来源：http://wz.nicolike.cn

crypto.randomUUID()
来源：http://vk.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://mb.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://fx.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://yf.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://yw.muxihuayi.cn

[U118] JS：开发服务器
来源：http://qv.lnxyls.cn

npm i -D vite;  npx vite
来源：http://xa.shtwfgs.cn

[U119] JS：生产构建
来源：http://gi.huanxung.cn

npx vite build
来源：http://vp.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://hh.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://nu.newstarts.cn

================================================================================
来源：http://he.shxzskj.cn

统计汇总
来源：http://zd.shtwfgs.cn

================================================================================
来源：http://aj.jctech888.com.cn

按语言统计（条）：
来源：http://ms.shxzukj.cn

Python ......... 252
来源：http://ze.szxytkj.cn

PHP ............ 252
来源：http://qu.hahajie.cn

JavaScript ..... 252
来源：http://je.chemitech.net.cn

TypeScript ..... 212
来源：http://qu.szxytkj.cn

Java ........... 212
来源：http://ep.szsharing.cn

Go ............. 212
来源：http://bo.yuexingan06.cn

Ruby ........... 212
来源：http://uf.haigaiapp.cn

C# ............. 212
来源：http://nd.huanxung.cn

C .............. 30
来源：http://ln.9csxet.cn

C++ ............ 30
来源：http://uv.chemitech.net.cn

SQL ............ 90
来源：http://yb.huanxung.cn

Bash ........... 80
来源：http://zv.chemitech.net.cn

Kotlin ......... 15
来源：http://mq.shtwfgs.cn

Swift .......... 15
来源：http://ab.jianghongdianzi.cn

Lua ............ 10
来源：http://ra.gzmigu.cn

Perl ........... 10
来源：http://wu.hnjuh.cn

Scala .......... 10
来源：http://sb.shxzukj.cn

------------------------------------
来源：http://vm.shxzukj.cn

合计 ........... 2106 条
来源：http://cy.lnxyls.cn

按章节统计：
来源：http://yg.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hk.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wu.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://id.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rt.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ik.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bq.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kr.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jf.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wc.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bm.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jc.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zq.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jq.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zl.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tm.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rc.lnxyls.cn

Q SQL 专题                              90
来源：http://un.szxytkj.cn

R Bash 专题                             80
来源：http://ph.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://ry.newstarts.cn

T 其他语言补充                          60
来源：http://np.jctech888.com.cn

U 高频实用片段                         120
来源：http://vj.chemitech.net.cn

------------------------------------
来源：http://hj.9csxet.cn

合计                                  2106 条
来源：http://cl.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://yw.hnjuh.cn

使用提醒
来源：http://en.huanxung.cn

--------------------------------------------------------------------------------
来源：http://eb.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ir.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dy.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vc.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pi.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bq.hahajie.cn

—— 文件结束 ——
来源：http://zz.huanxung.cn

================================================================================
来源：http://ad.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://it.szsharing.cn

Common Programming Examples Cheat Book
来源：http://xr.yuexingan06.cn

================================================================================
来源：http://ux.huanxung.cn

【收录内容】
来源：http://yq.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qg.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vx.jctech888.com.cn

SQL · Bash · C · C++
来源：http://qp.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ls.jctech888.com.cn

【使用说明】
来源：http://cl.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ka.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lf.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tc.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wo.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kt.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xz.jianghongdianzi.cn


<!-- 参考信息 -->