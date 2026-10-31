代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xm.muxihuayi.cn

================================================================================
来源：http://xx.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mf.gzmigu.cn

================================================================================
来源：http://bz.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://yv.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gi.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://pg.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zh.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://td.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hv.shxzukj.cn

[U04] Py：变量调试打印
来源：http://ur.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cf.9csxet.cn

[U05] Py：列表去重且保序
来源：http://at.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://st.colortex.cn

[U06] Py：合并两个字典
来源：http://se.huixinmuqiang.cn

{**a, **b}
来源：http://ux.shxzukj.cn

[U07] Py：反转字典键值
来源：http://ke.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://wx.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://hb.wgjwhj.cn

[y for x in nested for y in x]
来源：http://uy.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://wt.jianghongdianzi.cn

max(d, key=d.get)
来源：http://al.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://cg.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ay.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://fr.9csxet.cn

(x * 2 for x in arr)
来源：http://dy.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ey.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://iu.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://qe.shtwfgs.cn

deque(maxlen=10)
来源：http://jf.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://um.shxzskj.cn

defaultdict(list)
来源：http://yy.521024.cn

[U15] Py：高精度计时
来源：http://qk.521024.cn

t = time.perf_counter()
来源：http://fb.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://dp.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hd.nicolike.cn

[U17] Py：初始化日志
来源：http://ss.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://dk.huixiangedu.cn

[U18] Py：预编译正则
来源：http://fn.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ky.colortex.cn

[U19] Py：正则替换带回调
来源：http://ys.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gv.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://rr.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://wa.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://cd.nszjky.cn

@contextlib.contextmanager
来源：http://xh.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://hu.muxihuayi.cn

list(zip(*m))
来源：http://dj.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://zf.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rn.9csxet.cn

[U24] Py：路径操作
来源：http://eb.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gb.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://tj.jctech888.com.cn

csv.DictReader(f)
来源：http://sr.huixiangedu.cn

[U26] Py：并发下载
来源：http://xj.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://io.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://po.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://xr.gzmigu.cn

[U28] Py：类型别名
来源：http://de.hnjuh.cn

UserId = int
来源：http://ip.newstarts.cn

[U29] Py：属性校验
来源：http://ip.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://kg.9csxet.cn

[U30] Py：数据类
来源：http://zr.newstarts.cn

@dataclass(slots=True)
来源：http://au.szxytkj.cn

[U31] Py：单测
来源：http://ve.chemitech.net.cn

python -m pytest -q
来源：http://kv.haigaiapp.cn

[U32] Py：代码格式化
来源：http://ni.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://ij.521024.cn

[U33] Py：打包发布
来源：http://fx.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://fe.521024.cn

[U34] Py：判断编码
来源：http://ht.jianghongdianzi.cn

chardet.detect(raw)
来源：http://qm.huanxung.cn

[U35] Py：发送邮件
来源：http://vx.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gn.huanxung.cn

[U36] Py：定时任务
来源：http://oc.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://xs.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://ol.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bm.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://ya.lnxyls.cn

Path(__file__).resolve().parent
来源：http://jx.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://yh.huanxung.cn

sys.stdout.isatty()
来源：http://id.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://kt.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://ta.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://ys.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jp.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://hb.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://di.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://ds.hahajie.cn

namespace App\Http;
来源：http://cr.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://gf.nicolike.cn

declare(strict_types=1);
来源：http://bq.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://ze.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jj.chemitech.net.cn

[U46] PHP：可空类型
来源：http://jn.nicolike.cn

?string $name = null
来源：http://fr.jctech888.com.cn

[U47] PHP：联合类型
来源：http://di.bookmarksfly.cn

int|string $id
来源：http://ut.shxzukj.cn

[U48] PHP：纯枚举
来源：http://bh.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ng.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://rm.panjiajie.cn

public readonly string $name
来源：http://wc.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://dd.szsharing.cn

public function __construct(private int $id) {}
来源：http://og.muxihuayi.cn

[U51] PHP：数组解构
来源：http://nd.gzmigu.cn

