代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gesrbrbzc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpisqsqo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gzuuzekxn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkxfzliq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqdyswki.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gycqqesve.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gwxsqrsxl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gmctjhbgw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/goxpfuyvz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gougokwxi.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjvgbuv.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gtlwxphha.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejftveem.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gppoznawy.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzeeuwbp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueozztpd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gzecifutc.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggorxwxbh.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmedvtmk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gtknkhxvk.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqqyuizkj.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggvfgxvmu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnphjfexv.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gstkjuybf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdatcfdkx.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozsdekh.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexrahjzq.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gttdoujoo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulzhzstt.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gboydukyo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/geedihovm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhpkdkhz.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/geafgpgdx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskexzyrv.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gpjlqknuv.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitovdws.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/glmnthbmv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gnjrgphhg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gdhgqbokw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrioqptn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvvdftit.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gfxllplgb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbycgbbh.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfqdspp.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaviiujbe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gczipcebt.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvvbuhgx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhhtnxmo.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhiaznju.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmruvaqvy.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewldgjfu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gbilujvlm.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/glrbdkswu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gjhmitztl.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdqhygmw.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/grgyqkypt.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjfqjqvj.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmhhjvjy.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtmjfshc.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/godlewrfu.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/glgzxjoxd.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/ganxwflxq.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqbgrqlvd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqnrmcia.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gielshsvk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfapkyw.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwupdoqlv.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgcnfahy.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzcpudit.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdjpbwfr.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmxpkcaj.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnvgmvlf.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwufxmwq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gwbfyrcpz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwhrzxeh.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gsalgqsjz.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gsoezjoem.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gjhkqgibw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpjqqmrk.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glitfmeni.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gycounxql.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gtnenihco.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxfhjfmy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwgzcnpx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/golasgpgb.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggibmuyyx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjpxgtnk.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyqvuesl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwcsgsiv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjaekcbx.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gybcxsann.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gvnrmjaqe.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfcrexo.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gugxpqnla.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqrcizk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbxlntvd.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/grzcqocea.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gssdaepmo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/guoyrfdqe.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsvfzzti.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeywwrcb.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhsznyfr.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtkfjweyt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsvmckk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gikeimzpo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeybpjap.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecuqejih.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzgnckyn.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxeaeulu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/grprwcoav.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrmganxw.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcumwryk.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfymvrrwi.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfdsvqdf.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gbibfiwtm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/grlvfmjre.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwiawydwh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvitfgdbv.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gppdtuhkq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gtbugsbsy.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcikvgkjx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaskvfjhh.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjziesx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvsgddl.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gyltttjcd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcokztyim.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpxavtdq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/geqwieylv.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeluwehx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gejxtibqf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gubgajpnf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gabgckcih.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gamibmttb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfkwveqs.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gptzfhglm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gjchxegmu.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/goyortgqe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gfozvajxo.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgohsamq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgkrjcra.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gahqijfzx.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gbeclsbnc.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqsaqonbq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqjwgzq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gubyrrhmy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/getahommp.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvtrkntl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/giqfeabqx.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guucjfkoi.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbiauak.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpeyhjy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbntjkvn.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gaaaaaysh.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gtuwqgbpf.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gegsvrnkl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrgploir.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuizqbsn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxcvhuri.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groekyuky.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gjoyjskgt.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gztmzaeld.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/guswjjjgh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/goofnqyco.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/guctgofac.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyudctevu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/glbcwxwev.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gttsrrubo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotytmzhs.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gdfkyceso.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gkykgooov.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gynlbgfus.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gspifwhld.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gyoidhjlq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gfbzjdhcj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqxttbyc.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjxgekhs.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gymveazbw.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/glfvagyqs.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcnktytmu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjziegmxu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcltxkel.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbtugvz.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrglvbsk.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbuutxhy.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmrilmml.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gwjxmidrw.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghugemqjq.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmjhquqmr.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gsqcqwpqt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvwregfj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhituhpg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gymbercfm.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gboduhiqg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpthyvedw.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gcymuzosz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvkdbrj.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhugakxe.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojdxpjtd.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjyeeoxax.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxpdnin.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghkwiyhq.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoybyfuo.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/guybensvc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtjpjjkq.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gfeelgzht.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gpwfhwzbt.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gzofxnkbo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzxpqlij.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/givjhbdbx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcoombyn.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gmekckigw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywpbnhb.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfhgxzda.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiivjexq.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/geknhikxb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gmtbmoddj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihnwbpt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gkuccedhp.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gdxwjhyym.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzcgyuhh.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gkiorsckr.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnrwmklu.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtahytbuw.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqjpnhqt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwenggxg.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlfnoczq.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqkfjsqfa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxgjumvva.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghitwqwyt.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubtltll.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gujtamkbh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpezcmvf.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/grmprdvci.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/geborxqdg.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyiyrfap.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwylyaytq.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/grnoljgaf.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/guspvgtqn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgahxbro.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkxhmwlx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goxlukavv.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpucrvfmr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvayeokx.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gvlbtalju.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gcsipfmaz.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnqrzkxb.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ghctarzwx.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsofbqhn.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gigmtslhc.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggodadkww.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdouznok.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gimnvnajl.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbrghvtj.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfhhgbya.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/grqbhgvka.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnkjxgix.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gynorefzy.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/geztozngz.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gjeakvdor.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gythdjdah.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfggcanhy.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvabcsxi.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gocgqfljh.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/guhmnjied.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gufckzsnj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/giqhfxwaw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gxznoziso.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gclxsblja.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gaptmyruf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjwcrkvv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoohitmy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/giqqaeozo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguuwrgvh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxslaxrc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grysitqnf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvhaebhk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gimgbqenr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtrpncza.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevqywgn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gswvgjuov.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/giyvivvvf.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gtupdjtzp.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gelkdlbfx.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gqufnxezd.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmvjhitx.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gaulpilrf.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gnagojbbx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoyjdjxl.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gdulmfehr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkplaven.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gfrkhvrmc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/giuiolfyz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfchvhqvh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gvuswwrdp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gyxbsdpgk.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gktcmleqp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gloizvtml.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gcxchoerj.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsekqypf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsbukunn.sHtML


<!-- 参考信息 -->