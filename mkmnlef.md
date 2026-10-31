代发 wailian999

[T39] Lua：模式匹配
来源：http://bb.asd995.cn

string.find(s, "%d+")
来源：http://qy.shxzskj.cn

[T40] Lua：元表
来源：http://xp.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://yy.shxzukj.cn

[T41] Perl：Hello World
来源：http://xs.yuntaijiaju.cn

print "Hello\n";
来源：http://wh.jctech888.com.cn

[T42] Perl：变量类型
来源：http://wh.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vw.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://jp.shxzskj.cn

"值: $a"
来源：http://dm.yuntaijiaju.cn

[T44] Perl：条件
来源：http://jr.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://kw.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://sq.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ig.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://es.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tt.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://wu.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ll.lnxyls.cn

[T48] Perl：正则替换
来源：http://zq.szxytkj.cn

$s =~ s/old/new/g;
来源：http://zn.muxihuayi.cn

[T49] Perl：函数
来源：http://vx.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mh.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://nb.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://au.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://fc.panjiajie.cn

[T51] Scala：Hello World
来源：http://dp.chemitech.net.cn

println("Hello")
来源：http://wa.nszjky.cn

[T52] Scala：变量
来源：http://up.asd995.cn

val a = 1;  var b = 2
来源：http://aa.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://vw.newstarts.cn

s"值: $b"
来源：http://vb.yuexingan06.cn

[T54] Scala：集合映射
来源：http://me.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://iu.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://pt.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://de.chemitech.net.cn

[T56] Scala：样例类
来源：http://zf.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://yd.shxzukj.cn

[T57] Scala：模式匹配
来源：http://dh.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mf.9csxet.cn

[T58] Scala：函数定义
来源：http://cq.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://te.huixinmuqiang.cn

[T59] Scala：循环
来源：http://zw.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://am.gzmigu.cn

[T60] Scala：折叠
来源：http://rf.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zq.huanxung.cn

================================================================================
来源：http://jj.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dv.huixinmuqiang.cn

================================================================================
来源：http://zc.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://gs.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cy.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://pe.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sv.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://ie.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gn.huanxung.cn

[U04] Py：变量调试打印
来源：http://ai.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xp.521024.cn

[U05] Py：列表去重且保序
来源：http://wh.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://km.hnjuh.cn

[U06] Py：合并两个字典
来源：http://td.colortex.cn

{**a, **b}
来源：http://bd.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://zc.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://th.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://vm.szxytkj.cn

[y for x in nested for y in x]
来源：http://os.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://hj.huanxung.cn

max(d, key=d.get)
来源：http://ib.nszjky.cn

[U10] Py：按值排序字典
来源：http://xi.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fl.panjiajie.cn

[U11] Py：生成器表达式
来源：http://gt.shxzskj.cn

(x * 2 for x in arr)
来源：http://df.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qe.shxzukj.cn

Counter(arr).most_common(3)
来源：http://nm.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://if.jianghongdianzi.cn

deque(maxlen=10)
来源：http://xr.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://xa.huixinmuqiang.cn

defaultdict(list)
来源：http://bp.muxihuayi.cn

[U15] Py：高精度计时
来源：http://xr.hnjuh.cn

t = time.perf_counter()
来源：http://qw.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://vt.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eu.szsharing.cn

[U17] Py：初始化日志
来源：http://du.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://vv.9csxet.cn

[U18] Py：预编译正则
来源：http://mr.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://rk.newstarts.cn

[U19] Py：正则替换带回调
来源：http://dm.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oc.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://nz.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://ug.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://cd.nicolike.cn

@contextlib.contextmanager
来源：http://wt.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://ev.huixinmuqiang.cn

list(zip(*m))
来源：http://al.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://fp.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://po.9csxet.cn

[U24] Py：路径操作
来源：http://vp.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yf.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://ye.shtwfgs.cn

csv.DictReader(f)
来源：http://hn.9csxet.cn

[U26] Py：并发下载
来源：http://sw.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zz.colortex.cn

[U27] Py：异步 HTTP
来源：http://gm.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ka.gzmigu.cn

[U28] Py：类型别名
来源：http://me.huixinmuqiang.cn

UserId = int
来源：http://oj.521024.cn

