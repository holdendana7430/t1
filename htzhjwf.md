代发 wailian999

[T49] Perl：函数
来源：http://ug.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://la.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://vr.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zd.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://fo.bjjhwx.cn

[T51] Scala：Hello World
来源：http://es.szxytkj.cn

println("Hello")
来源：http://aw.bjjhwx.cn

[T52] Scala：变量
来源：http://li.jctech888.com.cn

val a = 1;  var b = 2
来源：http://vy.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ky.newstarts.cn

s"值: $b"
来源：http://ua.shtwfgs.cn

[T54] Scala：集合映射
来源：http://au.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://vc.9csxet.cn

[T55] Scala：集合过滤
来源：http://zo.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://id.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://xx.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://yc.huanxung.cn

[T57] Scala：模式匹配
来源：http://zr.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ig.shtwfgs.cn

[T58] Scala：函数定义
来源：http://qm.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fq.muxihuayi.cn

[T59] Scala：循环
来源：http://gk.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://ha.jctech888.com.cn

[T60] Scala：折叠
来源：http://lz.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xc.huixiangedu.cn

================================================================================
来源：http://fm.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zr.shxzukj.cn

================================================================================
来源：http://ko.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://fn.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ja.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ss.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hx.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://ym.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://st.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://py.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eo.nicolike.cn

[U05] Py：列表去重且保序
来源：http://ew.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://kj.gzmigu.cn

[U06] Py：合并两个字典
来源：http://qx.521024.cn

{**a, **b}
来源：http://ed.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://ph.szsharing.cn

{v: k for k, v in d.items()}
来源：http://kl.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://gw.521024.cn

[y for x in nested for y in x]
来源：http://og.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://es.bookmarksfly.cn

max(d, key=d.get)
来源：http://bn.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://yt.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ca.shxzukj.cn

[U11] Py：生成器表达式
来源：http://hi.521024.cn

(x * 2 for x in arr)
来源：http://fz.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gp.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://hl.gzmigu.cn

[U13] Py：固定长度队列
来源：http://jb.jianghongdianzi.cn

deque(maxlen=10)
来源：http://jn.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://gh.yuntaijiaju.cn

defaultdict(list)
来源：http://tl.gzmigu.cn

[U15] Py：高精度计时
来源：http://hk.chemitech.net.cn

t = time.perf_counter()
来源：http://sr.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://ef.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pr.colortex.cn

[U17] Py：初始化日志
来源：http://zt.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://eh.panjiajie.cn

[U18] Py：预编译正则
来源：http://vi.nicolike.cn

pat = re.compile(r"\d+")
来源：http://jc.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ph.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vj.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://sd.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://zf.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ox.nicolike.cn

@contextlib.contextmanager
来源：http://up.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://gj.huixinmuqiang.cn

list(zip(*m))
来源：http://zt.nicolike.cn

[U23] Py：分块读取大文件
来源：http://og.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dk.yuexingan06.cn

[U24] Py：路径操作
来源：http://hx.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cb.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://zm.chemitech.net.cn

csv.DictReader(f)
来源：http://ey.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://eg.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zv.asd995.cn

[U27] Py：异步 HTTP
来源：http://ko.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://dd.szxytkj.cn

[U28] Py：类型别名
来源：http://tm.jctech888.com.cn

UserId = int
来源：http://hk.wgjwhj.cn

[U29] Py：属性校验
来源：http://jq.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://to.jctech888.com.cn

[U30] Py：数据类
来源：http://vi.nicolike.cn

@dataclass(slots=True)
来源：http://hz.yuexingan06.cn

[U31] Py：单测
来源：http://dd.hahajie.cn

python -m pytest -q
来源：http://as.nszjky.cn

[U32] Py：代码格式化
来源：http://fw.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://xl.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://ok.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://cd.muxihuayi.cn

[U34] Py：判断编码
来源：http://rn.hnjuh.cn

chardet.detect(raw)
来源：http://qd.521024.cn

[U35] Py：发送邮件
来源：http://av.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ql.hahajie.cn

