代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://wv.shtwfgs.cn

[S59] C++：静态断言
来源：http://uc.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gm.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://vk.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mk.shtwfgs.cn

================================================================================
来源：http://bj.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tt.huixiangedu.cn

================================================================================
来源：http://hj.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://ne.yuntaijiaju.cn

println("Hello")
来源：http://mk.huanxung.cn

[T02] Kotlin：变量
来源：http://gh.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vh.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://be.gzmigu.cn

"值: $b"
来源：http://zd.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://oy.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://wi.asd995.cn

[T05] Kotlin：when 表达式
来源：http://an.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qk.nszjky.cn

[T06] Kotlin：集合映射
来源：http://cd.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fm.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://jv.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://od.newstarts.cn

[T08] Kotlin：数据类
来源：http://en.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://xs.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://kr.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ue.newstarts.cn

[T10] Kotlin：默认参数
来源：http://mu.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sc.hahajie.cn

[T11] Kotlin：协程
来源：http://oy.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kf.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://zi.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://np.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://jr.hahajie.cn

val m = mapOf("a" to 1)
来源：http://eh.nicolike.cn

[T14] Kotlin：循环
来源：http://pt.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://vi.jctech888.com.cn

[T15] Kotlin：接口
来源：http://sk.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://nr.huixiangedu.cn

[T16] Swift：Hello World
来源：http://oj.huixinmuqiang.cn

print("Hello")
来源：http://nu.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://al.9csxet.cn

var a = 1;  let b = 2
来源：http://dp.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://lz.hnjuh.cn

"值: \(b)"
来源：http://af.panjiajie.cn

[T19] Swift：可选绑定
来源：http://am.9csxet.cn

if let n = opt { print(n) }
来源：http://rw.shxzskj.cn

[T20] Swift：数组操作
来源：http://aw.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wf.shxzskj.cn

[T21] Swift：遍历
来源：http://di.jianghongdianzi.cn

for x in a { print(x) }
来源：http://wc.huixiangedu.cn

[T22] Swift：字典
来源：http://wb.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lj.bjjhwx.cn

[T23] Swift：函数
来源：http://ux.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ti.gzmigu.cn

[T24] Swift：闭包
来源：http://ek.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pt.hnjuh.cn

[T25] Swift：结构体
来源：http://tc.haigaiapp.cn

struct P { var x: Int }
来源：http://ef.huixiangedu.cn

[T26] Swift：类与重写
来源：http://et.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://vp.jctech888.com.cn

[T27] Swift：错误处理
来源：http://wv.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://an.panjiajie.cn

[T28] Swift：枚举
来源：http://ch.bookmarksfly.cn

enum Color { case red, green }
来源：http://fv.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://sv.haigaiapp.cn

guard let x = opt else { return }
来源：http://ss.chemitech.net.cn

[T30] Swift：协议
来源：http://bg.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://sy.panjiajie.cn

[T31] Lua：Hello World
来源：http://uv.huixinmuqiang.cn

print("Hello")
来源：http://on.nicolike.cn

[T32] Lua：局部变量
来源：http://yn.asd995.cn

local a = 1
来源：http://bn.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://qi.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fz.panjiajie.cn

[T34] Lua：遍历表
来源：http://tn.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nl.hnjuh.cn

[T35] Lua：字典表
来源：http://wu.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://xj.gzmigu.cn

[T36] Lua：函数
来源：http://mq.hahajie.cn

function add(a, b) return a + b end
来源：http://ts.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://pj.shxzskj.cn

"a" .. "b"
来源：http://wu.shxzskj.cn

[T38] Lua：条件
来源：http://rv.szxytkj.cn

if x > 0 then print("正") end
来源：http://dy.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://he.shtwfgs.cn

string.find(s, "%d+")
来源：http://vj.521024.cn

[T40] Lua：元表
来源：http://kz.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://um.bjjhwx.cn

[T41] Perl：Hello World
来源：http://gb.lnxyls.cn

print "Hello\n";
来源：http://wo.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://iv.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://et.nszjky.cn

[T43] Perl：字符串插值
来源：http://vv.521024.cn

"值: $a"
来源：http://xg.jctech888.com.cn

