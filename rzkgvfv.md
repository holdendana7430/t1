代发 wailian999

[T41] Perl：Hello World
来源：http://sg.hahajie.cn

print "Hello\n";
来源：http://wf.huanxung.cn

[T42] Perl：变量类型
来源：http://nd.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sj.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://aq.chemitech.net.cn

"值: $a"
来源：http://qh.newstarts.cn

[T44] Perl：条件
来源：http://xu.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://oi.huanxung.cn

[T45] Perl：数组遍历
来源：http://cz.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://bo.colortex.cn

[T46] Perl：哈希操作
来源：http://ip.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xx.lnxyls.cn

[T47] Perl：正则捕获
来源：http://qy.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rn.jctech888.com.cn

[T48] Perl：正则替换
来源：http://cu.newstarts.cn

$s =~ s/old/new/g;
来源：http://ll.szsharing.cn

[T49] Perl：函数
来源：http://pp.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pg.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://du.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yo.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://xo.panjiajie.cn

[T51] Scala：Hello World
来源：http://hy.bjjhwx.cn

println("Hello")
来源：http://xv.szsharing.cn

[T52] Scala：变量
来源：http://kf.hahajie.cn

val a = 1;  var b = 2
来源：http://rq.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://mc.nicolike.cn

s"值: $b"
来源：http://ad.hahajie.cn

[T54] Scala：集合映射
来源：http://xb.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://de.asd995.cn

[T55] Scala：集合过滤
来源：http://yw.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hg.wgjwhj.cn

[T56] Scala：样例类
来源：http://xz.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://dp.szsharing.cn

[T57] Scala：模式匹配
来源：http://ie.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hh.9csxet.cn

[T58] Scala：函数定义
来源：http://lw.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://to.bjjhwx.cn

[T59] Scala：循环
来源：http://jh.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://ei.huixiangedu.cn

[T60] Scala：折叠
来源：http://tc.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jy.wgjwhj.cn

================================================================================
来源：http://vy.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nm.hahajie.cn

================================================================================
来源：http://xq.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://dp.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rm.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://jn.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dm.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://ga.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ye.hahajie.cn

[U04] Py：变量调试打印
来源：http://tg.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xd.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://ka.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://jg.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://xk.szsharing.cn

{**a, **b}
来源：http://je.nszjky.cn

[U07] Py：反转字典键值
来源：http://br.hahajie.cn

{v: k for k, v in d.items()}
来源：http://fo.nicolike.cn

[U08] Py：展平二维列表
来源：http://vm.shtwfgs.cn

[y for x in nested for y in x]
来源：http://hs.521024.cn

[U09] Py：字典取最大值的键
来源：http://xt.hahajie.cn

max(d, key=d.get)
来源：http://ng.gzmigu.cn

[U10] Py：按值排序字典
来源：http://bq.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jz.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://pl.shxzskj.cn

(x * 2 for x in arr)
来源：http://wz.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rb.521024.cn

Counter(arr).most_common(3)
来源：http://dw.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://js.huixiangedu.cn

deque(maxlen=10)
来源：http://cm.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://xp.shxzskj.cn

defaultdict(list)
来源：http://je.nicolike.cn

[U15] Py：高精度计时
来源：http://qc.huixiangedu.cn

t = time.perf_counter()
来源：http://ip.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://lm.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mu.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://aq.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://wn.newstarts.cn

[U18] Py：预编译正则
来源：http://qh.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://dv.nicolike.cn

[U19] Py：正则替换带回调
来源：http://zx.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yi.nicolike.cn

[U20] Py：缓存函数结果
来源：http://of.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://jt.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://ca.wgjwhj.cn

@contextlib.contextmanager
来源：http://vf.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://hq.shxzskj.cn

list(zip(*m))
来源：http://sn.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://eu.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://an.nicolike.cn

[U24] Py：路径操作
来源：http://gf.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kv.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://lj.huanxung.cn

csv.DictReader(f)
来源：http://ax.521024.cn

[U26] Py：并发下载
来源：http://zi.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nf.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://al.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://ig.muxihuayi.cn

[U28] Py：类型别名
来源：http://kt.hahajie.cn

UserId = int
来源：http://en.hahajie.cn

[U29] Py：属性校验
来源：http://eu.colortex.cn

