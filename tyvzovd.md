代发 wailian999

[U07] Py：反转字典键值
来源：http://jh.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://hr.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://ld.521024.cn

[y for x in nested for y in x]
来源：http://iw.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://ot.shtwfgs.cn

max(d, key=d.get)
来源：http://wo.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://oq.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vw.nicolike.cn

[U11] Py：生成器表达式
来源：http://rx.lnxyls.cn

(x * 2 for x in arr)
来源：http://cl.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pl.521024.cn

Counter(arr).most_common(3)
来源：http://jm.huanxung.cn

[U13] Py：固定长度队列
来源：http://om.muxihuayi.cn

deque(maxlen=10)
来源：http://gy.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://qu.bjjhwx.cn

defaultdict(list)
来源：http://nm.yuexingan06.cn

[U15] Py：高精度计时
来源：http://rg.hahajie.cn

t = time.perf_counter()
来源：http://ut.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://yw.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ec.newstarts.cn

[U17] Py：初始化日志
来源：http://sp.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://uc.yuexingan06.cn

[U18] Py：预编译正则
来源：http://ad.szsharing.cn

pat = re.compile(r"\d+")
来源：http://kn.hahajie.cn

[U19] Py：正则替换带回调
来源：http://gu.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hi.huanxung.cn

[U20] Py：缓存函数结果
来源：http://zw.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://rp.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://wq.9csxet.cn

@contextlib.contextmanager
来源：http://pd.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://em.panjiajie.cn

list(zip(*m))
来源：http://tt.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://ho.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lg.lnxyls.cn

[U24] Py：路径操作
来源：http://jj.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nw.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://fl.szxytkj.cn

csv.DictReader(f)
来源：http://iz.huixiangedu.cn

[U26] Py：并发下载
来源：http://at.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://do.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://mh.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://ay.jctech888.com.cn

[U28] Py：类型别名
来源：http://kw.szsharing.cn

UserId = int
来源：http://ee.hahajie.cn

[U29] Py：属性校验
来源：http://xa.hnjuh.cn

@property 与 @x.setter 配合
来源：http://tr.gzmigu.cn

[U30] Py：数据类
来源：http://pp.hnjuh.cn

@dataclass(slots=True)
来源：http://tf.bjjhwx.cn

[U31] Py：单测
来源：http://qk.szxytkj.cn

python -m pytest -q
来源：http://rj.huanxung.cn

[U32] Py：代码格式化
来源：http://cl.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://om.jctech888.com.cn

[U33] Py：打包发布
来源：http://zi.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://cq.shxzskj.cn

[U34] Py：判断编码
来源：http://za.gzmigu.cn

chardet.detect(raw)
来源：http://jh.colortex.cn

[U35] Py：发送邮件
来源：http://aw.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hy.shtwfgs.cn

[U36] Py：定时任务
来源：http://ub.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://jg.szxytkj.cn

[U37] Py：读写 Excel
来源：http://ie.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mz.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://is.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ia.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://xd.nicolike.cn

sys.stdout.isatty()
来源：http://pk.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://ek.gzmigu.cn

print("err", file=sys.stderr)
来源：http://rt.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://qm.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oj.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://ws.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://no.asd995.cn

[U43] PHP：声明命名空间
来源：http://wn.shtwfgs.cn

namespace App\Http;
来源：http://jm.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://bc.521024.cn

declare(strict_types=1);
来源：http://zm.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://de.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lo.hahajie.cn

[U46] PHP：可空类型
来源：http://go.muxihuayi.cn

?string $name = null
来源：http://yy.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://pr.chemitech.net.cn

int|string $id
来源：http://tu.gzmigu.cn

[U48] PHP：纯枚举
来源：http://ow.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qf.wgjwhj.cn

[U49] PHP：只读属性
来源：http://hn.jianghongdianzi.cn

public readonly string $name
来源：http://ws.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://li.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ie.muxihuayi.cn

[U51] PHP：数组解构
来源：http://tz.9csxet.cn

[$a, $b] = $arr;
来源：http://un.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://df.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://yq.nicolike.cn

