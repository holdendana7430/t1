代发 wailian999

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gmsdhpbpe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxsssryc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvklrjbrj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggynxnlpa.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/grblotchp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjknhrivg.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gvouatkex.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gabebyzqz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gfvecxfvi.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxpkhjtc.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gacftqspm.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gbwjfzqng.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gnhgyrghp.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gdmqzvfhx.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gogftvfqc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmyrmxpx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gfwvsxpgs.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkbkfiwj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gypcpwrga.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gsyuiruwa.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/grlmtpeph.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/genlqwewb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfgryndb.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmcfdmwr.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gigwuerek.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glngvvanz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqyiatqx.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gfmvotcxp.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdpatgy.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gyljmfmpz.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gnpoegyug.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gjxywtzcv.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcrrccae.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkvmzden.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/guzlnsckh.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfksfsom.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmapmigc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglnqipqm.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqxyavg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvsrkhnl.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/ghcsgxtuu.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntlixwwl.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamgnbpza.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfnaisva.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakalgoto.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gfryyqtvh.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggivdnntt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gabvvdawd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/guumhtuge.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/goabcnumc.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxfxycn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoodasmd.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gwkbieoal.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/givshmprj.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwxaqhxn.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/goifvbzhi.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaanskgn.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxfnvuqz.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjgdqrbi.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gllpnchep.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gicftcpfg.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvtvrhgz.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gufmvaiyf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/ggdkawsld.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcmbgaal.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gfvfgqvty.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gjjukgyga.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/ghriatcvp.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gmmakxryl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gwsxihmyi.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqdkxho.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gtduvjfab.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/grenfkmyz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/glgztqnry.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/ginzywgzk.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gcqqmcndt.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcmaekvi.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gkizoqztz.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gnkmmimzj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdaioafd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/guegzvsni.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gcspgrnuu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoowhoep.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gewoiygsi.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgxxjqdh.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gaeeezjhs.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyumobibz.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gpakejnhq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvvnxhczy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gopmfaarr.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gymhvlllx.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/grywsyufb.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwsfolxgr.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/ggslbxfij.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbshlpevv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvnopwvrp.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlpoefup.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmysykak.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gswejnhrv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gytgbnlby.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/glarnmuwf.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdyveytb.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajosjmk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcwrzzel.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpddsov.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpecsmkxb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssmyiqei.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/glleuyqis.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsohfmzn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/grqlbtrnw.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcdbnhbgw.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzvlfoefi.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbsbsjptx.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gatqhwszh.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcrzsyom.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdonyjvv.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtqyxcsck.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpichgbum.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/ghlzpitxo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/goznjgbls.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gqszodjga.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugbpibvj.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuctwmjx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsqnlqju.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gqqnfowzd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/grobefrjd.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmffhwv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrpbephi.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecvzurnq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqrefqp.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnitzcgq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gizgavlfs.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpixnztbx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/goizqilzd.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsqyovqkp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gisuriyul.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhycabpw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/grglskdko.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/grfepnxld.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbigzqn.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafbfbayp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbzbtilm.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfnkwzrbe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gatdxiofv.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gfjaqvwqz.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gqabtodoy.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsjqsraer.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfbchlgq.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gpkwgaqfh.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gdknzriau.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuejtou.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzunvvplv.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxmcuzn.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gdtatpxoz.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gfbainpjt.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gjpndljib.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gmzzzifyz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyfanhmy.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gsjzzmyxh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/giyscqdpz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglsvcoah.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqugcxhc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxzjwdi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gjwlquguu.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gkydexzgv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/grkakgwtn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gccbuhnbz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gkgnmkfqx.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gkamwflqs.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gyfepdvpg.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/ghlabzjiu.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gwlwbkcdb.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gzwtoujjl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/ghlpgsznl.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpsyzihl.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gzndzdxrl.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/guflztuvz.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefqsjjpz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkwpxyky.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvjkzdbz.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gytfhcfmc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gewokquqz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gautfwdms.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/glfevsihq.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxhbisaiv.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gmaywalem.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gowqtohmk.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gscshsxlp.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gsbqvalup.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/ggvjcywrv.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gucymrrar.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gonrycuye.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gzabkqjkt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqepvnvn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekfiybuz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/guxxjwign.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gzwdxfjfp.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gqwjetwhc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ggelydekz.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrzuqplb.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gewcdwstl.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnwpoljl.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtnhtwur.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gymlpwcpu.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvrnogba.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrjpcom.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/grtyyahnt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoxllxos.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/glpyrevrt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/girarupza.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymvbpnws.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gqcqzdhoz.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuqzbfim.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaobugnfp.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/ggldxynta.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gxozcprla.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gszhgyisn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgytjjlj.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/glfesrbxt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gsnbsywgf.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquyamxeh.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gqgvozpkn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnwxecgw.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/geosixfuq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/guvgkyxmw.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gjnzdlbzf.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwxwgunm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobbxibev.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gnluodnsd.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiavlkob.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwoksizh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gentlrhry.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtcuxlo.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gewhwkrjn.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gwffmkcvi.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/guoxmvwyd.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/goqwhgnju.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfgkcfnf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gsxnkpfes.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/griocjnma.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqwdjfnl.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gckanvqbz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeyxsnen.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gepyyhrgd.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvzlhdp.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gxbsoyezk.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gzxkjxxhc.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/geprlvsew.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbrautou.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfkayeel.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gqxhzhgvn.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gfadddxbq.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbnmasba.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnsgpgkv.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwvoikcu.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdltzfxm.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpexnnr.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/grhxapgpm.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gzgwtqwax.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gynpxmoqh.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtomtygop.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwrgjhknt.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/grhqmilin.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gsubwleyk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/ggtxggsik.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxkedhri.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtumepz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzsaatdy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/glqcbpwmh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gwqgmvqrj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/grgmpwpzh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcnwruyr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdqyefqd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/ggrutyvms.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmxcjqqh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gsktsqusf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcibhqhs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gstcvhyqy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gpijkvazy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gupmkvkll.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gngjuiqru.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwjafukm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqitelmkx.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gdzavxzxp.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gwksvsghn.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gedoonmma.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbylycxe.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gteesosin.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gquscjidg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxslqgvl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/goyrnfbbc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcbdguse.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gpuxqllrs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzhapug.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmcgludw.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gttpfgpzw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gouosyyqa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcxesxdy.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvetvgmv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxzgziwz.sHtML


<!-- 参考信息 -->