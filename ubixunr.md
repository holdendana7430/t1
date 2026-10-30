代发 wailian999

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwzcmovc.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmuwueef.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnlexlrh.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwenknbb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhdzskos.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gzzlnwpiv.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gvvhipsup.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/ggjsrdbfh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezwqtnxy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvocsaxcm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfylayhc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggssztsbk.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gbasjdaro.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapavsrsu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gquiwohsg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuhhteng.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxagmqtw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhgzzdj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpayimkcw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/grwtdfygy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gaxkwbqoz.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gumppxnmx.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfzhhjlv.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/grxiqwtpr.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grannqpsz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/guspgnsmb.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gitscpxkx.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gbfjplfwv.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gnstdkadm.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gqsmctico.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxsqqpkk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqxwvjtv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gaapzvfkh.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gssjxmwdc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gsohifazk.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkuteum.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjltabmyb.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gjzkslbxv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcojymfod.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxzhxkim.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gpewwgniv.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gdkbkaqav.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gdiwmduts.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrxqsyjy.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjqafvgz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gymwzludt.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwlcgyx.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnoezgzu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gilscefcz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxbmdlzps.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdtsifim.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtlqtapa.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gnxubscst.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gwknwxxzw.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghofdvgzx.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gsggowkwl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwsinbmp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghshuhnrr.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/grfqtylbw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gbwvxwsax.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gykktrfhz.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gtefpisyd.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gvboqqfls.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefzdsjyg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/guqspaiso.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gglrpnfmj.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gjutomhve.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gapridixv.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gslebhotl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyumsapk.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gxcwfcwuv.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajnmdjbz.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gplugidow.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyomfffp.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gssftrafn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnfyfezj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbnxxqd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gxwjawmfj.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrtayfod.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepkluzqd.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gbagopqer.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gluplvblw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyufuojqt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbpwdgfs.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gccfhsyiw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gneqaatxa.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/ghwbcqkob.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gyxdimfkd.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gthpmyoin.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gckaodazf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gjnzfjkpa.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwndytusw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gszpfdbmq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuekckss.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxbinfpk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdgpjolj.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gsjquoehl.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gqslpswht.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdwvmcby.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gamoywzde.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurdqohgg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gllhbmfuy.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gouzxwnrv.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/giwjngvku.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgmhpoqr.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzkhyqey.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzeueoer.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gghkcafmd.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmulemu.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gkybmouwr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gyfbonbjo.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvwoviizd.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaqnmrcy.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcrbtmbt.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzamkypm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/geoltmbtk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvpjveyy.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gspunuqhw.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gokocubjh.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gwxupypql.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmexorugv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gtkgdnrqp.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyxpzuol.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkmlneqe.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gycqmaieg.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbignmpou.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gknppkteu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gswcsjwtc.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmijncwd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqshzhmmu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gwykbseau.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgkjjwvr.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/grnlqrwtj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gdxiizowp.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gydmhbrth.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/goioruebl.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwxxrphe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjzfkfhq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/govcbumqp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gvupkfmvc.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejrytdjj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmzuygylb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gtusjexrf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfursqsk.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhrssotp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gshmtqbvh.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemtjyynn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhoigyjo.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfuvwstv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvxuvpuz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzftmqp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjmarskx.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gxqfulzor.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaqicnsj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrxfaqts.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gzygwhdig.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gnalwayrx.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/glzfijxpx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzirukxds.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiyxahyb.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gyihaakeo.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/guefncobi.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/ggynbjpcj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusuqymbv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvphyaww.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gmnwicitq.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gaftehqws.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdddfsxb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glctzniwk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtyjvfct.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfgrqlez.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuobzryr.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/genyvlsco.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/geotifddk.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdtjovcm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggoyirtsx.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gewjbcwtq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjvttenq.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/guzsasbcu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gypjvjanp.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gudroufns.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gyfrlflbq.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnphquwbc.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/grmklrqpk.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmicaofh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuzvdzyf.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gvckhddly.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gavqnqolz.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gooqlpkrl.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzidyeae.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gragmhdqd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/geilqzsjw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpydedzt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gizxqimcc.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdeehizfb.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gtiwhbpbc.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwyytqoal.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/ghmpoxqbb.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyipgybo.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdksxstbt.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gznpoupau.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gzhmnjpms.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/glkpectrl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpcqthpfo.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gtdbhrofk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxexhpzbk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gfgiytmix.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssxdjkar.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gqevciivi.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuxhusij.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqyqlkbk.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtjaamna.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwapylsu.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/geefaceab.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/garvcpuqc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gybulkyyc.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/guihurtvs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeesdpit.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/glfutlmwz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdiqktirx.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gfowddymp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/guxclqzfp.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/glwybngho.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gakxlutqh.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gayxwlvyk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqzacpqw.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gtehoqich.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/glvdjrmjs.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/grgkdghvh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdxdagwb.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsybocswd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gaxafffax.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gteocogvp.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvrohmxs.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gayiobxno.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxkbijbl.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gheurhsxu.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchuqxjca.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbtquvij.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnbmuevi.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gqmcamjkt.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goggomggo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxoxofq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glknmxagw.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/glikdxhbw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdcqiyun.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/ghrmixysh.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gofdzwfsw.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gilzkufgc.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/grblbzslw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gfrncqwem.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnuxdpuq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjiwxzyac.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gcsosqzir.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbfahqym.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaabhepm.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gzrvdwerm.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gsynfjjvr.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvyrdvoz.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdkisegj.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxkjjjw.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gyyaxagsm.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gyrtgzgbu.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gobjlvyvn.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/glyissghx.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhmbtnny.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gcrcbdsds.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/grhaconmw.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greatsgwz.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/giddrjwtw.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcyxtbbs.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwvdehqea.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gozitjyhq.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpixrpiv.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gwktwqjmc.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrjdtcgg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkmjaugz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxkoampq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gccuzndva.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gderxeari.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmhigshx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gagovjdtt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gulzcbopn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gxucqzhlr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gembjdxhi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gftpddflr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/geiwlhqmi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgjmbukf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gzshxgjhf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ghivduyok.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gmpwbhfkn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gwyukiqyz.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcfedwfu.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gnhciibxv.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/grqtjxhgc.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezyetnov.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gtsbgxrlh.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkecesdzk.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceltmqdd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwlcydurj.sHtML


<!-- 参考信息 -->