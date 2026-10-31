代发 wailian999

[T45] Perl：数组遍历
来源：http://yn.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://oo.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ay.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ut.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ab.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iu.asd995.cn

[T48] Perl：正则替换
来源：http://bv.9csxet.cn

$s =~ s/old/new/g;
来源：http://dy.wgjwhj.cn

[T49] Perl：函数
来源：http://rj.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vn.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://iz.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ck.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://ri.asd995.cn

[T51] Scala：Hello World
来源：http://hd.jianghongdianzi.cn

println("Hello")
来源：http://ke.lnxyls.cn

[T52] Scala：变量
来源：http://fn.shxzskj.cn

val a = 1;  var b = 2
来源：http://qq.shxzukj.cn

[T53] Scala：字符串插值
来源：http://vp.9csxet.cn

s"值: $b"
来源：http://jf.lnxyls.cn

[T54] Scala：集合映射
来源：http://bb.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://qk.huanxung.cn

[T55] Scala：集合过滤
来源：http://bp.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ai.nicolike.cn

[T56] Scala：样例类
来源：http://od.nszjky.cn

case class User(name: String, age: Int)
来源：http://aj.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://mf.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jo.shxzskj.cn

[T58] Scala：函数定义
来源：http://id.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ox.panjiajie.cn

[T59] Scala：循环
来源：http://uf.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://rm.bookmarksfly.cn

[T60] Scala：折叠
来源：http://no.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rl.hahajie.cn

================================================================================
来源：http://ra.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gm.hnjuh.cn

================================================================================
来源：http://fb.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://wl.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tx.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://na.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yc.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://dk.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dm.colortex.cn

[U04] Py：变量调试打印
来源：http://nl.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ye.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://fg.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://au.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://wt.chemitech.net.cn

{**a, **b}
来源：http://fp.9csxet.cn

[U07] Py：反转字典键值
来源：http://gh.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://cx.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://iy.hnjuh.cn

[y for x in nested for y in x]
来源：http://xr.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://pv.panjiajie.cn

max(d, key=d.get)
来源：http://ge.521024.cn

[U10] Py：按值排序字典
来源：http://ci.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xc.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ri.szxytkj.cn

(x * 2 for x in arr)
来源：http://yv.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ib.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://bc.9csxet.cn

[U13] Py：固定长度队列
来源：http://lt.nszjky.cn

deque(maxlen=10)
来源：http://hq.hahajie.cn

[U14] Py：分组收集到列表
来源：http://py.nszjky.cn

defaultdict(list)
来源：http://bm.lnxyls.cn

[U15] Py：高精度计时
来源：http://kp.hnjuh.cn

t = time.perf_counter()
来源：http://gi.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://ta.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oa.bjjhwx.cn

[U17] Py：初始化日志
来源：http://od.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://vy.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://np.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://ns.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://sc.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pd.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://bs.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://zm.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://rs.wgjwhj.cn

@contextlib.contextmanager
来源：http://cx.gzmigu.cn

[U22] Py：矩阵转置
来源：http://bt.wgjwhj.cn

list(zip(*m))
来源：http://ol.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://yg.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://el.wgjwhj.cn

[U24] Py：路径操作
来源：http://kh.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cw.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://fq.shxzskj.cn

csv.DictReader(f)
来源：http://wf.szxytkj.cn

[U26] Py：并发下载
来源：http://io.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yh.asd995.cn

[U27] Py：异步 HTTP
来源：http://rz.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://pp.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://li.wgjwhj.cn

UserId = int
来源：http://gv.yuexingan06.cn

[U29] Py：属性校验
来源：http://qq.huanxung.cn

@property 与 @x.setter 配合
来源：http://hu.huanxung.cn

[U30] Py：数据类
来源：http://iu.gzmigu.cn

@dataclass(slots=True)
来源：http://vv.muxihuayi.cn

[U31] Py：单测
来源：http://ht.wgjwhj.cn

python -m pytest -q
来源：http://qb.521024.cn

[U32] Py：代码格式化
来源：http://oo.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://vo.shxzukj.cn

[U33] Py：打包发布
来源：http://if.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://xq.nszjky.cn

