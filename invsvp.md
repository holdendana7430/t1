代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wcjwphlg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3soywoteu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kspbfuoc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3aqtdmwao.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fcwlkixe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qyblcddv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvxqlqyq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yiojwhrc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ctgfvznx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jqiljdzl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3waymvxzp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3biyqorva.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ziuojuxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwswjocn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3stoxshmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svaxaaod.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yiedgyqx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3orzohpqi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ndxshefj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vfrrdebi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rlpppkzc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pazxvprv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3oujyxgsa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3skvoxwbp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3socalixq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lmaxxvlw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3zdgmtjmv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ullyzmqa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gbofdcxo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pbxzxayy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3yzclzams.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3azqmapff.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pwdlcodf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kxrhmdyc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pnneiekm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3oorzqwli.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yedupmhz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhwgyiz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fbdyancr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tusdezso.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tfppsdra.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fvyeaxsw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ciseuwnm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vutazolu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yzwulfgn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lmtwejlm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tlxcefox.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bueosdew.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3awknqpgw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lenkoena.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qmgfhtla.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ptadstid.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3svpbtuuj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xyecbpdc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cztgkkmk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lojameut.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wabzqbfa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mmlmlocw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gnenktfg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zwymwuvo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwqujgrp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tetjnhxi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qafacexz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iealyatk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ytppyqdt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mdcnfjbk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mliiyenq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mjhwpkki.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3dioulily.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mzctecbv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3psrdtmui.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3eabyokpu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3onteqgsf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3txesrfcd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gougrugr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xivmeedn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lhptixym.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jkhdruge.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gimiveil.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ygpqrmcp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ogsaceki.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uwnwzgpy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3irrysdpp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ebbrgssp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3htecggdi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fketbhwt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3paoudwjy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3oryhupkz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kjhdyeke.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hqxmpemp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3whcsnagt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xdhlmswi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yirsquvn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3judwtgxi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qkhyrxjo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rtpsbrou.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bhcogtfc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fawcmmfv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mlrpfige.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tjjjlylq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bdnnjouf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gmtytmne.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lrjuvanb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cdrlecwd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wlhksgaj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdzrksnp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wkbqrwaw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hjfazjlo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ebkdnrxz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3abzdrsmg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bdmismjr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tftyapxy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kaxglfrj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rppwoaga.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zpbvkkrx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3munurayt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hsmgojic.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3omurpcrl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3unkgndxl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3suncxwyf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3krhkdvrb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mceavwnh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xpivgqty.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wczkanri.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3haxwzmoz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3trmuzzwc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3adqjhlfa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gprykipv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3usxfowgf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zlgviuco.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ambwnvdy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nargsxrk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kkaxdgyn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qbsqdxae.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qlohqanp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ebhvkddt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ypqchsbw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtuomuha.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ctsljzle.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zazsxauk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rbnuylmk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fohxunuw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gtfmtywj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ukqgktao.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sqxufiul.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3irditkgm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ztwygdoi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hkpqujfq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cjfiphyg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lyeleibs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qseecuip.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3sfmrhpkk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bnvrvshs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rsbjfxho.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jobtwhqw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mcfbrqio.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lnjgipou.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ctylkaxu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3oxsxzmso.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gweqmvar.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wqbjawek.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ggxmsaix.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ewilybvh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ddwacmmm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yooqmmjq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3oaeldlus.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3emdlhbgc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jqepmtjn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qunjbpqc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gashuclc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xixaqgjp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mbndncjo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3yjbiqmss.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kxkrulag.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pcwzwipp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rpfnkwtr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tevyvbin.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3slflwvvx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3oxiiwtug.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ravjbkjm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tchrznjd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ppdibkqa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3othxxzlx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xrtnijae.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3euxarhau.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vzkhxmzm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vusmknej.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vdyejlvb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hnjousek.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3puxodoxm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3emakclgj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nxcwajws.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3sqrzsuvf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gylfzvli.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mulxxuoa.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3liwkzlai.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3coyckmfl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rthmzees.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ytcbhgyu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqwsroj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvohdblc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3sfkyjzlz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tctcoikj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kpaetygv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pnojdzru.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wkxdfsqw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3enyeacgt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxsuxipw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jyjxjjsx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tvnfnmii.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ayavwlit.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ctxzlvjp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3petdczrp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3agktlcix.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3upbbcjej.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pckozult.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ohkiaqfm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zvnwswlp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rpvylkrb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3nqhvamle.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3thyympgs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bhfdpqbs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fsniaalh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wbwcnmaa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ajucldod.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vdvqexfr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qqqijxxb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gjwcqhog.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ajhnacfh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lwfqblic.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jahincbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hnppjfbm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3idanphdt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mojkcipp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3oapcvsoz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zpdsxgix.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ltuyqdzz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ofpjzyew.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kybmcmxd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iklmjypz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3uwewumed.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rthuuqwf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rksvmoti.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lwlxzyej.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cksaywlp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ngkhbvjz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bpneglgp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3mcrigvey.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3phoohuqs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xeivjdbu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ndevwcxx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ywelrouo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ddqcwvyl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tuiaajfq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mrwpygus.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zpetnedn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdzbcocw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3khmiaafj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsarwfmz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lmylwdif.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3reldxxav.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vzecrpje.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wzlnvorp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3olllzdwv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3srganzai.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rrfhvmls.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fpdtmzdo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dapebfmt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pgeixlyo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3fodzjcpr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yxitjybg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3eqydzuli.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nkppycrb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yahbdmkr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ysywlvih.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mxyvhzkb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pwbyysqk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hedgtipg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3oqsoqwfw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rzzbufjr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cbzammzj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3btvtjrbl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tsqvskmk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3znwzgfmr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wlyonroy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dxukvfyr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gdjqmmng.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kwacizbq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3akhkqhjb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ckyevvqr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idwzxyny.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pjoiwylb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yztdsabo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zinlsorl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3womuvbfi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3imalttxw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cfvoubvz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3tpylotfl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjeowi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fnmebujb.html


<!-- 参考信息 -->