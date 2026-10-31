代发 wailian999

[T47] Perl：正则捕获
来源：http://ns.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://du.nszjky.cn

[T48] Perl：正则替换
来源：http://nw.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://ox.chemitech.net.cn

[T49] Perl：函数
来源：http://ha.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://od.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://nd.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yc.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://ny.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://nh.yuexingan06.cn

println("Hello")
来源：http://ca.hnjuh.cn

[T52] Scala：变量
来源：http://gk.hahajie.cn

val a = 1;  var b = 2
来源：http://uj.asd995.cn

[T53] Scala：字符串插值
来源：http://yd.newstarts.cn

s"值: $b"
来源：http://sb.szxytkj.cn

[T54] Scala：集合映射
来源：http://kz.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://wu.asd995.cn

[T55] Scala：集合过滤
来源：http://ja.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gc.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://mk.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://mg.nicolike.cn

[T57] Scala：模式匹配
来源：http://sl.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qx.chemitech.net.cn

[T58] Scala：函数定义
来源：http://xz.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gw.shtwfgs.cn

[T59] Scala：循环
来源：http://th.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://xr.shtwfgs.cn

[T60] Scala：折叠
来源：http://rk.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bx.nszjky.cn

================================================================================
来源：http://yw.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lv.yuexingan06.cn

================================================================================
来源：http://qe.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://hn.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xp.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://rc.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ff.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://gw.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gx.nszjky.cn

[U04] Py：变量调试打印
来源：http://is.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pb.nicolike.cn

[U05] Py：列表去重且保序
来源：http://un.hahajie.cn

list(dict.fromkeys(arr))
来源：http://ps.gzmigu.cn

[U06] Py：合并两个字典
来源：http://ek.jctech888.com.cn

{**a, **b}
来源：http://lr.hnjuh.cn

[U07] Py：反转字典键值
来源：http://fq.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://zy.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://cy.jctech888.com.cn

[y for x in nested for y in x]
来源：http://er.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://vy.huixinmuqiang.cn

max(d, key=d.get)
来源：http://nn.9csxet.cn

[U10] Py：按值排序字典
来源：http://ff.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jl.huanxung.cn

[U11] Py：生成器表达式
来源：http://dv.colortex.cn

(x * 2 for x in arr)
来源：http://oe.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://io.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://dg.hnjuh.cn

[U13] Py：固定长度队列
来源：http://bo.huixiangedu.cn

deque(maxlen=10)
来源：http://qy.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://uu.huixiangedu.cn

defaultdict(list)
来源：http://xs.shxzskj.cn

[U15] Py：高精度计时
来源：http://ql.szxytkj.cn

t = time.perf_counter()
来源：http://ut.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://lk.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://he.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://pa.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://xt.newstarts.cn

[U18] Py：预编译正则
来源：http://jk.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://km.nszjky.cn

[U19] Py：正则替换带回调
来源：http://pf.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ak.nszjky.cn

[U20] Py：缓存函数结果
来源：http://qc.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://jk.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://ag.newstarts.cn

@contextlib.contextmanager
来源：http://us.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://bx.bookmarksfly.cn

list(zip(*m))
来源：http://cw.huanxung.cn

[U23] Py：分块读取大文件
来源：http://eo.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oj.panjiajie.cn

[U24] Py：路径操作
来源：http://ty.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oj.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://fu.szxytkj.cn

csv.DictReader(f)
来源：http://lb.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://wh.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://am.521024.cn

[U27] Py：异步 HTTP
来源：http://oq.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://qz.521024.cn

[U28] Py：类型别名
来源：http://dv.chemitech.net.cn

UserId = int
来源：http://zw.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://yr.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://tt.muxihuayi.cn

[U30] Py：数据类
来源：http://la.asd995.cn

@dataclass(slots=True)
来源：http://wd.wgjwhj.cn

[U31] Py：单测
来源：http://kv.bookmarksfly.cn

python -m pytest -q
来源：http://sh.huanxung.cn

[U32] Py：代码格式化
来源：http://tr.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://hk.yuexingan06.cn

[U33] Py：打包发布
来源：http://zo.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://li.newstarts.cn

[U34] Py：判断编码
来源：http://hq.colortex.cn

chardet.detect(raw)
来源：http://kt.521024.cn