[U34] Py：判断编码
来源：http://mc.lnxyls.cn

chardet.detect(raw)
来源：http://hc.bjjhwx.cn

[U35] Py：发送邮件
来源：http://sz.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rh.yuexingan06.cn

[U36] Py：定时任务
来源：http://ul.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://ia.nicolike.cn

[U37] Py：读写 Excel
来源：http://xg.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yu.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://et.521024.cn

Path(__file__).resolve().parent
来源：http://ko.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://pb.chemitech.net.cn

sys.stdout.isatty()
来源：http://rr.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://ci.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://zq.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lm.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cv.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://oh.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ey.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://tk.nicolike.cn

namespace App\Http;
来源：http://pr.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://ee.colortex.cn

declare(strict_types=1);
来源：http://su.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://wn.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://we.szxytkj.cn

[U46] PHP：可空类型
来源：http://ll.shxzukj.cn

?string $name = null
来源：http://gw.muxihuayi.cn

[U47] PHP：联合类型
来源：http://kc.huixiangedu.cn

int|string $id
来源：http://he.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://zk.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yb.jctech888.com.cn

[U49] PHP：只读属性
来源：http://wq.shtwfgs.cn

public readonly string $name
来源：http://hn.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ig.newstarts.cn

public function __construct(private int $id) {}
来源：http://ni.shtwfgs.cn

[U51] PHP：数组解构
来源：http://hf.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://wm.asd995.cn

[U52] PHP：箭头函数
来源：http://hy.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://yx.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://xr.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://ne.lnxyls.cn

[U54] PHP：空安全调用
来源：http://mm.shxzukj.cn

$obj?->method()
来源：http://on.521024.cn

[U55] PHP：match 表达式
来源：http://bm.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wg.hahajie.cn

[U56] PHP：命名参数
来源：http://ih.bjjhwx.cn

f(a: 1, b: 2)
来源：http://nk.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://jl.shxzukj.cn

"值: {$a}"
来源：http://zz.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://pr.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kv.nicolike.cn

[U59] PHP：自定义排序
来源：http://hi.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xz.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://ac.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tf.muxihuayi.cn

[U61] PHP：正则
来源：http://it.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uj.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ws.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rb.521024.cn

[U63] PHP：文件读写
来源：http://qn.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rw.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://qt.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://tq.asd995.cn

[U65] PHP：会话
来源：http://vl.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dl.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://hc.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uh.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://zw.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tf.9csxet.cn

[U68] PHP：PDO 连接
来源：http://ic.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xk.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://na.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sq.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://ll.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gy.gzmigu.cn

[U71] PHP：抛出异常
来源：http://sa.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://hs.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://yj.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://oz.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://kx.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://zy.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://en.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://pl.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://qi.nszjky.cn

composer require psr/container
来源：http://ak.panjiajie.cn

[U76] PHP：简单路由
来源：http://xp.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qy.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://oe.bookmarksfly.cn

composer require twig/twig
来源：http://as.hnjuh.cn

[U78] PHP：单元测试
来源：http://hb.colortex.cn

composer require --dev phpunit/phpunit
来源：http://gg.newstarts.cn

[U79] PHP：静态分析
来源：http://oj.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://cg.asd995.cn

[U80] PHP：代码规范修复
来源：http://ul.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sf.521024.cn

[U81] JS：初始化项目
来源：http://kv.panjiajie.cn

npm init -y;  npm i express
来源：http://bv.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://kj.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ru.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://kt.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tc.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://yl.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://is.9csxet.cn

[U85] JS：可选链
来源：http://ur.haigaiapp.cn

a?.b?.c
来源：http://hm.huixiangedu.cn

[U86] JS：空值合并
来源：http://jt.jctech888.com.cn

a ?? b
来源：http://ev.panjiajie.cn

[U87] JS：解构默认值
来源：http://mk.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://kl.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://mb.nszjky.cn

{ ...a, ...b }
来源：http://hq.9csxet.cn

[U89] JS：数组去重
来源：http://kp.nszjky.cn

[...new Set(arr)]
来源：http://jm.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://xb.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://dr.szsharing.cn