[U53] PHP：空合并运算符
来源：http://zj.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://hd.panjiajie.cn

[U54] PHP：空安全调用
来源：http://gs.hnjuh.cn

$obj?->method()
来源：http://vc.colortex.cn

[U55] PHP：match 表达式
来源：http://hx.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ja.szsharing.cn

[U56] PHP：命名参数
来源：http://ma.yuexingan06.cn

f(a: 1, b: 2)
来源：http://at.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://vs.nszjky.cn

"值: {$a}"
来源：http://mj.9csxet.cn

[U58] PHP：数组三件套
来源：http://cf.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wk.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://or.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gf.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://me.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xr.muxihuayi.cn

[U61] PHP：正则
来源：http://vu.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qb.bjjhwx.cn

[U62] PHP：日期对象
来源：http://ma.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hp.shxzukj.cn

[U63] PHP：文件读写
来源：http://as.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rs.9csxet.cn

[U64] PHP：目录遍历
来源：http://xd.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://os.shxzskj.cn

[U65] PHP：会话
来源：http://wn.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xd.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://gv.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ge.newstarts.cn

[U67] PHP：处理文件上传
来源：http://eq.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ri.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ad.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ji.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://fx.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://re.hahajie.cn

[U70] PHP：PDO 事务
来源：http://nn.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wk.gzmigu.cn

[U71] PHP：抛出异常
来源：http://gd.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://pl.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://jx.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://jm.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://ar.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://qb.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://iu.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://pe.9csxet.cn

[U75] PHP：依赖注入
来源：http://gx.newstarts.cn

composer require psr/container
来源：http://ie.muxihuayi.cn

[U76] PHP：简单路由
来源：http://bc.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wq.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://la.haigaiapp.cn

composer require twig/twig
来源：http://vt.shxzskj.cn

[U78] PHP：单元测试
来源：http://xm.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://qk.lnxyls.cn

[U79] PHP：静态分析
来源：http://gx.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://rc.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://wd.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iv.colortex.cn

[U81] JS：初始化项目
来源：http://ko.szsharing.cn

npm init -y;  npm i express
来源：http://sa.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://be.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ew.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://bp.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uh.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://xj.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pt.haigaiapp.cn

[U85] JS：可选链
来源：http://kf.haigaiapp.cn

a?.b?.c
来源：http://qa.hnjuh.cn

[U86] JS：空值合并
来源：http://sr.asd995.cn

a ?? b
来源：http://zq.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://vi.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://vb.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://yj.szsharing.cn

{ ...a, ...b }
来源：http://fi.shxzukj.cn

[U89] JS：数组去重
来源：http://vm.nicolike.cn

[...new Set(arr)]
来源：http://fv.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ee.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://sn.9csxet.cn

[U91] JS：对象键值遍历
来源：http://gc.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hg.huixiangedu.cn

[U92] JS：深拷贝
来源：http://bu.yuntaijiaju.cn

structuredClone(obj)
来源：http://aq.9csxet.cn

[U93] JS：模板字符串
来源：http://pu.9csxet.cn

`共 ${n} 条`
来源：http://rt.521024.cn

[U94] JS：箭头函数
来源：http://ve.gzmigu.cn

const double = x => x * 2;
来源：http://tt.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://su.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://ux.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://jz.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wo.9csxet.cn

[U97] JS：并发请求
来源：http://xv.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://li.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://lq.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lo.shxzskj.cn

[U99] JS：事件监听
来源：http://bj.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://gf.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://mq.newstarts.cn

document.querySelector(".item")
来源：http://jb.hnjuh.cn

[U101] JS：classList 操作
来源：http://cj.muxihuayi.cn

el.classList.toggle("active")
来源：http://qs.asd995.cn

[U102] JS：本地存储
来源：http://ll.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xi.gzmigu.cn

[U103] JS：定时器
来源：http://gn.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ev.hahajie.cn

[U104] JS：防抖
来源：http://rv.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bc.bookmarksfly.cn

[U105] JS：节流
来源：http://ss.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cv.panjiajie.cn

