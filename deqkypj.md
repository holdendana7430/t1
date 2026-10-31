代发 wailian999

case class User(name: String, age: Int)
来源：http://ey.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://um.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uq.shxzskj.cn

[T58] Scala：函数定义
来源：http://rm.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sn.jianghongdianzi.cn

[T59] Scala：循环
来源：http://di.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://ns.shtwfgs.cn

[T60] Scala：折叠
来源：http://yc.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hf.hahajie.cn

================================================================================
来源：http://dm.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wu.huixinmuqiang.cn

================================================================================
来源：http://ab.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ha.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ky.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://sh.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qy.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://hf.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iu.9csxet.cn

[U04] Py：变量调试打印
来源：http://pw.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oo.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://vm.szsharing.cn

list(dict.fromkeys(arr))
来源：http://kj.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://he.nszjky.cn

{**a, **b}
来源：http://xt.gzmigu.cn

[U07] Py：反转字典键值
来源：http://vv.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://zv.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://qn.9csxet.cn

[y for x in nested for y in x]
来源：http://ci.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://if.nicolike.cn

max(d, key=d.get)
来源：http://ou.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://np.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uc.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://cv.shxzukj.cn

(x * 2 for x in arr)
来源：http://sx.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vg.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://hj.nszjky.cn

[U13] Py：固定长度队列
来源：http://us.nszjky.cn

deque(maxlen=10)
来源：http://kc.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ou.huixinmuqiang.cn

defaultdict(list)
来源：http://ax.shtwfgs.cn

[U15] Py：高精度计时
来源：http://sb.jctech888.com.cn

t = time.perf_counter()
来源：http://co.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ze.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ud.hahajie.cn

[U17] Py：初始化日志
来源：http://td.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://fz.asd995.cn

[U18] Py：预编译正则
来源：http://zg.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://we.nicolike.cn

[U19] Py：正则替换带回调
来源：http://kc.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zb.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://ab.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://tb.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://ju.hahajie.cn

@contextlib.contextmanager
来源：http://jp.newstarts.cn

[U22] Py：矩阵转置
来源：http://mg.chemitech.net.cn

list(zip(*m))
来源：http://ya.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://ai.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jo.jctech888.com.cn

[U24] Py：路径操作
来源：http://yb.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hj.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://kz.yuntaijiaju.cn

csv.DictReader(f)
来源：http://lu.nicolike.cn

[U26] Py：并发下载
来源：http://wv.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ao.hahajie.cn

[U27] Py：异步 HTTP
来源：http://me.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://ts.gzmigu.cn

[U28] Py：类型别名
来源：http://bk.yuntaijiaju.cn

UserId = int
来源：http://yi.hnjuh.cn

[U29] Py：属性校验
来源：http://uc.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://re.jctech888.com.cn

[U30] Py：数据类
来源：http://wj.huixiangedu.cn

@dataclass(slots=True)
来源：http://tk.gzmigu.cn

[U31] Py：单测
来源：http://wk.muxihuayi.cn

python -m pytest -q
来源：http://vm.jctech888.com.cn

[U32] Py：代码格式化
来源：http://fd.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://os.jctech888.com.cn

[U33] Py：打包发布
来源：http://rm.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://jv.wgjwhj.cn

[U34] Py：判断编码
来源：http://aw.szsharing.cn

chardet.detect(raw)
来源：http://xx.newstarts.cn

[U35] Py：发送邮件
来源：http://pb.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ol.lnxyls.cn

[U36] Py：定时任务
来源：http://lz.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://zg.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://ey.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dl.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://aa.szsharing.cn

Path(__file__).resolve().parent
来源：http://qh.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://im.huanxung.cn

sys.stdout.isatty()
来源：http://rv.szsharing.cn

[U40] Py：打印到标准错误
来源：http://po.shxzukj.cn

print("err", file=sys.stderr)
来源：http://yw.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://ra.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qp.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ao.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cl.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://so.shxzukj.cn

namespace App\Http;
来源：http://ab.szsharing.cn

[U44] PHP：开启严格类型
来源：http://cu.asd995.cn

declare(strict_types=1);
来源：http://jg.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://hp.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.huanxung.cn

[U46] PHP：可空类型
来源：http://sw.szxytkj.cn

