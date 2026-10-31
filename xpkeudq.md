代发 wailian999

[U03] Py：加载 .env 配置
来源：http://oz.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sq.521024.cn

[U04] Py：变量调试打印
来源：http://ui.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tb.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://vj.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://wy.hahajie.cn

[U06] Py：合并两个字典
来源：http://xh.szsharing.cn

{**a, **b}
来源：http://kp.9csxet.cn

[U07] Py：反转字典键值
来源：http://jv.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://iu.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://sj.newstarts.cn

[y for x in nested for y in x]
来源：http://ty.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://rm.szxytkj.cn

max(d, key=d.get)
来源：http://yh.newstarts.cn

[U10] Py：按值排序字典
来源：http://bt.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qo.shxzskj.cn

[U11] Py：生成器表达式
来源：http://qr.huixiangedu.cn

(x * 2 for x in arr)
来源：http://az.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xh.szxytkj.cn

Counter(arr).most_common(3)
来源：http://yx.huanxung.cn

[U13] Py：固定长度队列
来源：http://kn.jctech888.com.cn

deque(maxlen=10)
来源：http://sb.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://wb.hnjuh.cn

defaultdict(list)
来源：http://od.bjjhwx.cn

[U15] Py：高精度计时
来源：http://ka.huixiangedu.cn

t = time.perf_counter()
来源：http://zs.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://gp.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lz.szxytkj.cn

[U17] Py：初始化日志
来源：http://xy.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://fe.huanxung.cn

[U18] Py：预编译正则
来源：http://uj.521024.cn

pat = re.compile(r"\d+")
来源：http://km.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://nw.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://em.hahajie.cn

[U20] Py：缓存函数结果
来源：http://iq.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://yf.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://va.nicolike.cn

@contextlib.contextmanager
来源：http://qt.szxytkj.cn

[U22] Py：矩阵转置
来源：http://cc.bookmarksfly.cn

list(zip(*m))
来源：http://ff.nicolike.cn

[U23] Py：分块读取大文件
来源：http://bk.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dh.9csxet.cn

[U24] Py：路径操作
来源：http://pp.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hi.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://fr.jianghongdianzi.cn

csv.DictReader(f)
来源：http://tw.hahajie.cn

[U26] Py：并发下载
来源：http://qq.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hahajie.cn

[U27] Py：异步 HTTP
来源：http://vy.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://wj.shxzskj.cn

[U28] Py：类型别名
来源：http://oh.asd995.cn

UserId = int
来源：http://dq.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://zq.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ou.bjjhwx.cn

[U30] Py：数据类
来源：http://ms.shxzukj.cn

@dataclass(slots=True)
来源：http://hj.bjjhwx.cn

[U31] Py：单测
来源：http://pb.jctech888.com.cn

python -m pytest -q
来源：http://fh.lnxyls.cn

[U32] Py：代码格式化
来源：http://nu.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://oo.yuexingan06.cn

[U33] Py：打包发布
来源：http://wa.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://ek.huanxung.cn

[U34] Py：判断编码
来源：http://te.szxytkj.cn

chardet.detect(raw)
来源：http://ir.gzmigu.cn

[U35] Py：发送邮件
来源：http://sd.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lg.shxzukj.cn

[U36] Py：定时任务
来源：http://om.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://gk.hahajie.cn

[U37] Py：读写 Excel
来源：http://fq.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mz.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://tu.newstarts.cn

Path(__file__).resolve().parent
来源：http://cn.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://lb.colortex.cn

sys.stdout.isatty()
来源：http://bo.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://mw.9csxet.cn

print("err", file=sys.stderr)
来源：http://fd.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://fg.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://od.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ah.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vg.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ix.asd995.cn

namespace App\Http;
来源：http://xh.521024.cn

[U44] PHP：开启严格类型
来源：http://jk.muxihuayi.cn

declare(strict_types=1);
来源：http://gu.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://vm.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rf.chemitech.net.cn

[U46] PHP：可空类型
来源：http://uv.huanxung.cn

?string $name = null
来源：http://lp.lnxyls.cn

[U47] PHP：联合类型
来源：http://vy.9csxet.cn

int|string $id
来源：http://pf.521024.cn

[U48] PHP：纯枚举
来源：http://qe.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wn.yuexingan06.cn

