代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://ef.shxzskj.cn

[T59] Scala：循环
来源：http://ns.521024.cn

for (i <- 1 to 10) println(i)
来源：http://tk.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://fg.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sq.huanxung.cn

================================================================================
来源：http://xm.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jg.asd995.cn

================================================================================
来源：http://ay.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://dz.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eo.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://qh.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://te.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://ha.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uv.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://wu.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cn.huanxung.cn

[U05] Py：列表去重且保序
来源：http://ow.huanxung.cn

list(dict.fromkeys(arr))
来源：http://hf.hahajie.cn

[U06] Py：合并两个字典
来源：http://yw.haigaiapp.cn

{**a, **b}
来源：http://zw.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://yd.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://rd.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://nu.haigaiapp.cn

[y for x in nested for y in x]
来源：http://mu.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://uw.9csxet.cn

max(d, key=d.get)
来源：http://iz.hnjuh.cn

[U10] Py：按值排序字典
来源：http://mz.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lv.9csxet.cn

[U11] Py：生成器表达式
来源：http://nb.shtwfgs.cn

(x * 2 for x in arr)
来源：http://nf.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iy.lnxyls.cn

Counter(arr).most_common(3)
来源：http://cu.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://is.hahajie.cn

deque(maxlen=10)
来源：http://hm.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://dn.haigaiapp.cn

defaultdict(list)
来源：http://zu.nszjky.cn

[U15] Py：高精度计时
来源：http://pz.shxzskj.cn

t = time.perf_counter()
来源：http://wx.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://xb.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qi.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://st.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://rj.lnxyls.cn

[U18] Py：预编译正则
来源：http://vd.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ub.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://np.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pq.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://zl.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://fp.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://fc.szsharing.cn

@contextlib.contextmanager
来源：http://cw.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://te.newstarts.cn

list(zip(*m))
来源：http://lx.hahajie.cn

[U23] Py：分块读取大文件
来源：http://fv.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dr.haigaiapp.cn

[U24] Py：路径操作
来源：http://xc.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iu.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://oz.lnxyls.cn

csv.DictReader(f)
来源：http://xy.newstarts.cn

[U26] Py：并发下载
来源：http://qd.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vs.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://dk.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://sk.szxytkj.cn

[U28] Py：类型别名
来源：http://ka.huanxung.cn

UserId = int
来源：http://bg.huanxung.cn

[U29] Py：属性校验
来源：http://xe.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://bp.colortex.cn

[U30] Py：数据类
来源：http://lf.gzmigu.cn

@dataclass(slots=True)
来源：http://zj.lnxyls.cn

[U31] Py：单测
来源：http://rf.muxihuayi.cn

python -m pytest -q
来源：http://zt.panjiajie.cn

[U32] Py：代码格式化
来源：http://jg.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://ut.haigaiapp.cn

[U33] Py：打包发布
来源：http://sc.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://rn.huixiangedu.cn

[U34] Py：判断编码
来源：http://fu.chemitech.net.cn

chardet.detect(raw)
来源：http://aa.muxihuayi.cn

[U35] Py：发送邮件
来源：http://lv.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ex.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://rj.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://ki.huanxung.cn

[U37] Py：读写 Excel
来源：http://bf.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xo.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://pr.asd995.cn

Path(__file__).resolve().parent
来源：http://wj.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://si.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://ew.hahajie.cn

[U40] Py：打印到标准错误
来源：http://oc.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://lh.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://nu.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ny.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://ko.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rl.szsharing.cn

[U43] PHP：声明命名空间
来源：http://pw.newstarts.cn

namespace App\Http;
来源：http://lj.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://gi.huixiangedu.cn

declare(strict_types=1);
来源：http://dl.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://mt.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yj.521024.cn

[U46] PHP：可空类型
来源：http://xn.shxzskj.cn

?string $name = null
来源：http://vh.shtwfgs.cn

[U47] PHP：联合类型
来源：http://fe.hnjuh.cn

int|string $id
来源：http://ry.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://pn.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aa.newstarts.cn

[U49] PHP：只读属性
来源：http://uh.panjiajie.cn

