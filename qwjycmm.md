代发 wailian999

[T43] Perl：字符串插值
来源：http://nv.colortex.cn

"值: $a"
来源：http://fm.muxihuayi.cn

[T44] Perl：条件
来源：http://qu.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://qj.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://fk.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://xf.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://sz.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pk.newstarts.cn

[T47] Perl：正则捕获
来源：http://db.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://za.lnxyls.cn

[T48] Perl：正则替换
来源：http://tt.9csxet.cn

$s =~ s/old/new/g;
来源：http://sx.shtwfgs.cn

[T49] Perl：函数
来源：http://gn.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bm.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://xv.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rq.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://xt.nszjky.cn

[T51] Scala：Hello World
来源：http://ik.haigaiapp.cn

println("Hello")
来源：http://fx.yuexingan06.cn

[T52] Scala：变量
来源：http://fo.chemitech.net.cn

val a = 1;  var b = 2
来源：http://nt.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://dk.yuexingan06.cn

s"值: $b"
来源：http://mf.hnjuh.cn

[T54] Scala：集合映射
来源：http://wr.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://rn.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://wz.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dn.hahajie.cn

[T56] Scala：样例类
来源：http://rh.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://vq.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://wa.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vw.wgjwhj.cn

[T58] Scala：函数定义
来源：http://fx.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xg.jctech888.com.cn

[T59] Scala：循环
来源：http://dt.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ip.hnjuh.cn

[T60] Scala：折叠
来源：http://qw.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lx.szxytkj.cn

================================================================================
来源：http://ul.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wn.lnxyls.cn

================================================================================
来源：http://fb.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://ln.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ok.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://tb.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rt.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://wp.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bx.nicolike.cn

[U04] Py：变量调试打印
来源：http://na.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ak.huanxung.cn

[U05] Py：列表去重且保序
来源：http://gg.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://eh.9csxet.cn

[U06] Py：合并两个字典
来源：http://ta.huixinmuqiang.cn

{**a, **b}
来源：http://bb.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://jm.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://dp.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://hw.huanxung.cn

[y for x in nested for y in x]
来源：http://vd.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://mf.shtwfgs.cn

max(d, key=d.get)
来源：http://tk.shxzskj.cn

[U10] Py：按值排序字典
来源：http://ca.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hl.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://he.jctech888.com.cn

(x * 2 for x in arr)
来源：http://vm.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rj.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://ru.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://gp.asd995.cn

deque(maxlen=10)
来源：http://is.nicolike.cn

[U14] Py：分组收集到列表
来源：http://jw.panjiajie.cn

defaultdict(list)
来源：http://zj.shxzukj.cn

[U15] Py：高精度计时
来源：http://tu.muxihuayi.cn

t = time.perf_counter()
来源：http://zu.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://gb.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xr.shxzskj.cn

[U17] Py：初始化日志
来源：http://zj.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://uq.gzmigu.cn

[U18] Py：预编译正则
来源：http://om.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://uc.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://qw.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kp.szsharing.cn

[U20] Py：缓存函数结果
来源：http://wp.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://pv.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://do.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://lv.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://bx.yuexingan06.cn

list(zip(*m))
来源：http://ar.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://yd.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://px.521024.cn

[U24] Py：路径操作
来源：http://gb.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qj.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://ns.lnxyls.cn

csv.DictReader(f)
来源：http://nb.jctech888.com.cn

[U26] Py：并发下载
来源：http://ik.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yz.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://tt.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uc.huanxung.cn

[U28] Py：类型别名
来源：http://vd.panjiajie.cn

UserId = int
来源：http://qe.newstarts.cn

[U29] Py：属性校验
来源：http://vo.szxytkj.cn

@property 与 @x.setter 配合
来源：http://tq.lnxyls.cn

[U30] Py：数据类
来源：http://jz.nszjky.cn

@dataclass(slots=True)
来源：http://sq.asd995.cn

[U31] Py：单测
来源：http://bd.shxzskj.cn

python -m pytest -q
来源：http://wl.lnxyls.cn

[U32] Py：代码格式化
来源：http://is.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://oe.nszjky.cn

[U33] Py：打包发布
来源：http://qj.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://db.jctech888.com.cn

