代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dbznffah.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qzopfjzw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tekldizi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vobwpayi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovfdowrd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pltkxjrg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ylufmndf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tjfcmqvr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kfpraxkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aoffqkca.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gtrssljp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnzbvxqw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hwbzsfbr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hqdaicsp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fycuxivj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2awbkmdoc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ynfutjju.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2fwpxaann.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nkfoyqjh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cvgpawsb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2eannjjau.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2szptcksl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2scykgfdg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bevpvsnh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xehdkrbd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qdgnukyp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xwgolkpy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wyiicylg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2oqwwejvw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjnvcqk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nrnbnzzy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lgttatua.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2emzjzdjx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2smniwvik.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2govqhhxq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2saiwcfqi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxaeoxky.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uwoyqyhd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ppeoowlh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uxxftcgw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ibvzjzqq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2slhkunck.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ygwdcuad.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gyckojlb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jjrxlppm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vdaljrhe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2yepdtjfx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uutycswm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2shqfpuyk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xosxstgd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vqdstbja.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2veqsmifv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jvvqqnol.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jwvvrkrv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wvedrqgn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ilqowhlz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2whsiakiq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lhiboavf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2txmdqjqi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yhkbllwk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jzvkdihg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2trydpjpk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qcdrtnjr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2njwmixsn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wdwrpnah.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mnrxxcln.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hzkraphy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2inuyncrh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2urrsmhka.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fdmpguyz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2aajwtons.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zciovnuo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qglscsad.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fvbqhqpx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kqbuudlr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cjpzarhu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kgospvjw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2pleovksk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hctychpg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ivgfasai.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ifiyqcsb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jcemvdsi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2arqbidkt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnlbcvf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ferffeps.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qbkrvacn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2hegzzmrj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2obeukdsn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vkzyulwc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nvusyeth.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dqdmmria.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ugvtfvti.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lunhqrlj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2gcckgxij.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qkulyysa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2slqrjarv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xjbbxhjh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tkyprbyw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uxcezbnc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eqrzhjta.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gzzwsqtd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvfmhpe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lrulcjao.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mslhjdrs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewxceict.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mhxuvgkr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hywaukvw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2byjqmmzc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mmjyzddw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mfayjlqz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uaqekueb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gaysxatr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tqrsdizi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uamrfdpd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2otqrepwv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ksjqoxrd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2peihbwdw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mzhcoynq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qiqjduzm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kimqygqt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bomsqksi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ifuhlunz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bnpygdzr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dgdzkydz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kqykswff.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xcidftfh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rokziusf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2srbbtlto.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bxpmsigz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2irhcxtvj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bldgmens.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ucjodegj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xnuwqlfq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nkudkpvq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ckbmrouu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jmbselxs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2kmmwiayf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wmrjinwu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bbduyfws.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2usiamwdp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hwjvjyjw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwlnrmqq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fbkisefr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uxamfudz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tmomuoom.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pmbbjwpb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2oecswqhn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vuwojgbt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bbzbjwhh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lwtntmxu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hcrgvtss.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tnjugnna.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cqegecpu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ddhnzlfd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2welbfdyt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2eibtaazj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rttpfxmd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2oyqefend.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oppmjpsl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hmymmeaw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xbiimifl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hbukxrmq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qlosprsk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rbixzpay.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kyouzugm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2eawlqyeg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vowccvba.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2odmohbjz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2abwlhegj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wuexvqbj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wjzyhugl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pyamvmth.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2uqgjoydp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2roeslgeg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ozbalxae.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtqfvvos.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pngkxdoh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bssnjnem.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fdoywdmx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dbbavugv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2sqvyhlml.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qbswwbyd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nndowzwt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dougwknk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bspbaegn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iauydazg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yzuhuhsl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvheqbol.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ldyeddim.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2acfwdkyk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jlcvfkwa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hccamulh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2oycbxlou.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bwvqmujh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ulddhdrm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2msepfajp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djhgfuoh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bgtpyciu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbtyahpr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cbcodgvw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jufrsmrw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zwvtoizp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ibljmesl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wgqngrje.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2caophzuf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fpeogzyt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dkkwdfpo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2spjmgxzn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ykhljssd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ttiexmlm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ujyxkctg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rwfvpgjd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2owvjsqsb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pzntuieg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rmohyslw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rdvzpeyt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2skaqlxaj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cnjsrhck.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2sufjddcm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cwomlmhc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mhyrsiml.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sfylhfkt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mxwmxbpr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qxxxqruu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qbvrxzes.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bwgckrpk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2snwcjxpy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qtulhjkr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tdwpnmzv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pnyewsyf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jrqroyjz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2flwoyzba.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tkgtlats.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xbflhooc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zkyfppgb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2esvnfoxg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jljevhvv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tjgaestt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ebbujxyw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2olhzdcbu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2llbzndfy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2krakpgbz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fnwzemez.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hljxgxjw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2elyfzjly.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2oroeeucu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tqvplqku.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2tyeantye.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vxhrhoae.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ukdhtqju.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fenmcyrp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rlrblymr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlstbmrc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cwkcphvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmjpxskv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cthvvohd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2scsetftf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fcbhqijn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hniolnbw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2prdcshas.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2abrmwgzv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zjhqlwss.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jyokzjmy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2velkofrl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2krykpesj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2obzivvri.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2estigihh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bxedpbpd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tebcmlfe.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tkfptkux.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ppqnyqbc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dqpbueze.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hbbeuehi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2njgyospr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mtonjcsq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gxbhtrsa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2btlcfxvb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fxdqkyxk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ihylgnlw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rbpjvjoz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2smwlbpcg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2veuvfsnr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kugzqjja.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2skvjejms.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ubaolidd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ubpbjkac.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hxdgxtzd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rfeveead.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ladicxfw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ixxkmpnt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2hamimlvy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xbnegcdy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mpsdoear.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2nisklsnk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ktwuslra.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bzgzyfif.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2axwmfhhb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nolxulyq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cykxtdzn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jdvwyoce.html


<!-- 参考信息 -->