[U49] PHP：只读属性
来源：http://uy.panjiajie.cn

public readonly string $name
来源：http://tw.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://wg.521024.cn

public function __construct(private int $id) {}
来源：http://ms.szsharing.cn

[U51] PHP：数组解构
来源：http://jz.9csxet.cn

[$a, $b] = $arr;
来源：http://rn.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://rk.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://mf.521024.cn

[U53] PHP：空合并运算符
来源：http://fi.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://jy.hahajie.cn

[U54] PHP：空安全调用
来源：http://lw.nicolike.cn

$obj?->method()
来源：http://xf.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://mh.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rn.asd995.cn

[U56] PHP：命名参数
来源：http://xl.shxzukj.cn

f(a: 1, b: 2)
来源：http://af.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ql.szxytkj.cn

"值: {$a}"
来源：http://pg.newstarts.cn

[U58] PHP：数组三件套
来源：http://gl.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xc.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://pe.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qg.521024.cn

[U60] PHP：JSON 编解码
来源：http://tt.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iq.jianghongdianzi.cn

[U61] PHP：正则
来源：http://fk.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://on.chemitech.net.cn

[U62] PHP：日期对象
来源：http://ce.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nb.hnjuh.cn

[U63] PHP：文件读写
来源：http://xf.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yb.huanxung.cn

[U64] PHP：目录遍历
来源：http://wn.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://sx.9csxet.cn

[U65] PHP：会话
来源：http://cw.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ty.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://jj.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dz.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://mi.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vn.colortex.cn

[U68] PHP：PDO 连接
来源：http://vv.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zs.colortex.cn

[U69] PHP：PDO 预处理
来源：http://xz.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tx.szsharing.cn

[U70] PHP：PDO 事务
来源：http://tl.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ox.szsharing.cn

[U71] PHP：抛出异常
来源：http://qa.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://ec.gzmigu.cn

[U72] PHP：写错误日志
来源：http://mu.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://zb.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://sp.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://fw.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://kx.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ku.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://cq.shxzukj.cn

composer require psr/container
来源：http://zj.panjiajie.cn

[U76] PHP：简单路由
来源：http://xa.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iu.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://oy.panjiajie.cn

composer require twig/twig
来源：http://kv.nicolike.cn

[U78] PHP：单元测试
来源：http://we.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://en.shxzukj.cn

[U79] PHP：静态分析
来源：http://wk.521024.cn

composer require --dev phpstan/phpstan
来源：http://ro.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://ud.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nr.chemitech.net.cn

[U81] JS：初始化项目
来源：http://pn.huixiangedu.cn

npm init -y;  npm i express
来源：http://li.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://pl.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tg.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://tv.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cr.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://qh.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://co.nicolike.cn

[U85] JS：可选链
来源：http://ih.newstarts.cn

a?.b?.c
来源：http://vu.hnjuh.cn

[U86] JS：空值合并
来源：http://wc.jianghongdianzi.cn

a ?? b
来源：http://as.wgjwhj.cn

[U87] JS：解构默认值
来源：http://ni.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://gw.hahajie.cn

[U88] JS：对象展开合并
来源：http://bt.szxytkj.cn

{ ...a, ...b }
来源：http://np.newstarts.cn

[U89] JS：数组去重
来源：http://ne.colortex.cn

[...new Set(arr)]
来源：http://iy.colortex.cn

[U90] JS：数字数组排序
来源：http://il.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://tf.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://jy.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ul.jctech888.com.cn

[U92] JS：深拷贝
来源：http://tw.wgjwhj.cn

structuredClone(obj)
来源：http://ae.shtwfgs.cn

[U93] JS：模板字符串
来源：http://qn.hahajie.cn

`共 ${n} 条`
来源：http://zx.hahajie.cn

[U94] JS：箭头函数
来源：http://oq.nicolike.cn

const double = x => x * 2;
来源：http://ta.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://tm.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://nm.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://hz.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://as.hnjuh.cn

[U97] JS：并发请求
来源：http://py.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rf.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://sr.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zw.huixiangedu.cn

[U99] JS：事件监听
来源：http://rx.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://kg.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://dn.muxihuayi.cn

document.querySelector(".item")
来源：http://sj.hahajie.cn

[U101] JS：classList 操作
来源：http://aj.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://mv.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://fi.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fq.muxihuayi.cn

