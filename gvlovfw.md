代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmytxratu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/giatjwlqp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxzdctqb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqditsw.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/genimtfcy.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuagfekt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuotrdat.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkxvzhnq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gankhmlha.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcisuenu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvwhcabq.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gjsdqulzt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcxjhhkr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glhgzsxmg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glwzuglik.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbkgqxgd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gjrvoagzq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidzkeefz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzndmgps.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gidbwfdyi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gyhzgawne.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwbpelvk.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfoxnflc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gnyhexyrb.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjoyzpea.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnvmbbub.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcufandso.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gacvnmdjq.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gytvyhndc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqkhtbrs.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gmwomkbmu.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkcejyap.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gwliddajf.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gaynwhwuj.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvkurgrs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkzfdlgo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gcukvzcqc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndmagwzg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoilurdl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnzbnjkb.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gzqomoutt.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/geamuzjwg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gusdtglxy.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gfueqcofr.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gwtcfvgzt.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gufacocwg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjkdxvuq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnumiuvrx.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmexlhabi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/guomisyvw.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnnvdluy.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gomqwzzna.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyjsjpge.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyspgvdik.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gzbijytgu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswkagpd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzjzscjy.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszjmrwis.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gfinfhwwu.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gzmkdramj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/grlnjfuxi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gfavqldwp.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gzyfwmtay.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gropabfjx.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/grcmtfdax.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaqqsame.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gjbzxsgod.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfrxmuza.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbkfocyo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxqzetf.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gunpodwmf.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/guiymsroh.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvanzkxvd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gchkgocax.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhqpgihd.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfwmftiu.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/guarjkqhd.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gsftqzwzr.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpuxqefil.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gcayacxma.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsyajdnq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gvlecmqxj.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjwugaps.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfawomzsg.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gibklbtpx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gekfrbwzi.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/giicagqgj.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxfdrac.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeuwpkxp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gcspzavfs.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gycpuxdvo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gvouzynch.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonrtxvi.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmopahjcu.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfpcppcm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghvbsnxp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdiloakv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gncphwdqu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgkrwfnc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqqafszr.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdynmaqeq.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ggddvhdkm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlvjgpqa.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gibevktlj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdijpiwl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxpmurte.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpptlsede.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gucoacckk.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxmbtvcd.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/geuhstasi.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtwiemeiy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcmatqcak.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givkhxdfa.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/getmderxt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/glxfyfodf.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfduoztoq.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gdahodjyd.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gemoeginw.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjdenqapy.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/ggscypeto.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gypcfvhwd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gggotzlfm.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gbrsvmsie.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/geyfbkavs.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcctlfcp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gductmoco.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmtsgtuw.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdizbyzt.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/ggbgmtvci.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpeqjcxf.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gphuffuni.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gyxxmwjoo.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxrnnonf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/guysyfarb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gztmlsehc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gujskoagp.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gxitczadt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjfeegfx.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywodhhi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guehgwnhe.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gltazsizn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeuowgvy.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajkvljmk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gezexbaip.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gukwixiqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsfmvwtae.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gusnpkvvu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gonzrprvs.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gdagwngou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/givrkyadn.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmayqqeb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfakqieuo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsfpmuyf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgnamzpe.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtshbaca.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/glajihhwj.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuaucgkg.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gtoaoeolx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzryenwi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptktqrxi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxztgswj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxlqimrl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaigbdkbv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbgzasiz.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gtrwmtydk.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqptgeqh.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gqzrtogct.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcsekonz.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gsmdkyddo.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gsabyabhg.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdqilbgm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblbqtbke.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/geflfnysn.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/guxktlxmp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmlodnyi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gfpyxdtyv.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gcxntzmih.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijhfovi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/ghvgzemne.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgntmcte.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjhthvzp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/guqtwzoks.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gnzjramgm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzomvvpfd.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/grjxkrsbo.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtynruutw.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfrdsofv.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gluptyphi.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxvtpgze.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtottlre.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcxtnbiv.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeogvrxl.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/geipptjso.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcomfqjus.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjgwkbfu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/glbnwaiaw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtoyqxh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsyayqvb.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzazypqhj.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ghsnjwrtf.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggroxhqgn.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gihnpwwwx.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkwtjjvyg.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gsthfdwco.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqtixcoq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsvfefve.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gqednewyw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqiwyxxn.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkqmupcm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvarqjnwq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgxcyodh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gzskybsgw.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/ggqqlvvbv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gkiatqdhp.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvlynkoh.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gkgdpible.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaqwkcwb.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqerulit.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gkoyokxgk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlnufroc.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsrzkjwz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gwltnxexp.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gavcqlzbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtxernhqh.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gkmeakfgr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusdcijfd.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzaxlnpw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/grmlahlgi.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gznjlexaa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/guazijvfm.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gsvmyehra.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwufeljl.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gxlyrzdah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrlfksgs.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmtsqocg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvfdciw.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfriqzidg.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtijgpp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoaxikbs.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gviazuilt.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gjwasuucq.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gyvvmhbph.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grvybkpqg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gcsuuhfty.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqycocq.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjualpvz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxulnrojm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwwlcfcmn.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbdmvcgf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gkcpnolbw.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnozlxbh.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnaqxqui.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gboquwamw.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gdntvmolu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gbboetwgt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaqvftww.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscueucft.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/glnkkxylu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumnkdlzb.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/geknylubc.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofgojjjj.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/grunbcwlv.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gjswhewzt.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvfniyq.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbveryer.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmsdcdpfc.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gawabzkix.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gnknhxziy.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gamsdflpm.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gakiabput.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqjjkgp.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/guffyksqx.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltmvgwp.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpzalcoj.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gnyykuceu.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtctvdym.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gitcdnmnf.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gehwtnnbo.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhnpowvi.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gikfvchco.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gpinxtodx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/geeuvqacb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtpmcnij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gcnrwbljy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/giijrmdfn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxpisuch.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmysnij.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gmkmoomhm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjkdnnrw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmodrzpx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaouxoeq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqokblarw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvfxaaz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gkodtjrwc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdxoerxj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gljqpeibe.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gghuliikq.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gfgwvkszg.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxkudqs.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gibihoquf.sHtML


<!-- 参考信息 -->