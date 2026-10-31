代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://sy.hahajie.cn

[T55] Scala：集合过滤
来源：http://re.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gt.9csxet.cn

[T56] Scala：样例类
来源：http://ix.hahajie.cn

case class User(name: String, age: Int)
来源：http://wf.huanxung.cn

[T57] Scala：模式匹配
来源：http://td.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tr.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ri.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ma.huanxung.cn

[T59] Scala：循环
来源：http://io.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://pt.huanxung.cn

[T60] Scala：折叠
来源：http://yf.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://np.muxihuayi.cn

================================================================================
来源：http://xv.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sv.bookmarksfly.cn

================================================================================
来源：http://ge.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://is.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xw.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://lf.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sk.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://lk.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xn.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://ep.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ly.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://fg.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://qh.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://jy.jctech888.com.cn

{**a, **b}
来源：http://nj.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://wm.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://vj.hahajie.cn

[U08] Py：展平二维列表
来源：http://uh.szsharing.cn

[y for x in nested for y in x]
来源：http://qh.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://ef.nszjky.cn

max(d, key=d.get)
来源：http://yw.gzmigu.cn

[U10] Py：按值排序字典
来源：http://sa.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sr.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://wz.szsharing.cn

(x * 2 for x in arr)
来源：http://nv.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wc.521024.cn

Counter(arr).most_common(3)
来源：http://sf.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://hw.newstarts.cn

deque(maxlen=10)
来源：http://et.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://vm.521024.cn

defaultdict(list)
来源：http://ps.huixiangedu.cn

[U15] Py：高精度计时
来源：http://sk.bookmarksfly.cn

t = time.perf_counter()
来源：http://wn.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://gc.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wr.hnjuh.cn

[U17] Py：初始化日志
来源：http://rt.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://bb.bjjhwx.cn

[U18] Py：预编译正则
来源：http://yw.521024.cn

pat = re.compile(r"\d+")
来源：http://gf.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://zr.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://if.szsharing.cn

[U20] Py：缓存函数结果
来源：http://ge.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://zq.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://vq.nicolike.cn

@contextlib.contextmanager
来源：http://xd.hnjuh.cn

[U22] Py：矩阵转置
来源：http://fv.asd995.cn

list(zip(*m))
来源：http://mp.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://pe.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lb.newstarts.cn

[U24] Py：路径操作
来源：http://yb.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nu.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://px.haigaiapp.cn

csv.DictReader(f)
来源：http://iy.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://gr.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qf.hahajie.cn

[U27] Py：异步 HTTP
来源：http://aw.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://li.bjjhwx.cn

[U28] Py：类型别名
来源：http://pj.yuexingan06.cn

UserId = int
来源：http://in.shxzukj.cn

[U29] Py：属性校验
来源：http://op.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://gd.panjiajie.cn

[U30] Py：数据类
来源：http://ce.hahajie.cn

@dataclass(slots=True)
来源：http://ng.hnjuh.cn

[U31] Py：单测
来源：http://xx.yuexingan06.cn

python -m pytest -q
来源：http://pi.panjiajie.cn

[U32] Py：代码格式化
来源：http://tx.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://sv.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://zr.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://tv.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://tq.shtwfgs.cn

chardet.detect(raw)
来源：http://mr.wgjwhj.cn

[U35] Py：发送邮件
来源：http://jb.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qq.yuexingan06.cn

[U36] Py：定时任务
来源：http://jc.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://xf.9csxet.cn

[U37] Py：读写 Excel
来源：http://pf.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ed.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://cn.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://ar.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://jb.newstarts.cn

sys.stdout.isatty()
来源：http://ti.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://eo.szxytkj.cn

print("err", file=sys.stderr)
来源：http://yn.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://ln.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pk.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://fi.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rw.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://mi.hnjuh.cn

namespace App\Http;
来源：http://hq.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://kz.hahajie.cn

declare(strict_types=1);
来源：http://uy.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://iu.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://kl.asd995.cn

?string $name = null
来源：http://am.chemitech.net.cn

[U47] PHP：联合类型
来源：http://pj.bjjhwx.cn