@property 与 @x.setter 配合
来源：http://db.521024.cn

[U30] Py：数据类
来源：http://xp.521024.cn

@dataclass(slots=True)
来源：http://bt.jianghongdianzi.cn

[U31] Py：单测
来源：http://nj.colortex.cn

python -m pytest -q
来源：http://je.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://ly.colortex.cn

ruff format . && ruff check --fix .
来源：http://vs.bookmarksfly.cn

[U33] Py：打包发布
来源：http://qz.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://hb.shxzukj.cn

[U34] Py：判断编码
来源：http://jf.gzmigu.cn

chardet.detect(raw)
来源：http://zb.colortex.cn

[U35] Py：发送邮件
来源：http://hl.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ba.jctech888.com.cn

[U36] Py：定时任务
来源：http://bh.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://zu.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://nq.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yf.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://vm.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://dj.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://no.9csxet.cn

sys.stdout.isatty()
来源：http://ap.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://lo.hnjuh.cn

print("err", file=sys.stderr)
来源：http://nw.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://uc.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wu.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://je.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sr.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://hx.9csxet.cn

namespace App\Http;
来源：http://hl.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://oc.huanxung.cn

declare(strict_types=1);
来源：http://su.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://my.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bw.wgjwhj.cn

[U46] PHP：可空类型
来源：http://hf.asd995.cn

?string $name = null
来源：http://zf.asd995.cn

[U47] PHP：联合类型
来源：http://ls.gzmigu.cn

int|string $id
来源：http://zr.hnjuh.cn

[U48] PHP：纯枚举
来源：http://vb.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://on.haigaiapp.cn

[U49] PHP：只读属性
来源：http://jm.hnjuh.cn

public readonly string $name
来源：http://hb.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://rd.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://jy.chemitech.net.cn

[U51] PHP：数组解构
来源：http://vg.chemitech.net.cn

[$a, $b] = $arr;
来源：http://kv.newstarts.cn

[U52] PHP：箭头函数
来源：http://oi.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://la.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://fz.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://la.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://nx.chemitech.net.cn

$obj?->method()
来源：http://dw.shxzukj.cn

[U55] PHP：match 表达式
来源：http://vm.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fn.shxzukj.cn

[U56] PHP：命名参数
来源：http://uj.shtwfgs.cn

f(a: 1, b: 2)
来源：http://or.hnjuh.cn

[U57] PHP：字符串插值
来源：http://bv.521024.cn

"值: {$a}"
来源：http://sf.9csxet.cn

[U58] PHP：数组三件套
来源：http://dz.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nc.szxytkj.cn

[U59] PHP：自定义排序
来源：http://gd.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qx.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://kw.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pe.hnjuh.cn

[U61] PHP：正则
来源：http://hu.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cq.wgjwhj.cn

[U62] PHP：日期对象
来源：http://jb.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kw.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ng.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oi.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://qj.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://xd.hnjuh.cn

[U65] PHP：会话
来源：http://zk.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mg.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://de.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sx.hahajie.cn

[U67] PHP：处理文件上传
来源：http://kf.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pv.521024.cn

[U68] PHP：PDO 连接
来源：http://jl.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qq.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://lf.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vf.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://zp.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ka.nicolike.cn

[U71] PHP：抛出异常
来源：http://iu.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://cc.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://uy.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://uc.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://vr.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://px.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://oj.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://hd.shxzukj.cn

[U75] PHP：依赖注入
来源：http://ce.szsharing.cn

composer require psr/container
来源：http://re.colortex.cn

[U76] PHP：简单路由
来源：http://nn.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ws.panjiajie.cn

[U77] PHP：模板渲染
来源：http://xr.chemitech.net.cn

composer require twig/twig
来源：http://rp.nszjky.cn

[U78] PHP：单元测试
来源：http://zs.asd995.cn

composer require --dev phpunit/phpunit
来源：http://og.muxihuayi.cn

[U79] PHP：静态分析
来源：http://db.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://ft.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://el.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lz.szxytkj.cn

[U81] JS：初始化项目
来源：http://ax.wgjwhj.cn

npm init -y;  npm i express
来源：http://zn.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://vv.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://em.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://bs.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ql.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://ts.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rw.bjjhwx.cn

