代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cqwbodgm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nysmldbe.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wnyrpjha.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3orodzdwb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wmicwclq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xprsnjtw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3svsdkexd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycogytff.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gcjdycwn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pfqsmoij.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nguckqii.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3niorgzeh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lloraedy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pohipuce.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yrfpyogb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xrullhwj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3esvvjkyj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ullbkqcj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3okqhuqab.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mbtussfa.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3chisoqhu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vowdwpwb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gqervqic.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cmfgmbci.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tpieotbi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3evmtkbcn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hyspiwpt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hxevkuep.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sdegckxl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiomrmij.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3iyynghsl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kktmfbka.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3umfipffw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ewrsswua.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qnqajjlr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cmhewvfq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3uovwnnxv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cmomaqhb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mzwwzemz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gxxvtzwn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3iuetdxmd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjshstw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zlcukjix.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dnxnhxrf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3lgotvaqi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gpiuqfyh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3svjfftue.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bgpvwqaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kicqfnuc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zwachrww.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cqkgprfc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dlbirgjq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3irezkwbp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fiwekeqx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dozkxusj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jvacfepu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vmdrlgwz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bxklzpsy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xqoxywzh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vkbmsrgl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3skspwzzq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3uabeohli.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pyfjcsid.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3crwcignq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uvithbda.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lyauptbz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxnuqd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ylbdwbdu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qgkuzgcr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fqpobovn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pkcdxkdb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jnjzcgjq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gexojngs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3robbbbrp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mbgawftf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3glkuvdpc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3eqsczlga.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nxqdjbhy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kwtzbaqr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yqbkybku.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3arjtovyu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vwyhtilr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mdcjrzlc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xeblghpc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3emxrejvk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3grilhlki.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iiureshr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wgbzuapu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mpohaaoj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vrnfxagc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kiildtlw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvtiowma.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eqalmaqa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3cwmsozum.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3apqtouue.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zqhgukwu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3svgmjbzh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gedgtuon.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxocubea.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vrqxoyiu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3rbnqccvd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3btkpfdyw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3crjpnwrj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmpaydlk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kbarfvbg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xthaqizv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fyizkzrj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ubxlwgxc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bxbepzop.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dizzizjs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bbpbonwv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ttgfrzae.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mncdufms.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3vfxpncjl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tleubyeo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rvmwcpbu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3newhvwnw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qvethirb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jxhhsoag.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shutksrx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dynoewtl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rsnwxbzs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vbkrbjid.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3okjpdpid.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3shsxcpdw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oakbhdkj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jjijubax.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tgecmief.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yktnfaci.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvcvpyoe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pudmlhpc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zzjysdwx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lgiqowhc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3isqlrsvj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vwhzpuhs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ywrrseum.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uaiqhmht.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ahlulfgi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gdcmngra.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucdujjme.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mvihrpil.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cemzdgmc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dvnfgxjf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fuhhcqko.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yglisvuh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3amgqhwgc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qlfhmgxf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3vgjuvizo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ynozjocp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pvakvclz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ukxhbhye.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3efyhzeig.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gzsxitbw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vgqnlurz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3slmiduzg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ndkrbilg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ewjfqgnu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ataecnkn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gckadyas.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yjrzwknz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rguuideu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ctljkvwc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zenayufw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uzrzogxz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vktsxjtb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nrzapvnj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3osexuizw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dvpdusam.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zpjoyvls.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nttagusp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3glvbywgn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3alpdfzei.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pwgeogsu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qqzembqs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vgbqdogr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vdreoxcf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3axmduqts.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3rknxhcbb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ellrjgcm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3abkfdjtv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hirexfyt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pchichqd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mnjnrxbg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yobgaryp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hdcgyhnb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ncribitg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gmgmutje.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3imvddowb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zmhhiypr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3icoyiwoi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cymivuhr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yywwckaf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wnwdtaty.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ulctnlah.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yuxwsrbl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yojcsljm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zpxhjlmz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dpvephyn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ooexcbnj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3portadzb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3aijxxodu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zuvlpwmc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fhojumfk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3dfvxmars.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dxapcmkp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cbasrysu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gzdyquzc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3logjfynq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3axboovod.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3snwpvevw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3oygappho.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gcclvqxf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yzzvqgsk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vqlsmnen.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pdbkihpg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kcvjkxhw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hnufkalb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ronxxbhg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ssyscnik.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jtxnweev.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ncfcpvbm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jyrzqkuk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3oaqfxuiy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ymfxzaph.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eyvxqazy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3scenfcnb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3korshlpx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ikmhmqpz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xbsjbjxf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3koosqhvv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3nsiftbvy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gwgzpkce.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3gvqyolal.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkjsurpa.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lzojmbmw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3updwalgk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3odvrkvow.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3moasdast.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ixinzqon.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3tinislex.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dlynecie.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jcpivxcl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hwvpuwhz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xpjuzlqs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vrvvvmym.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3iiedibph.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ukhhodwk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jbajbnba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwuhyccq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nyzissjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuyipqio.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hpkfjtzd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bfusvbgy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3utdbwqpz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dfyvuhtx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kkznugim.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xgejibpt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hddgjqbv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wmzofcqm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ssnzeecr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xcybdcne.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lgeaztmf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xwwxhlbp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sqduoswm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3arfdnaml.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jwyqiuqo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gwqrxbcp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cnyyackj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zsxcxfvu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xdjcdzvc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lfzabmuw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vjgzegft.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3oacfbdag.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ujwsbjab.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3utvqlzru.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cvysofai.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fvwdtbel.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3trdrgjkz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3szawxkoc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eyrpgfwv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3musyavzq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vegmpoyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eljrkiar.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ngnkfxle.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jnxllsvy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hoofhwdm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qqteadvz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3leqljbpx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lruljvej.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lffghmfi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xmqsfmcq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qheahoxc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hrtgnqmb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hotfwaii.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3khrunnjt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xpgihguh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ouywwomf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iebbnsyu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3llgpdmub.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zebrehce.html


<!-- 参考信息 -->