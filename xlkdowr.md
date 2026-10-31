代发 wailian999

[T41] Perl：Hello World
来源：http://rb.hahajie.cn

print "Hello\n";
来源：http://ll.9csxet.cn

[T42] Perl：变量类型
来源：http://gr.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mn.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://nb.yuntaijiaju.cn

"值: $a"
来源：http://jw.newstarts.cn

[T44] Perl：条件
来源：http://ic.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://dp.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://sw.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://up.panjiajie.cn

[T46] Perl：哈希操作
来源：http://up.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ek.shxzukj.cn

[T47] Perl：正则捕获
来源：http://zs.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wd.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://ag.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://ek.panjiajie.cn

[T49] Perl：函数
来源：http://rb.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xh.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://nh.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mp.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://gy.wgjwhj.cn

[T51] Scala：Hello World
来源：http://vb.huanxung.cn

println("Hello")
来源：http://xj.wgjwhj.cn

[T52] Scala：变量
来源：http://ig.gzmigu.cn

val a = 1;  var b = 2
来源：http://cg.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://gd.chemitech.net.cn

s"值: $b"
来源：http://mc.wgjwhj.cn

[T54] Scala：集合映射
来源：http://tv.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://bm.huanxung.cn

[T55] Scala：集合过滤
来源：http://aw.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xn.asd995.cn

[T56] Scala：样例类
来源：http://ff.521024.cn

case class User(name: String, age: Int)
来源：http://kd.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://cq.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ng.shxzukj.cn

[T58] Scala：函数定义
来源：http://op.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tj.szsharing.cn

[T59] Scala：循环
来源：http://cu.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://ek.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://zf.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lu.wgjwhj.cn

================================================================================
来源：http://aj.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mn.hnjuh.cn

================================================================================
来源：http://ww.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://ch.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dp.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://ty.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ts.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://jq.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mn.shxzukj.cn

[U04] Py：变量调试打印
来源：http://pl.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://se.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://ie.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://py.nszjky.cn

[U06] Py：合并两个字典
来源：http://gd.huixinmuqiang.cn

{**a, **b}
来源：http://uh.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://cq.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://mm.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://ix.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://bz.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://vk.haigaiapp.cn

max(d, key=d.get)
来源：http://ht.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://ha.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vm.nicolike.cn

[U11] Py：生成器表达式
来源：http://kk.hnjuh.cn

(x * 2 for x in arr)
来源：http://hp.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://um.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://bk.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ja.shtwfgs.cn

deque(maxlen=10)
来源：http://nl.colortex.cn

[U14] Py：分组收集到列表
来源：http://eg.nszjky.cn

defaultdict(list)
来源：http://fp.521024.cn

[U15] Py：高精度计时
来源：http://lv.huixinmuqiang.cn

t = time.perf_counter()
来源：http://ly.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://ap.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kk.huixiangedu.cn

[U17] Py：初始化日志
来源：http://sg.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ei.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://mh.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://pt.huanxung.cn

[U19] Py：正则替换带回调
来源：http://ml.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yk.colortex.cn

[U20] Py：缓存函数结果
来源：http://pt.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://gu.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://fx.shtwfgs.cn

@contextlib.contextmanager
来源：http://qn.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://vi.gzmigu.cn

list(zip(*m))
来源：http://dz.521024.cn

[U23] Py：分块读取大文件
来源：http://nx.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qc.bookmarksfly.cn

[U24] Py：路径操作
来源：http://ry.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://km.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://px.shxzukj.cn

csv.DictReader(f)
来源：http://hm.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://zr.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jx.nszjky.cn

[U27] Py：异步 HTTP
来源：http://ka.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://wz.huixiangedu.cn

[U28] Py：类型别名
来源：http://gl.521024.cn

UserId = int
来源：http://qn.asd995.cn

[U29] Py：属性校验
来源：http://dl.panjiajie.cn

@property 与 @x.setter 配合
来源：http://rm.muxihuayi.cn

[U30] Py：数据类
来源：http://zi.wgjwhj.cn

@dataclass(slots=True)
来源：http://fn.shtwfgs.cn

[U31] Py：单测
来源：http://rz.szxytkj.cn