[U29] Py：属性校验
来源：http://ek.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://wx.colortex.cn

[U30] Py：数据类
来源：http://wk.jctech888.com.cn

@dataclass(slots=True)
来源：http://ie.shxzukj.cn

[U31] Py：单测
来源：http://qy.szsharing.cn

python -m pytest -q
来源：http://fa.huanxung.cn

[U32] Py：代码格式化
来源：http://dw.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://uc.szsharing.cn

[U33] Py：打包发布
来源：http://ny.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://en.haigaiapp.cn

[U34] Py：判断编码
来源：http://vq.hahajie.cn

chardet.detect(raw)
来源：http://lz.9csxet.cn

[U35] Py：发送邮件
来源：http://pg.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sq.jctech888.com.cn

[U36] Py：定时任务
来源：http://bh.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://qt.panjiajie.cn

[U37] Py：读写 Excel
来源：http://bd.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://br.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://pa.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://yl.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://yf.bookmarksfly.cn

sys.stdout.isatty()
来源：http://si.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://db.hnjuh.cn

print("err", file=sys.stderr)
来源：http://dh.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://tm.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gn.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://pp.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xh.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://dm.haigaiapp.cn

namespace App\Http;
来源：http://kl.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://tv.colortex.cn

declare(strict_types=1);
来源：http://dm.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://hi.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jk.szsharing.cn

[U46] PHP：可空类型
来源：http://wg.huixiangedu.cn

?string $name = null
来源：http://xm.hahajie.cn

[U47] PHP：联合类型
来源：http://dd.asd995.cn

int|string $id
来源：http://ia.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://gf.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gb.szxytkj.cn

[U49] PHP：只读属性
来源：http://dt.szxytkj.cn

public readonly string $name
来源：http://uo.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://jq.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://ei.huixiangedu.cn

[U51] PHP：数组解构
来源：http://wl.jctech888.com.cn

[$a, $b] = $arr;
来源：http://ii.asd995.cn

[U52] PHP：箭头函数
来源：http://wv.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://uv.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://cp.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://dz.szxytkj.cn

[U54] PHP：空安全调用
来源：http://ne.szxytkj.cn

$obj?->method()
来源：http://td.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://nh.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xc.newstarts.cn

[U56] PHP：命名参数
来源：http://ow.yuexingan06.cn

f(a: 1, b: 2)
来源：http://it.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://zq.muxihuayi.cn

"值: {$a}"
来源：http://db.9csxet.cn

[U58] PHP：数组三件套
来源：http://zh.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hk.shxzukj.cn

[U59] PHP：自定义排序
来源：http://ds.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pq.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://yp.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gy.bookmarksfly.cn

[U61] PHP：正则
来源：http://me.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ma.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://iz.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fx.jctech888.com.cn

[U63] PHP：文件读写
来源：http://wm.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pg.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://th.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://af.bjjhwx.cn

[U65] PHP：会话
来源：http://ni.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bb.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://yu.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rv.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://eh.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vn.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://dl.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xd.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://jg.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oz.hahajie.cn

[U70] PHP：PDO 事务
来源：http://ip.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aj.newstarts.cn

[U71] PHP：抛出异常
来源：http://hu.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://wi.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://bs.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://wm.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://hp.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://sg.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://gt.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://qg.shxzskj.cn

[U75] PHP：依赖注入
来源：http://ki.szxytkj.cn

composer require psr/container
来源：http://er.huixiangedu.cn

[U76] PHP：简单路由
来源：http://oc.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uq.colortex.cn

[U77] PHP：模板渲染
来源：http://se.521024.cn

composer require twig/twig
来源：http://fm.shxzukj.cn

[U78] PHP：单元测试
来源：http://ew.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://md.huixiangedu.cn

[U79] PHP：静态分析
来源：http://jv.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://cv.asd995.cn

[U80] PHP：代码规范修复
来源：http://fi.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xv.huanxung.cn

[U81] JS：初始化项目
来源：http://rb.jctech888.com.cn

npm init -y;  npm i express
来源：http://lg.asd995.cn

[U82] JS：package.json 脚本
来源：http://xm.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bd.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://az.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rb.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://oe.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qk.asd995.cn

[U85] JS：可选链
来源：http://dz.lnxyls.cn

