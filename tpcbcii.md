代发 wailian999

[T39] Lua：模式匹配
来源：http://ck.shtwfgs.cn

string.find(s, "%d+")
来源：http://mt.yuntaijiaju.cn

[T40] Lua：元表
来源：http://et.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://vh.asd995.cn

[T41] Perl：Hello World
来源：http://al.bookmarksfly.cn

print "Hello\n";
来源：http://xs.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://pb.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ue.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://nx.shtwfgs.cn

"值: $a"
来源：http://ru.521024.cn

[T44] Perl：条件
来源：http://gr.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://ng.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://zj.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://lm.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://lj.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bk.shxzukj.cn

[T47] Perl：正则捕获
来源：http://gl.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ux.9csxet.cn

[T48] Perl：正则替换
来源：http://hq.szxytkj.cn

$s =~ s/old/new/g;
来源：http://hy.yuntaijiaju.cn

[T49] Perl：函数
来源：http://nb.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yt.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://gy.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://he.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://xw.szsharing.cn

[T51] Scala：Hello World
来源：http://xt.huanxung.cn

println("Hello")
来源：http://uy.szxytkj.cn

[T52] Scala：变量
来源：http://ll.chemitech.net.cn

val a = 1;  var b = 2
来源：http://iw.521024.cn

[T53] Scala：字符串插值
来源：http://jx.nszjky.cn

s"值: $b"
来源：http://wc.shxzskj.cn

[T54] Scala：集合映射
来源：http://dz.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://of.lnxyls.cn

[T55] Scala：集合过滤
来源：http://jn.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qj.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://ya.hahajie.cn

case class User(name: String, age: Int)
来源：http://ae.nszjky.cn

[T57] Scala：模式匹配
来源：http://ik.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ga.lnxyls.cn

[T58] Scala：函数定义
来源：http://ci.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kk.nicolike.cn

[T59] Scala：循环
来源：http://ko.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://wb.bjjhwx.cn

[T60] Scala：折叠
来源：http://zo.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pn.haigaiapp.cn

================================================================================
来源：http://nj.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://my.hnjuh.cn

================================================================================
来源：http://zu.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://im.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sf.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://rf.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tc.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://ex.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://di.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://eu.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oo.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://ph.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://oc.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://gx.huanxung.cn

{**a, **b}
来源：http://cq.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ti.newstarts.cn

{v: k for k, v in d.items()}
来源：http://jn.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://ly.szsharing.cn

[y for x in nested for y in x]
来源：http://wu.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://xm.chemitech.net.cn

max(d, key=d.get)
来源：http://dp.newstarts.cn

[U10] Py：按值排序字典
来源：http://tu.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vd.szsharing.cn

[U11] Py：生成器表达式
来源：http://mj.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://nw.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tt.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://jk.shxzskj.cn

[U13] Py：固定长度队列
来源：http://cn.bookmarksfly.cn

deque(maxlen=10)
来源：http://hp.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://ku.nicolike.cn

defaultdict(list)
来源：http://ja.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://jb.muxihuayi.cn

t = time.perf_counter()
来源：http://af.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://gd.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ym.colortex.cn

[U17] Py：初始化日志
来源：http://by.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://lh.nszjky.cn

[U18] Py：预编译正则
来源：http://pl.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://fe.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://iz.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vl.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://pd.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ta.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://ly.gzmigu.cn

@contextlib.contextmanager
来源：http://ry.panjiajie.cn

[U22] Py：矩阵转置
来源：http://gk.nicolike.cn

list(zip(*m))
来源：http://wf.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://md.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qi.newstarts.cn

[U24] Py：路径操作
来源：http://ma.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rd.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://es.nicolike.cn

csv.DictReader(f)
来源：http://fy.9csxet.cn

[U26] Py：并发下载
来源：http://ov.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wf.huanxung.cn

[U27] Py：异步 HTTP
来源：http://vr.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://zv.haigaiapp.cn

[U28] Py：类型别名
来源：http://gz.hahajie.cn

UserId = int
来源：http://rg.muxihuayi.cn

[U29] Py：属性校验
来源：http://qd.gzmigu.cn