[$a, $b] = $arr;
来源：http://tc.newstarts.cn

[U52] PHP：箭头函数
来源：http://tn.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://pi.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://on.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://te.521024.cn

[U54] PHP：空安全调用
来源：http://zo.jianghongdianzi.cn

$obj?->method()
来源：http://bw.shxzskj.cn

[U55] PHP：match 表达式
来源：http://vo.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pl.nszjky.cn

[U56] PHP：命名参数
来源：http://wx.nicolike.cn

f(a: 1, b: 2)
来源：http://tj.newstarts.cn

[U57] PHP：字符串插值
来源：http://hf.gzmigu.cn

"值: {$a}"
来源：http://vz.gzmigu.cn

[U58] PHP：数组三件套
来源：http://gd.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cl.521024.cn

[U59] PHP：自定义排序
来源：http://ii.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wm.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://iv.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yd.hnjuh.cn

[U61] PHP：正则
来源：http://vv.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rk.newstarts.cn

[U62] PHP：日期对象
来源：http://co.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://on.chemitech.net.cn

[U63] PHP：文件读写
来源：http://ig.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ma.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://sr.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://yg.shxzukj.cn

[U65] PHP：会话
来源：http://nb.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wd.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://ar.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dk.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://tf.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://su.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://fe.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fk.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://wz.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uw.9csxet.cn

[U70] PHP：PDO 事务
来源：http://eq.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hl.newstarts.cn

[U71] PHP：抛出异常
来源：http://ni.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://ng.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://jq.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://ee.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://cc.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://zp.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://oz.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://jb.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://kh.hnjuh.cn

composer require psr/container
来源：http://up.shxzukj.cn

[U76] PHP：简单路由
来源：http://oq.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zl.szxytkj.cn

[U77] PHP：模板渲染
来源：http://aa.bookmarksfly.cn

composer require twig/twig
来源：http://uw.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://pi.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://oh.haigaiapp.cn

[U79] PHP：静态分析
来源：http://dn.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://wt.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://no.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ng.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://sa.nicolike.cn

npm init -y;  npm i express
来源：http://lv.9csxet.cn

[U82] JS：package.json 脚本
来源：http://cp.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lk.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://pv.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://re.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://wb.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://va.chemitech.net.cn

[U85] JS：可选链
来源：http://ka.huixinmuqiang.cn

a?.b?.c
来源：http://cm.huanxung.cn

[U86] JS：空值合并
来源：http://bt.jianghongdianzi.cn

a ?? b
来源：http://tu.hahajie.cn

[U87] JS：解构默认值
来源：http://tw.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ue.hnjuh.cn

[U88] JS：对象展开合并
来源：http://aj.szsharing.cn

{ ...a, ...b }
来源：http://lh.jctech888.com.cn

[U89] JS：数组去重
来源：http://pd.szxytkj.cn

[...new Set(arr)]
来源：http://qx.shxzskj.cn

[U90] JS：数字数组排序
来源：http://fg.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://xt.hahajie.cn

[U91] JS：对象键值遍历
来源：http://lf.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vc.shxzukj.cn

[U92] JS：深拷贝
来源：http://xs.nszjky.cn

structuredClone(obj)
来源：http://cb.haigaiapp.cn

[U93] JS：模板字符串
来源：http://jd.yuntaijiaju.cn

`共 ${n} 条`
来源：http://sq.newstarts.cn

[U94] JS：箭头函数
来源：http://zc.hnjuh.cn

const double = x => x * 2;
来源：http://ku.521024.cn

[U95] JS：Promise 包装
来源：http://lb.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://pp.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://pc.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ib.hnjuh.cn

[U97] JS：并发请求
来源：http://av.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xu.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ok.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jz.shxzskj.cn

[U99] JS：事件监听
来源：http://fd.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://nf.521024.cn

[U100] JS：DOM 查询
来源：http://tq.chemitech.net.cn

document.querySelector(".item")
来源：http://ev.bjjhwx.cn

[U101] JS：classList 操作
来源：http://nb.yuexingan06.cn

