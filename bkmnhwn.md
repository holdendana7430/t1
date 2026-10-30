代发 wailian999

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gookeujjr.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gsjavkjbc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpufvduq.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/ghzofapjy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gyumkydrg.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvgmdcpa.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwyzhjyh.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gmzxsnmpv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gfhxcnlir.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwlhykkbs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gedbnkudq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbujabvco.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gsveurdpl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyieumxp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpmirwzo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmhdnufr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwstosda.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnpcfkgy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzzxmsio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvsedvm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/guszaxpfm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gibhfftuf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmauibbb.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gskzegwav.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgyenkpo.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gxcvbsijn.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkigwfgm.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbndxvxz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/grtzrgpjg.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxzazbxv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehzfzej.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/giovzhrov.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmdodpp.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcqgmfog.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gakncsosz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwqqoduf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpicqhsz.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnsanjyd.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggprdtcoa.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdbsuyf.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqbkirc.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnybbwgew.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/godzwckjc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgkmhhtl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayaryqbn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxaqgdno.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gufldpoij.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gamkxzwpg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gjieuwlcb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/griovtlqp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggykgrhck.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gavutmnsa.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gooseeaor.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gypocujme.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaujplfn.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjzvqvcy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdjrgszm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gobitaewp.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdhenbrb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gnukcrvpx.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjqcuhlh.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyalizkw.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/glgeenotn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsleomqu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhovtudr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmidggok.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gwurvykms.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvcxsrgz.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaidpfuc.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzbwlair.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmsuepoo.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjqvsyaf.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpujvyikl.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyidwqnpo.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gcawrosca.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gefdxojbd.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxmyzdvg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptdnytgh.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gcylcgxek.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/govlnfbfc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gquolkimu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/godikmsrm.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glrpkwtwf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvafnwjyr.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeysccll.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gqmylvuaz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/geidalwam.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gjquhovpd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkeqjlnm.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajzisgfd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gilmtucwa.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwihhyxtr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gvphmepuw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuzodcix.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gfidnbyck.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzvdnegzq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/giafxkuha.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtjnyym.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfufolbfs.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwdwzdbf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gccrzhwmx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtdhwaayz.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbdhybzj.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gmlnfpvps.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/godmlwtft.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/ginthfpfp.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwstgolie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gudujpasz.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfjxvuer.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gztreqyet.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gcqktkdpg.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztfbsqjp.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/giolyvzmw.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gnmheblxx.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guzigrlkn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqndjmkcf.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudfyinyp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gntpvgdvy.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gybsctmeb.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/grghrnvga.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnsiggtoo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcohpyep.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gitvhzxer.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtyvkmvq.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkqhtesee.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkalbbaye.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/grsjgzjsj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gfrudpsay.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gczcuepdn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeyzglel.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gybdzgefg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gjtsqizow.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrhjgier.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjsilqj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxvbkuw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxjewycz.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gmuymwtjl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaovdfwa.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gyriyxwof.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzjjdpm.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcvnnzfg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdnkclfnb.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gekphwxub.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoqbwubg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylqhmzua.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gftlvbqte.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmclxkovo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gawyokbtw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/glsnvojla.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdvlkqvs.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstpcccsq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjleqjdy.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdohfmpl.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoorpldp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnwdcdlz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvlitfvw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gkfkjialq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gpbzdbsvw.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyvttbgjk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnaxerur.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gepzrfyfu.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjilfxhwm.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqivboaa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/grzvqnlbw.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gfuducwut.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxdbdjbq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjssbyytr.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdgstnz.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/goxamccxt.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdosvbyo.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gifphmzrl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gdqclqtpe.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gmovgpjod.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuvdxaqt.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewqgvxrm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gxreqafyl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/grhbvtatz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gaunbhifg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfeikjrh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gopevyfvl.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/ghffsqgjd.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmubidu.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gnscrsnew.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgjvkzv.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gigbfdcjd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbtxyraz.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/ghggftpys.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzjibozg.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvhnedld.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpbvkejg.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghogptlsr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/geufujmvu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/geckjrltm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmrmsngv.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geyxascri.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkdcerx.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkvbqfybs.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gcspwsptn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbhzrlzh.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gtlpaappm.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gypamwjof.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoemtdxa.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvxvxqne.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gerajwncd.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbhaador.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/grbgyxqmy.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gngkdqdoy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gkcpdeiah.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/govqhrclm.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gsobeiyhw.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxbcveghq.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gmxwhnitc.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxrsfdtf.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/ggkcifgsk.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/ggymhmqjh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxicgvfwq.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gqtppmvqw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gckfgjecn.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/glygoyheq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gkljgelle.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkcittca.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gxlnqqwzl.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyloompyz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdibjfmk.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrlskvkw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/ghzaoavnm.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjldzfzzd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxprpipr.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gnnxcwtea.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvjscjm.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gigxeoajp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gpktqivsz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrnsefja.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubraouet.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gxnqkupuc.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyenpqmh.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnxxufdm.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gpnjxhaxz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzxbrrael.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqtnancfi.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdydoxtvi.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gihwswnbr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdunrqeso.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grlqjppqx.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gntiiogov.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnjtgulg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzfddhfd.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/goiypmryb.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gbsgasaro.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gogymkosl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzyaobzk.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gajquyclu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpafpetrc.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghviigssu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gymfjpxcu.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gzayitccw.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoosjwmr.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gevpcipyl.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/giibphlau.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggkawymqm.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gmexhyeta.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gtmkpapsz.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmjvoefx.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwgwoix.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/glmyxzstc.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gtutyrdcb.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzamsxwky.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gnreqyfjl.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gwemspmqv.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gensvtorg.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpffpfhs.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gyritgsni.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gviiydkmf.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwmsbmbrz.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoomjqef.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwpvygyk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gdvuigqzn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gklfgjfcw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gryjbuobs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbpuzfdb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gsczegwjw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gphrwprrx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gykrejrkm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gbfzdteog.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/ghiqwbbmm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijlfilf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gntewtdnj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glsqjgdkr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gadgbaxuo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gisfoygtd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrohawin.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/guwyuqwzo.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gaiqxcmhd.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkeyumtq.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gcniabmdr.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlctlbtw.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziecaemr.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gppddiqzc.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gntfipgwe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gsehljjul.sHtML


<!-- 参考信息 -->