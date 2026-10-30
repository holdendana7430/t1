代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gomlckbtn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtqpngjhu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gnubdxscy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxothkwgj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gicvsxpxa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/grpmfvhvr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gozmkqvsi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gjzjybxpl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/ghvmrkhdx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gnfhifamw.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/glizepxir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gfsqhaldi.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/ggjsawmjs.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gsxrmfyfn.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gylbijmjn.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gkilgqamt.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gybqgmfjy.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gqpxiapvh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gcvqvcdrd.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/graurunhr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/ggsgmwzmw.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gvxkdbwmn.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gyjbumylt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gmrwylezi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gjcndrpjy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gntnrvuep.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gmaotecxu.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gbpngktfs.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/ggdhzucoj.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gwnaofipj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/genervebs.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gffxxsjbq.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gvxqwedag.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gvdhozpqh.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gceolklol.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gybbpqwwj.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gvduouleh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/glmdxnenl.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gevallrwt.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gqosttcfu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gtfsbqbar.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gdbgtwfxi.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gscgfdkui.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gbxvvyrnt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gzsivmosa.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/goglphlmi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gprrhaktr.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gdygowsde.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gcpqsrnqa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/guasjhpzh.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gxtuqbesn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmbetnmat.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gskxrmeee.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gwuyaprlr.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/guoyfteiq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gjqiaxrka.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gsibtqffh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gyjykulke.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gazjlzvcx.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/grixzhwic.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gzbrlfhou.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gjrgjllog.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gqojxclci.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gnqjsrtif.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gasjqjuke.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gwxzbnojb.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gugpywtdr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gxlzmghpj.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gpwqfywdn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gvlleztna.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/glomxucvl.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gparejlqx.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gootafxle.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/glruvylup.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gebantcvy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gtctrltlq.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gngerhuom.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/giwlxqrnb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gwlamholn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gqpkdhvrr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/glzfcyxcx.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gxektimfm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gpquxwjvf.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gdmqhdaqn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/glqtbdtbq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/ggemqanzu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/geiuvvria.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmddwuna.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gcaltoylb.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gocdxrcis.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gjvhmthki.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/ggxretpqs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gpmcmlycs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/geplqyqhf.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/ghiwtqlcj.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gnhawfwsl.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gyxkefuva.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxmsuye.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/goaedjmzj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gpqjsufhx.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gljgznuqi.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gjjeghlhk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gzaqbjhds.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gqepvjdhy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/grzvuffxp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gizbwtrmj.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gapifpkdd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/glrvtaxlo.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gbotaohic.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gciynailq.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gimvezyyb.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/ggbtdiarg.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gjthtbvvh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gccrrrflo.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gxmobwzic.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glajqcdvo.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/ggogulrpg.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gwdfgzrvr.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gilhvncvr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gnglortcs.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gqtsyfqgo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gylrjygja.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gfnmkaulz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gycierewa.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gtxmmnczt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/ggyiwnwtp.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/glmunwwrd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gdirwjrit.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gjcuyuzhm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gnbsqcasv.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gyiaqzrrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gvvgdxwkd.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gjmwigqlj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfsxbcidf.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gcexibsap.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/grbugsown.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gzcgrzdac.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gfsnjhdlt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gfdxetkbc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gdfobjrsh.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gciuxnnnq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/guizlczui.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gfjrnehif.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gpyhuoxfg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gdyjtmitv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gafaywlso.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gbzsstjir.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gcvcesuqp.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gppunfkbt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gqjobzpst.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/golvfnpkg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gcaaelaap.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/guonbhdhd.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gsifunesm.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gnnxibwjd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gmfmedwrg.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gblwnwngq.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gkuhqsuqz.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gshbfwbvl.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gaqyxvgtb.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gjizkybqh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gnrpzjyvc.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gvxupibnp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gdnenttun.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gtwbfwaiq.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gsimdvckk.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/grpypvkim.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gtajxkcsn.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gckzztwtx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gfqyzjpqt.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gsumtssio.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gaiojyrcf.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gxjoecqbi.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/ghxjsxxxo.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/glzikhhoz.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/goyfeokdn.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gpyjtvxue.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gfggsqrbk.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gvhigajkp.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/guozdvnou.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gshpatvdk.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gsukitrvw.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gwemxnlbu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsmiffgwf.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gzixryruw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/ghlpdpuic.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/ggmtkizhe.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gumxossve.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpilbzxrn.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gbugiscxj.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gfcnzvhyo.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gxjuiiltr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gpojneohb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gdvqgvcrx.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gtupvlfir.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gnqbauvpk.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gvbpqlvfu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gtugwvrky.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/ggofepptk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gjbutpraq.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gqoxtttjm.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gnrveegal.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gnmsgkwaf.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gmakvxewh.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gjqqtmmlg.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/grwzdihxc.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gitmyvpez.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gahkykzzq.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gzdnsozqb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/glnhzlmtq.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gvxrahxof.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gpoofskrs.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gpiunkihu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/grldrxtdz.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/ggmcekmny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gkucqgckq.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gjuykamif.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gjvgougfi.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gcpbsjcyn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gxmzggdec.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gzpinyxhq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gmceeeirw.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gmabmrctl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gubmougyf.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/guvdouyas.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gahjkmswz.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/goilyesyf.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gqsetfjvy.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gvtbokhzm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gusopqgug.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gfssmxkro.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ghuuriaqi.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gpmborwip.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfhfgqftf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gkwpryuhv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/ghwgerllq.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gpikwdgsz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/galbxnjly.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gwvnqxzki.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gghdhucai.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/ggdynhaat.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gpabzhmch.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gaulxclqf.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gunlebhry.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/girxctiie.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gtklkvbzg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxrkbgs.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gcrzxvvwh.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gltrzgobj.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/ggwftpovm.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/glkxlbmyu.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gdlzsvxzh.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gtkgvhfci.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gazgohroz.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gcrxxpxdf.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ggumhqhyr.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gplzdupgl.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gzypgdvih.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/guxfgdvee.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gzcqdtsmf.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gkduscszu.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gdxmgjnsm.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gcxfraezw.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gwomroslq.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/ginzbqpuj.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gukeekvfr.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gtdgtuahi.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/guckkupiu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gmthcubmh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gwthmnqbp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvyucwyrt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gttgzxanc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gyxcqepsw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gxiifnjav.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/glccyspwj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gmtmlppzw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gjucpjtkn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gjyywlbjg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwkdzel.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gulkspwcu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gzmhicytu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gdmiiaibb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gjpippivh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpnzlrggd.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/ggpwzzvtl.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/ggveknehs.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gpjwrlici.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gtaxxkztu.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gyosanlrl.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/ganjzbiur.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/ghfrhtiki.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxpchzwfl.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gisntebpu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gobrvdyyf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gkfdnnuvi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/guaexigtm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gwfmbgtnj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gtqhmczml.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gwblgkzze.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/ggqmidfmh.sHtML


<!-- 参考信息 -->