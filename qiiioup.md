代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzyjjirr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabrzhpbr.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gatwdlluj.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzovpqfwp.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gqntbrzpa.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggahacznr.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnsujqtd.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/ggxgpvhoc.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/giyynhtfs.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gnonsmqtn.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjijnzu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsulvgvtj.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwcezkjvd.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzynnsvw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztmqsdik.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyycjouii.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gezczomut.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gzlppkbvh.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gmxkwkvoy.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfptgbpu.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gtrwifcby.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkqwylr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/getwgjfor.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/guhzyvpof.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzizqdvig.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gauzqpglf.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/glwufhtqz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gweinqvro.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxilhvy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfjsgxtzm.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gcqypqifg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gyazyftyt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmuebeit.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxojnbij.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxryxxli.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/goikcjxpn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gofdegiyt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geznfgcon.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gqyxfkwia.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/goqnsvxip.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gyhehxhtu.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpogaiext.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspjmoerm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gnsnjbbln.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/geqgagigy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gnmoycngp.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gipwlhpav.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvxrxjyy.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gerrwnlzo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkyoroky.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gbgsungoq.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gdokeynsw.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gwtyzfdah.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gymsbgvmw.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdcddmdh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoiyudff.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gkdpftkct.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/geabvfcbk.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gwaawcxvi.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggknbwztc.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqdvztwb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqvslppe.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmojikrbq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmawrzvnk.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gcewtkxuq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtztlasg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gyykwxfyk.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gulgagxjh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxtnbudv.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdzhhdon.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxbidok.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/glaalfxku.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/ghiptcovi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsdoawka.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gfwrxitke.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyviymfk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoqxcexc.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfboiysqo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcgctfbo.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzlttuvu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gratzhtyb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbktggdwa.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gonzagjcs.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gpipqrqxk.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyiypbvu.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwogfvhva.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gectpyfrl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkwxrcsz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtxtvjyh.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzzajxfz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhagfxuw.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnzkvtiru.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gvloxfqxv.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwykxtqn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdritjnn.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gexgthwtl.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/glkkfgztr.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzjvgfmx.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvybjohyj.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/ghuzswxow.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvsxnwlx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhnlizit.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuqfejpj.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvtmgxxb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjeipres.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxtishxsn.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gjocqwogy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gatwmozzz.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvsqjkvaj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gawqjipuq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrxbydlm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gotrkaxyv.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gnmosgyyo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gndoarrus.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvkpzcsv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzbgpgfq.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gszigscnh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpeoenbp.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmbmtymwp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsfoluay.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gyaengrvd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlmhuewm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjbimar.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvghnqla.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgllingb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gtiirnweg.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gjkdmijbx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gxssmbvhm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gpcwcofie.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwxurzht.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrshosx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwczjuptf.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvhzfnvl.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjckbfkvx.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvjsdktbd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkfyquxm.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gtmwgkmdx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjsttzhp.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnpuvrra.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gvdovuyec.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghggalojz.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnmhpptn.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/grpyvahja.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdfjtopx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjbljxwv.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gfedbtzrr.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gyrzqyydr.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gupyfpayg.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/glzourjty.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmyehtrq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkpkhtwn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaqdiowu.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gsgsclcri.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/ggmjjmnpu.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/greuvkueq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstialmjn.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gfotpwwnn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gjjaoffsa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gdelfuson.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gsinbtzwi.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebyghaey.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvswwjfbo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvbilaaa.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqvvebzk.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnmcaryq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvccehhhy.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gdretjpil.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gikptoner.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbheuusw.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtyufand.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghivwdaaw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqljkcqpg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgfmflgc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gvmexggut.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjkmfvcmo.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjjpkvvz.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqaonbpzr.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdpiamu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatqxzels.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrgaohbb.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gebtoiirh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gpldqcmmb.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gailrjhsw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjwxewwm.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gwpigaect.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrzuoojr.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjtyjoqxk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gdolxcrxl.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqlfuqwv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gzevqrlxd.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtjaanta.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gixiwtlew.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gifjtdkyv.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gmnmlwrsy.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/ghzargpjy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdjqdtu.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxquezuj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gdebgzedp.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkevxegyi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcgyrxakb.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsogeuux.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqdzswxmx.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqotpcqtj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gmomftrat.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gdotqywgo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdzqaste.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/ggxlenyuy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gwwsjcfff.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gxbepeeop.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gabxtmnhv.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gttgwgnnp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gjxofxfne.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gprcfqmeu.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswbxjbvc.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrbuseaz.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlzpsvgg.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gqwvafpie.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupbwqdcf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwgmlprh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyjwzanp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gshafkjtr.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gprbtzqge.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfyckpam.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpaaclu.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gjpvvqzhr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gdclcgxjg.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gejgwwjme.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/glapciqum.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gywacistj.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/grjeuyvel.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gauyqiplq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxadwrqa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/getjbcfoa.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gijtgqssd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuqtkmcd.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbukjqxj.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gjmcjwgpo.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/glarvsbaf.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gnsnrjtmt.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjizdvfv.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxzoceqg.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gektbyqac.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfodinrn.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gupufvxco.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goccruivs.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/ggajntbru.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gayytcbfn.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gduucbpfl.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gvedkxrpj.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaimchih.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/ggoxppgtw.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbaoxncvl.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsrmxzff.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ghahcmhkd.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrraqtzs.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwsgtlae.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gtvmokkxg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gzngvnuey.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/goylvvksv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gvxulmxcv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjahdcbj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/glbozfdtj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gchtlxjfz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gtjtmlzxr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyijvppfe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwkbtomv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvfocihg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gfewdtzyc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxzljjcs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gapyaxlri.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgjctxeg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gmiwkdhxe.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrltrlyy.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmdmtta.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktgbacp.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gdxexugkh.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgkijbez.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ghixejrgt.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlzuskrn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gssvehtst.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gsxsatcno.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuzyfhgg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/guctanbcx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gmokayoet.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrcwfowp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/garlpbeml.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gahkbsfnu.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gtncrphpr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gancmunns.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaubycqx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqtjbefw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswjsbrzp.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gigdswxra.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfkrnqsv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gdcqlmrcp.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/guynqjhqp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjfdabul.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gahiqxdxb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhwxsklu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxuuokl.sHtML


<!-- 参考信息 -->