[U36] Py：定时任务
来源：http://rn.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://na.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://zu.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qg.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://ed.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://xy.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://hq.wgjwhj.cn

sys.stdout.isatty()
来源：http://xs.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://qs.nicolike.cn

print("err", file=sys.stderr)
来源：http://pe.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://ts.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hh.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://ih.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lm.szsharing.cn

[U43] PHP：声明命名空间
来源：http://xh.colortex.cn

namespace App\Http;
来源：http://wx.huanxung.cn

[U44] PHP：开启严格类型
来源：http://zi.huixiangedu.cn

declare(strict_types=1);
来源：http://hh.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://ay.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.huanxung.cn

[U46] PHP：可空类型
来源：http://xt.muxihuayi.cn

?string $name = null
来源：http://uj.shxzukj.cn

[U47] PHP：联合类型
来源：http://cc.yuntaijiaju.cn

int|string $id
来源：http://am.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://fn.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tm.9csxet.cn

[U49] PHP：只读属性
来源：http://sk.shxzskj.cn

public readonly string $name
来源：http://sj.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://lw.asd995.cn

public function __construct(private int $id) {}
来源：http://io.huixiangedu.cn

[U51] PHP：数组解构
来源：http://pk.szxytkj.cn

[$a, $b] = $arr;
来源：http://od.9csxet.cn

[U52] PHP：箭头函数
来源：http://ih.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://gm.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://nw.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://vn.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://cg.huixinmuqiang.cn

$obj?->method()
来源：http://gw.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://nu.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kl.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://gv.jctech888.com.cn

f(a: 1, b: 2)
来源：http://ax.lnxyls.cn

[U57] PHP：字符串插值
来源：http://le.9csxet.cn

"值: {$a}"
来源：http://oi.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ta.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kp.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://sy.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sg.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://wc.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wt.bookmarksfly.cn

[U61] PHP：正则
来源：http://bs.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://da.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://mp.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oj.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://tu.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pd.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://fi.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://jy.521024.cn

[U65] PHP：会话
来源：http://va.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ws.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://pp.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ph.asd995.cn

[U67] PHP：处理文件上传
来源：http://uz.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wf.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://ta.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yx.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://qj.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yw.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://df.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wv.hnjuh.cn

[U71] PHP：抛出异常
来源：http://bq.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://ua.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://xz.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://ix.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://dc.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://kj.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://tb.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://fn.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://uj.newstarts.cn

composer require psr/container
来源：http://ma.shxzukj.cn

[U76] PHP：简单路由
来源：http://mm.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://te.asd995.cn

[U77] PHP：模板渲染
来源：http://kp.bookmarksfly.cn

composer require twig/twig
来源：http://dw.shxzskj.cn

[U78] PHP：单元测试
来源：http://ty.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://fa.haigaiapp.cn

[U79] PHP：静态分析
来源：http://zk.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://tu.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://qx.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://om.gzmigu.cn

[U81] JS：初始化项目
来源：http://jk.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://po.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://pb.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ke.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://mb.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://as.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://sp.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dx.jianghongdianzi.cn

[U85] JS：可选链
来源：http://ni.shxzukj.cn

a?.b?.c
来源：http://zb.hnjuh.cn

[U86] JS：空值合并
来源：http://rc.jianghongdianzi.cn

a ?? b
来源：http://op.yuexingan06.cn

[U87] JS：解构默认值
来源：http://fc.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://cs.gzmigu.cn

[U88] JS：对象展开合并
来源：http://cq.bjjhwx.cn

{ ...a, ...b }
来源：http://lo.shxzukj.cn

[U89] JS：数组去重
来源：http://sz.haigaiapp.cn

[...new Set(arr)]
来源：http://at.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://eo.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://hp.szsharing.cn

[U91] JS：对象键值遍历
来源：http://km.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jo.jctech888.com.cn

[U92] JS：深拷贝
来源：http://bc.newstarts.cn

structuredClone(obj)
来源：http://wf.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ex.bookmarksfly.cn

`共 ${n} 条`
来源：http://ep.huixiangedu.cn

