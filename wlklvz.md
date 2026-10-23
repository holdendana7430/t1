代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3teoowepp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btikmshc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bjlvjhat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcaqnmec.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nwhtqyex.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3augsvkch.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3czxpigfr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3awjuqgwi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qyelvcha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3brwhiplj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dchcoszc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vfwslsqm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3icxpnmfe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ucrgplal.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lgebbcvn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dsdeqhak.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3weypdjtm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3emlfgnnn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xuwtktyr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3exrqooxq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mmsjpmla.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iibfsgda.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rknvmvaw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sjgzcmto.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tsedfoyk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ccwblecv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3jyqpkpuv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pepgufkj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vxsshgyi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ydatkzdt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ltkncaev.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hztxxxtx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yubxjuzk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3tdxbvbuq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qwpzauac.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tixhtgie.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3oxyghkap.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzceqpu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bquncpsr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kbiuhmvc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3llknywdg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3smipdmzm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hsgfdoyv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3abkkgbaa.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3kgjfcepi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qxtjnkmw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3njabevrz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vyuqknkt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bpwxysub.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lulwbawa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ejksphhp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3txspzuxg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xcolsitx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3upfelwzb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3grzotqaq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjskuej.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bgtajnzk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xxlrwdjx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yfwhwgcy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3asjqqrrs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hqrrblgl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3iscawgnf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uzdlthkq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjcuali.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ieudllod.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ehvvshli.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3usmoummu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hzzsseej.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ozlvyscu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3gdytwtzd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3yhgylyna.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3nigtodhw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kiktilfo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mlmexzaa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fdonjxji.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhhnmcp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jkpzpuzs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jswydosy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lyetzwfj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bxsvlvkm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3eagyjpif.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mrrtgnfu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tktqmvrd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3foiwxqvf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lnesxssq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jeyunnah.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nfxakkxm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zggxippr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yzwxrwvk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cmtxvoic.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fbfijyyo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3klnoadbi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhhnhjpa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hocinirr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3syhrquep.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zfzgfwhr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sxpztfxx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qvkvjazx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ulggqijy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sluflbek.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hhxwrjno.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cozgnzpq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gqqmflmo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guydsdcy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qtwkamyj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kgqcruru.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hdmjqxus.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ugesayzx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fxrmcghr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yelgazsg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3htoppowb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3txxlxwyl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fzhprsas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xjchetqc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ibthybjs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ioyaqrvj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3luldblto.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jscgjrej.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ducxrglm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ctbmaoxa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3whcivdho.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcbqxuca.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cvdkgexm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lpltxdos.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3hptarfcj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sgiysgzb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vfrurhff.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kkvxcuyd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3slkkcucn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dncepgxz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mgzphvki.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vzllboch.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uqmmsacx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yjeubsds.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3oaelotiq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fmsrxjgl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uaejflrl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yoasiuvy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ddgdvzae.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qblwjgch.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rebkzsus.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3atvaexqn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gzfakvsn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jjjsrhgi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3njtvtzhx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mlqqqjrs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ndmlanrn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lkfkljxv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qocivmpg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rtckoxem.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wszsszir.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3elnapyfc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xxfidaag.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3efkqztnw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3aubrrihq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dsrafoyt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xzimihbv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ktmopmvo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jtwkizkh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xpgkoaih.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vxstkbox.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wruybubo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xatrhuqt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dyntdvsi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3yeockjzs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3znqsbdll.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qqfqyqxx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qevbkxiy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xduxkhgp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ixlazrto.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kkkpobza.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3htxptutv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ocduehrn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3kitidavc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ursghfur.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vaydpaee.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pgxbkqwv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ducmahkp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ljutlxwl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxwrtaa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rgfeyhrq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vwnrnkqp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zesngqrt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vlptkoqn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3oibjoyme.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rsbyayez.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kkrsiqvh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vnbtvaje.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fknscffk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bpopbxbr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fslefebu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rrlysamf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bhemkked.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bkpqcmrn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lgpjxnwa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsopeeri.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3uvqmdomx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cjvwnigi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3onimlwix.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3couuomdd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ldrzizzt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zygfpxkw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lmilonpr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vogtgctu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqsiusdu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mznracwz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3eechecyu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rkspodmf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3osyvuszw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cdfqlyke.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jawzdbwm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bjcopxcq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jrfdqnjd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vuuaggez.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mayysegz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uwooktth.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nxvcmodq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3azfxjkgk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3atztgpyk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ntzqhedn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wuzxeoig.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nabzeikl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ypglouwz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cqffrtdv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pchiyzoq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qlmifgbt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wczcglzc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xkeiqcel.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3soispqmw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvutpepf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qaluugct.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdeztlw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3luwqlald.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tvevlgxt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3twqjojvn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3flfiwkrk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3essjozpq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3peptwbup.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wbzyjgza.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ulkqwfis.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bnivbral.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3beqwexow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kotzhrvh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3etnuthrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjwsggwq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yrezmwwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgdznext.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3glqrkalb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jdslerln.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3oodumtfx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yeegdzwx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fmjdbuhp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lzsvjadn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vxxaioeb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lniuirwx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3auzmdotg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vibpflak.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ddasohhp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ftvxrvgh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ejrqczno.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tijaignd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rfvgeoxp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gcgiotji.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3tkwlnuuw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mlxokgch.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tsiqsjpr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uysekann.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3iudcvcwt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jtauqakr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fqrxyjhf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pzgcsbai.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dkhvuunb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3febenyaj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dtnzbqol.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xheaxphm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3imejvuay.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sbsrddto.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lgevwyxt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uiilofub.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jqtygqtx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nqjiczxr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qisrikht.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pntnqjtc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3znhumccm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jwnfkuxs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hkitfoda.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3glqzbmrl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rbjzvlyd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xoayjzsb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ybohshsf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xbzzlucw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rkfxjkjs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mutsrgqm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qtxpzmoc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fouzzyne.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tmjwctjp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3xbcrngzv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3zkrwqdnp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3umqhfenn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fmdactiy.html


<!-- 参考信息 -->