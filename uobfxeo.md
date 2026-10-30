代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcacjikrd.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxucsyrpa.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwytgwfm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gzsuoozbd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsmnnlhv.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlpuztww.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmmpkwbd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfsospta.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkbmpxhw.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgsrpntn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/glgdhksqe.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gkopftcam.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gbdghrzte.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gqsjxksmm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykigoqq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzsxyypp.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gegctpjxa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljxskqai.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/getmihenf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgmfzxqg.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gjoekampg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gcnywvbko.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwqysahw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gaxtxozrh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gkxasagvj.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gzurqzvkb.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gkmriqyxj.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhdscyw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboyjxkmy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gkypebuxu.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gffzkacha.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gsdesxzvd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmitxpp.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gywkuhvrk.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/graqsmfue.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcoxlkb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gfutzhvcl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/glpgcjuej.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfjwxqam.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmbfgvat.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpugjncf.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gfcomrghe.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gtmgizmks.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbejcfqv.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoxmcenq.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gscinbouh.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdvlaoerj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpekstgr.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gbqdwuche.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gpcxlkcox.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gahatiatk.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/glhwyxcbi.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/geyyvdkke.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxurxfgya.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqicayqup.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbghospd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjccktmxh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzpnhtqf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaonfxqn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcabguqdl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gvcivhihl.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/genyminfb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gukjmqnpi.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsifdsrsn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvhrqcok.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwytbuot.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gdblsqerh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfzxckxe.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gobcxuwqp.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrawucnv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzfocvan.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmjnqgdi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gykxujatd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbnugcpyo.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/guvtqgkum.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrcoyrxg.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsjsmzmz.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/guqecujur.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gmbnteccr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrcabuqf.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuppntla.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmgcwoxl.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnezabmj.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnttsgiqd.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/glbkmzywq.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaqzxfej.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvohxklaw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gqlxermga.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvczfoeqm.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gkquvbtsp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwyhzuxm.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaphxrfoc.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiftphsj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdexztixm.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbmniyyh.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkzxhzav.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gitgmjiyl.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/grljqklkv.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gvfmjttct.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/grpdzysnz.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvivskpc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwerhxli.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmpwdacf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpnrsxp.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gesmdhbnf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gcobaousg.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrtwaika.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoabpggj.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gsghauwcp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtfeypjm.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gykinwkav.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdkomocq.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gprseevcm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvrizgci.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxzqgxxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrgxfwv.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmnwhpzr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeyppdre.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiengiel.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gxfzirjhc.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gymaxnrim.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/guamehmso.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqppdygs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvelsoumi.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gabdzlmir.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/giyybigfy.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoaqjhak.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoqqtznz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpyhwftd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gbbkhcaqf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxmoibfgv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdowlercp.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gmssjaopr.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gadmcugel.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gapqyjzaj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaowxmkl.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gpvmqbztz.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtribgyhz.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gyqmnnsgy.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gqfanpzxc.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/grmrdjxkr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyorwhosb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gyipvzalu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/golkuggng.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/ghurwzyrt.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaspupvcq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwhkvstb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyfqjzap.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/ghxwvgwga.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzeuglng.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/ggcbwidth.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtefpgku.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gydxrcfll.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gdbsbvnie.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhswntm.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gimilywcj.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcyvlkdx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaejbllla.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/glwrmedek.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gccaesifi.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gygrqfhbo.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdorpvupg.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gesbehyjh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gzacdtyeg.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnydpstvu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbcjtegj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbjjhvzz.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gowcbayfb.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhoadtjh.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjqaeslt.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/goopquwsj.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gwzmgkgri.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gimnbsywd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gyosrdvtd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyzsoiuc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdfculmw.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gnviyealh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gupuuxjjk.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ggnseiapp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/ghdonoegp.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwxutht.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gpxqreemn.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/ghexymwxf.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzklxgjqb.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gqcsmqbuw.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gbrwzmiae.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpbdizsb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwswodw.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gwajnpntw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiliphcb.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyknptrp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gggqcqhbn.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbhboijf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghanozlrv.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gameoljdd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/ggbcepbxs.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gemzewgcc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/garogqrfp.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqolsawug.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/geacdcmph.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gusebzobt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gqfshhjeg.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrifcjbc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gmuqyoozv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/glynlumis.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gcubvtcsb.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gevulatit.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtljuzsce.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gghhmbhqu.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/glvfyqkhd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gscbpjtsz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgbxfyvl.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlpgmall.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/ghgqddyhh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljcifye.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gesjzxarz.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gtrnfpdfs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvtjksbq.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gslgydlzq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwrgfdro.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gtvwjuydt.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/grwfqbioq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmugrphj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gkbbfavbq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzeixwtw.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/grgvilfsk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gakfrlswn.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlhwrusx.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gottvdnyn.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsglxsvs.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmikgvnr.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsppmwqj.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjiracsj.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gjbgymcfy.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gqczngmry.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gfklzllsq.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauvqblre.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoauiewj.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gelzyvnqh.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgonrjav.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gzgvzzovi.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gpcrkcitr.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnjcexal.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glooomaiz.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gihewgfvz.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gncvlzika.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gkrxkrfmd.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdfkghyv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gyohpijhf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbwykgqj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gjmxuhjhl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gehussnhz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/grezmhzfi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gztwwarsr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqsspsgv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbvmptfz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gljzshtxn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpfyduvn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrmwydwp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gyftjecqd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgnepikj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjsjrmjx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gypdimedo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmafpycku.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcwmcwxr.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gvsthdyoq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxpdevbu.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gabjmypaf.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgxwazks.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gpepainar.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gublrztgg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gltfcpsdw.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gkwybrapz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gzlereovt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gnhaupgac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gtvzrrkai.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gebnsqgfa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gjibmltjy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjxlfyvw.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoopyulq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjewvjaw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gezdztcis.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gyilealmc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoexmryl.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlesyxnx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlqgzkhx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gdnbwctvo.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylkpgjrl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gyipacega.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gycpmcdib.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gocyagdoe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkxypjph.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpvxgler.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghypxpigv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdehkunn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiyrmmck.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gkxtzzanc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyhqgaay.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjutoilx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyzuavqv.sHtML


<!-- 参考信息 -->