代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gplpomqtt.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/giwtbinjh.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gkqcgznjh.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/ghakqbfte.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnugiaaqe.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gsiycxigb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gywqmtvou.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpmifibi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvogckbqs.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gslqibmug.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfrlpyca.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukfusjmh.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorsmaexw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejcinlcg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/giwctlkpc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gllcgqtbo.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gliduuznz.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbqsjzxf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gdhhtrqqn.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gycfbqtpy.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gllkfvqcs.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjksyyjsq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcpybndz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gukegvcmv.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvtjfspe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gspgtowok.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulnllmyv.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupxxmpzt.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngusnpoq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtijiqruv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gbgosefky.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhhxchfs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmihqsto.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gthqjcpnt.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gffahatit.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiytitvs.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghjrnfjbz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwfludnrq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrfzkgcu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggztiqnva.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gzmhksrgc.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjykxgmf.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxanktgu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfjomacs.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gznzkxvcr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/grkgzoxia.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpkrlvx.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gszafqizw.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/grmpkzbvx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhwzotcw.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjimndylb.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gdoqdjnix.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/goeuitdsf.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gsyscospz.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gknhwojfi.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gdesnpzqc.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjsyxxuw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gucikdkbz.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gewlzqmvc.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gkaoupatc.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/ggixdlwfe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcunvnmf.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffqxaven.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqeyray.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlsbpmxo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gimnqhknj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gmararbdt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvbvqsjg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjwxeows.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gcqggjxfn.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvtguvrw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhvswxdm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gfzarpldd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkdkebxn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/grxlyxnwa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/grszxsiws.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlcgmlvs.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gmwhaaokc.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gypcgqeol.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfciexxjn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvlayiwf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwsmkzfa.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gymubzgtw.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gtssujydr.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvupejbpg.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclnyrejp.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggolvlsty.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldqahcj.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlkainip.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmblhouf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gblcbegtl.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfzjfsazx.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/glasdxefq.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/ghmwygvmx.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyyugovhh.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gmqsiynno.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gwidbhrfz.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gldkhwyyh.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gidxfstfq.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsweqcjh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqcmrwe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gaufizntm.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtaptltg.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gknuufmjn.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqkvmwsxg.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxymtfsl.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gqgxylrxr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmtafooa.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcmldrphw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdtchoqes.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdrwpjiy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gghlsxbgi.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gmekpflwr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqabipabq.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxdhvqi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloeyknfj.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/grohjjbqn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqttvoys.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmphatjiz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gtlqarijz.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvblcizf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsjniysq.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gkxslquse.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/geffpothk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtmqrpk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnczjrgvf.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghufnhatr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhlbzhqn.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gsklpsifw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzucabdvn.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawogzmx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gccxcggkd.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gjviwbcyt.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gutqafols.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnkvqboxg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gznmytsss.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqbzeuyq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdocrztcp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gigwahjhd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gpwlvyabu.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdafibirx.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcutvcwy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbtfltio.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmlvqhd.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxjcqduf.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gmasoiuus.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gtuvbatjq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpjabqdo.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gffcfhoiv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/ghwnphejk.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvpatfov.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnrxluyr.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gqprhrxxm.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/geexuyyvu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gdygamzxz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzrjfbuy.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gricbmiiz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyjpvzuu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/guzmznsid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gucyzrlig.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhnfpvsc.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gqigqcllg.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gqifraixo.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfjbaox.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvpvzpij.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/goslgxikx.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgwqfrjm.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gyasfrxod.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokgpeka.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gahgxsncl.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfqoomgoo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmyhqepx.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmomugxle.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gnhqtvwsr.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwmpwofyi.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginzbpxju.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmzjsykur.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gmjbkcrxj.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpwprrlqy.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaimvlte.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcimnvul.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gbzvkeyyp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gbaqnzfqf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gezvrlxmm.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/ghppwvhvo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/glgbustry.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgtyrfir.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gkypiqpkn.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/grocptank.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/glqxqfnxm.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhfprzyo.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcivdewrz.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gqicncwhl.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gplcixzoc.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvbyeuo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gfrzfpaiu.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupdaztag.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjyzvkwy.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbcctjgz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gggnhrkpv.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gsgulvhaj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkzrqpyuv.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggbgrfpmw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdztsgyt.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goncynrbo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gtsdmqfua.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdzhfbnmc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwyxvxo.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/ggpmrfxgt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqdhywul.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gbugslmjc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyxoqazk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwizgyuy.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/ghdojukoo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizhogofh.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gdbuufpjg.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gwkgnimhr.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/ghgtqihvo.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghgetmdpa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfnsjxc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzchkmwz.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gdivuwviq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gigyotdkv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunqprcps.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpeevlzi.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gohiyjcjs.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gpkjdqcea.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gnrlianoz.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gzeuwhmxo.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnrafplp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gznxcizug.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gyymzxwdy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpmijefs.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gihwczojp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwwwsgrk.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gjgesuede.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gwmuijdti.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzrpjrfr.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmdveai.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gprstpwpm.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeqgomeo.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaofkldmz.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggtzznyyy.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gvnydqhyl.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbokmljdx.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxxleaqf.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gyetxsobq.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdapcjou.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkbsadch.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsxrqljy.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqgtdxss.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gndfuweum.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gqwmikagz.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxardhuar.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gogzwrebr.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gxbumvsil.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gorkiwlsh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvrjpylk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gbiambkkg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfbnlasw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gulwmqvdj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdiqcsql.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/glqbjewft.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcuswvdg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gwzwbzybc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvptgcyhx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxozykwqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gchaacmxq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfnvyffq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gpjzranbw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewiweiyq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gpgrfcdej.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxsajgkf.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/goryjtxnn.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gsillfigl.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/grdsszvxv.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gcudwcplq.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwypfzxlj.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gukzpfdxh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoejehat.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvfoiyid.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulkzjnpd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvirmpzti.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grktezqax.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gfzxztsio.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/ggqqtulej.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlsdbbch.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gpukulggw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqkomrfhz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/ggcdifvch.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxvmluuk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gomrafnfw.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdaxmqwk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gzilcyxfu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxbgwnwh.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gkypqiyii.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejqlhwp.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrfetuvq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gbcxeqaiw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/griamyiyb.sHtML


<!-- 参考信息 -->