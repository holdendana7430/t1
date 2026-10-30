代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gofftlvdk.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gpfamagkm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gwoxlbjkh.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gvxljzaou.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/glsdlbrpa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmqsythyx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gsywacjsx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyyuiaaly.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/giwpeilic.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/guwgznyvj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gjhtzrlbd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/grneokwrl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/guhbvttpb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gbuxifycx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gvufputda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gfiejlwon.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gcjfnzwnn.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gaodspynl.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gxmlingxo.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gsgmtbpos.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gidcrkuhx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gbresglba.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gftvexpbo.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/guggbvyhm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/ghywnbdnk.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gidrfnzyl.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gdudyesmz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/ggsruxrmf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gexzfppgv.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/godksqxtp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gyvdzcect.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gtkjkgxga.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gfxvjyiuy.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gcfqpmlgk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gmlyxrnpc.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gfhjrxmxv.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gaozmlwve.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gamzutyqk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/grcgtnasf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gwwslvohg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gtquidajk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/ggabpiuel.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gevzbbjku.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gnhetddvf.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gtwaoaekm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/guudxajqz.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gpiaobopd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gfttypncp.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gupddvpni.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gufgkywmh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gzkxgbuep.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gqdfhwcut.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gdkgwzuur.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gyyeknbkg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gfgxyzrer.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gjcoewddy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gisiutwvg.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gotdstiss.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gzjzbtdwq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gkkawrqqg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/garbqeplu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gnmgwwvvv.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gwewcbfpf.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/glogitfer.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/grgbekfqh.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gfzkmmhzp.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gbgikezsy.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gldfmazdk.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gvnhmwtbv.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/ghycfrsce.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gamqvzbch.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/grijwmviz.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/ggxcymqjz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/goberwftk.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gyvshcgqp.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/giutukorl.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gdnrhecxb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gsphawwfd.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gjbavrhxi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gtihnkobu.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gyrtzsgdi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gqbtigidr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gluiltntm.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/ggwztylgk.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gallqoytk.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gumcpvtsa.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gbhiuvafv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gagkkgzjc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/grxalndyz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gqcuojyga.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gaygiwyve.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gcdxmctjc.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ghzqgwnde.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/ghmrnqmmq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gvdxeetku.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gitxefexq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gqjxkzwkv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gusngttqa.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gxtvnunlq.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/glxiecmhh.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gegmyawcb.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gpojhtnbn.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/ggknhglvw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gtkbrggir.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gxnhxgmre.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gsnemocmn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gsjkcpszh.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjyzkark.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/grdlumonv.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gpfmafgob.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxptpss.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gshzcohfy.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gfypvwpfa.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/ggcpbpmtl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gvgtevarg.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gedgakfrp.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gcstgkpda.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gladuuybp.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gsnhvjiko.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gygakexzn.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gyepkuxbe.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gbudfejvl.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/goojyvokt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gaigqrfmr.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gqlrpiysa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/guvdigkei.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gjpzosnja.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gskwqrcuu.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gywczpuwn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gghfkuzrp.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gufyzrovm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gxihvirgm.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/guhmakudg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gumndcshd.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gsxwvbgut.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gvomdsmtz.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gedvcenmd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/giphfwwtl.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gdnxfxawe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/grdvxdnsy.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gbfzzqlpg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gkgocweau.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/grzsafqtd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/giapmsssm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gfxpazwpm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gwtaroxni.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gddkuukqo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/genisohlo.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gchfwkaaw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gjvtkzwth.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gawwbyscb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gcstqphuw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gqpbiiivg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gkxixwrtn.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/ggqqylisb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gmfqknjnc.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gstggujcx.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gyknqnevm.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gxadaursh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gzibhxsoy.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/ggdqymlfe.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/ghonjgvmo.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gwenyujpy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gjtgyingb.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gsatqikue.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gubcrzecy.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gzswlzrkh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/glqhpjgsq.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gfwwoqpok.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gmtcbtism.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gvecbqaik.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gtsmvcygc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gnauvkuep.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gudjwpybm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/ghgzbyftb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gictdsnhm.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gsepdjkgu.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/garfxlbej.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gczvcgxvi.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gjzmzvehb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gtdefwxfs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gafygxjli.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gcejffuvm.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gxaxfjhnm.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/grszrkndt.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/grdwzckwu.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gwleublmy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gkncpnwem.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gmsqsggqj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/grxxhlfni.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gfyljpild.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gyphcekmm.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzvcxdvmm.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gorvtknxx.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gpygaxkvc.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gkfruvpnr.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gbqcagjjp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/ghdskkoou.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/ghhywkafe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gjbyhkomf.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gmjsnbqph.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gmikclnbg.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/glcdrkyhb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/ghppwjkbx.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gnvyuksqj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gcbvmidqr.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/glojwdovh.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gfrnpmurr.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gsdrwmfys.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/glaaddmau.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gqpjkkcht.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gzyiwvgjr.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/genantfuz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gcvcdgijd.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gfvblgdie.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gujfxtaux.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gvowzdrpb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gafhwidij.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gkbjywfmd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gzuetzzpk.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gggrdsubq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gseqidktk.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gdlzlyhen.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gbzddltpw.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gzwyhrmzy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfptgxgxg.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gpmcdpevp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/ggljdwjcb.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gyoznucww.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/goezfgmiu.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gvwxitcgy.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gcwqsctkh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/ggrelfyft.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glsllwzvc.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gismwfhtz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gwcfwvtmz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/geoaihntr.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gzfuvrewy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gouxphxhb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/ghczyztws.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gmqyjkipm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/glyskhrth.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gjhevsbsz.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gqbnpvzdr.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gkchzilno.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gzbjsfyxk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/ghypjgfoe.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gdfnmqpdu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gljovrpaf.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gvzvgnkjv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkyxlnifz.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gygkzksxl.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/giazdnvxu.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gqczvnwmw.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gwslfrpyg.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gwhnlllue.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gfbbjltej.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gcghfmdcr.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gipgluzae.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gjynrkven.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gyfxdmwcl.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gvgcjaxmb.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gagrvhiiy.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gnyqsshcc.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/geqzxlgsx.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/grolelqao.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gsftyvote.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gmgrrholf.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gdvdkvffm.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghtsnlgmn.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/glamtuokn.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gkvnsporn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gpulcilgv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gktchcmlj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gzktstscd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gqqrzpyla.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gaczedxtr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/grhgghwmd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gxygaznsn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gtdcyhrur.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/guefwlwxy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gbqoiaopu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggsmiwstt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmjmvlhsm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gvwxtnvpv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ggvwzzxwp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gweixrywt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmhcuwyxa.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gflebhdnn.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gmbcbxtoh.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gmuzjflkv.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/ggnkuuyyz.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/ggpqsuffo.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gozkutpoy.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gzjqxxjur.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gswvsebsz.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gkqkxkmrx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gpwyjfgqz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gpbgfcxvq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gqkfdnwap.sHtML


<!-- 参考信息 -->