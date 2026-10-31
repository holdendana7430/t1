代发 wailian999

[U01] Py：创建虚拟环境
来源：http://jl.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uu.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ca.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gg.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://sc.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yu.colortex.cn

[U04] Py：变量调试打印
来源：http://as.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://td.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://br.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://gf.hnjuh.cn

[U06] Py：合并两个字典
来源：http://oc.9csxet.cn

{**a, **b}
来源：http://wa.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://hq.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://hf.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://jk.wgjwhj.cn

[y for x in nested for y in x]
来源：http://kl.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://sp.jctech888.com.cn

max(d, key=d.get)
来源：http://pa.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://az.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gx.shxzukj.cn

[U11] Py：生成器表达式
来源：http://iz.nicolike.cn

(x * 2 for x in arr)
来源：http://ky.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xa.szsharing.cn

Counter(arr).most_common(3)
来源：http://cq.hahajie.cn

[U13] Py：固定长度队列
来源：http://pn.wgjwhj.cn

deque(maxlen=10)
来源：http://np.521024.cn

[U14] Py：分组收集到列表
来源：http://ew.shxzskj.cn

defaultdict(list)
来源：http://to.szxytkj.cn

[U15] Py：高精度计时
来源：http://bi.muxihuayi.cn

t = time.perf_counter()
来源：http://tn.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://ry.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nm.shxzskj.cn

[U17] Py：初始化日志
来源：http://lz.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://mt.hahajie.cn

[U18] Py：预编译正则
来源：http://eh.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://gx.newstarts.cn

[U19] Py：正则替换带回调
来源：http://sb.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jb.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://oa.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://tz.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://ge.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://eu.hahajie.cn

[U22] Py：矩阵转置
来源：http://gw.chemitech.net.cn

list(zip(*m))
来源：http://xi.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://en.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zt.jctech888.com.cn

[U24] Py：路径操作
来源：http://lb.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wq.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://kn.szxytkj.cn

csv.DictReader(f)
来源：http://kz.nicolike.cn

[U26] Py：并发下载
来源：http://km.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mg.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://tc.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://wo.bookmarksfly.cn

[U28] Py：类型别名
来源：http://wv.yuntaijiaju.cn

UserId = int
来源：http://ds.szxytkj.cn

[U29] Py：属性校验
来源：http://tw.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://vr.szsharing.cn

[U30] Py：数据类
来源：http://bl.szxytkj.cn

@dataclass(slots=True)
来源：http://sr.shxzukj.cn

[U31] Py：单测
来源：http://yn.521024.cn

python -m pytest -q
来源：http://pf.hahajie.cn

[U32] Py：代码格式化
来源：http://hz.nicolike.cn

ruff format . && ruff check --fix .
来源：http://pu.521024.cn

[U33] Py：打包发布
来源：http://ms.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://hh.panjiajie.cn

[U34] Py：判断编码
来源：http://km.lnxyls.cn

chardet.detect(raw)
来源：http://dc.hnjuh.cn

[U35] Py：发送邮件
来源：http://xw.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nz.lnxyls.cn

[U36] Py：定时任务
来源：http://cg.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://gg.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://xu.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gi.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://qo.hahajie.cn

Path(__file__).resolve().parent
来源：http://eq.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://ow.huanxung.cn

sys.stdout.isatty()
来源：http://af.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://hl.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://xi.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://ir.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qp.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://ti.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fm.colortex.cn

[U43] PHP：声明命名空间
来源：http://sp.huixiangedu.cn

namespace App\Http;
来源：http://kh.9csxet.cn

[U44] PHP：开启严格类型
来源：http://kv.shxzukj.cn

declare(strict_types=1);
来源：http://gx.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://aw.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ai.shtwfgs.cn

[U46] PHP：可空类型
来源：http://xm.chemitech.net.cn

?string $name = null
来源：http://dn.huanxung.cn

[U47] PHP：联合类型
来源：http://tu.yuexingan06.cn

int|string $id
来源：http://on.colortex.cn

[U48] PHP：纯枚举
来源：http://ik.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ux.shtwfgs.cn

[U49] PHP：只读属性
来源：http://wb.asd995.cn

