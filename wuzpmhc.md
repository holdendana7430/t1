代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gnjsltkfb.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzphpteyd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmrsacqb.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxqjhtrf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelybkwva.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkuybxzfw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgrortgw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gedafdmes.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnreysnm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhjnjynq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqzlnoff.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjgwrnzr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbrdlgwo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmofjwpmi.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsrkbyz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzqabozy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfswoyga.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gysuautid.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjxtyotu.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gotlnmkat.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gofkaidoq.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gfpxpciiv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gujlqnved.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/govcgfaxr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnvmexuk.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/ganrquqhj.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gycwgoccw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/ggpahaliy.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjyjovns.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvgpjpkxl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmmzjvqx.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gpcagugex.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmznucvq.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsqgswkd.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjivlcpn.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfedbbzxz.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/grwoozlir.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gtzqhtlxa.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdxecfwe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/grvlcbvjb.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gskeqnbki.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gokirhinq.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gnnusynmq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gnzdxegqt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxliwvrg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtopjhgoy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjnicgqh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlwtusg.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/geirpbvea.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmvajjq.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gnrotuuif.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtobtcguz.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaolenkgt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gktepfzkt.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjlfjmno.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glicrbwpo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvobusuen.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotbglquh.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkaraoyc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnsmabmv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcxhnaeu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvkbgkhz.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/girdjjjwu.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjvaoegx.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gldppoybx.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gvwyvodlj.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gngebpset.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwfegdms.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gdxbzuedd.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/grbgicwnc.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gciaxbypa.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/glgrrcyul.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gmjrhkynp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsfolwov.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gwdyawpkg.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gwollucak.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgonluwx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrhxekou.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsapzejo.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gqlwwvqhi.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmvtueem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsducnugu.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gxpecupdd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gegcyupaa.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/ghjalpukt.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdidkxwa.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvvovsgy.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibsgwahf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjstgqjfw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gqczonksg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gjzouilkq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamdnkfyg.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gyqxikpjf.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gfwkgtnkj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvadaoabs.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gvgqqhhag.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/guydrlzsl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwcbsqltm.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkcieefd.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gffugoapt.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gomkwgxcs.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gilijbhsb.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknjdtcda.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqfwtzepm.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gznqmietu.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbbumzra.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepwompan.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzpbjabko.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gensxpoti.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gywchgpvq.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmyguwxbv.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/groxtmgfi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gwraushcg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gveugsvcd.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoxhcfzy.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/goeztvfxq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfypobssr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gcofumgbs.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfupmzsit.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtpoavtd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjwfbjhs.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqrfrkfij.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/glpptotku.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gifccgpqw.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxqgggey.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/grddbcdtt.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gviafsynn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gburotlpw.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gpegptfod.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmohivsfc.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmenbbuv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxnqnya.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsymzjux.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gekcpzdfd.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/geqtkxuwg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gfzqeyspb.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gxkhsmvzn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxtbhyuzv.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzggsxqw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghihkyfan.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/guocfdfdq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gwiadleyi.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gadcywqtx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gxgflsblo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/grizvjury.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuysfcae.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gwgcugjsl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/ghzqpmnkx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxuitcem.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbhwxqnj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/giedxkqrg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gdxmbzepp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gnhpsdrim.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/genpdpjkx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geprqdfar.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzlnxtfk.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gsunlzbtb.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gixqvaial.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhfbxrfl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyywziqid.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqtjcmvh.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gtblngowd.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gxjpcxoew.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnduybuj.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltknyban.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfvfmlmt.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmpnxrga.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgjspjsc.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gidusrbdi.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gjzyfulzc.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gicgoffxs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeglggml.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gmbsdzhba.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gmodhmahf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvthmohp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gwwbuoaqn.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaiuaksv.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gykbeamga.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gagecnqmh.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gvvpusgeh.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjuupnty.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgdgumrk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gnimpulrk.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gtqyrcdsg.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gvaydcrfb.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gpcrhzldm.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbthdsoh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqiqlyzf.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gcouxuhol.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gjhluacxo.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzktrkbd.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gutbxcjip.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyggigzw.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/grtqssmzr.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdckveaqj.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gwuipekcc.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqrwtfy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvvbtkvc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/ghdrpjaua.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxcfmvpc.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gnkpuntjx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gsgqaxzhl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoopfevb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gthpkaybu.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfljfwzo.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/ghzmzjtte.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gezvjkdwo.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacnigyzb.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpgpsxrg.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqehyvno.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gvkocfkig.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaphdrcik.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gknvajjad.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gnysfywal.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gznmzazhn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdflcybtj.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuvhywrs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gxtulxlxy.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlbvclbq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gefickenw.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gnjjcbrkl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobbsqvcc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbalfnhf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gguvbkele.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gdvatkkvx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gqmvegncf.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gqzxfukto.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjjaorjg.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gbxrbyaax.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcyxeeoy.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/glpvqsuxa.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/geibbegib.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gppabvvqw.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgjrrbap.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbicnrcnf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmljzkioq.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gejttgkuk.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnltwwqps.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/ghbgldspu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzcnbgfbu.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gngsnbnir.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/giurnboeh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsixoyjcz.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gutaudhji.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivnozcg.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/griforbnp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gjwjynqdi.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtpozjis.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkpokxoc.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcmecson.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gezfuuwqr.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggytxnake.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gmqyxlubh.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gixpuwqqq.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ggykghdmd.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/grffmzcrb.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglahowev.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxvtwmfo.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnumfwkl.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdrjkdan.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqsbaqm.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhpdvayx.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/giilgiyuq.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmzuznin.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmxehuzw.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/goremrikq.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gmliggrbo.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/grnvglcgm.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gzaywumzl.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzucbgrkd.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glevofbzr.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbnwyxho.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdiamezhu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkignbqp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gjwslitzz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gyjmgvecu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrquegxj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gfuerzplm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbflpbmi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeuuassf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghohxvsym.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpxbzyzm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/glxrenovs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gilcgtjuk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluhnbjhf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmbqtajg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklmszipx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfthhqqt.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gnmalhjmv.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gyfgiojpo.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gliesulxp.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/girteiyrn.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpqbgwkc.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuiqhomi.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gcmsitvic.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gcevlbmde.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gvvbbkahk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuuomqnh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctlntwvr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gmroulafg.sHtML


<!-- 参考信息 -->