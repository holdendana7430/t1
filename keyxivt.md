代发 wailian999

case class User(name: String, age: Int)
来源：http://sg.huanxung.cn

[T57] Scala：模式匹配
来源：http://kg.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fv.yuexingan06.cn

[T58] Scala：函数定义
来源：http://hu.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sj.521024.cn

[T59] Scala：循环
来源：http://le.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://up.panjiajie.cn

[T60] Scala：折叠
来源：http://mx.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mt.colortex.cn

================================================================================
来源：http://ds.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mi.panjiajie.cn

================================================================================
来源：http://ht.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://sw.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qc.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://sb.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gj.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://wv.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tr.nszjky.cn

[U04] Py：变量调试打印
来源：http://cb.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tc.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://nt.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://in.9csxet.cn

[U06] Py：合并两个字典
来源：http://uz.wgjwhj.cn

{**a, **b}
来源：http://tk.nicolike.cn

[U07] Py：反转字典键值
来源：http://uz.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://dw.9csxet.cn

[U08] Py：展平二维列表
来源：http://xx.huanxung.cn

[y for x in nested for y in x]
来源：http://ir.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://lc.shtwfgs.cn

max(d, key=d.get)
来源：http://xm.9csxet.cn

[U10] Py：按值排序字典
来源：http://jc.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gv.hnjuh.cn

[U11] Py：生成器表达式
来源：http://gg.szxytkj.cn

(x * 2 for x in arr)
来源：http://yz.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gi.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://zv.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://wz.panjiajie.cn

deque(maxlen=10)
来源：http://la.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://qb.gzmigu.cn

defaultdict(list)
来源：http://cz.haigaiapp.cn

[U15] Py：高精度计时
来源：http://aa.yuntaijiaju.cn

t = time.perf_counter()
来源：http://yr.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://bp.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://id.wgjwhj.cn

[U17] Py：初始化日志
来源：http://cj.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://pm.bjjhwx.cn

[U18] Py：预编译正则
来源：http://kh.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://vw.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://ax.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tf.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://bi.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://zl.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://rd.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://oz.nicolike.cn

[U22] Py：矩阵转置
来源：http://zu.hnjuh.cn

list(zip(*m))
来源：http://jj.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://vg.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lc.asd995.cn

[U24] Py：路径操作
来源：http://ut.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cw.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://pe.asd995.cn

csv.DictReader(f)
来源：http://zv.huixiangedu.cn

[U26] Py：并发下载
来源：http://ur.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ja.colortex.cn

[U27] Py：异步 HTTP
来源：http://mk.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://tg.haigaiapp.cn

[U28] Py：类型别名
来源：http://ds.hnjuh.cn

UserId = int
来源：http://fw.hnjuh.cn

[U29] Py：属性校验
来源：http://ov.panjiajie.cn

@property 与 @x.setter 配合
来源：http://if.hahajie.cn

[U30] Py：数据类
来源：http://ho.panjiajie.cn

@dataclass(slots=True)
来源：http://da.bookmarksfly.cn

[U31] Py：单测
来源：http://ux.gzmigu.cn

python -m pytest -q
来源：http://bg.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://dh.hahajie.cn

ruff format . && ruff check --fix .
来源：http://sc.hahajie.cn

[U33] Py：打包发布
来源：http://mq.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://aq.bjjhwx.cn

[U34] Py：判断编码
来源：http://vj.jctech888.com.cn

chardet.detect(raw)
来源：http://zz.szsharing.cn

[U35] Py：发送邮件
来源：http://bn.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ci.asd995.cn

[U36] Py：定时任务
来源：http://gp.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://wt.colortex.cn

[U37] Py：读写 Excel
来源：http://af.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://th.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://pf.szsharing.cn

Path(__file__).resolve().parent
来源：http://es.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://es.muxihuayi.cn

sys.stdout.isatty()
来源：http://ll.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ry.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://bl.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://tq.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ck.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://bf.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ek.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://qq.yuexingan06.cn

namespace App\Http;
来源：http://bp.nicolike.cn

[U44] PHP：开启严格类型
来源：http://bq.nszjky.cn

declare(strict_types=1);
来源：http://dk.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://ex.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nb.colortex.cn