[U103] JS：定时器
来源：http://ah.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rn.nicolike.cn

[U104] JS：防抖
来源：http://if.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://az.haigaiapp.cn

[U105] JS：节流
来源：http://sz.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mm.yuexingan06.cn

[U106] JS：日期格式化
来源：http://rp.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ul.521024.cn

[U107] JS：数字千分位
来源：http://md.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rx.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://mt.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vs.huanxung.cn

[U109] JS：数组分组
来源：http://vt.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://lw.gzmigu.cn

[U110] JS：数组分块
来源：http://vg.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tx.newstarts.cn

[U111] JS：对象转 Map
来源：http://lk.shxzskj.cn

new Map(Object.entries(obj))
来源：http://dj.muxihuayi.cn

[U112] JS：字符串补位
来源：http://xp.wgjwhj.cn

"7".padStart(3, "0")
来源：http://xs.gzmigu.cn

[U113] JS：正则替换全部
来源：http://ec.9csxet.cn

s.replaceAll("a", "b")
来源：http://uh.521024.cn

[U114] JS：JSON 深比较
来源：http://df.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://et.lnxyls.cn

[U115] JS：生成 UUID
来源：http://si.yuexingan06.cn

crypto.randomUUID()
来源：http://qo.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://ys.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://xq.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://td.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://bn.szxytkj.cn

[U118] JS：开发服务器
来源：http://zt.hahajie.cn

npm i -D vite;  npx vite
来源：http://gg.lnxyls.cn

[U119] JS：生产构建
来源：http://il.szxytkj.cn

npx vite build
来源：http://gg.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://nz.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://lf.nicolike.cn

================================================================================
来源：http://gu.newstarts.cn

统计汇总
来源：http://du.shxzukj.cn

================================================================================
来源：http://ki.chemitech.net.cn

按语言统计（条）：
来源：http://am.bjjhwx.cn

Python ......... 252
来源：http://gx.asd995.cn

PHP ............ 252
来源：http://zx.chemitech.net.cn

JavaScript ..... 252
来源：http://kl.hnjuh.cn

TypeScript ..... 212
来源：http://dc.huixiangedu.cn

Java ........... 212
来源：http://zj.shtwfgs.cn

Go ............. 212
来源：http://ej.bjjhwx.cn

Ruby ........... 212
来源：http://hp.nszjky.cn

C# ............. 212
来源：http://qo.haigaiapp.cn

C .............. 30
来源：http://zb.jianghongdianzi.cn

C++ ............ 30
来源：http://cp.bookmarksfly.cn

SQL ............ 90
来源：http://ck.shxzukj.cn

Bash ........... 80
来源：http://ng.gzmigu.cn

Kotlin ......... 15
来源：http://xq.nszjky.cn

Swift .......... 15
来源：http://ih.yuntaijiaju.cn

Lua ............ 10
来源：http://aw.9csxet.cn

Perl ........... 10
来源：http://it.huixiangedu.cn

Scala .......... 10
来源：http://mb.shxzukj.cn

------------------------------------
来源：http://hi.muxihuayi.cn

合计 ........... 2106 条
来源：http://rz.haigaiapp.cn

按章节统计：
来源：http://dd.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://im.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ie.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vv.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bl.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bo.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uk.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://be.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yw.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://va.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rc.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yb.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gb.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dc.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ps.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://te.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cq.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://ly.nicolike.cn

R Bash 专题                             80
来源：http://bx.shxzukj.cn

S C / C++ 专题                          60
来源：http://ol.hahajie.cn

T 其他语言补充                          60
来源：http://vo.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://hd.huixiangedu.cn

------------------------------------
来源：http://va.szxytkj.cn

合计                                  2106 条
来源：http://yv.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ef.huanxung.cn

使用提醒
来源：http://jt.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://rt.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ky.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tq.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hm.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wi.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cx.shxzskj.cn

—— 文件结束 ——
来源：http://rs.shtwfgs.cn

================================================================================
来源：http://bm.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://nt.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://ey.hahajie.cn

================================================================================
来源：http://bz.asd995.cn

【收录内容】
来源：http://qv.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ez.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bw.yuexingan06.cn

SQL · Bash · C · C++
来源：http://ae.shxzskj.cn


<!-- 参考信息 -->