代发 wailian999

[T39] Lua：模式匹配
来源：http://nm.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://wj.szxytkj.cn

[T40] Lua：元表
来源：http://hy.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://jt.nicolike.cn

[T41] Perl：Hello World
来源：http://zy.huixiangedu.cn

print "Hello\n";
来源：http://ij.panjiajie.cn

[T42] Perl：变量类型
来源：http://kf.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nj.colortex.cn

[T43] Perl：字符串插值
来源：http://ud.shtwfgs.cn

"值: $a"
来源：http://uf.wgjwhj.cn

[T44] Perl：条件
来源：http://gq.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://di.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://yz.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ye.szxytkj.cn

[T46] Perl：哈希操作
来源：http://rg.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pc.shxzukj.cn

[T47] Perl：正则捕获
来源：http://wb.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tl.huixiangedu.cn

[T48] Perl：正则替换
来源：http://pr.colortex.cn

$s =~ s/old/new/g;
来源：http://so.hahajie.cn

[T49] Perl：函数
来源：http://sj.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ct.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://tk.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qt.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ba.lnxyls.cn

[T51] Scala：Hello World
来源：http://yg.szxytkj.cn

println("Hello")
来源：http://fm.newstarts.cn

[T52] Scala：变量
来源：http://yd.colortex.cn

val a = 1;  var b = 2
来源：http://al.asd995.cn

[T53] Scala：字符串插值
来源：http://tr.wgjwhj.cn

s"值: $b"
来源：http://bv.hnjuh.cn

[T54] Scala：集合映射
来源：http://kw.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ac.shxzskj.cn

[T55] Scala：集合过滤
来源：http://us.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rl.colortex.cn

[T56] Scala：样例类
来源：http://op.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://gs.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://rc.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kh.hahajie.cn

[T58] Scala：函数定义
来源：http://ek.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lu.huixinmuqiang.cn

[T59] Scala：循环
来源：http://vk.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://td.jctech888.com.cn

[T60] Scala：折叠
来源：http://vg.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://od.shtwfgs.cn

================================================================================
来源：http://hb.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pp.jianghongdianzi.cn

================================================================================
来源：http://ic.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://dg.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zu.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://vy.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xp.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ki.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://en.nicolike.cn

[U04] Py：变量调试打印
来源：http://yr.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vu.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://it.newstarts.cn

list(dict.fromkeys(arr))
来源：http://kb.szxytkj.cn

[U06] Py：合并两个字典
来源：http://bt.yuexingan06.cn

{**a, **b}
来源：http://lf.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://gu.colortex.cn

{v: k for k, v in d.items()}
来源：http://pv.szsharing.cn

[U08] Py：展平二维列表
来源：http://dj.huanxung.cn

[y for x in nested for y in x]
来源：http://mk.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://vh.haigaiapp.cn

max(d, key=d.get)
来源：http://pp.hahajie.cn

[U10] Py：按值排序字典
来源：http://bq.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mk.lnxyls.cn

[U11] Py：生成器表达式
来源：http://vi.colortex.cn

(x * 2 for x in arr)
来源：http://we.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://re.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://cv.newstarts.cn

[U13] Py：固定长度队列
来源：http://bo.huixinmuqiang.cn

deque(maxlen=10)
来源：http://zb.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://wh.nszjky.cn

defaultdict(list)
来源：http://vp.bjjhwx.cn

[U15] Py：高精度计时
来源：http://wo.huixinmuqiang.cn

t = time.perf_counter()
来源：http://sa.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://px.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bm.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://xa.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://as.chemitech.net.cn

[U18] Py：预编译正则
来源：http://xh.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://xc.asd995.cn

[U19] Py：正则替换带回调
来源：http://fn.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jt.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://aa.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://xa.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://id.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://nn.9csxet.cn

[U22] Py：矩阵转置
来源：http://zn.nicolike.cn

list(zip(*m))
来源：http://wz.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://if.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://av.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://hb.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hg.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://jd.521024.cn

csv.DictReader(f)
来源：http://nt.bjjhwx.cn

[U26] Py：并发下载
来源：http://gd.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wp.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://mg.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://tv.gzmigu.cn

[U28] Py：类型别名
来源：http://ru.jctech888.com.cn