@property 与 @x.setter 配合
来源：http://hw.muxihuayi.cn

[U30] Py：数据类
来源：http://vi.shxzskj.cn

@dataclass(slots=True)
来源：http://ok.newstarts.cn

[U31] Py：单测
来源：http://ih.huanxung.cn

python -m pytest -q
来源：http://rl.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://jp.nszjky.cn

ruff format . && ruff check --fix .
来源：http://cz.szxytkj.cn

[U33] Py：打包发布
来源：http://xl.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://xj.hnjuh.cn

[U34] Py：判断编码
来源：http://qr.nszjky.cn

chardet.detect(raw)
来源：http://an.nszjky.cn

[U35] Py：发送邮件
来源：http://lt.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sy.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://bz.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://lh.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://sd.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cv.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://sd.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://ki.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://nr.jctech888.com.cn

sys.stdout.isatty()
来源：http://kr.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://zg.hnjuh.cn

print("err", file=sys.stderr)
来源：http://hk.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://zz.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://se.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://in.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://un.9csxet.cn

[U43] PHP：声明命名空间
来源：http://ml.panjiajie.cn

namespace App\Http;
来源：http://qo.asd995.cn

[U44] PHP：开启严格类型
来源：http://xc.haigaiapp.cn

declare(strict_types=1);
来源：http://np.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://dv.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bj.521024.cn

[U46] PHP：可空类型
来源：http://ig.hahajie.cn

?string $name = null
来源：http://ot.9csxet.cn

[U47] PHP：联合类型
来源：http://xr.huanxung.cn

int|string $id
来源：http://ee.hnjuh.cn

[U48] PHP：纯枚举
来源：http://ck.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fw.szsharing.cn

[U49] PHP：只读属性
来源：http://qm.bookmarksfly.cn

public readonly string $name
来源：http://fl.521024.cn

[U50] PHP：构造器属性提升
来源：http://kk.szxytkj.cn

public function __construct(private int $id) {}
来源：http://ww.szsharing.cn

[U51] PHP：数组解构
来源：http://yt.nszjky.cn

[$a, $b] = $arr;
来源：http://pb.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://wv.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://as.hahajie.cn

[U53] PHP：空合并运算符
来源：http://ro.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://mh.nicolike.cn

[U54] PHP：空安全调用
来源：http://gl.gzmigu.cn

$obj?->method()
来源：http://va.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://zg.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bc.panjiajie.cn

[U56] PHP：命名参数
来源：http://xf.hahajie.cn

f(a: 1, b: 2)
来源：http://df.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://lf.hnjuh.cn

"值: {$a}"
来源：http://nc.asd995.cn

[U58] PHP：数组三件套
来源：http://fu.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eg.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://om.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://wt.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zf.yuexingan06.cn

[U61] PHP：正则
来源：http://rk.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pl.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://nj.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oz.asd995.cn

[U63] PHP：文件读写
来源：http://ts.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pc.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://rw.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://es.gzmigu.cn

[U65] PHP：会话
来源：http://ms.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tf.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://aq.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tk.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://kw.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wm.hahajie.cn

[U68] PHP：PDO 连接
来源：http://ju.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fo.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://tf.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://es.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://gm.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nx.newstarts.cn

[U71] PHP：抛出异常
来源：http://vp.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://bp.szsharing.cn

[U72] PHP：写错误日志
来源：http://rl.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://mx.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://yr.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://pv.huanxung.cn

[U74] PHP：读取环境变量
来源：http://cr.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://go.shxzskj.cn

[U75] PHP：依赖注入
来源：http://gf.muxihuayi.cn

composer require psr/container
来源：http://cw.9csxet.cn

[U76] PHP：简单路由
来源：http://vf.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ky.shxzskj.cn

[U77] PHP：模板渲染
来源：http://fk.huanxung.cn

composer require twig/twig
来源：http://xq.9csxet.cn

[U78] PHP：单元测试
来源：http://bd.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://lh.huanxung.cn

[U79] PHP：静态分析
来源：http://nc.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://bt.szsharing.cn