python -m pytest -q
来源：http://so.yuexingan06.cn

[U32] Py：代码格式化
来源：http://pm.521024.cn

ruff format . && ruff check --fix .
来源：http://cl.haigaiapp.cn

[U33] Py：打包发布
来源：http://ps.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://by.newstarts.cn

[U34] Py：判断编码
来源：http://kx.jianghongdianzi.cn

chardet.detect(raw)
来源：http://vm.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://ab.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vk.lnxyls.cn

[U36] Py：定时任务
来源：http://pa.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://fm.521024.cn

[U37] Py：读写 Excel
来源：http://vq.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://og.521024.cn

[U38] Py：获取脚本所在目录
来源：http://vn.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ek.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://hf.newstarts.cn

sys.stdout.isatty()
来源：http://pl.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://oj.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://pn.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://hq.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uc.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://nw.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uf.9csxet.cn

[U43] PHP：声明命名空间
来源：http://xz.newstarts.cn

namespace App\Http;
来源：http://ya.nicolike.cn

[U44] PHP：开启严格类型
来源：http://xs.shxzukj.cn

declare(strict_types=1);
来源：http://do.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://qa.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.shtwfgs.cn

[U46] PHP：可空类型
来源：http://rt.yuntaijiaju.cn

?string $name = null
来源：http://ip.colortex.cn

[U47] PHP：联合类型
来源：http://qi.haigaiapp.cn

int|string $id
来源：http://fs.hnjuh.cn

[U48] PHP：纯枚举
来源：http://fk.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bk.shtwfgs.cn

[U49] PHP：只读属性
来源：http://ji.nicolike.cn

public readonly string $name
来源：http://wa.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://bc.huanxung.cn

public function __construct(private int $id) {}
来源：http://mu.jctech888.com.cn

[U51] PHP：数组解构
来源：http://cb.hnjuh.cn

[$a, $b] = $arr;
来源：http://jh.colortex.cn

[U52] PHP：箭头函数
来源：http://es.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://ji.huanxung.cn

[U53] PHP：空合并运算符
来源：http://lu.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://cu.huanxung.cn

[U54] PHP：空安全调用
来源：http://rh.hahajie.cn

$obj?->method()
来源：http://zr.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ue.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jw.panjiajie.cn

[U56] PHP：命名参数
来源：http://ft.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://sm.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://ib.panjiajie.cn

"值: {$a}"
来源：http://em.9csxet.cn

[U58] PHP：数组三件套
来源：http://ri.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ja.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://fp.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://si.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://ks.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://er.panjiajie.cn

[U61] PHP：正则
来源：http://kp.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vv.nicolike.cn

[U62] PHP：日期对象
来源：http://fn.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gi.colortex.cn

[U63] PHP：文件读写
来源：http://sr.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nh.gzmigu.cn

[U64] PHP：目录遍历
来源：http://vm.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://na.bjjhwx.cn

[U65] PHP：会话
来源：http://bw.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uk.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://fb.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://az.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://ut.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cg.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://et.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xb.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://gx.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qd.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://kz.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://id.lnxyls.cn

[U71] PHP：抛出异常
来源：http://oi.521024.cn

throw new RuntimeException("失败", 500);
来源：http://gk.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://cv.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://pl.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://ib.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://pd.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://fl.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://ct.hahajie.cn

[U75] PHP：依赖注入
来源：http://jh.yuntaijiaju.cn

composer require psr/container
来源：http://ms.colortex.cn

[U76] PHP：简单路由
来源：http://qe.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ee.newstarts.cn

[U77] PHP：模板渲染
来源：http://qs.szsharing.cn

composer require twig/twig
来源：http://ze.shxzskj.cn

[U78] PHP：单元测试
来源：http://om.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://hr.nicolike.cn

[U79] PHP：静态分析
来源：http://kv.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://qg.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://wi.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zr.muxihuayi.cn

[U81] JS：初始化项目
来源：http://qd.hnjuh.cn

npm init -y;  npm i express
来源：http://hh.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://oj.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kj.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://nh.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zd.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://th.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dl.chemitech.net.cn