?string $name = null
来源：http://al.huanxung.cn

[U47] PHP：联合类型
来源：http://kd.jianghongdianzi.cn

int|string $id
来源：http://xv.panjiajie.cn

[U48] PHP：纯枚举
来源：http://in.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ka.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://bp.chemitech.net.cn

public readonly string $name
来源：http://li.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://xf.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://vs.colortex.cn

[U51] PHP：数组解构
来源：http://um.nicolike.cn

[$a, $b] = $arr;
来源：http://bb.521024.cn

[U52] PHP：箭头函数
来源：http://lx.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ad.szsharing.cn

[U53] PHP：空合并运算符
来源：http://yi.521024.cn

$v = $a ?? $b ?? "default";
来源：http://ca.huanxung.cn

[U54] PHP：空安全调用
来源：http://ti.shtwfgs.cn

$obj?->method()
来源：http://kr.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://sk.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fo.panjiajie.cn

[U56] PHP：命名参数
来源：http://uy.shtwfgs.cn

f(a: 1, b: 2)
来源：http://rd.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://li.yuntaijiaju.cn

"值: {$a}"
来源：http://zr.9csxet.cn

[U58] PHP：数组三件套
来源：http://ph.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qc.newstarts.cn

[U59] PHP：自定义排序
来源：http://yy.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fb.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://pw.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yj.huixiangedu.cn

[U61] PHP：正则
来源：http://he.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zs.jctech888.com.cn

[U62] PHP：日期对象
来源：http://ou.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dm.shxzskj.cn

[U63] PHP：文件读写
来源：http://om.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gl.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ru.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://kq.huixinmuqiang.cn

[U65] PHP：会话
来源：http://fl.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://im.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://vq.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ip.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://di.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://of.szsharing.cn

[U68] PHP：PDO 连接
来源：http://kk.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nz.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://ps.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nd.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://zd.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nu.shxzukj.cn

[U71] PHP：抛出异常
来源：http://tc.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://kv.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://cu.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://mg.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://qg.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://uw.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://df.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://tl.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://xz.bookmarksfly.cn

composer require psr/container
来源：http://xi.yuexingan06.cn

[U76] PHP：简单路由
来源：http://uj.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://et.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://va.gzmigu.cn

composer require twig/twig
来源：http://mu.wgjwhj.cn

[U78] PHP：单元测试
来源：http://zv.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://jw.lnxyls.cn

[U79] PHP：静态分析
来源：http://to.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://vx.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://gg.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lv.haigaiapp.cn

[U81] JS：初始化项目
来源：http://hk.szxytkj.cn

npm init -y;  npm i express
来源：http://zy.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://ce.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rh.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://bx.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rz.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://lu.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jp.bjjhwx.cn

[U85] JS：可选链
来源：http://ih.panjiajie.cn

a?.b?.c
来源：http://ez.asd995.cn

[U86] JS：空值合并
来源：http://pa.shxzukj.cn

a ?? b
来源：http://hw.nicolike.cn

[U87] JS：解构默认值
来源：http://bz.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://kt.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://hb.521024.cn

{ ...a, ...b }
来源：http://fs.hahajie.cn

[U89] JS：数组去重
来源：http://gm.9csxet.cn

[...new Set(arr)]
来源：http://ms.hahajie.cn

[U90] JS：数字数组排序
来源：http://ee.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://eg.newstarts.cn

[U91] JS：对象键值遍历
来源：http://zj.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ls.chemitech.net.cn

[U92] JS：深拷贝
来源：http://wa.huanxung.cn

structuredClone(obj)
来源：http://gw.asd995.cn

[U93] JS：模板字符串
来源：http://qz.muxihuayi.cn

`共 ${n} 条`
来源：http://ro.colortex.cn

[U94] JS：箭头函数
来源：http://dw.jianghongdianzi.cn

const double = x => x * 2;
来源：http://sx.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://by.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://jc.huanxung.cn

[U96] JS：async/await 与异常
来源：http://js.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vf.panjiajie.cn

[U97] JS：并发请求
来源：http://vr.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ea.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://vu.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ef.yuexingan06.cn

[U99] JS：事件监听
来源：http://pt.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://po.9csxet.cn

