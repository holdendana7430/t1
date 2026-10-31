代发 wailian999

[T19] Swift：可选绑定
来源：http://eb.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ec.9csxet.cn

[T20] Swift：数组操作
来源：http://zt.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ex.shxzukj.cn

[T21] Swift：遍历
来源：http://xj.521024.cn

for x in a { print(x) }
来源：http://pj.521024.cn

[T22] Swift：字典
来源：http://co.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ef.chemitech.net.cn

[T23] Swift：函数
来源：http://xh.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pm.colortex.cn

[T24] Swift：闭包
来源：http://ij.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kr.yuexingan06.cn

[T25] Swift：结构体
来源：http://iu.jianghongdianzi.cn

struct P { var x: Int }
来源：http://sj.asd995.cn

[T26] Swift：类与重写
来源：http://ea.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://jv.colortex.cn

[T27] Swift：错误处理
来源：http://jx.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ot.hahajie.cn

[T28] Swift：枚举
来源：http://wd.asd995.cn

enum Color { case red, green }
来源：http://dn.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://bc.jctech888.com.cn

guard let x = opt else { return }
来源：http://th.wgjwhj.cn

[T30] Swift：协议
来源：http://iv.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://kc.wgjwhj.cn

[T31] Lua：Hello World
来源：http://dd.521024.cn

print("Hello")
来源：http://zg.hahajie.cn

[T32] Lua：局部变量
来源：http://gk.jianghongdianzi.cn

local a = 1
来源：http://uu.szxytkj.cn

[T33] Lua：表（数组）
来源：http://wd.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://py.521024.cn

[T34] Lua：遍历表
来源：http://ah.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://em.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://rm.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://dv.nszjky.cn

[T36] Lua：函数
来源：http://vc.panjiajie.cn

function add(a, b) return a + b end
来源：http://ah.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://dh.chemitech.net.cn

"a" .. "b"
来源：http://gw.huanxung.cn

[T38] Lua：条件
来源：http://qx.shtwfgs.cn

if x > 0 then print("正") end
来源：http://ne.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://oq.nszjky.cn

string.find(s, "%d+")
来源：http://jc.huixiangedu.cn

[T40] Lua：元表
来源：http://wd.asd995.cn

setmetatable({}, { __index = base })
来源：http://ff.yuexingan06.cn

[T41] Perl：Hello World
来源：http://id.9csxet.cn

print "Hello\n";
来源：http://kd.hahajie.cn

[T42] Perl：变量类型
来源：http://ky.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fo.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://dj.szxytkj.cn

"值: $a"
来源：http://jd.bjjhwx.cn

[T44] Perl：条件
来源：http://kr.colortex.cn

if ($a > 0) { print "正"; }
来源：http://wy.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://wi.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://cm.nicolike.cn

[T46] Perl：哈希操作
来源：http://lv.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sx.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://zr.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dk.yuexingan06.cn

[T48] Perl：正则替换
来源：http://mq.szxytkj.cn

$s =~ s/old/new/g;
来源：http://ji.shxzskj.cn

[T49] Perl：函数
来源：http://kd.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vo.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://hs.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ak.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://yt.shxzukj.cn

[T51] Scala：Hello World
来源：http://ub.nicolike.cn

println("Hello")
来源：http://xh.szsharing.cn

[T52] Scala：变量
来源：http://og.shxzukj.cn

val a = 1;  var b = 2
来源：http://gy.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://uk.colortex.cn

s"值: $b"
来源：http://jn.521024.cn

[T54] Scala：集合映射
来源：http://xk.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://mx.nicolike.cn

[T55] Scala：集合过滤
来源：http://te.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kd.shxzskj.cn

[T56] Scala：样例类
来源：http://vi.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://sc.lnxyls.cn

[T57] Scala：模式匹配
来源：http://qy.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sc.chemitech.net.cn

[T58] Scala：函数定义
来源：http://do.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://px.huanxung.cn

[T59] Scala：循环
来源：http://xs.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://gf.haigaiapp.cn

[T60] Scala：折叠
来源：http://pl.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sg.yuexingan06.cn