UserId = int
来源：http://ru.gzmigu.cn

[U29] Py：属性校验
来源：http://fh.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://tu.bjjhwx.cn

[U30] Py：数据类
来源：http://cy.huanxung.cn

@dataclass(slots=True)
来源：http://tq.shtwfgs.cn

[U31] Py：单测
来源：http://hh.yuntaijiaju.cn

python -m pytest -q
来源：http://im.gzmigu.cn

[U32] Py：代码格式化
来源：http://ye.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://uq.shtwfgs.cn

[U33] Py：打包发布
来源：http://mg.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://ff.shtwfgs.cn

[U34] Py：判断编码
来源：http://mv.shtwfgs.cn

chardet.detect(raw)
来源：http://xr.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ld.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hs.szsharing.cn

[U36] Py：定时任务
来源：http://li.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://vq.szxytkj.cn

[U37] Py：读写 Excel
来源：http://dw.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://te.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://oe.shxzukj.cn

Path(__file__).resolve().parent
来源：http://zr.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://ma.nicolike.cn

sys.stdout.isatty()
来源：http://ro.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://bm.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://nt.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://xq.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qe.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://bm.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wj.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://tr.panjiajie.cn

namespace App\Http;
来源：http://sy.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://uv.newstarts.cn

declare(strict_types=1);
来源：http://fg.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://jm.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hb.szsharing.cn

[U46] PHP：可空类型
来源：http://xc.yuntaijiaju.cn

?string $name = null
来源：http://jf.haigaiapp.cn

[U47] PHP：联合类型
来源：http://lp.bjjhwx.cn

int|string $id
来源：http://or.huanxung.cn

[U48] PHP：纯枚举
来源：http://eo.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tk.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://kt.521024.cn

public readonly string $name
来源：http://rn.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://gy.9csxet.cn

public function __construct(private int $id) {}
来源：http://oa.hahajie.cn

[U51] PHP：数组解构
来源：http://fh.nszjky.cn

[$a, $b] = $arr;
来源：http://yg.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://zc.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://ru.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://ef.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://aw.hahajie.cn

[U54] PHP：空安全调用
来源：http://ht.huixinmuqiang.cn

$obj?->method()
来源：http://yd.colortex.cn

[U55] PHP：match 表达式
来源：http://da.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uu.haigaiapp.cn

[U56] PHP：命名参数
来源：http://xa.wgjwhj.cn

f(a: 1, b: 2)
来源：http://mo.hnjuh.cn

[U57] PHP：字符串插值
来源：http://st.muxihuayi.cn

"值: {$a}"
来源：http://zo.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://nt.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mb.panjiajie.cn

[U59] PHP：自定义排序
来源：http://zs.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qj.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://ku.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uk.yuntaijiaju.cn

[U61] PHP：正则
来源：http://ub.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ng.wgjwhj.cn

[U62] PHP：日期对象
来源：http://zf.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vx.huanxung.cn

[U63] PHP：文件读写
来源：http://ni.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://li.newstarts.cn

[U64] PHP：目录遍历
来源：http://uf.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://so.huixinmuqiang.cn

[U65] PHP：会话
来源：http://cr.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yb.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://yz.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zv.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://uz.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cz.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ug.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ne.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://qe.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fl.nicolike.cn

[U70] PHP：PDO 事务
来源：http://ud.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sb.panjiajie.cn

[U71] PHP：抛出异常
来源：http://um.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://ni.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://rj.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://kz.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://vy.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://dt.nszjky.cn

[U74] PHP：读取环境变量
来源：http://kh.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://aw.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://by.huanxung.cn

composer require psr/container
来源：http://jr.asd995.cn

[U76] PHP：简单路由
来源：http://fh.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uz.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://cq.hahajie.cn

composer require twig/twig
来源：http://vd.shxzukj.cn

[U78] PHP：单元测试
来源：http://tq.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://fz.9csxet.cn

[U79] PHP：静态分析
来源：http://gz.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://ny.newstarts.cn

[U80] PHP：代码规范修复
来源：http://hl.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://or.newstarts.cn

[U81] JS：初始化项目
来源：http://xy.muxihuayi.cn

npm init -y;  npm i express
来源：http://eg.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://jo.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lp.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://ux.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kj.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://yw.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qw.hnjuh.cn