[T44] Perl：条件
来源：http://fr.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://wn.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://lz.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://bw.nicolike.cn

[T46] Perl：哈希操作
来源：http://qg.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kr.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ym.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://su.jctech888.com.cn

[T48] Perl：正则替换
来源：http://bt.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://su.hahajie.cn

[T49] Perl：函数
来源：http://xv.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vx.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://vc.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hj.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://rq.shtwfgs.cn

[T51] Scala：Hello World
来源：http://lf.huanxung.cn

println("Hello")
来源：http://gz.szsharing.cn

[T52] Scala：变量
来源：http://ls.hnjuh.cn

val a = 1;  var b = 2
来源：http://rj.panjiajie.cn

[T53] Scala：字符串插值
来源：http://nb.asd995.cn

s"值: $b"
来源：http://ml.hnjuh.cn

[T54] Scala：集合映射
来源：http://iy.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://iz.colortex.cn

[T55] Scala：集合过滤
来源：http://rz.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uy.nszjky.cn

[T56] Scala：样例类
来源：http://up.lnxyls.cn

case class User(name: String, age: Int)
来源：http://ko.hnjuh.cn

[T57] Scala：模式匹配
来源：http://xw.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bp.shtwfgs.cn

[T58] Scala：函数定义
来源：http://bn.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gk.521024.cn

[T59] Scala：循环
来源：http://ph.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://oy.newstarts.cn

[T60] Scala：折叠
来源：http://bw.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hj.9csxet.cn

================================================================================
来源：http://mi.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lm.9csxet.cn

================================================================================
来源：http://lc.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://nw.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pl.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://dd.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yh.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://ca.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tk.nicolike.cn

[U04] Py：变量调试打印
来源：http://zd.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eb.szsharing.cn

[U05] Py：列表去重且保序
来源：http://wc.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://aa.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://mz.hnjuh.cn

{**a, **b}
来源：http://qu.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://yw.newstarts.cn

{v: k for k, v in d.items()}
来源：http://ev.gzmigu.cn

[U08] Py：展平二维列表
来源：http://mu.nicolike.cn

[y for x in nested for y in x]
来源：http://tq.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://co.haigaiapp.cn

max(d, key=d.get)
来源：http://co.hahajie.cn

[U10] Py：按值排序字典
来源：http://gx.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://co.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://bt.jctech888.com.cn

(x * 2 for x in arr)
来源：http://ov.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xb.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://au.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://hz.nicolike.cn

deque(maxlen=10)
来源：http://ce.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://mp.huanxung.cn

defaultdict(list)
来源：http://sl.nicolike.cn

[U15] Py：高精度计时
来源：http://qm.nszjky.cn

t = time.perf_counter()
来源：http://bm.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://lc.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gw.nszjky.cn

[U17] Py：初始化日志
来源：http://pi.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://dy.wgjwhj.cn

[U18] Py：预编译正则
来源：http://cx.hahajie.cn

pat = re.compile(r"\d+")
来源：http://il.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://cu.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fr.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://sw.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ln.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://wj.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://kn.nszjky.cn

[U22] Py：矩阵转置
来源：http://xz.newstarts.cn

list(zip(*m))
来源：http://sj.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://kd.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gn.huanxung.cn

[U24] Py：路径操作
来源：http://uk.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zj.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://pi.521024.cn

csv.DictReader(f)
来源：http://sf.newstarts.cn

[U26] Py：并发下载
来源：http://lx.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kp.nicolike.cn

[U27] Py：异步 HTTP
来源：http://pg.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://wt.panjiajie.cn

[U28] Py：类型别名
来源：http://uj.wgjwhj.cn

UserId = int
来源：http://sk.muxihuayi.cn

[U29] Py：属性校验
来源：http://ki.lnxyls.cn

@property 与 @x.setter 配合
来源：http://xz.asd995.cn

[U30] Py：数据类
来源：http://ip.yuexingan06.cn

@dataclass(slots=True)
来源：http://bm.asd995.cn

[U31] Py：单测
来源：http://wh.newstarts.cn

python -m pytest -q
来源：http://um.nszjky.cn

[U32] Py：代码格式化
来源：http://zq.9csxet.cn

