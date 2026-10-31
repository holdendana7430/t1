代发 wailian999

[T45] Perl：数组遍历
来源：http://fu.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://yb.hahajie.cn

[T46] Perl：哈希操作
来源：http://il.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cr.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://rt.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hh.nszjky.cn

[T48] Perl：正则替换
来源：http://bf.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://rc.szxytkj.cn

[T49] Perl：函数
来源：http://bv.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uw.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://cf.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lx.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://us.jctech888.com.cn

[T51] Scala：Hello World
来源：http://st.jianghongdianzi.cn

println("Hello")
来源：http://so.shtwfgs.cn

[T52] Scala：变量
来源：http://df.nszjky.cn

val a = 1;  var b = 2
来源：http://qq.szxytkj.cn

[T53] Scala：字符串插值
来源：http://gr.asd995.cn

s"值: $b"
来源：http://kx.huanxung.cn

[T54] Scala：集合映射
来源：http://mw.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://kq.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://mr.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rp.hnjuh.cn

[T56] Scala：样例类
来源：http://wb.nicolike.cn

case class User(name: String, age: Int)
来源：http://ud.hahajie.cn

[T57] Scala：模式匹配
来源：http://rv.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ch.muxihuayi.cn

[T58] Scala：函数定义
来源：http://je.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rm.shtwfgs.cn

[T59] Scala：循环
来源：http://fk.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://nr.yuexingan06.cn

[T60] Scala：折叠
来源：http://ax.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zl.colortex.cn

================================================================================
来源：http://ay.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ec.huixinmuqiang.cn

================================================================================
来源：http://kc.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://ys.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://km.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://lw.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rb.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://hh.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wn.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://ob.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nu.nszjky.cn

[U05] Py：列表去重且保序
来源：http://sc.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://zs.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://ls.szxytkj.cn

{**a, **b}
来源：http://gk.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://ob.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://kh.lnxyls.cn

[U08] Py：展平二维列表
来源：http://uy.hahajie.cn

[y for x in nested for y in x]
来源：http://yw.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://wu.bjjhwx.cn

max(d, key=d.get)
来源：http://po.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://vp.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uy.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://ub.yuexingan06.cn

(x * 2 for x in arr)
来源：http://zn.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://va.lnxyls.cn

Counter(arr).most_common(3)
来源：http://jl.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://oc.huanxung.cn

deque(maxlen=10)
来源：http://wp.newstarts.cn

[U14] Py：分组收集到列表
来源：http://vz.szsharing.cn

defaultdict(list)
来源：http://no.huanxung.cn

[U15] Py：高精度计时
来源：http://xd.muxihuayi.cn

t = time.perf_counter()
来源：http://vn.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://ao.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lu.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://ue.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://rj.szsharing.cn

[U18] Py：预编译正则
来源：http://fp.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://qq.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://ez.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://on.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://wk.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://ys.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://oa.jctech888.com.cn

@contextlib.contextmanager
来源：http://cf.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://fn.muxihuayi.cn

list(zip(*m))
来源：http://he.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://bv.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fa.shtwfgs.cn

[U24] Py：路径操作
来源：http://bu.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://od.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://hk.hnjuh.cn

csv.DictReader(f)
来源：http://tu.huixiangedu.cn

[U26] Py：并发下载
来源：http://op.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mq.newstarts.cn

[U27] Py：异步 HTTP
来源：http://av.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://mp.hahajie.cn

[U28] Py：类型别名
来源：http://on.jianghongdianzi.cn

UserId = int
来源：http://wn.newstarts.cn

[U29] Py：属性校验
来源：http://ql.shxzukj.cn

@property 与 @x.setter 配合
来源：http://zd.panjiajie.cn

[U30] Py：数据类
来源：http://mo.521024.cn

@dataclass(slots=True)
来源：http://ay.nicolike.cn

[U31] Py：单测
来源：http://wa.chemitech.net.cn

python -m pytest -q
来源：http://ti.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://uy.szsharing.cn

ruff format . && ruff check --fix .
来源：http://wu.9csxet.cn

[U33] Py：打包发布
来源：http://os.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://rh.colortex.cn

[U34] Py：判断编码
来源：http://nm.lnxyls.cn