[U34] Py：判断编码
来源：http://wy.bookmarksfly.cn

chardet.detect(raw)
来源：http://xv.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://iq.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kx.haigaiapp.cn

[U36] Py：定时任务
来源：http://mo.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ly.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://yz.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xt.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ca.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://qx.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://ge.nszjky.cn

sys.stdout.isatty()
来源：http://gb.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://dq.9csxet.cn

print("err", file=sys.stderr)
来源：http://jp.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://wv.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lv.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://mt.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lw.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://lw.bookmarksfly.cn

namespace App\Http;
来源：http://pb.colortex.cn

[U44] PHP：开启严格类型
来源：http://vd.colortex.cn

declare(strict_types=1);
来源：http://eb.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://la.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zn.hnjuh.cn

[U46] PHP：可空类型
来源：http://aw.bookmarksfly.cn

?string $name = null
来源：http://sj.521024.cn

[U47] PHP：联合类型
来源：http://ml.shtwfgs.cn

int|string $id
来源：http://km.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://yf.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oj.szsharing.cn

[U49] PHP：只读属性
来源：http://dm.nicolike.cn

public readonly string $name
来源：http://dl.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://rm.newstarts.cn

public function __construct(private int $id) {}
来源：http://he.jctech888.com.cn

[U51] PHP：数组解构
来源：http://cb.haigaiapp.cn

[$a, $b] = $arr;
来源：http://iq.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://gk.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://xw.9csxet.cn

[U53] PHP：空合并运算符
来源：http://sr.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://qw.szsharing.cn

[U54] PHP：空安全调用
来源：http://bv.yuntaijiaju.cn

$obj?->method()
来源：http://xy.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ma.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ha.huanxung.cn

[U56] PHP：命名参数
来源：http://mq.hnjuh.cn

f(a: 1, b: 2)
来源：http://tz.hahajie.cn

[U57] PHP：字符串插值
来源：http://ys.nszjky.cn

"值: {$a}"
来源：http://qo.gzmigu.cn

[U58] PHP：数组三件套
来源：http://wb.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qy.shxzskj.cn

[U59] PHP：自定义排序
来源：http://hu.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://he.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://ya.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lc.hahajie.cn

[U61] PHP：正则
来源：http://nn.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dw.huixiangedu.cn

[U62] PHP：日期对象
来源：http://vf.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vp.hahajie.cn

[U63] PHP：文件读写
来源：http://rh.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cy.colortex.cn

[U64] PHP：目录遍历
来源：http://qy.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://cy.asd995.cn

[U65] PHP：会话
来源：http://wf.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ec.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://qd.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fx.nicolike.cn

[U67] PHP：处理文件上传
来源：http://cb.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ww.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://uf.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ie.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://vv.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://ei.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cu.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://oe.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://bi.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://jp.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://nx.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://fo.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://wb.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://nh.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://lp.colortex.cn

[U75] PHP：依赖注入
来源：http://iw.newstarts.cn

composer require psr/container
来源：http://gh.muxihuayi.cn

[U76] PHP：简单路由
来源：http://rz.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dm.huanxung.cn

[U77] PHP：模板渲染
来源：http://hw.hahajie.cn

composer require twig/twig
来源：http://ob.yuexingan06.cn

[U78] PHP：单元测试
来源：http://op.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://xz.nicolike.cn

[U79] PHP：静态分析
来源：http://ge.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://nc.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://bl.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ri.bjjhwx.cn

[U81] JS：初始化项目
来源：http://fx.muxihuayi.cn

npm init -y;  npm i express
来源：http://kk.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://fl.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kn.521024.cn

[U83] JS：ES Module 导入导出
来源：http://ie.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zl.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://ae.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nf.shxzukj.cn

[U85] JS：可选链
来源：http://ol.colortex.cn

a?.b?.c
来源：http://zy.9csxet.cn

[U86] JS：空值合并
来源：http://md.jctech888.com.cn

a ?? b
来源：http://fu.shtwfgs.cn

[U87] JS：解构默认值
来源：http://lr.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://ox.521024.cn

[U88] JS：对象展开合并
来源：http://yb.yuntaijiaju.cn

{ ...a, ...b }
来源：http://yl.haigaiapp.cn