el.classList.toggle("active")
来源：http://zc.bookmarksfly.cn

[U102] JS：本地存储
来源：http://on.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dx.lnxyls.cn

[U103] JS：定时器
来源：http://xm.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ka.jctech888.com.cn

[U104] JS：防抖
来源：http://ve.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kt.shtwfgs.cn

[U105] JS：节流
来源：http://cf.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://if.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://ya.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qv.szxytkj.cn

[U107] JS：数字千分位
来源：http://dx.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://md.yuexingan06.cn

[U108] JS：随机整数
来源：http://uf.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rm.newstarts.cn

[U109] JS：数组分组
来源：http://fi.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://rf.asd995.cn

[U110] JS：数组分块
来源：http://wx.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sh.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://tt.newstarts.cn

new Map(Object.entries(obj))
来源：http://ad.shxzukj.cn

[U112] JS：字符串补位
来源：http://vd.haigaiapp.cn

"7".padStart(3, "0")
来源：http://lg.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://mz.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://ic.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://em.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lo.9csxet.cn

[U115] JS：生成 UUID
来源：http://sr.hahajie.cn

crypto.randomUUID()
来源：http://vd.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://hf.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://jo.nszjky.cn

[U117] JS：单元测试
来源：http://hf.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://ny.muxihuayi.cn

[U118] JS：开发服务器
来源：http://qm.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://hp.shxzskj.cn

[U119] JS：生产构建
来源：http://in.yuntaijiaju.cn

npx vite build
来源：http://ai.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://ub.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://qy.shxzskj.cn

================================================================================
来源：http://eq.yuexingan06.cn

统计汇总
来源：http://vl.jianghongdianzi.cn

================================================================================
来源：http://vr.9csxet.cn

按语言统计（条）：
来源：http://lb.huixiangedu.cn

Python ......... 252
来源：http://ob.jctech888.com.cn

PHP ............ 252
来源：http://th.chemitech.net.cn

JavaScript ..... 252
来源：http://dl.yuntaijiaju.cn

TypeScript ..... 212
来源：http://sd.shxzskj.cn

Java ........... 212
来源：http://sd.jianghongdianzi.cn

Go ............. 212
来源：http://td.bookmarksfly.cn

Ruby ........... 212
来源：http://xx.yuexingan06.cn

C# ............. 212
来源：http://ha.bookmarksfly.cn

C .............. 30
来源：http://ev.bookmarksfly.cn

C++ ............ 30
来源：http://yf.szsharing.cn

SQL ............ 90
来源：http://me.huanxung.cn

Bash ........... 80
来源：http://ns.newstarts.cn

Kotlin ......... 15
来源：http://ai.jctech888.com.cn

Swift .......... 15
来源：http://hx.chemitech.net.cn

Lua ............ 10
来源：http://ru.szsharing.cn

Perl ........... 10
来源：http://sy.521024.cn

Scala .......... 10
来源：http://kd.asd995.cn

------------------------------------
来源：http://iy.lnxyls.cn

合计 ........... 2106 条
来源：http://kj.jianghongdianzi.cn

按章节统计：
来源：http://zy.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://md.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uu.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rd.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uv.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ap.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vc.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vm.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fl.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nc.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ij.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://js.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yr.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nv.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xc.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://od.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fh.colortex.cn

Q SQL 专题                              90
来源：http://od.9csxet.cn

R Bash 专题                             80
来源：http://gm.szsharing.cn

S C / C++ 专题                          60
来源：http://pt.shtwfgs.cn

T 其他语言补充                          60
来源：http://ot.hahajie.cn

U 高频实用片段                         120
来源：http://qa.hahajie.cn

------------------------------------
来源：http://hg.hahajie.cn

合计                                  2106 条
来源：http://lq.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://os.521024.cn

使用提醒
来源：http://mt.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ul.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yh.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qs.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nv.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wm.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ug.yuntaijiaju.cn

—— 文件结束 ——
来源：http://rt.huixiangedu.cn


<!-- 参考信息 -->