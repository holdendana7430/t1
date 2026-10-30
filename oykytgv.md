代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gkvuwcqyl.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/glkquhgiv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gtlumqxbr.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gtxxvmepr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gvtrhhchf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfkmelk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/grubnjwge.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glphgvhci.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/ggawantzh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gegrummyw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/guldkxbjw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gptjtchkk.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/grpbablqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gectiuvxo.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gtpferiwy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gstnfikla.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gintvyxad.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gxkmjgryd.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/ggfzxjdit.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/ghghehckr.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gzxfwjcgb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gmxzdxpgb.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gbsqzbvja.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gxakpydkr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gzuqalhfq.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gzivpfyom.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gvjlcddxt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gfyasxtiq.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/grjarxyxs.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gioohlaln.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gynfvloce.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gssfdmuwr.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gitrwdszo.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gfqpeidel.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gezdesyhh.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gwvfhvtee.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gfvoxcgxm.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gigtjuhst.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gnxvqgtju.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/glscdluet.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/geesceofx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gfjdquqsa.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gnzrtwfvq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gzyibwvwq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/guikwqfwr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gknjzyrvm.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gyikoclpn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/ghabmvnmt.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/goplbjttl.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gozwdfngx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gpcjjjeox.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gdinjuvuw.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/ghwkdxgdy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gtwgfoxov.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gdjykxjta.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gkrulyplh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gkrclvdul.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gryttudeu.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gdppqqldb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gupamdlmq.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gtjnpzmtf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gukddxhqz.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gyijyyfuk.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/glisljoay.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gtnwndvnn.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/geyrawjvp.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gvhmizrbv.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gvjissmfq.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gtxiuibwh.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/grtoqybkc.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/ggztxqvlv.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/glrrhmols.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/geeqvzznd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gcfqytwtl.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gpsbfevlc.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/grqeqvvsw.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gfmzdtuge.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gxkxszfmg.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gwlndophu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/giocxnubh.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gxoqyuipu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gouseyvvu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gidjafuzk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gbugrfrqe.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/glyvulgbk.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gcenomdoa.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gcxlimpzw.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gjqzmexrm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/geistpnvo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gnlkjjsbq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gkpzhrawy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gingsoleo.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/ghbpwctxp.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/glvguruij.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gqfrgquro.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gehrdldfq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcsnuxclh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjplswuaa.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gocjiakvz.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gdajsqdmc.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gudpwxkxb.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gsosrqrmk.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/ggcnlroru.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/geilazkjh.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gwhvedgep.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gywndauyy.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gdpnqdtam.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gpkhfuixc.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghedfxyen.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/ggekjqyas.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gjnetfbfk.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gzetbgcqi.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gdyxtfgfo.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gyjtpusgi.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gutrznwhe.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gaoeevvsp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gshalqbdx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gkeszpeaq.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gmttscygx.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gnggfgask.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gogaqsspy.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gdzqfnovs.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gnyydpqxz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gsffjobji.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gwxmqmtxk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gzudlwnzl.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gbkglmtze.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/giqrtlhvi.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gstwwgihv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/geguwbjtz.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gspmkbktv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gjkasywlm.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/glyptrsjr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/ggpkqkcuu.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gqujxxaqu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gctoesjvd.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gzjwsibdj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gplmszszi.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gbdjjiksl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gdhhtggyc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gojzlrbdr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gmixvtvry.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/giegabuzv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gbymficeo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gppfwhluz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/ghwwsewyy.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/guroxdnvv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gsjwwsfhr.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/givnehbim.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gdqrsquaw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gyiqoqkpj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gxeumjoed.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/geflqeiwt.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gurvhfhpc.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/givlznrns.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gmtcwbcvw.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gobbcrbem.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/ghpycvyub.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gseofhicp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gfwgftxau.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gzkgvibba.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gqnkpnles.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gmuzvqsws.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gtywmdapc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gfrdntpdc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gdrrqejau.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gkceyllyz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gcvainrjg.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gaxwufdxo.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/glivbyrbw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gibmhvyqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gttzxmgxu.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gzhtmerdv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkftipmkt.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/ggtsyavbd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gygjymfun.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gztrdlmor.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gluhniyvd.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gcsjxysco.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gjmlpsevq.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gkvcrtwvm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gnkltbpyi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gxrucikti.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/goziwmbhq.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/giykxudaj.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gxkaipzpo.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gvbnpgftw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gaojpahip.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvevmykts.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gzfoffahi.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gvfciqehp.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxjdibiza.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/ghufnysdl.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gcosexizq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/ggpextlwk.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gqmmchpjk.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gqhogiytv.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/giednhywd.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gowfwojyz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gdolnpzmm.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gopiigifm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkiwfmcir.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gecbmwkkf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gkcinguwi.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gddmcghtv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gffcttman.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdubeucis.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gsikkuqqm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gbqqxjzat.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gdbopkfep.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gojpdswrl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/grraeikjr.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gsuyqcrno.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gfgkurwyy.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gasexgevt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdwgvtofv.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gwtwqrwlc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/getwfurvq.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gzwexzgax.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/ggcnajnpa.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/glzpwztkh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gmphardgn.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gcrmbuvjx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gifskdjqc.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gosmdbedt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gfjegezvr.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gzaphlhyx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gwykyguye.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gunfhmrqs.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gqqbugyma.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gwkrhitoa.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gunsjksul.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gqlsspxzu.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjqvbdlbm.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/ggmvzubab.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gmzndjpff.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gvhgyhdvo.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gogjavnjs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gedxpcgyh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gkezvljsa.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gniyunwfw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gtjlfffez.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gvelfzaas.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gsjkwuenk.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gxjajnuyw.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gqfyoecub.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/guzricknl.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/grpeetnec.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grikdgxjt.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gqnxlgwrc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfxdrqibi.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/genkfxrdb.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gtjgnednx.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gxidsfzzj.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gzobiaslk.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ghgkefruf.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/grnndocgy.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gmdxyjhgc.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gqfpvqwgl.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gwxdccnar.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gddhcxivc.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gbhmzwtam.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gqumaglgp.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gsllpfthz.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gvcgedfxg.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gopdbmbxl.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/ghndjnobn.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gzkuxgabx.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gwjxoreox.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gzmrghbsj.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gngmffesy.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gimoalyww.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/geqwwdtih.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/getmhvkqu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gelxtiaat.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gfjjknqnu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/ghmhnwuwz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gxdyprkab.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gifseplie.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gxlslvmlg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gckihbaqr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gbhmilcoe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/girqdkptx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gkywdjroz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gpxcxsrqw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gfowmcqid.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/ggryirpmi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gaxcqpvxp.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/ggxhoaqjq.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gxmtarndr.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gkzrrvifk.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gknqashpd.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/ghzkcywzq.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghgsshibs.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdosjndzd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gumikonli.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/geaodqjir.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjhqkihbo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gnijtsuct.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/ggeczpavs.sHtML


<!-- 参考信息 -->