[U89] JS：数组去重
来源：http://hv.nszjky.cn

[...new Set(arr)]
来源：http://xr.newstarts.cn

[U90] JS：数字数组排序
来源：http://nj.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://cj.hahajie.cn

[U91] JS：对象键值遍历
来源：http://st.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jz.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://im.shtwfgs.cn

structuredClone(obj)
来源：http://xl.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://sv.lnxyls.cn

`共 ${n} 条`
来源：http://kp.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://jn.huixinmuqiang.cn

const double = x => x * 2;
来源：http://sl.hahajie.cn

[U95] JS：Promise 包装
来源：http://we.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://or.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://wd.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aj.lnxyls.cn

[U97] JS：并发请求
来源：http://aa.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sm.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://gs.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vm.colortex.cn

[U99] JS：事件监听
来源：http://ke.asd995.cn

el.addEventListener("click", e => {})
来源：http://xw.nicolike.cn

[U100] JS：DOM 查询
来源：http://jv.huixinmuqiang.cn

document.querySelector(".item")
来源：http://do.9csxet.cn

[U101] JS：classList 操作
来源：http://vz.yuexingan06.cn

el.classList.toggle("active")
来源：http://ri.gzmigu.cn

[U102] JS：本地存储
来源：http://ir.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dl.nicolike.cn

[U103] JS：定时器
来源：http://fm.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ko.nszjky.cn

[U104] JS：防抖
来源：http://uo.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ij.shxzukj.cn

[U105] JS：节流
来源：http://vk.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qa.lnxyls.cn

[U106] JS：日期格式化
来源：http://gw.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nq.9csxet.cn

[U107] JS：数字千分位
来源：http://mb.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://db.gzmigu.cn

[U108] JS：随机整数
来源：http://kv.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iw.szsharing.cn

[U109] JS：数组分组
来源：http://ph.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://zt.bookmarksfly.cn

[U110] JS：数组分块
来源：http://rb.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bo.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://lw.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://sw.chemitech.net.cn

[U112] JS：字符串补位
来源：http://fj.muxihuayi.cn

"7".padStart(3, "0")
来源：http://wb.shxzskj.cn

[U113] JS：正则替换全部
来源：http://vl.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://fw.nicolike.cn

[U114] JS：JSON 深比较
来源：http://pm.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ud.newstarts.cn

[U115] JS：生成 UUID
来源：http://kj.szxytkj.cn

crypto.randomUUID()
来源：http://si.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://zv.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://ow.szsharing.cn

[U117] JS：单元测试
来源：http://wu.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://uc.gzmigu.cn

[U118] JS：开发服务器
来源：http://pq.lnxyls.cn

npm i -D vite;  npx vite
来源：http://cu.huixiangedu.cn

[U119] JS：生产构建
来源：http://oy.hahajie.cn

npx vite build
来源：http://cb.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://tp.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://nw.huixinmuqiang.cn

================================================================================
来源：http://mx.jctech888.com.cn

统计汇总
来源：http://vs.bookmarksfly.cn

================================================================================
来源：http://lf.jianghongdianzi.cn

按语言统计（条）：
来源：http://gk.nicolike.cn

Python ......... 252
来源：http://vn.nicolike.cn

PHP ............ 252
来源：http://qs.shxzskj.cn

JavaScript ..... 252
来源：http://bs.panjiajie.cn

TypeScript ..... 212
来源：http://jn.jianghongdianzi.cn

Java ........... 212
来源：http://st.szsharing.cn

Go ............. 212
来源：http://ij.bjjhwx.cn

Ruby ........... 212
来源：http://mg.huixinmuqiang.cn

C# ............. 212
来源：http://kb.shtwfgs.cn

C .............. 30
来源：http://qv.shtwfgs.cn

C++ ............ 30
来源：http://sz.shtwfgs.cn

SQL ............ 90
来源：http://st.szsharing.cn

Bash ........... 80
来源：http://wx.szxytkj.cn

Kotlin ......... 15
来源：http://ry.huixinmuqiang.cn

Swift .......... 15
来源：http://xt.nszjky.cn

Lua ............ 10
来源：http://fo.muxihuayi.cn

Perl ........... 10
来源：http://nz.huanxung.cn


<!-- 参考信息 -->