================================================================================
来源：http://tt.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yz.yuntaijiaju.cn

================================================================================
来源：http://gc.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://vy.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://br.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://fm.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cf.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://bu.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pq.gzmigu.cn

[U04] Py：变量调试打印
来源：http://bm.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pp.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://hz.9csxet.cn

list(dict.fromkeys(arr))
来源：http://vc.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://el.yuexingan06.cn

{**a, **b}
来源：http://mn.9csxet.cn

[U07] Py：反转字典键值
来源：http://wd.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://ur.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://uh.szxytkj.cn

[y for x in nested for y in x]
来源：http://jj.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://fe.wgjwhj.cn

max(d, key=d.get)
来源：http://ox.nicolike.cn

[U10] Py：按值排序字典
来源：http://gw.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vj.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://rh.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://pu.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tn.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://wj.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ob.hnjuh.cn

deque(maxlen=10)
来源：http://fy.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://wv.yuntaijiaju.cn

defaultdict(list)
来源：http://rj.521024.cn

[U15] Py：高精度计时
来源：http://lr.szsharing.cn

t = time.perf_counter()
来源：http://hv.9csxet.cn

[U16] Py：命令行参数解析
来源：http://qa.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gb.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://ok.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ql.huixiangedu.cn

[U18] Py：预编译正则
来源：http://ys.huanxung.cn

pat = re.compile(r"\d+")
来源：http://km.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://nh.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xv.nszjky.cn

[U20] Py：缓存函数结果
来源：http://mq.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://gq.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://yv.chemitech.net.cn

@contextlib.contextmanager
来源：http://bo.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://mt.shxzskj.cn

list(zip(*m))
来源：http://up.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ir.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tk.panjiajie.cn

[U24] Py：路径操作
来源：http://dy.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xn.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://tb.newstarts.cn

csv.DictReader(f)
来源：http://tc.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://je.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fw.huanxung.cn

[U27] Py：异步 HTTP
来源：http://uy.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://rr.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://uu.jctech888.com.cn

UserId = int
来源：http://mv.wgjwhj.cn

[U29] Py：属性校验
来源：http://rh.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://wr.gzmigu.cn

[U30] Py：数据类
来源：http://jh.bookmarksfly.cn

@dataclass(slots=True)
来源：http://ri.shtwfgs.cn

[U31] Py：单测
来源：http://od.wgjwhj.cn

python -m pytest -q
来源：http://wl.gzmigu.cn

[U32] Py：代码格式化
来源：http://jf.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://yc.bjjhwx.cn

[U33] Py：打包发布
来源：http://yl.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://ey.wgjwhj.cn

[U34] Py：判断编码
来源：http://mg.asd995.cn

chardet.detect(raw)
来源：http://lq.szsharing.cn

[U35] Py：发送邮件
来源：http://xr.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qr.huixiangedu.cn

[U36] Py：定时任务
来源：http://hk.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://rm.colortex.cn

[U37] Py：读写 Excel
来源：http://aq.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yi.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://ah.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://rd.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://bb.haigaiapp.cn

sys.stdout.isatty()
来源：http://az.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://mz.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://sx.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://oz.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nb.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://sh.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ke.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://uo.shtwfgs.cn

namespace App\Http;
来源：http://kv.9csxet.cn

[U44] PHP：开启严格类型
来源：http://iy.bjjhwx.cn

declare(strict_types=1);
来源：http://jw.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://lm.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xp.bjjhwx.cn

[U46] PHP：可空类型
来源：http://ti.lnxyls.cn

?string $name = null
来源：http://wu.yuexingan06.cn

[U47] PHP：联合类型
来源：http://wb.szsharing.cn

int|string $id
来源：http://gi.colortex.cn

[U48] PHP：纯枚举
来源：http://gm.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dw.jctech888.com.cn

[U49] PHP：只读属性
来源：http://hd.szsharing.cn

public readonly string $name
来源：http://fq.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://sk.gzmigu.cn

public function __construct(private int $id) {}
来源：http://rk.hnjuh.cn

[U51] PHP：数组解构
来源：http://gx.hahajie.cn