[U91] JS：对象键值遍历
来源：http://ap.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://we.shtwfgs.cn

[U92] JS：深拷贝
来源：http://ys.szxytkj.cn

structuredClone(obj)
来源：http://ke.colortex.cn

[U93] JS：模板字符串
来源：http://pm.hnjuh.cn

`共 ${n} 条`
来源：http://kf.shxzskj.cn

[U94] JS：箭头函数
来源：http://zs.wgjwhj.cn

const double = x => x * 2;
来源：http://tt.lnxyls.cn

[U95] JS：Promise 包装
来源：http://ab.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://oo.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://je.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nv.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://pl.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://al.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://un.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://no.bookmarksfly.cn

[U99] JS：事件监听
来源：http://bo.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://ix.colortex.cn

[U100] JS：DOM 查询
来源：http://rv.muxihuayi.cn

document.querySelector(".item")
来源：http://wv.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ib.panjiajie.cn

el.classList.toggle("active")
来源：http://fk.haigaiapp.cn

[U102] JS：本地存储
来源：http://dc.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wa.hnjuh.cn

[U103] JS：定时器
来源：http://vp.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vg.hahajie.cn

[U104] JS：防抖
来源：http://nk.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qf.shxzukj.cn

[U105] JS：节流
来源：http://zp.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cs.gzmigu.cn

[U106] JS：日期格式化
来源：http://ci.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mb.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://zf.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dn.asd995.cn

[U108] JS：随机整数
来源：http://lx.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://te.hahajie.cn

[U109] JS：数组分组
来源：http://mr.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://nh.panjiajie.cn

[U110] JS：数组分块
来源：http://pi.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kh.nszjky.cn

[U111] JS：对象转 Map
来源：http://gv.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://zd.szxytkj.cn

[U112] JS：字符串补位
来源：http://sd.hnjuh.cn

"7".padStart(3, "0")
来源：http://nn.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://uk.hahajie.cn

s.replaceAll("a", "b")
来源：http://ps.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://bw.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lr.hahajie.cn

[U115] JS：生成 UUID
来源：http://rp.hnjuh.cn

crypto.randomUUID()
来源：http://pn.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://zn.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://rz.hnjuh.cn

[U117] JS：单元测试
来源：http://ao.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://tk.shxzukj.cn

[U118] JS：开发服务器
来源：http://yk.nicolike.cn

npm i -D vite;  npx vite
来源：http://rq.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://ps.asd995.cn

npx vite build
来源：http://nc.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://ju.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://yy.asd995.cn

================================================================================
来源：http://yl.muxihuayi.cn

统计汇总
来源：http://gh.asd995.cn

================================================================================
来源：http://jq.szsharing.cn

按语言统计（条）：
来源：http://sn.jctech888.com.cn

Python ......... 252
来源：http://kl.9csxet.cn

PHP ............ 252
来源：http://wq.wgjwhj.cn

JavaScript ..... 252
来源：http://jh.asd995.cn

TypeScript ..... 212
来源：http://so.yuexingan06.cn

Java ........... 212
来源：http://rn.szxytkj.cn

Go ............. 212
来源：http://ob.nicolike.cn

Ruby ........... 212
来源：http://gr.shxzukj.cn

C# ............. 212
来源：http://rs.colortex.cn

C .............. 30
来源：http://eh.lnxyls.cn

C++ ............ 30
来源：http://yw.szsharing.cn

SQL ............ 90
来源：http://yk.shtwfgs.cn

Bash ........... 80
来源：http://hk.panjiajie.cn

Kotlin ......... 15
来源：http://pf.chemitech.net.cn

Swift .......... 15
来源：http://di.newstarts.cn

Lua ............ 10
来源：http://ra.nicolike.cn

Perl ........... 10
来源：http://qj.szxytkj.cn

Scala .......... 10
来源：http://oh.muxihuayi.cn

------------------------------------
来源：http://az.newstarts.cn

合计 ........... 2106 条
来源：http://hl.yuntaijiaju.cn

按章节统计：
来源：http://oc.shxzukj.cn


<!-- 参考信息 -->