public readonly string $name
来源：http://vz.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://pt.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://fl.huixiangedu.cn

[U51] PHP：数组解构
来源：http://st.newstarts.cn

[$a, $b] = $arr;
来源：http://je.hnjuh.cn

[U52] PHP：箭头函数
来源：http://yh.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://wz.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://op.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://fr.asd995.cn

[U54] PHP：空安全调用
来源：http://hy.huixinmuqiang.cn

$obj?->method()
来源：http://lo.szxytkj.cn

[U55] PHP：match 表达式
来源：http://xv.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qp.yuexingan06.cn

[U56] PHP：命名参数
来源：http://iq.shxzukj.cn

f(a: 1, b: 2)
来源：http://nc.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://ze.hnjuh.cn

"值: {$a}"
来源：http://uh.shxzskj.cn

[U58] PHP：数组三件套
来源：http://bf.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zr.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ow.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fy.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://zy.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sd.hahajie.cn

[U61] PHP：正则
来源：http://fb.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vf.bjjhwx.cn

[U62] PHP：日期对象
来源：http://cd.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yc.9csxet.cn

[U63] PHP：文件读写
来源：http://tp.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://va.asd995.cn

[U64] PHP：目录遍历
来源：http://yj.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://rw.bookmarksfly.cn

[U65] PHP：会话
来源：http://du.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yq.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://dg.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xl.asd995.cn

[U67] PHP：处理文件上传
来源：http://tr.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dc.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://hz.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jr.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://ic.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vd.huanxung.cn

[U70] PHP：PDO 事务
来源：http://mq.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ax.szsharing.cn

[U71] PHP：抛出异常
来源：http://ga.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ct.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://yc.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://nj.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://vk.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://nu.nicolike.cn

[U74] PHP：读取环境变量
来源：http://vu.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://wo.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://te.nszjky.cn

composer require psr/container
来源：http://ss.wgjwhj.cn

[U76] PHP：简单路由
来源：http://fd.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mb.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ht.lnxyls.cn

composer require twig/twig
来源：http://ir.gzmigu.cn

[U78] PHP：单元测试
来源：http://xk.asd995.cn

composer require --dev phpunit/phpunit
来源：http://ul.9csxet.cn

[U79] PHP：静态分析
来源：http://kx.asd995.cn

composer require --dev phpstan/phpstan
来源：http://mr.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://ae.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jq.huixiangedu.cn

[U81] JS：初始化项目
来源：http://ke.muxihuayi.cn

npm init -y;  npm i express
来源：http://pj.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://cd.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lf.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://kz.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bn.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://pp.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://se.shxzukj.cn

[U85] JS：可选链
来源：http://sg.bjjhwx.cn

a?.b?.c
来源：http://gn.huixiangedu.cn

[U86] JS：空值合并
来源：http://jk.chemitech.net.cn

a ?? b
来源：http://ya.gzmigu.cn

[U87] JS：解构默认值
来源：http://pi.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://dq.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://ra.newstarts.cn

{ ...a, ...b }
来源：http://ji.panjiajie.cn

[U89] JS：数组去重
来源：http://uu.colortex.cn

[...new Set(arr)]
来源：http://ih.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://ze.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://tu.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://wk.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://me.nszjky.cn

[U92] JS：深拷贝
来源：http://nf.jianghongdianzi.cn

structuredClone(obj)
来源：http://pf.wgjwhj.cn

[U93] JS：模板字符串
来源：http://kj.szxytkj.cn

`共 ${n} 条`
来源：http://eu.huanxung.cn

[U94] JS：箭头函数
来源：http://kc.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ir.nicolike.cn

[U95] JS：Promise 包装
来源：http://wi.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://ds.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://dr.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hp.asd995.cn

[U97] JS：并发请求
来源：http://fz.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://do.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://nm.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lz.shxzukj.cn

[U99] JS：事件监听
来源：http://zi.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://rx.nszjky.cn

[U100] JS：DOM 查询
来源：http://mw.asd995.cn

document.querySelector(".item")
来源：http://st.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://dd.bookmarksfly.cn

el.classList.toggle("active")
来源：http://ct.bjjhwx.cn