[$a, $b] = $arr;
来源：http://bt.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://pc.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://xp.huanxung.cn

[U53] PHP：空合并运算符
来源：http://vi.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://go.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://lz.huixiangedu.cn

$obj?->method()
来源：http://hp.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://sh.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yw.lnxyls.cn

[U56] PHP：命名参数
来源：http://hh.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://zj.szsharing.cn

[U57] PHP：字符串插值
来源：http://jj.newstarts.cn

"值: {$a}"
来源：http://fd.newstarts.cn

[U58] PHP：数组三件套
来源：http://io.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://th.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ly.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sz.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://vp.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xr.huixinmuqiang.cn

[U61] PHP：正则
来源：http://rm.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rn.szxytkj.cn

[U62] PHP：日期对象
来源：http://gg.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xc.yuexingan06.cn

[U63] PHP：文件读写
来源：http://bc.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://im.szsharing.cn

[U64] PHP：目录遍历
来源：http://xj.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://ca.yuntaijiaju.cn

[U65] PHP：会话
来源：http://dv.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fr.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://pg.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ap.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://mr.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vp.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://nv.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gu.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://ls.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qk.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://ng.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ep.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://gy.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://lb.nicolike.cn

[U72] PHP：写错误日志
来源：http://sg.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://nd.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://ao.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://zp.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://qu.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://nx.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://de.bjjhwx.cn

composer require psr/container
来源：http://kg.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ha.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nu.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://eh.hnjuh.cn

composer require twig/twig
来源：http://pv.shxzskj.cn

[U78] PHP：单元测试
来源：http://hy.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://fv.shtwfgs.cn

[U79] PHP：静态分析
来源：http://pm.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://et.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://vm.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vn.muxihuayi.cn

[U81] JS：初始化项目
来源：http://nd.wgjwhj.cn

npm init -y;  npm i express
来源：http://ci.colortex.cn

[U82] JS：package.json 脚本
来源：http://lr.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://go.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://nk.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wv.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://sw.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ng.wgjwhj.cn

[U85] JS：可选链
来源：http://jb.shtwfgs.cn

a?.b?.c
来源：http://fb.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://ax.huixinmuqiang.cn

a ?? b
来源：http://pa.huixiangedu.cn

[U87] JS：解构默认值
来源：http://kq.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://tb.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://zu.jctech888.com.cn

{ ...a, ...b }
来源：http://id.asd995.cn

[U89] JS：数组去重
来源：http://tg.jianghongdianzi.cn

[...new Set(arr)]
来源：http://wn.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://qp.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://zd.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://yl.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dj.asd995.cn

[U92] JS：深拷贝
来源：http://ks.szsharing.cn

structuredClone(obj)
来源：http://pi.newstarts.cn

[U93] JS：模板字符串
来源：http://al.shtwfgs.cn

`共 ${n} 条`
来源：http://xq.panjiajie.cn

[U94] JS：箭头函数
来源：http://eq.shxzskj.cn

const double = x => x * 2;
来源：http://eg.hnjuh.cn

[U95] JS：Promise 包装
来源：http://wo.colortex.cn

new Promise((resolve, reject) => {})
来源：http://ex.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://pg.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ko.bookmarksfly.cn

[U97] JS：并发请求
来源：http://fr.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tb.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://pl.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zv.bjjhwx.cn

[U99] JS：事件监听
来源：http://hq.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://sh.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://mm.521024.cn

document.querySelector(".item")
来源：http://hf.gzmigu.cn

[U101] JS：classList 操作
来源：http://rv.yuexingan06.cn

el.classList.toggle("active")
来源：http://eq.521024.cn

[U102] JS：本地存储
来源：http://vq.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://li.haigaiapp.cn

[U103] JS：定时器
来源：http://ut.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zl.chemitech.net.cn

[U104] JS：防抖
来源：http://df.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xm.521024.cn

[U105] JS：节流
来源：http://nz.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://us.asd995.cn

[U106] JS：日期格式化
来源：http://cq.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://et.haigaiapp.cn


<!-- 参考信息 -->