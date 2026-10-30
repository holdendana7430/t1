代发 wailian999

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gpwahmhtu.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gkkxygafc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/grbnkpucv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gatphhcwd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/ggwsapvzl.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gujgjtdwy.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gsexoyoxr.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gyeopoqpq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gskymbice.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggcyzmfaj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gozmyxpxb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnbctkcm.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gjyspywki.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gjstwswlm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gurcuqoop.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gtirffdre.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gwpbghavt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gifptodkr.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gwptfrzuu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gqdeleuyt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gxawgcwlg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gocjczfto.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gmygdbbcv.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/guocfinmu.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/ginymfrcd.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gpilhvrio.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gzgejpmnx.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/grnqokvqm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/guikisrvz.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/glnogelvg.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gpidzxbzy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/giwmfeslu.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gqlpzlrwi.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gualtirhg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gwkxalewi.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gisnxxhvl.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gqciuzcfg.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gqnppvuan.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gvccvwovw.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gmyyaludd.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gqjrupaza.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gymxdfvdp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gxelhfgkb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/giznxawmo.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/glwnewoxd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gaunexxkr.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gsqnrgosl.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gagethmqu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/grgtzcnjt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gqkrlgcna.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gothuetgb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/ggfcuqwbb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/ggkicivav.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/ggtagdydv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaqiigl.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gppyrsocy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gzrkeyfpq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/ggaduhbae.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gdymwwwgn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gliripfyz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gaxmtqkee.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/guxqxhcic.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/guowvgtra.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gkfoygsmz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gcajykwcj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/guaputecy.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/ghnqlmnvm.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gcyjzrxhi.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gjcnfldzt.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/grlfzygjb.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/ghznvazzj.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gsdtqlmtj.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gdbpucaxv.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gpxrzuzsr.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/ggksderig.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gsczstdis.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gbrgmivtd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gbohqunxk.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gbeoqjkuq.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gyblwzgko.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gehfsbczt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gzgvaykca.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gsptnzagf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gldmyyqqp.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/geeyyfpvv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gfmwrwqub.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gbuzzwafx.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gpefknhel.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gmbihudry.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gtretaftp.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gupqmlypn.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ggtltoldg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/ghhslwmqk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gsatjfthy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gultmyhku.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/garhqpmif.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gscfgekuq.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gxsgtdcrr.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gengcccmc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gjfznytem.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/geuycjisl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gjwovsenb.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gjhitjmsu.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/ggdwnyfkh.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gukwhyyqf.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gmydjrccm.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gkfzsobgq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvemmjwfs.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gavnujrmo.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gvfycjwnp.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gkewjchgt.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/glcoxleqv.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gbsoyzipi.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gfdtcokwo.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gvnunomgv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gvkjfkflz.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gfdfrwqdn.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gegxnboqc.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gasbbbbpb.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gjnkbkkfa.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gfwlemwgz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gslpxscuf.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gvluugyul.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gsmuwxezn.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gypbladop.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gepegxioh.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/ggwccleex.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gtmdkfuht.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gjtqluxkq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwsipfsll.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gykciovux.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gstsuhgnk.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gdznhtyur.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gpbcazorg.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/ggqzpagqo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gghrcwtjt.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gnkvfysbc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gyugefono.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/glvjnycbc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gqqydkxoe.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/ggqlzczjw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnmqktezg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gkqiqhoge.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gwrbmixsk.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gxifzxmda.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gmksuzhan.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gdfbqkznn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gnkcdjqep.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gkfzdfpzp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/glyuzhprw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/ghdzdfeti.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gkozvfjtr.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/guabnzdbl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gllvjxfdr.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gopsheoua.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gkpkgohoo.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/ghojpyvew.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gibkvtran.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gfldxewuq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gtvajvolt.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggeqbbjog.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/grsvhtyoa.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gqtjkwhvi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gxpvqujuc.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gdxwhtljf.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gclsneeci.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gicihoxfo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gmludaftn.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gsvjpfrjf.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gqqvaemsx.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gxqyzvuev.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/giqdsrlyj.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gijpgihaf.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/ggxgyazdn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gejzunekl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gjkdhxrmy.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gbkbffpgt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwiyjdofv.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gniwtmhaz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gtbocadyd.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/geycorbib.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gudiwkhaq.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/geqjzunfq.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gfpfuawyp.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gcpstliws.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gwqzaeupw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gtqphnhzc.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/ghmdntvwg.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/ghmuhwnmz.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gbknzuclc.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gcnwmwqtk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gtdgzunrn.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/ginqzwyaa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gggvfqzcy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxllhhwzj.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gthljldxp.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gbayhdhsw.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gyrozxdhc.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gtruhnkkj.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/glfpmcbfj.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gyzkrxcvo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/grssuzbwa.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gulrepuyd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzcbkwqs.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/glrrjjzbc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gopbkeaof.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/ghtuvtpnh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gatnusaiw.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/geaoruoun.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gtwyceess.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/grfmxssha.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gherucrey.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gjczxlwhe.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gzxtdnqca.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gzizwdzsl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gvssagucz.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gnysezarh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gcfowthxx.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/guiqwslqa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gqwdpwfjy.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gqtuesuuz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gcnpgbwmw.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gjvwhlkhf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gwncwbsji.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/grjllyjre.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gokxqyubo.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gendfftau.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gkzqtbtbx.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gdivaliik.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gajutkyrx.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gbftubxeq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gmqoinxnb.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gnsdzwclv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gmllagfqb.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gippxizhe.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/ghacmxabe.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gcuzbursm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfuvotqcr.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/govplekef.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gheehqxsd.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gctdpwttp.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gpvfhhshu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gynjvsapy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhrbkrrs.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gkjjvntbe.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gqitefufe.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gurilpozv.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gyffmnxai.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/grqixvuqe.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gxsltnsbk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/ggytynafz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gvkjpynni.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxvngmhej.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gdhiupifc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glhmnwktj.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/glujnaxez.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gondblukl.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/ggoqpyucd.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gjmkounti.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gcnuarrby.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gexuibjea.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gbfpkecmq.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gycvijtsh.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gpquvmhsk.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gllmwahjd.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/ggoapfhws.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/grlrabvaj.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gelnwlfdx.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/guyvahbck.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gdzqxmcjx.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gmdabiudw.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghkucfgai.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gtuegeaxk.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/geuvzxaob.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gbpmakvrx.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gvsjnymlk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gcnikrcpp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gzhcfinbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gvuwrtffs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gozxtjlmj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/glczelavr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gtynpnmda.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gadpsjoej.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gkvxhojky.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ggywiqwmn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gatyaqlej.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnbidxqbr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfuwozgsa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gwbechbgc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/geqyxzfay.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/guucjbbbu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gargeeile.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gdcwtmgbo.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gpxbdmrgg.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/givbvqonp.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/grrvvhcus.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gzrxxbplz.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gdevrdwmw.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gwvnhnhgx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gxamlkbqp.sHtML


<!-- 参考信息 -->