chardet.detect(raw)
来源：http://pn.nszjky.cn

[U35] Py：发送邮件
来源：http://uc.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bg.newstarts.cn

[U36] Py：定时任务
来源：http://da.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://ui.lnxyls.cn

[U37] Py：读写 Excel
来源：http://tm.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://na.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://pe.shxzukj.cn

Path(__file__).resolve().parent
来源：http://um.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://de.lnxyls.cn

sys.stdout.isatty()
来源：http://lb.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://hk.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://kg.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://sv.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://su.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://ay.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yt.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://fr.lnxyls.cn

namespace App\Http;
来源：http://nm.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://cc.newstarts.cn

declare(strict_types=1);
来源：http://ez.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://xu.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ni.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://cx.jianghongdianzi.cn

?string $name = null
来源：http://mt.asd995.cn

[U47] PHP：联合类型
来源：http://ec.shtwfgs.cn

int|string $id
来源：http://wl.hahajie.cn

[U48] PHP：纯枚举
来源：http://ch.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wq.wgjwhj.cn

[U49] PHP：只读属性
来源：http://qx.jctech888.com.cn

public readonly string $name
来源：http://jn.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://wk.hnjuh.cn

public function __construct(private int $id) {}
来源：http://li.shtwfgs.cn

[U51] PHP：数组解构
来源：http://yo.hnjuh.cn

[$a, $b] = $arr;
来源：http://ro.szxytkj.cn

[U52] PHP：箭头函数
来源：http://od.521024.cn

$double = fn($x) => $x * 2;
来源：http://hm.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://gb.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://vf.colortex.cn

[U54] PHP：空安全调用
来源：http://vq.521024.cn

$obj?->method()
来源：http://zm.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://fh.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ut.yuexingan06.cn

[U56] PHP：命名参数
来源：http://nw.hnjuh.cn

f(a: 1, b: 2)
来源：http://mx.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://zd.jianghongdianzi.cn

"值: {$a}"
来源：http://qb.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://gz.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://es.9csxet.cn

[U59] PHP：自定义排序
来源：http://tt.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vs.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://il.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mr.yuntaijiaju.cn

[U61] PHP：正则
来源：http://qw.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wz.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://bq.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sl.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://om.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pn.panjiajie.cn

[U64] PHP：目录遍历
来源：http://gr.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ah.muxihuayi.cn

[U65] PHP：会话
来源：http://jw.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gs.521024.cn

[U66] PHP：设置 Cookie
来源：http://cq.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kh.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://ds.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aq.szsharing.cn

[U68] PHP：PDO 连接
来源：http://vk.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ra.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://pn.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dk.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://oc.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sa.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://ul.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://pb.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://ae.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://wv.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://al.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://la.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://sl.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://xf.shxzukj.cn

[U75] PHP：依赖注入
来源：http://tq.hahajie.cn

composer require psr/container
来源：http://bt.muxihuayi.cn

[U76] PHP：简单路由
来源：http://fm.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xz.hnjuh.cn

[U77] PHP：模板渲染
来源：http://yh.haigaiapp.cn

composer require twig/twig
来源：http://iv.shtwfgs.cn

[U78] PHP：单元测试
来源：http://zb.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://pj.szxytkj.cn

[U79] PHP：静态分析
来源：http://go.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://js.asd995.cn

[U80] PHP：代码规范修复
来源：http://sn.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ia.nicolike.cn

[U81] JS：初始化项目
来源：http://wq.yuexingan06.cn

npm init -y;  npm i express
来源：http://zo.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://hi.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gm.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://zk.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cj.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://iy.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pm.huanxung.cn

[U85] JS：可选链
来源：http://qg.muxihuayi.cn

a?.b?.c
来源：http://ry.panjiajie.cn

[U86] JS：空值合并
来源：http://tb.newstarts.cn

a ?? b
来源：http://vi.shxzukj.cn

[U87] JS：解构默认值
来源：http://gx.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://nc.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://qe.hnjuh.cn

{ ...a, ...b }
来源：http://ve.shxzukj.cn

[U89] JS：数组去重
来源：http://gu.nszjky.cn

[...new Set(arr)]
来源：http://of.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://ud.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://fy.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://rj.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pp.huanxung.cn