[U85] JS：可选链
来源：http://da.huanxung.cn

a?.b?.c
来源：http://fj.hahajie.cn

[U86] JS：空值合并
来源：http://cl.bjjhwx.cn

a ?? b
来源：http://oz.szsharing.cn

[U87] JS：解构默认值
来源：http://nf.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://eo.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://li.colortex.cn

{ ...a, ...b }
来源：http://xv.lnxyls.cn

[U89] JS：数组去重
来源：http://po.panjiajie.cn

[...new Set(arr)]
来源：http://ii.huanxung.cn

[U90] JS：数字数组排序
来源：http://fb.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://py.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://es.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://th.521024.cn

[U92] JS：深拷贝
来源：http://ll.muxihuayi.cn

structuredClone(obj)
来源：http://ns.asd995.cn

[U93] JS：模板字符串
来源：http://vq.huixinmuqiang.cn

`共 ${n} 条`
来源：http://nw.hahajie.cn

[U94] JS：箭头函数
来源：http://dp.haigaiapp.cn

const double = x => x * 2;
来源：http://la.gzmigu.cn

[U95] JS：Promise 包装
来源：http://vf.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://qw.asd995.cn

[U96] JS：async/await 与异常
来源：http://mp.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dg.szsharing.cn

[U97] JS：并发请求
来源：http://sp.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dz.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://dc.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pr.yuexingan06.cn

[U99] JS：事件监听
来源：http://bp.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://gp.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://yb.asd995.cn

document.querySelector(".item")
来源：http://ec.szsharing.cn

[U101] JS：classList 操作
来源：http://hf.nszjky.cn

el.classList.toggle("active")
来源：http://wr.nszjky.cn

[U102] JS：本地存储
来源：http://cs.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ev.hnjuh.cn

[U103] JS：定时器
来源：http://ml.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qn.yuntaijiaju.cn

[U104] JS：防抖
来源：http://zu.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oi.bjjhwx.cn

[U105] JS：节流
来源：http://wi.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://re.szxytkj.cn

[U106] JS：日期格式化
来源：http://ry.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gv.jctech888.com.cn

[U107] JS：数字千分位
来源：http://ic.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wa.colortex.cn

[U108] JS：随机整数
来源：http://cb.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bf.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://ok.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://gu.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://tk.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pj.newstarts.cn

[U111] JS：对象转 Map
来源：http://kt.asd995.cn

new Map(Object.entries(obj))
来源：http://lb.9csxet.cn

[U112] JS：字符串补位
来源：http://xn.gzmigu.cn

"7".padStart(3, "0")
来源：http://wc.shxzukj.cn

[U113] JS：正则替换全部
来源：http://ww.shxzukj.cn

s.replaceAll("a", "b")
来源：http://wr.newstarts.cn

[U114] JS：JSON 深比较
来源：http://cv.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kx.nszjky.cn

[U115] JS：生成 UUID
来源：http://qz.9csxet.cn

crypto.randomUUID()
来源：http://rk.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://bw.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://yw.panjiajie.cn

[U117] JS：单元测试
来源：http://cg.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://rd.yuexingan06.cn

[U118] JS：开发服务器
来源：http://ag.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://br.shxzskj.cn

[U119] JS：生产构建
来源：http://kl.huixinmuqiang.cn

npx vite build
来源：http://xx.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://bn.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://wi.shxzskj.cn

================================================================================
来源：http://zn.bjjhwx.cn

统计汇总
来源：http://lf.jctech888.com.cn

================================================================================
来源：http://pe.nszjky.cn

按语言统计（条）：
来源：http://ik.panjiajie.cn

Python ......... 252
来源：http://rd.shtwfgs.cn

PHP ............ 252
来源：http://pz.jctech888.com.cn

JavaScript ..... 252
来源：http://hg.hnjuh.cn

TypeScript ..... 212
来源：http://ht.chemitech.net.cn

Java ........... 212
来源：http://qf.shxzskj.cn

Go ............. 212
来源：http://ji.hahajie.cn

Ruby ........... 212
来源：http://bd.bjjhwx.cn

C# ............. 212
来源：http://yj.newstarts.cn


<!-- 参考信息 -->