int|string $id
来源：http://fw.shxzskj.cn

[U48] PHP：纯枚举
来源：http://xy.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hb.szsharing.cn

[U49] PHP：只读属性
来源：http://dd.jctech888.com.cn

public readonly string $name
来源：http://oa.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://jl.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://xa.hnjuh.cn

[U51] PHP：数组解构
来源：http://wq.jctech888.com.cn

[$a, $b] = $arr;
来源：http://qu.newstarts.cn

[U52] PHP：箭头函数
来源：http://cm.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://im.szsharing.cn

[U53] PHP：空合并运算符
来源：http://os.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://nx.shxzukj.cn

[U54] PHP：空安全调用
来源：http://yq.colortex.cn

$obj?->method()
来源：http://zf.521024.cn

[U55] PHP：match 表达式
来源：http://tz.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vt.nszjky.cn

[U56] PHP：命名参数
来源：http://dw.nszjky.cn

f(a: 1, b: 2)
来源：http://lx.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://il.asd995.cn

"值: {$a}"
来源：http://jx.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ou.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qv.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://cu.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sc.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://jy.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gz.nicolike.cn

[U61] PHP：正则
来源：http://gp.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pv.bjjhwx.cn

[U62] PHP：日期对象
来源：http://ui.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://og.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://jb.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lh.szsharing.cn

[U64] PHP：目录遍历
来源：http://dm.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://pz.asd995.cn

[U65] PHP：会话
来源：http://dt.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vk.521024.cn

[U66] PHP：设置 Cookie
来源：http://yl.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fj.nszjky.cn

[U67] PHP：处理文件上传
来源：http://pi.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ax.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://pw.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uf.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://dn.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fg.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://de.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rj.szsharing.cn

[U71] PHP：抛出异常
来源：http://wo.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://xi.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://gy.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://oq.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://xy.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://hf.521024.cn

[U74] PHP：读取环境变量
来源：http://rs.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://iy.shxzskj.cn

[U75] PHP：依赖注入
来源：http://vh.yuntaijiaju.cn

composer require psr/container
来源：http://xz.hahajie.cn

[U76] PHP：简单路由
来源：http://le.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://si.newstarts.cn

[U77] PHP：模板渲染
来源：http://eh.huixinmuqiang.cn

composer require twig/twig
来源：http://wp.hnjuh.cn

[U78] PHP：单元测试
来源：http://bl.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://fo.chemitech.net.cn

[U79] PHP：静态分析
来源：http://al.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://zr.szsharing.cn

[U80] PHP：代码规范修复
来源：http://zn.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bq.hahajie.cn

[U81] JS：初始化项目
来源：http://we.shxzukj.cn

npm init -y;  npm i express
来源：http://lk.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://oa.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kl.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://xa.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yu.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://ny.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ex.lnxyls.cn

[U85] JS：可选链
来源：http://kx.huixiangedu.cn

a?.b?.c
来源：http://yz.shtwfgs.cn

[U86] JS：空值合并
来源：http://gd.gzmigu.cn

a ?? b
来源：http://oy.yuexingan06.cn

[U87] JS：解构默认值
来源：http://sb.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://cg.szxytkj.cn

[U88] JS：对象展开合并
来源：http://xk.muxihuayi.cn

{ ...a, ...b }
来源：http://ut.chemitech.net.cn

[U89] JS：数组去重
来源：http://uz.shtwfgs.cn

[...new Set(arr)]
来源：http://sx.9csxet.cn

[U90] JS：数字数组排序
来源：http://dz.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://jl.nszjky.cn

[U91] JS：对象键值遍历
来源：http://op.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xl.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://jy.jctech888.com.cn

structuredClone(obj)
来源：http://hh.9csxet.cn

[U93] JS：模板字符串
来源：http://gy.lnxyls.cn

`共 ${n} 条`
来源：http://wa.asd995.cn

[U94] JS：箭头函数
来源：http://ig.shtwfgs.cn

const double = x => x * 2;
来源：http://ji.nszjky.cn

[U95] JS：Promise 包装
来源：http://dm.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://st.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ge.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://il.colortex.cn