[U100] JS：DOM 查询
来源：http://cw.colortex.cn

document.querySelector(".item")
来源：http://ej.nicolike.cn

[U101] JS：classList 操作
来源：http://wb.newstarts.cn

el.classList.toggle("active")
来源：http://mb.hahajie.cn

[U102] JS：本地存储
来源：http://ce.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kq.jctech888.com.cn

[U103] JS：定时器
来源：http://jj.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ur.bjjhwx.cn

[U104] JS：防抖
来源：http://yg.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ns.huixinmuqiang.cn

[U105] JS：节流
来源：http://zl.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qo.bjjhwx.cn

[U106] JS：日期格式化
来源：http://cn.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mq.shxzukj.cn

[U107] JS：数字千分位
来源：http://lx.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cx.szsharing.cn

[U108] JS：随机整数
来源：http://mr.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ww.hahajie.cn

[U109] JS：数组分组
来源：http://az.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://th.asd995.cn

[U110] JS：数组分块
来源：http://pi.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ym.9csxet.cn

[U111] JS：对象转 Map
来源：http://fy.nicolike.cn

new Map(Object.entries(obj))
来源：http://rj.huanxung.cn

[U112] JS：字符串补位
来源：http://kl.newstarts.cn

"7".padStart(3, "0")
来源：http://py.shxzskj.cn

[U113] JS：正则替换全部
来源：http://xl.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://dz.szsharing.cn

[U114] JS：JSON 深比较
来源：http://mw.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sn.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://jw.gzmigu.cn

crypto.randomUUID()
来源：http://oc.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://hx.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://mv.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://ij.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://co.gzmigu.cn

[U118] JS：开发服务器
来源：http://vq.colortex.cn

npm i -D vite;  npx vite
来源：http://rf.nszjky.cn

[U119] JS：生产构建
来源：http://cp.bookmarksfly.cn

npx vite build
来源：http://as.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://wa.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://yy.haigaiapp.cn

================================================================================
来源：http://uy.haigaiapp.cn

统计汇总
来源：http://tb.shtwfgs.cn

================================================================================
来源：http://fp.haigaiapp.cn

按语言统计（条）：
来源：http://sj.szsharing.cn

Python ......... 252
来源：http://ul.9csxet.cn

PHP ............ 252
来源：http://yy.colortex.cn

JavaScript ..... 252
来源：http://dw.bookmarksfly.cn

TypeScript ..... 212
来源：http://kz.yuexingan06.cn

Java ........... 212
来源：http://so.shxzukj.cn

Go ............. 212
来源：http://mq.huixiangedu.cn

Ruby ........... 212
来源：http://dn.hnjuh.cn

C# ............. 212
来源：http://ti.bjjhwx.cn

C .............. 30
来源：http://go.muxihuayi.cn

C++ ............ 30
来源：http://zc.haigaiapp.cn

SQL ............ 90
来源：http://nb.lnxyls.cn

Bash ........... 80
来源：http://hz.bookmarksfly.cn

Kotlin ......... 15
来源：http://rd.haigaiapp.cn

Swift .......... 15
来源：http://zs.9csxet.cn

Lua ............ 10
来源：http://hy.colortex.cn

Perl ........... 10
来源：http://cg.jianghongdianzi.cn

Scala .......... 10
来源：http://ni.shxzukj.cn

------------------------------------
来源：http://co.bookmarksfly.cn

合计 ........... 2106 条
来源：http://wb.wgjwhj.cn

按章节统计：
来源：http://xr.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cj.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sq.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://le.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gr.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vy.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cf.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ti.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yc.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sc.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qa.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://li.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://op.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://us.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vx.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xw.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xj.nszjky.cn

Q SQL 专题                              90
来源：http://ly.gzmigu.cn

R Bash 专题                             80
来源：http://np.shtwfgs.cn

S C / C++ 专题                          60
来源：http://my.asd995.cn

T 其他语言补充                          60
来源：http://qf.panjiajie.cn

U 高频实用片段                         120
来源：http://wp.nicolike.cn

------------------------------------
来源：http://ie.wgjwhj.cn

合计                                  2106 条
来源：http://ca.colortex.cn

--------------------------------------------------------------------------------
来源：http://yo.hnjuh.cn


<!-- 参考信息 -->