ruff format . && ruff check --fix .
来源：http://cg.jctech888.com.cn

[U33] Py：打包发布
来源：http://qq.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://uo.haigaiapp.cn

[U34] Py：判断编码
来源：http://hi.panjiajie.cn

chardet.detect(raw)
来源：http://zq.wgjwhj.cn

[U35] Py：发送邮件
来源：http://uv.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jx.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://dn.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://mn.szxytkj.cn

[U37] Py：读写 Excel
来源：http://gb.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tf.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://dq.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ip.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ns.haigaiapp.cn

sys.stdout.isatty()
来源：http://ia.newstarts.cn

[U40] Py：打印到标准错误
来源：http://mo.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://dh.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://em.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cn.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://jr.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hy.huanxung.cn

[U43] PHP：声明命名空间
来源：http://nb.gzmigu.cn

namespace App\Http;
来源：http://we.colortex.cn

[U44] PHP：开启严格类型
来源：http://oi.9csxet.cn

declare(strict_types=1);
来源：http://jn.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://hn.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://au.yuexingan06.cn

[U46] PHP：可空类型
来源：http://ig.bookmarksfly.cn

?string $name = null
来源：http://gk.huixiangedu.cn

[U47] PHP：联合类型
来源：http://xp.szsharing.cn

int|string $id
来源：http://zs.asd995.cn

[U48] PHP：纯枚举
来源：http://qs.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://au.nicolike.cn

[U49] PHP：只读属性
来源：http://en.szsharing.cn

public readonly string $name
来源：http://zl.521024.cn

[U50] PHP：构造器属性提升
来源：http://gv.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://cf.hahajie.cn

[U51] PHP：数组解构
来源：http://ki.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ok.nicolike.cn

[U52] PHP：箭头函数
来源：http://cs.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://jf.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://pb.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://sp.colortex.cn

[U54] PHP：空安全调用
来源：http://li.lnxyls.cn

$obj?->method()
来源：http://nb.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://jy.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qp.szsharing.cn

[U56] PHP：命名参数
来源：http://df.panjiajie.cn

f(a: 1, b: 2)
来源：http://lz.lnxyls.cn

[U57] PHP：字符串插值
来源：http://nn.newstarts.cn

"值: {$a}"
来源：http://xf.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://sj.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://th.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://nx.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oy.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://tj.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qf.hahajie.cn

[U61] PHP：正则
来源：http://qu.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wq.gzmigu.cn

[U62] PHP：日期对象
来源：http://hm.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qb.wgjwhj.cn

[U63] PHP：文件读写
来源：http://ah.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gq.panjiajie.cn

[U64] PHP：目录遍历
来源：http://no.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://vv.shxzskj.cn

[U65] PHP：会话
来源：http://tv.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bx.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://rt.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lz.hahajie.cn

[U67] PHP：处理文件上传
来源：http://gr.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://el.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://fj.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ji.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://rh.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iw.hahajie.cn

[U70] PHP：PDO 事务
来源：http://at.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jy.hahajie.cn

[U71] PHP：抛出异常
来源：http://ss.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://qk.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://yj.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://ic.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://ly.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://cy.colortex.cn

[U74] PHP：读取环境变量
来源：http://hj.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://ai.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://kt.yuntaijiaju.cn

composer require psr/container
来源：http://ip.muxihuayi.cn

[U76] PHP：简单路由
来源：http://hs.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ph.nszjky.cn

[U77] PHP：模板渲染
来源：http://hm.9csxet.cn

composer require twig/twig
来源：http://fd.521024.cn

[U78] PHP：单元测试
来源：http://fc.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://sp.shtwfgs.cn

[U79] PHP：静态分析
来源：http://tu.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://zt.hahajie.cn

[U80] PHP：代码规范修复
来源：http://od.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rh.chemitech.net.cn

[U81] JS：初始化项目
来源：http://jw.hahajie.cn

npm init -y;  npm i express
来源：http://ft.nszjky.cn

[U82] JS：package.json 脚本
来源：http://aq.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ns.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://ys.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qk.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://ft.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lz.huixiangedu.cn


<!-- 参考信息 -->