[U35] Py：发送邮件
来源：http://vd.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://di.jctech888.com.cn

[U36] Py：定时任务
来源：http://gw.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://fa.hnjuh.cn

[U37] Py：读写 Excel
来源：http://kc.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ar.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://pw.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://gd.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://mr.9csxet.cn

sys.stdout.isatty()
来源：http://rc.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://pj.nicolike.cn

print("err", file=sys.stderr)
来源：http://oo.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://rk.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://me.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://pf.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ds.asd995.cn

[U43] PHP：声明命名空间
来源：http://ip.gzmigu.cn

namespace App\Http;
来源：http://vf.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://sa.haigaiapp.cn

declare(strict_types=1);
来源：http://fc.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://uu.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rn.521024.cn

[U46] PHP：可空类型
来源：http://ws.shxzskj.cn

?string $name = null
来源：http://ua.hnjuh.cn

[U47] PHP：联合类型
来源：http://so.lnxyls.cn

int|string $id
来源：http://wx.gzmigu.cn

[U48] PHP：纯枚举
来源：http://fe.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rh.shxzskj.cn

[U49] PHP：只读属性
来源：http://ra.huixinmuqiang.cn

public readonly string $name
来源：http://jp.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://uj.panjiajie.cn

public function __construct(private int $id) {}
来源：http://bk.huixiangedu.cn

[U51] PHP：数组解构
来源：http://zs.shxzukj.cn

[$a, $b] = $arr;
来源：http://is.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://pr.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://cx.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://sx.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://vb.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://da.nszjky.cn

$obj?->method()
来源：http://nm.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://mg.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ue.chemitech.net.cn

[U56] PHP：命名参数
来源：http://qj.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://cu.nszjky.cn

[U57] PHP：字符串插值
来源：http://cm.521024.cn

"值: {$a}"
来源：http://qo.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ng.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://el.szxytkj.cn

[U59] PHP：自定义排序
来源：http://vc.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nd.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://jd.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oj.panjiajie.cn

[U61] PHP：正则
来源：http://um.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xh.huanxung.cn

[U62] PHP：日期对象
来源：http://kz.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cr.521024.cn

[U63] PHP：文件读写
来源：http://jq.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tj.szxytkj.cn

[U64] PHP：目录遍历
来源：http://go.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://bv.muxihuayi.cn

[U65] PHP：会话
来源：http://uz.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://of.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://lw.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hi.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://ve.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sm.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://cn.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qe.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://ck.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://md.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://rr.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gx.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://lr.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://lr.521024.cn

[U72] PHP：写错误日志
来源：http://jo.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://df.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://am.asd995.cn

parse_ini_file("config.ini", true)
来源：http://sb.521024.cn

[U74] PHP：读取环境变量
来源：http://xc.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://mc.nszjky.cn

[U75] PHP：依赖注入
来源：http://rl.hahajie.cn

composer require psr/container
来源：http://nf.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://xx.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ou.szxytkj.cn

[U77] PHP：模板渲染
来源：http://dg.jctech888.com.cn

composer require twig/twig
来源：http://di.lnxyls.cn

[U78] PHP：单元测试
来源：http://pb.colortex.cn

composer require --dev phpunit/phpunit
来源：http://pm.gzmigu.cn

[U79] PHP：静态分析
来源：http://nu.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://ep.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://aw.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sl.hahajie.cn

[U81] JS：初始化项目
来源：http://jf.szsharing.cn

npm init -y;  npm i express
来源：http://vh.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://sy.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gj.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://bh.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ca.colortex.cn

[U84] JS：CommonJS 写法
来源：http://vr.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xt.hahajie.cn

[U85] JS：可选链
来源：http://oy.lnxyls.cn

a?.b?.c
来源：http://zn.newstarts.cn

[U86] JS：空值合并
来源：http://yz.chemitech.net.cn

a ?? b
来源：http://bc.jctech888.com.cn

[U87] JS：解构默认值
来源：http://ov.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://dp.9csxet.cn

[U88] JS：对象展开合并
来源：http://en.haigaiapp.cn

{ ...a, ...b }
来源：http://bp.huixiangedu.cn

[U89] JS：数组去重
来源：http://ox.bookmarksfly.cn

[...new Set(arr)]
来源：http://my.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://ua.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://zo.huanxung.cn