[U85] JS：可选链
来源：http://mw.huixiangedu.cn

a?.b?.c
来源：http://nx.bookmarksfly.cn

[U86] JS：空值合并
来源：http://py.jctech888.com.cn

a ?? b
来源：http://xe.nszjky.cn

[U87] JS：解构默认值
来源：http://mh.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://ps.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://du.huixiangedu.cn

{ ...a, ...b }
来源：http://ca.jctech888.com.cn

[U89] JS：数组去重
来源：http://re.bjjhwx.cn

[...new Set(arr)]
来源：http://xi.asd995.cn

[U90] JS：数字数组排序
来源：http://ox.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://wv.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://is.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jp.hnjuh.cn

[U92] JS：深拷贝
来源：http://bn.colortex.cn

structuredClone(obj)
来源：http://nx.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://kv.bookmarksfly.cn

`共 ${n} 条`
来源：http://ma.szxytkj.cn

[U94] JS：箭头函数
来源：http://ww.jianghongdianzi.cn

const double = x => x * 2;
来源：http://ak.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://do.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://qb.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://sh.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kl.wgjwhj.cn

[U97] JS：并发请求
来源：http://sh.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://br.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://pz.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pq.shxzskj.cn

[U99] JS：事件监听
来源：http://mi.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://py.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://sg.yuexingan06.cn

document.querySelector(".item")
来源：http://tr.hahajie.cn

[U101] JS：classList 操作
来源：http://cy.newstarts.cn

el.classList.toggle("active")
来源：http://ur.bookmarksfly.cn

[U102] JS：本地存储
来源：http://yd.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ll.bjjhwx.cn

[U103] JS：定时器
来源：http://dc.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vk.haigaiapp.cn

[U104] JS：防抖
来源：http://et.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vl.asd995.cn

[U105] JS：节流
来源：http://at.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ht.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://zl.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ub.nicolike.cn

[U107] JS：数字千分位
来源：http://po.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://od.bjjhwx.cn

[U108] JS：随机整数
来源：http://gq.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qb.bookmarksfly.cn

[U109] JS：数组分组
来源：http://zd.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://nh.nszjky.cn

[U110] JS：数组分块
来源：http://xi.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ed.huanxung.cn

[U111] JS：对象转 Map
来源：http://om.asd995.cn

new Map(Object.entries(obj))
来源：http://ng.newstarts.cn

[U112] JS：字符串补位
来源：http://uf.huanxung.cn

"7".padStart(3, "0")
来源：http://yo.521024.cn

[U113] JS：正则替换全部
来源：http://wk.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://ar.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://fv.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://er.gzmigu.cn

[U115] JS：生成 UUID
来源：http://vy.lnxyls.cn

crypto.randomUUID()
来源：http://wj.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://lo.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://xq.521024.cn

[U117] JS：单元测试
来源：http://sn.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://ef.chemitech.net.cn

[U118] JS：开发服务器
来源：http://pz.gzmigu.cn

npm i -D vite;  npx vite
来源：http://ou.jctech888.com.cn

[U119] JS：生产构建
来源：http://qk.shtwfgs.cn

npx vite build
来源：http://ac.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://kb.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://fi.szsharing.cn

================================================================================
来源：http://td.nszjky.cn

统计汇总
来源：http://wf.panjiajie.cn

================================================================================
来源：http://nl.newstarts.cn

按语言统计（条）：
来源：http://vt.asd995.cn

Python ......... 252
来源：http://go.panjiajie.cn

PHP ............ 252
来源：http://id.newstarts.cn

JavaScript ..... 252
来源：http://ts.haigaiapp.cn

TypeScript ..... 212
来源：http://ct.muxihuayi.cn

Java ........... 212
来源：http://os.chemitech.net.cn

Go ............. 212
来源：http://gg.yuntaijiaju.cn

Ruby ........... 212
来源：http://az.jctech888.com.cn

C# ............. 212
来源：http://oo.chemitech.net.cn

C .............. 30
来源：http://mr.asd995.cn

C++ ............ 30
来源：http://ts.huanxung.cn

SQL ............ 90
来源：http://th.521024.cn

Bash ........... 80
来源：http://zo.colortex.cn


<!-- 参考信息 -->