[U106] JS：日期格式化
来源：http://qd.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hq.newstarts.cn

[U107] JS：数字千分位
来源：http://ni.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://co.muxihuayi.cn

[U108] JS：随机整数
来源：http://za.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fk.wgjwhj.cn

[U109] JS：数组分组
来源：http://lf.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://rb.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://eb.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fz.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://rx.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://qh.bjjhwx.cn

[U112] JS：字符串补位
来源：http://sc.lnxyls.cn

"7".padStart(3, "0")
来源：http://mj.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://vx.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://mz.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://dm.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nj.asd995.cn

[U115] JS：生成 UUID
来源：http://hp.szxytkj.cn

crypto.randomUUID()
来源：http://lt.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://va.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://xu.huanxung.cn

[U117] JS：单元测试
来源：http://by.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://za.asd995.cn

[U118] JS：开发服务器
来源：http://yx.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://ix.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://bz.wgjwhj.cn

npx vite build
来源：http://sw.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://bk.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://kh.yuntaijiaju.cn

================================================================================
来源：http://ty.521024.cn

统计汇总
来源：http://ez.bookmarksfly.cn

================================================================================
来源：http://ow.asd995.cn

按语言统计（条）：
来源：http://rn.jctech888.com.cn

Python ......... 252
来源：http://bx.wgjwhj.cn

PHP ............ 252
来源：http://pq.muxihuayi.cn

JavaScript ..... 252
来源：http://em.nszjky.cn

TypeScript ..... 212
来源：http://va.chemitech.net.cn

Java ........... 212
来源：http://ti.nszjky.cn

Go ............. 212
来源：http://ay.nszjky.cn

Ruby ........... 212
来源：http://tz.asd995.cn

C# ............. 212
来源：http://pz.newstarts.cn

C .............. 30
来源：http://pw.wgjwhj.cn

C++ ............ 30
来源：http://ql.lnxyls.cn

SQL ............ 90
来源：http://em.newstarts.cn

Bash ........... 80
来源：http://vr.szsharing.cn

Kotlin ......... 15
来源：http://vb.huanxung.cn

Swift .......... 15
来源：http://za.colortex.cn

Lua ............ 10
来源：http://il.newstarts.cn

Perl ........... 10
来源：http://gj.jctech888.com.cn

Scala .......... 10
来源：http://cz.shxzskj.cn

------------------------------------
来源：http://bq.bookmarksfly.cn

合计 ........... 2106 条
来源：http://sc.shxzskj.cn

按章节统计：
来源：http://gk.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fn.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yt.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wi.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://az.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://py.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rw.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://si.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zl.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xm.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iy.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fs.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hm.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://op.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jv.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ch.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mv.hnjuh.cn

Q SQL 专题                              90
来源：http://ub.muxihuayi.cn

R Bash 专题                             80
来源：http://tq.yuexingan06.cn

S C / C++ 专题                          60
来源：http://wf.panjiajie.cn

T 其他语言补充                          60
来源：http://bt.newstarts.cn

U 高频实用片段                         120
来源：http://kz.gzmigu.cn

------------------------------------
来源：http://ih.nszjky.cn

合计                                  2106 条
来源：http://pb.nszjky.cn

--------------------------------------------------------------------------------
来源：http://zg.bjjhwx.cn

使用提醒
来源：http://ep.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://pd.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zb.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cq.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cb.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tg.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uq.haigaiapp.cn

—— 文件结束 ——
来源：http://ww.hnjuh.cn

================================================================================
来源：http://pm.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://uv.nicolike.cn

Common Programming Examples Cheat Book
来源：http://tk.nszjky.cn

================================================================================
来源：http://lu.panjiajie.cn

【收录内容】
来源：http://ei.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wk.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wl.huixiangedu.cn

SQL · Bash · C · C++
来源：http://rn.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nl.nicolike.cn

【使用说明】
来源：http://vw.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gi.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vh.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rj.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vc.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aj.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tu.huixinmuqiang.cn


<!-- 参考信息 -->