[U97] JS：并发请求
来源：http://uo.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wh.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://sx.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gp.hahajie.cn

[U99] JS：事件监听
来源：http://co.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://oe.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://tr.huanxung.cn

document.querySelector(".item")
来源：http://dx.panjiajie.cn

[U101] JS：classList 操作
来源：http://lq.asd995.cn

el.classList.toggle("active")
来源：http://wv.bookmarksfly.cn

[U102] JS：本地存储
来源：http://yn.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qc.haigaiapp.cn

[U103] JS：定时器
来源：http://gu.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qn.521024.cn

[U104] JS：防抖
来源：http://qg.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.asd995.cn

[U105] JS：节流
来源：http://lx.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ck.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://jr.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lr.szxytkj.cn

[U107] JS：数字千分位
来源：http://vw.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dz.nszjky.cn

[U108] JS：随机整数
来源：http://sr.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fq.haigaiapp.cn

[U109] JS：数组分组
来源：http://nb.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://sf.bookmarksfly.cn

[U110] JS：数组分块
来源：http://jt.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gj.huanxung.cn

[U111] JS：对象转 Map
来源：http://wr.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://cz.colortex.cn

[U112] JS：字符串补位
来源：http://io.szsharing.cn

"7".padStart(3, "0")
来源：http://rh.nicolike.cn

[U113] JS：正则替换全部
来源：http://jh.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://px.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://wm.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ds.hnjuh.cn

[U115] JS：生成 UUID
来源：http://jm.jctech888.com.cn

crypto.randomUUID()
来源：http://uf.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://iv.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://gf.gzmigu.cn

[U117] JS：单元测试
来源：http://wz.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://xx.panjiajie.cn

[U118] JS：开发服务器
来源：http://pl.hnjuh.cn

npm i -D vite;  npx vite
来源：http://pb.521024.cn

[U119] JS：生产构建
来源：http://la.9csxet.cn

npx vite build
来源：http://ef.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://bj.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://ca.muxihuayi.cn

================================================================================
来源：http://lx.newstarts.cn

统计汇总
来源：http://cm.huanxung.cn

================================================================================
来源：http://un.huixiangedu.cn

按语言统计（条）：
来源：http://ai.newstarts.cn

Python ......... 252
来源：http://oo.asd995.cn

PHP ............ 252
来源：http://gy.asd995.cn

JavaScript ..... 252
来源：http://be.shtwfgs.cn

TypeScript ..... 212
来源：http://zs.nszjky.cn

Java ........... 212
来源：http://aj.muxihuayi.cn

Go ............. 212
来源：http://vt.huixinmuqiang.cn

Ruby ........... 212
来源：http://wi.yuexingan06.cn

C# ............. 212
来源：http://np.yuntaijiaju.cn

C .............. 30
来源：http://cu.huixiangedu.cn

C++ ............ 30
来源：http://rj.jctech888.com.cn

SQL ............ 90
来源：http://sb.szxytkj.cn

Bash ........... 80
来源：http://uk.muxihuayi.cn

Kotlin ......... 15
来源：http://ar.nszjky.cn

Swift .......... 15
来源：http://oa.shxzskj.cn

Lua ............ 10
来源：http://xq.yuntaijiaju.cn

Perl ........... 10
来源：http://el.nszjky.cn

Scala .......... 10
来源：http://ha.jianghongdianzi.cn

------------------------------------
来源：http://ph.bjjhwx.cn

合计 ........... 2106 条
来源：http://er.bookmarksfly.cn

按章节统计：
来源：http://mi.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ed.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hp.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yc.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nb.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://di.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ei.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dd.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rc.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cn.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yr.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wb.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kb.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jk.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zk.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ei.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yt.bookmarksfly.cn

Q SQL 专题                              90
来源：http://wk.huixiangedu.cn

R Bash 专题                             80
来源：http://ey.huanxung.cn

S C / C++ 专题                          60
来源：http://oy.asd995.cn

T 其他语言补充                          60
来源：http://ik.chemitech.net.cn


<!-- 参考信息 -->