a?.b?.c
来源：http://hh.szsharing.cn

[U86] JS：空值合并
来源：http://nq.bookmarksfly.cn

a ?? b
来源：http://ak.nszjky.cn

[U87] JS：解构默认值
来源：http://cu.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://wb.gzmigu.cn

[U88] JS：对象展开合并
来源：http://ss.huixinmuqiang.cn

{ ...a, ...b }
来源：http://fa.9csxet.cn

[U89] JS：数组去重
来源：http://al.hnjuh.cn

[...new Set(arr)]
来源：http://op.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://zp.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://mz.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://qr.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fg.szxytkj.cn

[U92] JS：深拷贝
来源：http://wa.huixiangedu.cn

structuredClone(obj)
来源：http://dx.gzmigu.cn

[U93] JS：模板字符串
来源：http://mm.chemitech.net.cn

`共 ${n} 条`
来源：http://sa.hnjuh.cn

[U94] JS：箭头函数
来源：http://nx.jianghongdianzi.cn

const double = x => x * 2;
来源：http://cy.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://vi.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://yu.nicolike.cn

[U96] JS：async/await 与异常
来源：http://jw.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nm.lnxyls.cn

[U97] JS：并发请求
来源：http://ft.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://md.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://ym.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rg.yuexingan06.cn

[U99] JS：事件监听
来源：http://qm.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://ck.hnjuh.cn

[U100] JS：DOM 查询
来源：http://jw.shtwfgs.cn

document.querySelector(".item")
来源：http://tq.bjjhwx.cn

[U101] JS：classList 操作
来源：http://dh.colortex.cn

el.classList.toggle("active")
来源：http://pi.huanxung.cn

[U102] JS：本地存储
来源：http://tp.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wx.asd995.cn

[U103] JS：定时器
来源：http://qd.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oy.9csxet.cn

[U104] JS：防抖
来源：http://kx.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://id.muxihuayi.cn

[U105] JS：节流
来源：http://pt.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ke.newstarts.cn

[U106] JS：日期格式化
来源：http://hm.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yz.nicolike.cn

[U107] JS：数字千分位
来源：http://fo.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vx.shxzukj.cn

[U108] JS：随机整数
来源：http://zs.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ex.panjiajie.cn

[U109] JS：数组分组
来源：http://rl.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://bn.nicolike.cn

[U110] JS：数组分块
来源：http://df.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ta.hahajie.cn

[U111] JS：对象转 Map
来源：http://eu.hahajie.cn

new Map(Object.entries(obj))
来源：http://oy.szxytkj.cn

[U112] JS：字符串补位
来源：http://dr.hahajie.cn

"7".padStart(3, "0")
来源：http://kc.shxzskj.cn

[U113] JS：正则替换全部
来源：http://vh.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://xk.9csxet.cn

[U114] JS：JSON 深比较
来源：http://lu.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mg.hahajie.cn

[U115] JS：生成 UUID
来源：http://ab.shxzukj.cn

crypto.randomUUID()
来源：http://rp.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://ka.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://mn.hahajie.cn

[U117] JS：单元测试
来源：http://vm.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://cf.muxihuayi.cn

[U118] JS：开发服务器
来源：http://yr.nicolike.cn

npm i -D vite;  npx vite
来源：http://uu.bjjhwx.cn

[U119] JS：生产构建
来源：http://kk.shtwfgs.cn

npx vite build
来源：http://st.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://xz.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://zf.shtwfgs.cn

================================================================================
来源：http://pt.shxzskj.cn

统计汇总
来源：http://cj.shtwfgs.cn

================================================================================
来源：http://en.yuntaijiaju.cn

按语言统计（条）：
来源：http://nj.szsharing.cn

Python ......... 252
来源：http://gk.chemitech.net.cn

PHP ............ 252
来源：http://ef.panjiajie.cn

JavaScript ..... 252
来源：http://ga.gzmigu.cn

TypeScript ..... 212
来源：http://jk.shtwfgs.cn

Java ........... 212
来源：http://jf.colortex.cn

Go ............. 212
来源：http://ed.wgjwhj.cn

Ruby ........... 212
来源：http://cp.hnjuh.cn

C# ............. 212
来源：http://ua.521024.cn


<!-- 参考信息 -->