[U92] JS：深拷贝
来源：http://xm.nszjky.cn

structuredClone(obj)
来源：http://nq.panjiajie.cn

[U93] JS：模板字符串
来源：http://qu.bjjhwx.cn

`共 ${n} 条`
来源：http://vm.jctech888.com.cn

[U94] JS：箭头函数
来源：http://ho.muxihuayi.cn

const double = x => x * 2;
来源：http://li.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://bt.asd995.cn

new Promise((resolve, reject) => {})
来源：http://xs.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://ca.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gy.asd995.cn

[U97] JS：并发请求
来源：http://ea.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zy.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://qv.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zj.szsharing.cn

[U99] JS：事件监听
来源：http://qr.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://ye.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://te.shxzukj.cn

document.querySelector(".item")
来源：http://tb.jctech888.com.cn

[U101] JS：classList 操作
来源：http://jg.chemitech.net.cn

el.classList.toggle("active")
来源：http://vj.jctech888.com.cn

[U102] JS：本地存储
来源：http://ae.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://od.huanxung.cn

[U103] JS：定时器
来源：http://vn.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jj.newstarts.cn

[U104] JS：防抖
来源：http://vq.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bt.haigaiapp.cn

[U105] JS：节流
来源：http://ob.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fs.muxihuayi.cn

[U106] JS：日期格式化
来源：http://rb.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rk.shxzukj.cn

[U107] JS：数字千分位
来源：http://sp.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wf.szsharing.cn

[U108] JS：随机整数
来源：http://da.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tx.huanxung.cn

[U109] JS：数组分组
来源：http://ft.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://kj.521024.cn

[U110] JS：数组分块
来源：http://jz.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jo.gzmigu.cn

[U111] JS：对象转 Map
来源：http://px.gzmigu.cn

new Map(Object.entries(obj))
来源：http://he.hahajie.cn

[U112] JS：字符串补位
来源：http://sn.huixiangedu.cn

"7".padStart(3, "0")
来源：http://lw.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://vw.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://nl.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://cx.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cg.shxzskj.cn

[U115] JS：生成 UUID
来源：http://io.yuexingan06.cn

crypto.randomUUID()
来源：http://fa.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://yj.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://nh.asd995.cn

[U117] JS：单元测试
来源：http://xr.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://pk.shxzskj.cn

[U118] JS：开发服务器
来源：http://jv.shxzskj.cn

npm i -D vite;  npx vite
来源：http://sb.bookmarksfly.cn

[U119] JS：生产构建
来源：http://os.nicolike.cn

npx vite build
来源：http://ss.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://lp.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://js.panjiajie.cn

================================================================================
来源：http://tx.hahajie.cn

统计汇总
来源：http://en.huixinmuqiang.cn

================================================================================
来源：http://oo.muxihuayi.cn

按语言统计（条）：
来源：http://bt.jianghongdianzi.cn

Python ......... 252
来源：http://ak.shxzskj.cn

PHP ............ 252
来源：http://uo.yuexingan06.cn

JavaScript ..... 252
来源：http://dj.huanxung.cn

TypeScript ..... 212
来源：http://qr.lnxyls.cn

Java ........... 212
来源：http://og.huixinmuqiang.cn

Go ............. 212
来源：http://do.shxzskj.cn

Ruby ........... 212
来源：http://rm.huixinmuqiang.cn

C# ............. 212
来源：http://ic.hnjuh.cn

C .............. 30
来源：http://qr.shxzskj.cn

C++ ............ 30
来源：http://wv.szsharing.cn

SQL ............ 90
来源：http://xg.huanxung.cn

Bash ........... 80
来源：http://uk.newstarts.cn

Kotlin ......... 15
来源：http://pk.wgjwhj.cn

Swift .......... 15
来源：http://xt.szsharing.cn

Lua ............ 10
来源：http://al.huixinmuqiang.cn

Perl ........... 10
来源：http://en.panjiajie.cn

Scala .......... 10
来源：http://xf.521024.cn

------------------------------------
来源：http://sc.chemitech.net.cn

合计 ........... 2106 条
来源：http://mj.haigaiapp.cn

按章节统计：
来源：http://xn.szxytkj.cn


<!-- 参考信息 -->