[U102] JS：本地存储
来源：http://sk.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hg.szxytkj.cn

[U103] JS：定时器
来源：http://tj.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://el.huixiangedu.cn

[U104] JS：防抖
来源：http://er.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uk.muxihuayi.cn

[U105] JS：节流
来源：http://pe.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lx.hnjuh.cn

[U106] JS：日期格式化
来源：http://jl.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xm.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://vg.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yq.nszjky.cn

[U108] JS：随机整数
来源：http://up.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ga.shtwfgs.cn

[U109] JS：数组分组
来源：http://ps.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://oc.shxzukj.cn

[U110] JS：数组分块
来源：http://do.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oy.szxytkj.cn

[U111] JS：对象转 Map
来源：http://rz.colortex.cn

new Map(Object.entries(obj))
来源：http://sy.shtwfgs.cn

[U112] JS：字符串补位
来源：http://cs.muxihuayi.cn

"7".padStart(3, "0")
来源：http://gm.panjiajie.cn

[U113] JS：正则替换全部
来源：http://tw.521024.cn

s.replaceAll("a", "b")
来源：http://qj.hahajie.cn

[U114] JS：JSON 深比较
来源：http://gx.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lx.lnxyls.cn

[U115] JS：生成 UUID
来源：http://cb.wgjwhj.cn

crypto.randomUUID()
来源：http://ke.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://he.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://nf.huixiangedu.cn

[U117] JS：单元测试
来源：http://eq.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://bm.chemitech.net.cn

[U118] JS：开发服务器
来源：http://sp.gzmigu.cn

npm i -D vite;  npx vite
来源：http://nb.panjiajie.cn

[U119] JS：生产构建
来源：http://jt.hahajie.cn

npx vite build
来源：http://gy.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://yg.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://bp.szsharing.cn

================================================================================
来源：http://vq.gzmigu.cn

统计汇总
来源：http://qp.huixiangedu.cn

================================================================================
来源：http://ne.nicolike.cn

按语言统计（条）：
来源：http://jk.huixiangedu.cn

Python ......... 252
来源：http://bm.huixinmuqiang.cn

PHP ............ 252
来源：http://mo.521024.cn

JavaScript ..... 252
来源：http://yx.shxzukj.cn

TypeScript ..... 212
来源：http://lk.wgjwhj.cn

Java ........... 212
来源：http://gj.colortex.cn

Go ............. 212
来源：http://mh.newstarts.cn

Ruby ........... 212
来源：http://xh.wgjwhj.cn

C# ............. 212
来源：http://jq.asd995.cn

C .............. 30
来源：http://ej.newstarts.cn

C++ ............ 30
来源：http://cg.nszjky.cn

SQL ............ 90
来源：http://rc.panjiajie.cn

Bash ........... 80
来源：http://jl.wgjwhj.cn

Kotlin ......... 15
来源：http://sp.colortex.cn

Swift .......... 15
来源：http://as.haigaiapp.cn

Lua ............ 10
来源：http://lw.shxzukj.cn

Perl ........... 10
来源：http://up.muxihuayi.cn

Scala .......... 10
来源：http://kr.haigaiapp.cn

------------------------------------
来源：http://wv.9csxet.cn

合计 ........... 2106 条
来源：http://wf.yuntaijiaju.cn

按章节统计：
来源：http://rh.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zl.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wc.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yt.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xw.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ow.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nb.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ys.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pc.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lg.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://he.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hj.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uy.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mm.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ie.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://al.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nw.521024.cn

Q SQL 专题                              90
来源：http://ut.yuexingan06.cn

R Bash 专题                             80
来源：http://xv.nszjky.cn

S C / C++ 专题                          60
来源：http://iz.lnxyls.cn

T 其他语言补充                          60
来源：http://tu.jctech888.com.cn

U 高频实用片段                         120
来源：http://gp.nicolike.cn

------------------------------------
来源：http://xq.lnxyls.cn

合计                                  2106 条
来源：http://sm.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ym.newstarts.cn

使用提醒
来源：http://hi.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://fm.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cf.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gf.yuntaijiaju.cn


<!-- 参考信息 -->