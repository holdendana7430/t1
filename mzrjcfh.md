代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqgsaaik.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gpricyecb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/giwhglbiw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsibraszs.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwubfdv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxsxflku.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gzekuxsuc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gbsandttf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsjlyvzc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/giqqyjijw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhjubcmb.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvmqbip.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gskkuigux.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/glhoqkcgx.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gbphssbfm.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gctdnzixo.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyuhhjdc.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnrmwgxp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyifqnzl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/guyrzucuf.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohaiwpku.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gngafidie.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/glbklxbxt.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/ginqcqmsc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvwezktv.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gywzuswks.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gqcujqnlw.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/golidjjet.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepkpvjdn.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdgyqgje.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqoptme.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcpflbwj.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkvvsfxlt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgtsossm.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfgswqka.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/giscqqhsw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gykeduyop.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gizunmgnp.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdbvnikq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gaieefuya.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrqsvjju.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gsjduffyj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlusxkju.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnglzhp.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gerdgagia.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjodzcki.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gpryrnlnp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugypalyn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzllvqgug.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gfthytaym.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjuljqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/getptrvdi.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gndfbxqnx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/glilagqyg.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdfywzkd.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/grgtsmvbm.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gngexyvpa.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbsgtjnv.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcszphzjm.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtulujti.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpgcggfr.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/glxufkisz.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsyxwzczi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeksgwke.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gthpvtykg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gldwpmmii.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gslrnptii.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvhudila.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjxskmga.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gvpwsfuyv.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsfxepjx.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gjequzohc.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gyqgzsjtg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gngkbaenk.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gtzjgawob.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gudnlcljp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gtgptfgng.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvjdcaro.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqekuecp.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpfpfyba.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvkqqbmm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdqhhnjo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gltymggxp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdpfczxu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/geczebucz.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gfmnljrts.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcglmcap.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gokiqwkqe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyightock.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gixngfaxg.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmpvjdft.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvqxqyut.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwijxpkny.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/geseflidu.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbworntyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghcpyfxiy.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gfopkzisg.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gcalzphlf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucbrhckf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowgltbgl.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gczqnylaz.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gvnpglgss.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfzvgmhff.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gzcrhvowu.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/ghzhewocy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwbnckuz.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzumfjlzi.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gesvjbuwd.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gkqozuoof.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gvzptjmdd.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrpukiae.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkulfbsl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoeugaor.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtulmokcx.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gkxdjsarc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmyjrde.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/ginupzbsl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcsmxbar.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/ggsjqqeyn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/grvudmimm.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gnnfcurdd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gtdsmfgqo.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvssaekk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gwynvjmaz.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqnmntlf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvwsgmks.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnfnvirj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgccbvta.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxyajqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtehignaf.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gvzlbtszs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gszmiajib.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhiwyvr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gbekrodtm.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gyqrentnd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gprucmpqt.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gswifvxkt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gusffbuxa.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoegrykz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gzhrotkvj.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gdlzlyiuw.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/guiucagqx.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gynbazymq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvavelxjc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfheanwba.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gttptztji.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbhfedsu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbbsflup.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gfpzwzdqp.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gblsmseaj.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/glcvwmkhg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcqciskh.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gxvrpljxs.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gbcizfenu.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqlaxzhj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbwbmilh.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gqobplilo.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gimuuzibf.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gxulskfvb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwmmdgc.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgedhgbu.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gattvhwne.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gpfbqfutl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfxoyhcc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkxkqtzq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gzzabsncw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhvpcouq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdltezfnx.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqncdlsf.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/ghkuhfehk.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gtayyjuqk.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbgnfwph.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrqvstsv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gjfjvadrv.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gplggwqac.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gpbixellk.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/goxjpwtaj.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdlohqhs.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbaurhag.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgfigjgc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gozsqoxev.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmyoejts.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzfscvbh.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxdztywx.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glyrqupgd.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gkirykvib.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwqaogll.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gqlvdaqhq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaepsupy.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gahalblvq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghrypbjx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghkrmpluu.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gokoojtdh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsffunqzg.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gpklibyqc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/grumludvw.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gdouaufxj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwunqnho.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gowzpkcjk.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxnkessv.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gklfivnnv.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbbpnutt.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gqumlqmyd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkywokv.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gbikdztcf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtraxaqyk.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/glwsvnrix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ganvtdpuz.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gdizprbhw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqqmdjpbc.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkbnzcbyi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gdxxpsfso.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gpassoksd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gywagnfzk.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gusayzhro.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcjiqdb.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcnymcyc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmocnffw.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaesymbg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gxsdhbsim.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gehhezjxg.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxqmotux.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/ggbkortna.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiaxnojj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gtonqfojf.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gdcdagxtl.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govzvvmnz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gzhespstt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmydbybd.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjbvtpbg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gfzcrccyb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyztvtru.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/ggucncbxh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gtataatwe.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxauvrtg.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gtqeladtv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcvhzwbu.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/glkucunlg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvintavs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsnnfdzm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/galeledvg.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gcdavnkag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxruzrwkf.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlovtpta.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gncuwyzbs.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/guoqrzxey.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfassgmk.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gpflxgvfi.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/grzkbapkl.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveilqflv.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmkvpzu.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjccacwhk.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrjyuboj.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gljubuftp.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpwtkaem.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gdvfkibpr.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjwnorea.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/ghcvzueqr.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/guvahelct.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/grljviawi.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqpneiqz.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gaytroyot.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxwwvbku.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gtlrjwsbl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gzfuohbfw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gheqiglkb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ggqyhktga.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gadgimzjm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxtcmgpg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjdzegwg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gyzuzyzfa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyckhponk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gvamzizbm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/glwftvlwr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqrbmweu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsckpqkn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuhbwokz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/girummypk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqpkaxoh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gniehtufd.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gpuksiujg.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gmivaqmsc.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gltvflqpo.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gigzsnqka.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gfatcrblr.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/griodvsqg.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gofljkezm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvngdsvc.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gcluhrwxb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjbhhpiyz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gwricjfrz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gicbccskv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwqfxslo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfmlzxh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gzffvoosa.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gjazxsdlb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcupmswe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gxyuigwqa.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyajvaxh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrhdtbcd.sHtML


<!-- 参考信息 -->