[U46] PHP：可空类型
来源：http://yf.haigaiapp.cn

?string $name = null
来源：http://dq.shtwfgs.cn

[U47] PHP：联合类型
来源：http://nr.huanxung.cn

int|string $id
来源：http://na.lnxyls.cn

[U48] PHP：纯枚举
来源：http://rt.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://st.shxzskj.cn

[U49] PHP：只读属性
来源：http://do.yuexingan06.cn

public readonly string $name
来源：http://dp.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://ms.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://aj.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://qf.9csxet.cn

[$a, $b] = $arr;
来源：http://bj.newstarts.cn

[U52] PHP：箭头函数
来源：http://nz.asd995.cn

$double = fn($x) => $x * 2;
来源：http://mc.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://sr.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://je.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://zj.muxihuayi.cn

$obj?->method()
来源：http://cq.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://gt.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gz.9csxet.cn

[U56] PHP：命名参数
来源：http://ca.nicolike.cn

f(a: 1, b: 2)
来源：http://wc.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://ku.521024.cn

"值: {$a}"
来源：http://hw.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://mt.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vh.hahajie.cn

[U59] PHP：自定义排序
来源：http://tq.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ix.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://ro.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uy.gzmigu.cn

[U61] PHP：正则
来源：http://fy.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bb.lnxyls.cn

[U62] PHP：日期对象
来源：http://pc.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://it.bjjhwx.cn

[U63] PHP：文件读写
来源：http://ff.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://px.huanxung.cn

[U64] PHP：目录遍历
来源：http://cr.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://gg.jianghongdianzi.cn

[U65] PHP：会话
来源：http://cd.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://cq.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fa.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://zj.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kd.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://vk.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eo.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://pj.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vi.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://gg.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zt.hahajie.cn

[U71] PHP：抛出异常
来源：http://xw.521024.cn

throw new RuntimeException("失败", 500);
来源：http://xa.shxzskj.cn

[U72] PHP：写错误日志
来源：http://bw.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://if.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://wq.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://te.9csxet.cn

[U74] PHP：读取环境变量
来源：http://wn.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ge.asd995.cn

[U75] PHP：依赖注入
来源：http://pg.shxzukj.cn

composer require psr/container
来源：http://ma.yuexingan06.cn

[U76] PHP：简单路由
来源：http://af.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pz.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://yp.jianghongdianzi.cn

composer require twig/twig
来源：http://yz.nszjky.cn

[U78] PHP：单元测试
来源：http://kb.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://xn.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://dg.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://zq.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://qa.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gw.nszjky.cn

[U81] JS：初始化项目
来源：http://an.szxytkj.cn

npm init -y;  npm i express
来源：http://ad.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://sn.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vt.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://pv.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hp.asd995.cn

[U84] JS：CommonJS 写法
来源：http://jc.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://te.wgjwhj.cn

[U85] JS：可选链
来源：http://xc.gzmigu.cn

a?.b?.c
来源：http://rd.yuexingan06.cn

[U86] JS：空值合并
来源：http://pz.asd995.cn

a ?? b
来源：http://kg.szsharing.cn

[U87] JS：解构默认值
来源：http://cn.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://vu.asd995.cn

[U88] JS：对象展开合并
来源：http://gu.yuntaijiaju.cn

{ ...a, ...b }
来源：http://gz.asd995.cn

[U89] JS：数组去重
来源：http://kz.nicolike.cn

[...new Set(arr)]
来源：http://jr.szsharing.cn

[U90] JS：数字数组排序
来源：http://pg.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://kn.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://bu.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dj.lnxyls.cn

[U92] JS：深拷贝
来源：http://sw.521024.cn

structuredClone(obj)
来源：http://gh.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://iy.huixinmuqiang.cn

`共 ${n} 条`
来源：http://rq.shxzukj.cn

[U94] JS：箭头函数
来源：http://jt.yuntaijiaju.cn

const double = x => x * 2;
来源：http://ib.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://lg.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://oi.9csxet.cn

[U96] JS：async/await 与异常
来源：http://xi.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mp.wgjwhj.cn

[U97] JS：并发请求
来源：http://ot.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://an.521024.cn

[U98] JS：fetch 带 JSON
来源：http://rr.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zy.haigaiapp.cn