public readonly string $name
来源：http://hx.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://gg.521024.cn

public function __construct(private int $id) {}
来源：http://hc.hnjuh.cn

[U51] PHP：数组解构
来源：http://ef.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ij.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://gv.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://de.521024.cn

[U53] PHP：空合并运算符
来源：http://iv.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://rk.szxytkj.cn

[U54] PHP：空安全调用
来源：http://ai.gzmigu.cn

$obj?->method()
来源：http://sd.shxzskj.cn

[U55] PHP：match 表达式
来源：http://ry.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wd.nicolike.cn

[U56] PHP：命名参数
来源：http://dg.nicolike.cn

f(a: 1, b: 2)
来源：http://hk.hnjuh.cn

[U57] PHP：字符串插值
来源：http://pe.muxihuayi.cn

"值: {$a}"
来源：http://rd.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://bq.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hn.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://kr.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://al.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://jg.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lc.nszjky.cn

[U61] PHP：正则
来源：http://qg.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zz.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ih.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mp.huixiangedu.cn

[U63] PHP：文件读写
来源：http://xb.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gw.lnxyls.cn

[U64] PHP：目录遍历
来源：http://cm.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://sg.9csxet.cn

[U65] PHP：会话
来源：http://rk.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://je.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://ov.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fk.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://gc.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pi.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://lm.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ws.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://bv.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qh.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://vn.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mg.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://jx.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://cq.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://zx.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://na.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://gg.colortex.cn

parse_ini_file("config.ini", true)
来源：http://qw.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://dt.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://nv.9csxet.cn

[U75] PHP：依赖注入
来源：http://gw.nicolike.cn

composer require psr/container
来源：http://gf.haigaiapp.cn

[U76] PHP：简单路由
来源：http://pl.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tn.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://za.shxzukj.cn

composer require twig/twig
来源：http://jf.muxihuayi.cn

[U78] PHP：单元测试
来源：http://xp.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://sf.newstarts.cn

[U79] PHP：静态分析
来源：http://ij.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://pl.newstarts.cn

[U80] PHP：代码规范修复
来源：http://qz.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ai.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ov.bjjhwx.cn

npm init -y;  npm i express
来源：http://qw.asd995.cn

[U82] JS：package.json 脚本
来源：http://gl.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ny.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://rl.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jz.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://cq.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wp.bookmarksfly.cn

[U85] JS：可选链
来源：http://gh.szsharing.cn

a?.b?.c
来源：http://xz.huanxung.cn

[U86] JS：空值合并
来源：http://la.muxihuayi.cn

a ?? b
来源：http://cq.shxzskj.cn

[U87] JS：解构默认值
来源：http://uq.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://xl.gzmigu.cn

[U88] JS：对象展开合并
来源：http://gj.szxytkj.cn

{ ...a, ...b }
来源：http://sl.shtwfgs.cn

[U89] JS：数组去重
来源：http://dc.521024.cn

[...new Set(arr)]
来源：http://fm.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://sn.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://hq.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://ul.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://re.huixiangedu.cn

[U92] JS：深拷贝
来源：http://wi.hnjuh.cn

structuredClone(obj)
来源：http://vc.huanxung.cn

[U93] JS：模板字符串
来源：http://pq.lnxyls.cn

`共 ${n} 条`
来源：http://qc.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://pi.hahajie.cn

const double = x => x * 2;
来源：http://ak.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://el.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://tv.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://am.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wk.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://px.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ij.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ro.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zp.hnjuh.cn

[U99] JS：事件监听
来源：http://dg.colortex.cn

el.addEventListener("click", e => {})
来源：http://qu.szxytkj.cn

[U100] JS：DOM 查询
来源：http://ee.nszjky.cn

document.querySelector(".item")
来源：http://wo.hahajie.cn

[U101] JS：classList 操作
来源：http://ob.yuexingan06.cn

el.classList.toggle("active")
来源：http://wg.chemitech.net.cn

[U102] JS：本地存储
来源：http://px.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tr.haigaiapp.cn

[U103] JS：定时器
来源：http://qt.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://me.nicolike.cn

[U104] JS：防抖
来源：http://vp.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kr.bookmarksfly.cn

