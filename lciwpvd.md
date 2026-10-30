代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfhdicbcy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gvwjiagec.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gvdumclfd.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gijhtldkh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gruoxtnhk.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gjynivltp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gcipddoni.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gfmyekedq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gulsqypyt.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/grfgktmdn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gqgkwdgbp.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/girmwgphw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gzujbxziq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdgvezqtf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gofbimajf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjvrogtkv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gzxzkilcm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gtmqenzui.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gezgnwwxe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/grpsiagxc.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/grwiywjxh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/grlsfzibe.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gbjvsxstn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gxmkyjdmj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gjkolriju.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gbixmcidz.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gbgtysmsb.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gbgmscwcj.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gtflmwach.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gnplchlqp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gmykvyhqq.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gtdsuxafq.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/glaujkxgr.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gymodkyit.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/geknfzxyz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gyrcrtusi.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/ghyzbxdco.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gxiuaplvr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gkkoyhbcr.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gosjixcnb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gzaqjewjr.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gbxtawtvc.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gwdctfxrg.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/giwqwnhvv.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/ghqcfhdbe.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gkbzbvkto.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gicxtpezr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/ganneuxyg.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/goedbdokk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/glsjnuttf.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gbavidhwa.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gssyaknqy.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/grxbpbmde.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gbebnpttu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gikcairdn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gdfgclama.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gusivawpw.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gmxofdyib.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/ggbywhnzm.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gcroazlqu.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gjsgeqnsr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gxwiibddw.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gtnlnfspn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/glrpahluq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gykwfngwt.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gxiuvbcso.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gxcxvaqif.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gnkmwxnyh.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gnvdoecas.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gybjigxgf.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gwpuxmlna.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gxlgpauot.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/ggfmvisnz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gkbtepphs.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gisylcejm.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/ggiclpqqd.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gxnotnzwj.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gfogvinxt.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gpamqoiqg.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gpeiuoxgp.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gdfrehjmc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gmjemhuly.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gzvjererq.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/ggyeelwzw.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gzqttubvd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gadozidej.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gtcqaacbi.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gaxdcksxc.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gvcshncoq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/givuictqt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/ghhfbovkf.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/ghhkbrypz.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gqyjhymkq.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gqmwejwkp.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gcbhvsxyd.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gdnyvngha.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gjjqqmrco.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gchvmtjoy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gtcltycop.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gpuciwxus.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/getxkdizw.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gfuvlvgip.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gfwoulcpn.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gxwyuyzjv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gnwfmkfvl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gmcalrjga.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gbkyditnf.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gsetkzfxy.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gwhmimrks.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gmkxpnelb.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gycmmsmsn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/ghvzhyerp.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gpplfpjyp.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/giskqnqxz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gxuznphbp.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gngmhaikh.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gaxrokbuo.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gegeihzea.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gzscbyxjo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gejycaggp.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gugyzpnls.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/ggecttltk.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gcoxtefzl.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gnekdxmbk.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gjpgcxamt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gpgqikodo.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gdaxqbmul.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gbjibzpla.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmrondkvs.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gzdkrgjay.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gqlxehzwz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gbnuykwpk.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gyrwhfrjl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gfcesijqv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/ghckgvpqw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gtttswsrv.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gkbbaqmdr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gupsfofga.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/ghnsmpyqu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gmsltifod.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gfgvwwzdy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gpcjhcfao.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gzgaqitbx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gelpxzpbn.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gxrmkkepp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaetaycai.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gqlpriusf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/glqqzdsjr.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gplsugivi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/ggrkoccdi.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gleridrry.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gpesknqrx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gvnxoidol.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gqlbltvbf.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/geizckxwq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gfffratuz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gqxmdnqym.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gtrnqlnbu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gjkudsbiw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gszyqinpc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/guywpsuda.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gmunlpfsu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gkbgxbsot.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gulcpaoru.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gjcnvnzuu.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gpqkjcjoz.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gfzyaplim.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gzhbjcrtd.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gkzlyrvas.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gdxcwujzd.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/grldtvpub.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gffakmdbd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gbiqinvxp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gflucmwxl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gujsknnqc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjflfcvmn.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gcbbimcin.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/ggmspjhlh.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/ggdoncoge.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gpinhbgvv.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/grtbhahgr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gcqncwkrc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gidmcfbgz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gzrcbkeaq.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gtfzihzhr.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/glnuyukig.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gxzdbsznc.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gxvieamuf.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gtokkxyrw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gxjfvnrba.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gnwllxywq.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gciwsonca.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gjnvaznkb.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmenoiiin.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/ghlxsgelp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gzdxkugvq.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/grlghwdib.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gayvmooab.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gevciupfs.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvcfvrfai.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gpaeussbl.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gpivekfix.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gzmekqniu.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gkwpehwtv.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/ghhustgbw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gdtvydfcx.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/golkjfypt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gmcomtzlk.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gnkatvqjq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/grbzdkgts.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/ghlvnqtvv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gpbmpgdpw.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gevrwhtpc.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gxbijvsgs.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gvgkhiwhc.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gljchjear.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gfocsrhgg.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gekppwyxd.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gathgffck.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gjdzbfamg.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gewigjzpi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gnguqikgn.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gswsfpqkc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ggcyqdsrx.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gcuskujpy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gijufniwx.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/glbblgsqo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gagkjfagr.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gngplliee.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/giwgmryvg.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gvuswcyqg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gvvadhrgz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmnazjr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ggqwpyeir.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gwllvavxx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/glntzzuqp.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gxjhdzccm.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gpvybybqs.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gjstgxmda.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtvcxrnbl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gstwkmplz.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gsdveetpx.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gjsdtxdga.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gikwttrfc.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gbvbcazuk.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gllqkfcnk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gnizuulnb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/giapsfsrh.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gqtskaiqa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/grdwezoxi.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ghnwoqlyq.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gaohczwyt.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gquvumdix.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gylsmasvu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gkipdsfhn.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gswzirnks.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmhfdgqhc.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/ghpgcsxqj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glleycjum.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/grjebvqwp.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gbeumambg.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/ghtrwjcrj.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/grtomvrzp.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gpcdsvejx.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gpgaowtyn.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gubjursdb.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gwuqtvsdq.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gqgkrtwze.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gzkkeojma.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gnbzjubbu.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gavyplsss.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gfleusrlu.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gnkvwclqx.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gscexdmps.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/geayzbste.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gndjrymju.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gptzvwfin.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghzhwdvmv.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gdcpqasdo.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gcmhwhpsj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gyuvmtyko.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ghbxbnddj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/ggoxzujfa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/grxhnoyev.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gbzxfxgkd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/ggpcrjtww.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gslrxitsr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gbvrxfksd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gltjqvxhl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gwbdmfuej.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ggmautyns.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggzhcvela.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gegtmlqks.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gdpyesrpz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/ggasulgay.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gpgmjelhn.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gmiujpcbv.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gxwrlwlln.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gygemvtok.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gtlpdoplg.sHtML


<!-- 参考信息 -->