[U99] JS：事件监听
来源：http://px.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://hv.hahajie.cn

[U100] JS：DOM 查询
来源：http://je.huixiangedu.cn

document.querySelector(".item")
来源：http://kr.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://if.hahajie.cn

el.classList.toggle("active")
来源：http://xa.lnxyls.cn

[U102] JS：本地存储
来源：http://nx.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gv.huixiangedu.cn

[U103] JS：定时器
来源：http://ur.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hl.jianghongdianzi.cn

[U104] JS：防抖
来源：http://ln.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://db.panjiajie.cn

[U105] JS：节流
来源：http://oi.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rr.bjjhwx.cn

[U106] JS：日期格式化
来源：http://jg.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ga.panjiajie.cn

[U107] JS：数字千分位
来源：http://dl.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ad.newstarts.cn

[U108] JS：随机整数
来源：http://en.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wd.newstarts.cn

[U109] JS：数组分组
来源：http://fc.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://gv.asd995.cn

[U110] JS：数组分块
来源：http://qy.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ht.shxzukj.cn

[U111] JS：对象转 Map
来源：http://kn.shxzskj.cn

new Map(Object.entries(obj))
来源：http://pb.wgjwhj.cn

[U112] JS：字符串补位
来源：http://al.szsharing.cn

"7".padStart(3, "0")
来源：http://wo.szsharing.cn

[U113] JS：正则替换全部
来源：http://cx.521024.cn

s.replaceAll("a", "b")
来源：http://gl.huanxung.cn

[U114] JS：JSON 深比较
来源：http://hi.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sq.asd995.cn

[U115] JS：生成 UUID
来源：http://tn.nicolike.cn

crypto.randomUUID()
来源：http://ww.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://sv.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://jh.lnxyls.cn

[U117] JS：单元测试
来源：http://nz.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://zq.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://up.shxzskj.cn

npm i -D vite;  npx vite
来源：http://le.newstarts.cn

[U119] JS：生产构建
来源：http://ug.jctech888.com.cn

npx vite build
来源：http://ia.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://zc.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://vp.yuntaijiaju.cn

================================================================================
来源：http://bb.lnxyls.cn

统计汇总
来源：http://yf.521024.cn

================================================================================
来源：http://cu.muxihuayi.cn

按语言统计（条）：
来源：http://zl.colortex.cn

Python ......... 252
来源：http://qv.shtwfgs.cn

PHP ............ 252
来源：http://uk.9csxet.cn

JavaScript ..... 252
来源：http://ls.nicolike.cn

TypeScript ..... 212
来源：http://ig.shxzskj.cn

Java ........... 212
来源：http://hr.jianghongdianzi.cn

Go ............. 212
来源：http://uy.jctech888.com.cn

Ruby ........... 212
来源：http://ov.colortex.cn

C# ............. 212
来源：http://vs.shxzskj.cn

C .............. 30
来源：http://mp.panjiajie.cn

C++ ............ 30
来源：http://bb.colortex.cn

SQL ............ 90
来源：http://xo.huanxung.cn

Bash ........... 80
来源：http://ey.shxzukj.cn

Kotlin ......... 15
来源：http://xc.bjjhwx.cn

Swift .......... 15
来源：http://za.bookmarksfly.cn

Lua ............ 10
来源：http://fb.newstarts.cn

Perl ........... 10
来源：http://hn.521024.cn

Scala .......... 10
来源：http://yz.hnjuh.cn

------------------------------------
来源：http://nc.bookmarksfly.cn

合计 ........... 2106 条
来源：http://zy.colortex.cn

按章节统计：
来源：http://xp.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eb.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wo.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dk.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nh.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hd.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rm.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mw.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qp.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ad.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zq.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pj.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zg.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vn.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rm.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ik.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://im.hnjuh.cn

Q SQL 专题                              90
来源：http://wg.panjiajie.cn

R Bash 专题                             80
来源：http://vx.asd995.cn

S C / C++ 专题                          60
来源：http://fh.nszjky.cn

T 其他语言补充                          60
来源：http://zn.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://oc.bjjhwx.cn

------------------------------------
来源：http://ay.chemitech.net.cn

合计                                  2106 条
来源：http://qb.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://hd.newstarts.cn


<!-- 参考信息 -->