[U85] JS：可选链
来源：http://sx.jianghongdianzi.cn

a?.b?.c
来源：http://tm.shtwfgs.cn

[U86] JS：空值合并
来源：http://wv.nicolike.cn

a ?? b
来源：http://xg.nszjky.cn

[U87] JS：解构默认值
来源：http://ok.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://qy.asd995.cn

[U88] JS：对象展开合并
来源：http://ff.nszjky.cn

{ ...a, ...b }
来源：http://nn.szxytkj.cn

[U89] JS：数组去重
来源：http://wj.nszjky.cn

[...new Set(arr)]
来源：http://tw.szsharing.cn

[U90] JS：数字数组排序
来源：http://kr.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://mb.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://dl.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gc.muxihuayi.cn

[U92] JS：深拷贝
来源：http://rf.huixinmuqiang.cn

structuredClone(obj)
来源：http://vy.shtwfgs.cn

[U93] JS：模板字符串
来源：http://am.panjiajie.cn

`共 ${n} 条`
来源：http://vc.nicolike.cn

[U94] JS：箭头函数
来源：http://qw.huixiangedu.cn

const double = x => x * 2;
来源：http://rm.gzmigu.cn

[U95] JS：Promise 包装
来源：http://xx.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://wf.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://pj.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sn.nicolike.cn

[U97] JS：并发请求
来源：http://fu.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://tv.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sf.huanxung.cn

[U99] JS：事件监听
来源：http://wa.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://sg.521024.cn

[U100] JS：DOM 查询
来源：http://ej.huixinmuqiang.cn

document.querySelector(".item")
来源：http://yg.shtwfgs.cn

[U101] JS：classList 操作
来源：http://jg.521024.cn

el.classList.toggle("active")
来源：http://cm.nicolike.cn

[U102] JS：本地存储
来源：http://jh.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ha.521024.cn

[U103] JS：定时器
来源：http://kg.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hf.huanxung.cn

[U104] JS：防抖
来源：http://hu.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yj.gzmigu.cn

[U105] JS：节流
来源：http://iw.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hn.szxytkj.cn

[U106] JS：日期格式化
来源：http://xu.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vs.szxytkj.cn

[U107] JS：数字千分位
来源：http://ts.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://km.9csxet.cn

[U108] JS：随机整数
来源：http://se.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vz.shxzukj.cn

[U109] JS：数组分组
来源：http://gx.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://ey.gzmigu.cn

[U110] JS：数组分块
来源：http://ez.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nj.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://xs.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://qw.huixiangedu.cn

[U112] JS：字符串补位
来源：http://tu.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://mq.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://ha.9csxet.cn

s.replaceAll("a", "b")
来源：http://cs.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://uh.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hy.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://qm.haigaiapp.cn

crypto.randomUUID()
来源：http://hd.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://wp.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://yh.huanxung.cn

[U117] JS：单元测试
来源：http://mn.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://yh.wgjwhj.cn

[U118] JS：开发服务器
来源：http://on.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://ln.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://nh.yuexingan06.cn

npx vite build
来源：http://vk.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ua.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://tm.shxzukj.cn

================================================================================
来源：http://py.gzmigu.cn

统计汇总
来源：http://zu.521024.cn

================================================================================
来源：http://ua.nicolike.cn

按语言统计（条）：
来源：http://iy.hnjuh.cn

Python ......... 252
来源：http://kp.521024.cn

PHP ............ 252
来源：http://xy.jianghongdianzi.cn

JavaScript ..... 252
来源：http://td.chemitech.net.cn

TypeScript ..... 212
来源：http://ko.panjiajie.cn

Java ........... 212
来源：http://bf.bjjhwx.cn

Go ............. 212
来源：http://pt.huixiangedu.cn

Ruby ........... 212
来源：http://ha.gzmigu.cn

C# ............. 212
来源：http://nw.yuntaijiaju.cn

C .............. 30
来源：http://qq.hahajie.cn

C++ ............ 30
来源：http://pj.panjiajie.cn

SQL ............ 90
来源：http://np.szsharing.cn

Bash ........... 80
来源：http://ji.shxzskj.cn


<!-- 参考信息 -->