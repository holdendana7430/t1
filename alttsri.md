代发 wailian999

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gitiyvjgm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gspofndjt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/golwfoowj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/ghjpldibt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/ghfqtyfjg.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gbwucpasv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ghkwqkcep.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gxcpvpnmg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gqvpjeibm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grqjrpfkv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gtlefybij.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbuaaahmp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gifrjrqjg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/grhuaputd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gebjscdph.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gfmgbdnrj.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/guyjyfsqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gtygaxbla.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gijwidhzg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gdeufqddv.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gzhfcljyp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gouykhdji.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gqfmtntpv.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/grgzjpkzd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gfjweoany.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gmlfujisa.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gktxfefma.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gwklqtbcs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gccmmyats.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gpqvgsshb.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gwoggapvx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/grxsuscal.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/giprqlhag.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gidjtgmoj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gylrfhdfo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/glqfjwjjd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gslfmmclg.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrcgrxm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbygupx.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gddgqmjyd.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gznmdhdjk.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/grytylana.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gjiiqhadg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gykafbtrz.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gnjvxuvud.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gedoqtnqu.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gilxhhoqq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gcdvsztyv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gtabrkwfz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gvjbylhbe.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gabhzhzxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gzjczzmdw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gmagmqyjc.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/grrxuukqd.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gjjrortsn.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gtxqthlid.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gkhjzvbse.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gqtbhfuan.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gpvclsouu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gakemphjp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/grbrvhunm.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/grdpfdjrc.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gtfghlpzy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/ghpyavwki.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gyvfzjdwx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gxavvvjgj.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gzklgcxkz.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gamnsebud.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gbiocygks.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/ggzsuwgry.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/glxwwfeqn.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gdrfuresv.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gvjuwayeg.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gqdyjkuyg.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gkhrcdscm.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gkslogibm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/ghhtkvskk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gvajnkxbl.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gmgooxufb.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/goqjhjbli.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gafrqwfaz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gqwzaiymm.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gpsqzdgzy.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gwefnhvgj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gynknjrpg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gnvdzuhco.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gvppuhbka.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gjasvytjb.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gnjcbwnsp.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/ggzznchfr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gmclgewxc.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ghliduhwc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gvbunxpts.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gyiinvcpp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gtfzwadob.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gnyrnswzy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gbosfamib.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gvwwjwbks.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gavtusvso.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gfkkmipai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ggqeddwos.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gsthmcgnm.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gmzeascne.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gibqtkruy.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/grptfmuwc.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gzyrnzizd.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gnnmbrmpw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfuevxmp.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gvmmlkqwq.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/grhnyhgik.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gdozmflsx.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gjwcswaoj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gtocjcogn.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gxxleqgcu.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gseaslzjl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gtqvqskdf.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/guhptuxhs.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gxawjjsol.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gbogkexyv.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gplwoxkiv.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gafnhixqo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gcftxvkem.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gumrmacpt.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsobeizkd.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/guhlqatuq.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gfwucbadi.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gyvxdulow.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmfybuuuf.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gpuyamxrm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gqxlkualr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gblhibnmd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gyegabqxx.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gvgryaonm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gfupgsjqn.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gxhuybrrw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gdjjtwtoe.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gjbakccbm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gxnbbzrxk.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/ghyalwhdj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gaofavyra.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gzsyhqqxo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqehlknuy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gfqufbtnq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gnwphpnhj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gkzsjxtdw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gbqrhwatk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gwolnxtiw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkkhkpg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/ghunlurfl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gsfyciied.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/ggqpbhrpx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/grymehgvo.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/grvdailot.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gmnlpaptj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gwtnrdryj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gnhqjrmdk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gzrzzfqid.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gidjevgja.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gehaherrd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gembysqpd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/govugzrpm.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/grzghnhjl.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gyltlvgkl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gqrzdfsrp.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/glntukmry.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gihpzvdrk.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gzrjrummg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gdintjzzk.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gfuynvedr.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/glsnnclgh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gydggbvxs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gjtxqoqjy.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/ghsjmicga.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gqtqiowiz.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gxvfbznuy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gktqeurvc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gqhgngnia.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gfdvgnczw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gqwhxatsy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gezjkdwdv.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gqdoqpvhd.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrrumgh.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gcfeksshz.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gmykjjvzm.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gxjtsdjoa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/griaunvlm.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gdevftdrd.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gmdqcpsqv.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/ghjukfgam.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/goqltfocy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gmoiijvwm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gxzlglkax.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gojkymwea.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gykdvksly.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gaxaetmuk.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gbztbpxmj.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gmdiqyvan.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gsatkthxz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/giqzovncm.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gpyybunqn.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gmklmjzdb.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gcbjtkxsb.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gzykynitn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gkvpefshz.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/ggwcfjjut.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gurarnolc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfccakpso.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gahtkigid.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gvirgavha.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gumvkemfr.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gpixzktre.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gzulackie.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gbtkiubww.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/giyirehho.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/glldiiyij.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/ghwajjqtz.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gzhxyznid.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gjcxvwbzq.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gghxpksfn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gsnhxvqlr.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/ggvwebrah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gywrzmgjh.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gyetpuknp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gkeeiuvhu.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gknebnujl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gtrvtjwqz.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gmfxyxjff.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/giejjjooe.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gmhrgpxyx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/goczfgbhg.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gtimixthi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gdjsxkswf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gewtobtxo.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gxwsumygo.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gygcmbtdl.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzsmpwkgf.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gpigvjdug.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gsegvgmcd.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gzuvtyfqh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghzwevaib.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ghxkzeovc.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gqooubltn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gpntgrjvm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gdfvvqhzv.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gqwzugtjx.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gbtmhckzc.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gnxcdkcea.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gjipwhqav.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gtellhhdd.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/glegleoah.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gcyfbcrff.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/geaxmovqz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glxzbeyvy.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gbwretgzx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grsdmxfsq.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gphcpezqe.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gleqzsuxd.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gemulyntx.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gixxnfyqy.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gcubjwqci.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gujeicybs.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gimhyqhpf.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gtbfzwgjz.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/grsspywfa.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmvudsz.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/giepwqzpw.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gvawxtuvs.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gphlhyhcp.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/griwrktlz.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gxcgbxuyz.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gijraijbc.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gkzdnfjpq.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gtoubgywe.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ghxtpydxz.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/ghkjujfri.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gbensgnmk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gdlfejumv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gpvnnwrti.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ggguctqwt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/ggzsckmgf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gibdpjvqb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gjdlirxpu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gujwdvsqp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gblpaipjq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gypzmalwr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gtauodgvz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ghkfigzrc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gfiiaqtrh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gcfreoroo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gcyjfdzil.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gpiqakcuv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gksmkfwta.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gbvazmwky.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gjrakpiar.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/ghtxfwjmm.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/ggjeqlmbs.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gfwxqsgkb.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gteegzkzo.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gaxnvneql.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gylhtfgbv.sHtML


<!-- 参考信息 -->