[U80] PHP：代码规范修复
来源：http://pp.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rg.newstarts.cn

[U81] JS：初始化项目
来源：http://nh.asd995.cn

npm init -y;  npm i express
来源：http://ku.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://yg.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pc.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://qo.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nj.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://kl.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pv.wgjwhj.cn

[U85] JS：可选链
来源：http://pr.521024.cn

a?.b?.c
来源：http://hu.nicolike.cn

[U86] JS：空值合并
来源：http://yz.gzmigu.cn

a ?? b
来源：http://vg.panjiajie.cn

[U87] JS：解构默认值
来源：http://sm.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://pk.colortex.cn

[U88] JS：对象展开合并
来源：http://dg.szsharing.cn

{ ...a, ...b }
来源：http://cl.huanxung.cn

[U89] JS：数组去重
来源：http://pg.yuexingan06.cn

[...new Set(arr)]
来源：http://op.521024.cn

[U90] JS：数字数组排序
来源：http://eg.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://ri.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://du.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jr.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://xa.hnjuh.cn

structuredClone(obj)
来源：http://io.nicolike.cn

[U93] JS：模板字符串
来源：http://gv.wgjwhj.cn

`共 ${n} 条`
来源：http://or.colortex.cn

[U94] JS：箭头函数
来源：http://vu.colortex.cn

const double = x => x * 2;
来源：http://lz.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://fx.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://sz.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://vx.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qz.lnxyls.cn

[U97] JS：并发请求
来源：http://ya.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jd.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://pt.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rh.jctech888.com.cn

[U99] JS：事件监听
来源：http://ps.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://hc.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://uk.shtwfgs.cn

document.querySelector(".item")
来源：http://pa.szxytkj.cn

[U101] JS：classList 操作
来源：http://jj.colortex.cn

el.classList.toggle("active")
来源：http://jc.panjiajie.cn

[U102] JS：本地存储
来源：http://ti.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://db.huanxung.cn

[U103] JS：定时器
来源：http://ko.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ev.wgjwhj.cn

[U104] JS：防抖
来源：http://lw.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.9csxet.cn

[U105] JS：节流
来源：http://ff.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hc.szsharing.cn

[U106] JS：日期格式化
来源：http://qs.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qs.asd995.cn

[U107] JS：数字千分位
来源：http://eg.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bw.wgjwhj.cn

[U108] JS：随机整数
来源：http://op.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rr.hnjuh.cn

[U109] JS：数组分组
来源：http://ph.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://gy.jctech888.com.cn

[U110] JS：数组分块
来源：http://pr.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wj.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://yi.gzmigu.cn

new Map(Object.entries(obj))
来源：http://vq.newstarts.cn

[U112] JS：字符串补位
来源：http://mc.521024.cn

"7".padStart(3, "0")
来源：http://zb.nicolike.cn

[U113] JS：正则替换全部
来源：http://bb.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://kb.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://kj.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://su.colortex.cn

[U115] JS：生成 UUID
来源：http://by.panjiajie.cn

crypto.randomUUID()
来源：http://ug.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://hn.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://mc.lnxyls.cn

[U117] JS：单元测试
来源：http://ng.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://fb.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://vp.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://kn.nszjky.cn

[U119] JS：生产构建
来源：http://wt.huanxung.cn

npx vite build
来源：http://yp.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://ew.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://jk.gzmigu.cn

================================================================================
来源：http://ul.lnxyls.cn

统计汇总
来源：http://yl.hnjuh.cn

================================================================================
来源：http://ka.hnjuh.cn

按语言统计（条）：
来源：http://ce.9csxet.cn

Python ......... 252
来源：http://wv.shxzskj.cn

PHP ............ 252
来源：http://ay.gzmigu.cn

JavaScript ..... 252
来源：http://km.hnjuh.cn

TypeScript ..... 212
来源：http://tf.wgjwhj.cn

Java ........... 212
来源：http://dq.muxihuayi.cn

Go ............. 212
来源：http://nw.colortex.cn

Ruby ........... 212
来源：http://sq.9csxet.cn

C# ............. 212
来源：http://xb.521024.cn


<!-- 参考信息 -->