[U91] JS：对象键值遍历
来源：http://hn.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://id.gzmigu.cn

[U92] JS：深拷贝
来源：http://mw.newstarts.cn

structuredClone(obj)
来源：http://ib.yuexingan06.cn

[U93] JS：模板字符串
来源：http://fz.hnjuh.cn

`共 ${n} 条`
来源：http://vi.gzmigu.cn

[U94] JS：箭头函数
来源：http://se.hnjuh.cn

const double = x => x * 2;
来源：http://lx.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://bb.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://fc.9csxet.cn

[U96] JS：async/await 与异常
来源：http://ge.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uq.9csxet.cn

[U97] JS：并发请求
来源：http://wi.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://wp.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ub.huanxung.cn

[U99] JS：事件监听
来源：http://pb.nicolike.cn

el.addEventListener("click", e => {})
来源：http://tf.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://wf.panjiajie.cn

document.querySelector(".item")
来源：http://wk.chemitech.net.cn

[U101] JS：classList 操作
来源：http://ru.colortex.cn

el.classList.toggle("active")
来源：http://nm.9csxet.cn

[U102] JS：本地存储
来源：http://qk.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sy.szxytkj.cn

[U103] JS：定时器
来源：http://et.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yt.szxytkj.cn

[U104] JS：防抖
来源：http://sq.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ie.szxytkj.cn

[U105] JS：节流
来源：http://bo.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fk.huixiangedu.cn

[U106] JS：日期格式化
来源：http://uv.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sd.9csxet.cn

[U107] JS：数字千分位
来源：http://md.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iy.colortex.cn

[U108] JS：随机整数
来源：http://kv.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rh.szxytkj.cn

[U109] JS：数组分组
来源：http://lg.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://so.521024.cn

[U110] JS：数组分块
来源：http://dr.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vc.hahajie.cn

[U111] JS：对象转 Map
来源：http://fd.colortex.cn

new Map(Object.entries(obj))
来源：http://mm.nicolike.cn

[U112] JS：字符串补位
来源：http://qx.huanxung.cn

"7".padStart(3, "0")
来源：http://xv.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://ib.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://lm.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://vi.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cf.gzmigu.cn

[U115] JS：生成 UUID
来源：http://vf.haigaiapp.cn

crypto.randomUUID()
来源：http://ng.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://sf.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://yl.panjiajie.cn

[U117] JS：单元测试
来源：http://zg.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://oz.shtwfgs.cn

[U118] JS：开发服务器
来源：http://in.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ab.shtwfgs.cn

[U119] JS：生产构建
来源：http://kh.nszjky.cn

npx vite build
来源：http://my.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://df.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://qo.muxihuayi.cn

================================================================================
来源：http://hv.bjjhwx.cn

统计汇总
来源：http://hv.haigaiapp.cn

================================================================================
来源：http://av.yuntaijiaju.cn

按语言统计（条）：
来源：http://hl.yuexingan06.cn

Python ......... 252
来源：http://pi.bookmarksfly.cn

PHP ............ 252
来源：http://fy.shxzukj.cn

JavaScript ..... 252
来源：http://co.bjjhwx.cn

TypeScript ..... 212
来源：http://fp.nszjky.cn

Java ........... 212
来源：http://on.panjiajie.cn

Go ............. 212
来源：http://be.shxzukj.cn

Ruby ........... 212
来源：http://vo.shtwfgs.cn

C# ............. 212
来源：http://jy.lnxyls.cn

C .............. 30
来源：http://ey.shtwfgs.cn

C++ ............ 30
来源：http://uj.hahajie.cn

SQL ............ 90
来源：http://py.shxzskj.cn

Bash ........... 80
来源：http://nm.haigaiapp.cn

Kotlin ......... 15
来源：http://si.521024.cn

Swift .......... 15
来源：http://rk.bjjhwx.cn

Lua ............ 10
来源：http://ve.asd995.cn

Perl ........... 10
来源：http://kt.hnjuh.cn

Scala .......... 10
来源：http://au.huanxung.cn

------------------------------------
来源：http://yd.nicolike.cn

合计 ........... 2106 条
来源：http://yl.shxzskj.cn

按章节统计：
来源：http://or.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sf.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uk.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ed.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ge.szxytkj.cn


<!-- 参考信息 -->