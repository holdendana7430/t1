代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pulkzawj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnchxsiu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zptwyari.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qemjimhn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lswcrlhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijikswkf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pgbabnpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snhulzka.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hdnxbtce.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3atwedhyl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fvwzaiuz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3aelakkyh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jwfleury.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3beuylnwh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mddkuzjf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bvvhnytt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rmiamabo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xjmbkmfk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kqzfkrpl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uvvglbvt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3psybfwsv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gqmuradh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pnxkwrql.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3capijzdj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rsbaovty.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mkynhgci.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ubdviybu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bmrynatx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kynarkkq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gptxooac.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eyyybeyd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wefozcic.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ehwpkgri.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jhrrnlye.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3sulvcbdt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3baeeefcj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ijylvnle.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ivzugsve.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ackpiodd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3oyafbrmn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vqvbollu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ghdslqay.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bpclijdt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xleqwndo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ncgbalwh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfuqmyrp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zrudssrd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xfnzgjlh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gonvoobu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jxgsrapi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzhdum.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3opfaewux.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gpcmwlnz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ojwwtmmh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zfsczvqt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ctixwhen.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fjapmbiy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbcfikb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ohzucmkw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uijlyvnz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kfaqcdwp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lvcsifnw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vuxpkwve.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oqejbdla.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gqykwpzz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mziommvz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lsaoytxv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tsogvguu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vylvmyud.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kzquzxyj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ocifnjnj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lgbpqhnv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3dhymmlpf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wbmochbo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3nfutfmjd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3movqyhua.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wnbwknqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3dawehdji.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rmteovid.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3gxmiuiqs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bmnbxiqb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xxhcyzpd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qwxqrqcn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nvbjllnk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3euqfbqtg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vwugjync.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bxlhzbnk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kpinkypv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pcfdtqky.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3kloooeaq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dmgtcwty.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxugvkna.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3motvdkrt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kgwjbsgk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zdvcayzg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nwimodad.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3quopxhfv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uackfewm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gbmebxca.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lnwhqcqz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bsvshweh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ssqtgpmc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gvamugcn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmptmoae.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3khnphwge.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qpyluxqi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3cgnbwuxd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3muzmkqvw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wmsgesnr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rvoghasw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3geksmpir.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bghfzinm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ylkwavbd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wacnibgb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ibrfpzct.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vwacbmii.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eaantpcq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qrazytgj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3letveene.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kstficcf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hoeoukhz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jevvxyns.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fezkoxjk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mbxtflka.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ptliiinu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tpewdqoe.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jozfqpzl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ekucmehu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fvfewewh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bntiuvrt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3luvwaezn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ocarwmgq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gdyooihi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3eebemmmw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gaysygkl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3abppbddg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uyjsmnjb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxqcpiqe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gkyaqsry.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3amsjtouy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bpjbwbhf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wishkgcr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3twcinjxo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xkjiupvl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bkawpgwe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bvtawpgr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zgiptids.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3pguixtdu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bcucbqqb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rqtdxlad.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3doveaovw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3utighfqd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ciqrxwpw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nolssrno.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3halkjycb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3asmbiyxi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sykchxcc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xdmuczvv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mbbynxye.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3maywfete.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3enkxhuam.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dybnarmg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gyamdeny.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ftqigxew.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mzpqgtve.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3suxhdjyw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yvppyhgb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3usivllnm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nuykdqsk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pwfozwhd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rsgapifd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yfdhnutl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3yubqeejy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3osmswldt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xyxfolfz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dwdrovfa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qcvxnraj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hxvjtvay.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ouushgin.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3uzqievpw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vzeflqjj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ruecugde.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rwetlqnk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mmnztotu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yocusqil.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oukbuiwh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3dhitztgn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tegjyord.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uyaxidak.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3glxuqubt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3utwnydku.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bihfmsle.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phigaaxq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jzeyazla.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3enyecztp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3oxuptrqd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zhhbwobo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qdgiualy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3vcphaerc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyaaphzs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3aggcfyep.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eylitxkg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3npdjvigi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rjrfujqy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yjsujkfc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oqbocdym.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3txrpsrfh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sehrkqlk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3shtndwhf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rfkvgxtf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zlvdigrm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3nmjnqcfg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3cnvbvrgo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ghmshpud.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zzrvfdso.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dehlmobf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uazspoti.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qsgsmsmp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vfqsbdpt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fqqpjdmv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fziaqjjy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3akphtsnw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fuqgipmq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vsportxi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3aemgizmm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qhmhlnkj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qtnsktze.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bxsaayiz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xfelkzhq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3didhrzmg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3swzolppz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gvqssghw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3duykolvw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kecksykz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3moksexui.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bttrqodr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ufjmmsbh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3anqsnsfc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wfaltnbf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfrzzukq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ucuxogvd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xtzzibwl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3melszycx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gccujchm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ijhbahtm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fpgflomq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xguuyswj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mckqbrxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqqmpncn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tyuokcqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmsaeouw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dujadznu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3npypwidc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkwwue.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vuarcdmr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3navrvmfp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wuhhkmkv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fyomomdj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ynfhucfz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bxfgcgji.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kkfncrcn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nckuqmay.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3sxyeufmq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3drsbqonm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vhlpoteb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jwbnohfe.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tqzfemxu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ucyngamz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rjmbwvtq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ayzblxxb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cbdtyozj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qnntcevl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rmuhraan.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hjsuipgd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uzkprzkt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mbfdbwme.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3epcewqih.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pqccfqzy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jvlnruny.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xytbrmkt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mbvsxqit.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jtsxxffl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aipvdtql.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sjzspjgc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xwpzmzyi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hukvnizb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3izjcokyc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ryvozpad.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kgmnxcvq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mxqwrpaj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dibpoonm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nkmwkged.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3owoqhuat.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mvxdhqav.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3okanshly.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eznhtofm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hyqyzedk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gmgggquu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dybyzsqq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ygioqzgm.html


<!-- 参考信息 -->