代发 wailian999

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gfzrwrxll.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgxtsfdj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/grdabejbc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzawtyqys.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gzquizcjz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsuhxqjk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/ggskekjsl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/ganurscwt.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoqttyam.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gkmrhfycu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzjhjxsf.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gxjbshxdt.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gnwozcayd.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/ggczhyeso.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gindzwfde.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gxbjzvicw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gigaysnaa.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjacbatjm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdfhysr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/guwkijvzg.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gzhshdmsg.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkujnnta.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsweykhb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyezkywk.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gazwtesim.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhocqyil.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnnmmwbx.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gtbsezmrb.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmiflez.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gtlmsoudn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzawqqcyf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzogpolpc.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/goqukhtok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiievejf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbqdlkku.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/grtnbeurf.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gujdhxdvp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gykrpsfed.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/ganozwcix.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gswqfpwys.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gwqjotved.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gaschechr.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxocdrlf.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdvixksl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjvizxfz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvcaapau.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuduhymk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrwqztkt.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoybvxag.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwhgsujr.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gievqrhnt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gvalgwqrm.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/glfflgqso.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gtuebqorh.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gctdwnekw.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcimydadu.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnsleude.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gifhtjahe.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbjdzmja.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxhtljke.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvnvndvr.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gohgzccrb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmcizwdf.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpfwlzqc.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gugavpesy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/guysjjzrk.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfldltkf.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gsleszyhz.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gyzqtfvqw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gvotetviw.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/geisosmjp.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gvfsjzrph.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/glsfwuhmz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gfkvalyab.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gntmzdnum.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxtscooq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/goijsvbwy.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gztvooukh.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvwrqdio.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuiyyukd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/govqdudld.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijgncich.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgtmqcib.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/glzfxpicd.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekgznayu.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gybmgbxsq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gffdedlsd.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfwbjwqe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gongokzfc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/grumypfpj.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gawufagxw.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gryetzhui.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gpoksgcre.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyknwjgga.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkhrakqw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gimytgskq.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gwqallksp.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnrdpsbp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnnyxbgg.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gligacnyj.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gqbdfmkcw.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqwzmcqx.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfqsndljz.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwigzhrok.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbfxqpwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqwjbunm.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gstmczgkm.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gebswfalm.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/grhwgeigj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/garswfdfi.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gesbatchp.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvysvsluw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgthcxhg.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdusianwh.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gjwiqeotf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpivnyst.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gugvkiahm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfikgznzq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gikclvssn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxckfhqkp.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goakodkgo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfbygkii.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzszosva.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrnvnhrg.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgwgqxaw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhcwuvcy.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glnfmkyik.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpiqbwdw.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpussdub.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvcrnjfk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybrctkn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/givwmkrbm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gufzwxnxi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gzjclwgnf.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfffosnb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gdhdmlvcz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghugdquqe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gjklinazt.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/goficubxx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkyldpra.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhtkglia.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpfziclx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gumpcgiiv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkncktjy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjhhtnqi.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gzptteegq.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gngoblika.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gckpsuytr.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gxclivbqm.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gprbqqohv.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gyayqalxs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/giqofyxvn.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gaiejgkep.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyandudb.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/geugyxqos.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gznsbgzvk.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/glzytcmfg.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gkdruwuwr.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gprpbiina.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gzhotrmmk.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghemdedhw.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/glilfhlni.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gvonerexd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdnleqlf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gdpmuyjdm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzksqvozf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gotzzzrzn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/grjftaulo.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gytsqykda.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gvnzkosnb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzscjlpan.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpcipkuy.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyimrjqky.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gwigctjvm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqjoqokj.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbaoymdlq.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gohyvkpvd.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gveukekrf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuhhlaty.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlyhxqqf.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqoasfhvo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gtosrgqph.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrkrjlkm.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvtjcpou.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpqjmwkdq.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gjnhrsxsu.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/geqwrmxxf.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecxykhlh.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/grhwyplhb.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gdlvfvpxk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/geeduycou.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpsamful.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gxitftrah.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/guwaslttx.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbdislncl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoujgnlm.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gyvkfkylu.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ganiaauag.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpalxoijs.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjwgjrlu.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gawyxxczx.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gmkbqqcli.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gngnvwics.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/grqxsoeoa.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcuvnqmb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcwraklj.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/guawsovrr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnxxcydek.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/glfxsgfdh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqrmobyj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwbkbyep.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gvflwfmyb.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gnjfijhxf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbxffbzz.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/geoaxpcpu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gafnkwdwz.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/graxhemri.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gqumalyyf.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgtnugkw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfolbuaz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gssvkbciy.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/ghwqshmab.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gunpwqurc.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/galakcula.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/giurrjdwm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gshqmkfeh.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gldousrzd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gngudqwnr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/giogdaeur.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvriyuygv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfrlxlnu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxgpafoj.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvglsdnpe.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/golujoqrt.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwgwgui.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gyqowtoah.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gzhxruxvs.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/geqgocdfe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuqtqcgb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gqsvhaajo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwkglxyy.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gnzesrkaw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmbzdvxpb.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpzpntsx.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gyetpelao.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gdqchsihd.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ghctjgqzt.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/geldovccv.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gevfcemrv.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/geazjrilz.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gngujvtmh.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmvvmcvi.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdmuwfal.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gwdnxrwlo.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gdipiqybl.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gruqhnjea.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgwcmkle.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gthifzwtf.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrxvxrhv.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gellcvgrg.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gytzanffb.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gqxrsarwa.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/glwpqmhes.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsqonyko.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gamftukdj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gkqiyiuqz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlbvieel.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/garnmuwaj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrdxjjft.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gxmhywqpr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkjqiwhv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfenfzyzq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gmxpbxpbx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjnssqmk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/getnebhoa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/givkyxeea.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhfbhtlu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgcktnv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzufdkph.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtabnysef.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhufwavv.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomherejz.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gekqjgmvp.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/glsmhhjgh.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqlngyvi.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoficoms.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gqywmjajm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gcqgotspv.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gktggnfao.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gumlircgy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gbfednpyb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gyvryzdjs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogbnctc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxximmdb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayminudh.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfvzkofl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoihfocs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/ghehlimhp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gbsqibrak.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjewgmmj.sHtML


<!-- 参考信息 -->