[U105] JS：节流
来源：http://ja.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lz.shxzskj.cn

[U106] JS：日期格式化
来源：http://kf.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ki.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://ki.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qj.jctech888.com.cn

[U108] JS：随机整数
来源：http://xm.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vq.shxzukj.cn

[U109] JS：数组分组
来源：http://vn.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://iz.hnjuh.cn

[U110] JS：数组分块
来源：http://wi.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://km.lnxyls.cn

[U111] JS：对象转 Map
来源：http://wh.colortex.cn

new Map(Object.entries(obj))
来源：http://tn.panjiajie.cn

[U112] JS：字符串补位
来源：http://iu.521024.cn

"7".padStart(3, "0")
来源：http://gk.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://iq.9csxet.cn

s.replaceAll("a", "b")
来源：http://wf.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://np.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://on.szsharing.cn

[U115] JS：生成 UUID
来源：http://cj.shxzukj.cn

crypto.randomUUID()
来源：http://oz.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://yk.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://bp.lnxyls.cn

[U117] JS：单元测试
来源：http://yl.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://lh.yuexingan06.cn

[U118] JS：开发服务器
来源：http://xq.asd995.cn

npm i -D vite;  npx vite
来源：http://tx.9csxet.cn

[U119] JS：生产构建
来源：http://dn.bjjhwx.cn

npx vite build
来源：http://vz.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://lo.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://lw.shtwfgs.cn

================================================================================
来源：http://vd.haigaiapp.cn

统计汇总
来源：http://tj.huanxung.cn

================================================================================
来源：http://ny.gzmigu.cn

按语言统计（条）：
来源：http://en.shxzukj.cn

Python ......... 252
来源：http://ho.haigaiapp.cn

PHP ............ 252
来源：http://sz.chemitech.net.cn

JavaScript ..... 252
来源：http://yx.huixinmuqiang.cn

TypeScript ..... 212
来源：http://yq.hahajie.cn

Java ........... 212
来源：http://wu.chemitech.net.cn

Go ............. 212
来源：http://nm.panjiajie.cn

Ruby ........... 212
来源：http://em.jianghongdianzi.cn

C# ............. 212
来源：http://lk.chemitech.net.cn

C .............. 30
来源：http://ts.nszjky.cn

C++ ............ 30
来源：http://lh.huixinmuqiang.cn

SQL ............ 90
来源：http://rz.jianghongdianzi.cn

Bash ........... 80
来源：http://ga.jctech888.com.cn

Kotlin ......... 15
来源：http://ni.shxzskj.cn

Swift .......... 15
来源：http://ep.nszjky.cn

Lua ............ 10
来源：http://zi.asd995.cn

Perl ........... 10
来源：http://ah.newstarts.cn

Scala .......... 10
来源：http://qu.nszjky.cn

------------------------------------
来源：http://pr.yuexingan06.cn

合计 ........... 2106 条
来源：http://mi.huanxung.cn

按章节统计：
来源：http://ne.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fr.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pg.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tw.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uq.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://on.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wi.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xr.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xk.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jg.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ix.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nd.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cw.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lk.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ih.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mm.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hn.shxzukj.cn

Q SQL 专题                              90
来源：http://fr.wgjwhj.cn

R Bash 专题                             80
来源：http://ye.wgjwhj.cn

S C / C++ 专题                          60
来源：http://qn.hnjuh.cn

T 其他语言补充                          60
来源：http://wb.521024.cn

U 高频实用片段                         120
来源：http://vg.nicolike.cn

------------------------------------
来源：http://et.hnjuh.cn

合计                                  2106 条
来源：http://sx.hahajie.cn

--------------------------------------------------------------------------------
来源：http://uw.colortex.cn

使用提醒
来源：http://in.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://rd.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pl.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nf.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pm.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gr.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jr.huixiangedu.cn

—— 文件结束 ——
来源：http://ss.huanxung.cn

================================================================================
来源：http://lm.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://uy.asd995.cn

Common Programming Examples Cheat Book
来源：http://ep.shtwfgs.cn

================================================================================
来源：http://yt.gzmigu.cn


<!-- 参考信息 -->