[U94] JS：箭头函数
来源：http://qt.yuntaijiaju.cn

const double = x => x * 2;
来源：http://tj.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://gp.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://az.521024.cn

[U96] JS：async/await 与异常
来源：http://iw.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xi.asd995.cn

[U97] JS：并发请求
来源：http://fr.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vh.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ma.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nz.nszjky.cn

[U99] JS：事件监听
来源：http://ui.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://ki.nszjky.cn

[U100] JS：DOM 查询
来源：http://nq.huixinmuqiang.cn

document.querySelector(".item")
来源：http://fd.gzmigu.cn

[U101] JS：classList 操作
来源：http://wk.huanxung.cn

el.classList.toggle("active")
来源：http://on.shxzskj.cn

[U102] JS：本地存储
来源：http://ni.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cg.wgjwhj.cn

[U103] JS：定时器
来源：http://zy.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tg.gzmigu.cn

[U104] JS：防抖
来源：http://oy.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jf.hahajie.cn

[U105] JS：节流
来源：http://gb.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bj.jctech888.com.cn

[U106] JS：日期格式化
来源：http://wb.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fv.panjiajie.cn

[U107] JS：数字千分位
来源：http://yz.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rc.asd995.cn

[U108] JS：随机整数
来源：http://ob.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ya.shtwfgs.cn

[U109] JS：数组分组
来源：http://lf.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://xd.huixiangedu.cn

[U110] JS：数组分块
来源：http://wm.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nc.shxzskj.cn

[U111] JS：对象转 Map
来源：http://rg.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://ez.szxytkj.cn

[U112] JS：字符串补位
来源：http://to.lnxyls.cn

"7".padStart(3, "0")
来源：http://kv.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ae.newstarts.cn

s.replaceAll("a", "b")
来源：http://dy.9csxet.cn

[U114] JS：JSON 深比较
来源：http://hx.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pf.huanxung.cn

[U115] JS：生成 UUID
来源：http://uw.huanxung.cn

crypto.randomUUID()
来源：http://ix.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://rc.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://aj.shtwfgs.cn

[U117] JS：单元测试
来源：http://ga.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://zr.9csxet.cn

[U118] JS：开发服务器
来源：http://jx.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://wj.nicolike.cn

[U119] JS：生产构建
来源：http://vv.shxzskj.cn

npx vite build
来源：http://jk.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://ys.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://ma.gzmigu.cn

================================================================================
来源：http://wu.panjiajie.cn

统计汇总
来源：http://va.hahajie.cn

================================================================================
来源：http://sm.colortex.cn

按语言统计（条）：
来源：http://ah.hnjuh.cn

Python ......... 252
来源：http://wi.hahajie.cn

PHP ............ 252
来源：http://fv.yuexingan06.cn

JavaScript ..... 252
来源：http://nd.gzmigu.cn

TypeScript ..... 212
来源：http://zp.szxytkj.cn

Java ........... 212
来源：http://as.newstarts.cn

Go ............. 212
来源：http://xg.haigaiapp.cn

Ruby ........... 212
来源：http://qo.hahajie.cn

C# ............. 212
来源：http://sq.bjjhwx.cn

C .............. 30
来源：http://zo.shtwfgs.cn

C++ ............ 30
来源：http://xf.521024.cn

SQL ............ 90
来源：http://yl.haigaiapp.cn

Bash ........... 80
来源：http://tv.jianghongdianzi.cn

Kotlin ......... 15
来源：http://bq.chemitech.net.cn

Swift .......... 15
来源：http://gm.yuntaijiaju.cn

Lua ............ 10
来源：http://aw.panjiajie.cn

Perl ........... 10
来源：http://mw.muxihuayi.cn

Scala .......... 10
来源：http://qb.wgjwhj.cn

------------------------------------
来源：http://py.bookmarksfly.cn

合计 ........... 2106 条
来源：http://vd.yuntaijiaju.cn

按章节统计：
来源：http://ls.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cg.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xb.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vp.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vp.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lm.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jf.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://du.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://th.muxihuayi.cn


<!-- 参考信息 -->