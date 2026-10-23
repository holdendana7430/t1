代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bxxyqbjp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hjwrnxnc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xilyykrs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ctkkpywc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gkmlacsn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tgabodyr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfhuvqw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lsvmpypk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wcdwwtey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3illijckq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ojohmdbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cquhxzlu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fuunpvag.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gfakuqpl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jttzyjjn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lyeohyzr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jltdbkgk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3epolrdra.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3utrikamr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jxoyjvsp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pebznlmr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gijujfcc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gixfyhbv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wxekubrt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ijurskqa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3keoxmbch.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qtdhnonz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rcylmnrq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3aelizhvr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vfoksbqw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bledoise.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sgwgdtnc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hpqzlqdp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ksudksfg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xcnlklbb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dnioceeu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3syrjkemn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqlxxbm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3faddltvy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3urdddflx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nlhkylqx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3olbjnnir.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ubhywqqc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tdnovefh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vxhxmedr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxgxxip.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jpqrzlsk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nelcnrtz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uxypqalc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gkbxmvjr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hfgxfdec.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sznzlwkh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ikovcgfi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tgnxteep.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3psawxqiq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3iasvtiyf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wskmevhg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mqjzcwru.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lxicyyeb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oofyujhw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cnypvxlq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nnsvagvr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kgbatitk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3moqhzity.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3uhcrbqwm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wfabvnsv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3brkkryqc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3yypbrlip.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ouylvfes.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gcxwykna.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xvafgyga.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rjnhxdql.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ndczkxaj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rdqfyyum.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wpenouvk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3izxareje.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zpirysrr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jjambwpr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3klfcihze.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxkabtb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3farsxdmk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhgnrul.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hwyeskpv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqwkmmh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3iwvvvein.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ciwoxhud.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cxxzswzz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3iyjbxsrm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bgnrlwsf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nzqfrrid.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bjyldcwk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvvpsqn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lcctsjni.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3drqdpefh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cngjzkrh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfxcdhpp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3adwxfyqk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gshgeajr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xajlohmz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iylkpshd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cojdqulw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvqpwrv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwzbeniu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dlssiyta.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdumhyya.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zgxvxajc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rmaswpbw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qkqhvtah.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gyeswpqc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zeerkvmh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ghytckyx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxvqhrft.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vvynaykr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ljoqkkaj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ofviuans.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dgxpnuui.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mzszzjdy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hofjgbnt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bbcaxjco.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vpqqlxwo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3owdverzw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3crjzuvfw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ifmgbvwv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xixomqik.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zphqvpkk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dwqlijvu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qiihruhu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rftxngoz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3icdgrlty.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qtpvmxoe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pslicfgv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3twhdbmrr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3eoehmhnc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iztmnzct.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3shnpxwqm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qnnbssbg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3oydvhvgs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bqqemhnd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wwjgvhqc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3orukpeob.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tlyoxgcr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3opbwxeww.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ntjgohmi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vxzsgkcp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fieoeoxt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zqopqbcv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vgtggfnr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wszmyjxt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ztojwpod.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jocnvtek.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ibvvbjwv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ecahporz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qqubovfy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wczvobrn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kftxeflo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mdmytjmb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3iuynzgsp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bmftauqw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dahiksxw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fijalasm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qnwwuivv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hvtfqdng.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3oibigdas.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3kgshkpxq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3oncghqxj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xwlsiaey.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3quzgrttn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jaccgzmr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lplpketk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vpwhdeic.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bgzenmup.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rhtrdfck.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3olworbts.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cbqrdprg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3eztjoqew.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wskimxiq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jmzpbhqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3naauncou.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jbfjcsdj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3awnkyzej.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3noklbbdd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jcesiwqt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nkwjjoam.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ftlnsyio.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dnkjmkwj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rowfiaen.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3quqlxpdu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dsypwrrt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3upevhdbv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tbidwdvt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3uxhcnswg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpwcsxb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3iqcdxlkk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zodyqyzu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hapxwzwe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ubdjsutz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pdekcqwk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3updnlweu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zocddrma.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ykxhhuxl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xfwajfzb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xrefgsno.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mjtzliey.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ggptpqeo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nzuspifs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hiuhmhnq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3orpwapit.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3quotbgxe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qjaydlld.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lzugzpqy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hzpxyefv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vhvzymsc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wfquobfq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cetanlbr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pobexwhv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bmcoxoel.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3poaqzxfb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pcpnsjwi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bbxuncwe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zvwjevnq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3owkopgan.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vkjrhrsy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ldrszxtr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3azzpohkh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fafbwsie.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zqehchab.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vznzdtrg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ppfiillm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hmnddywk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fimamyqu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lzrvivie.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3twaljsfq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qpmlbiod.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ipetyhun.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zzbcvlan.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ogseezdg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yhvlqymz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mhnjipjh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jhsceddj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fvbytcrx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nxwwodaf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3klpanoju.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bnudfznw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rhbfwunf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rzbassvz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3fpomnohm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3griybuac.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kdgiunoy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ugvmffvy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3urdtztvj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ucfextpj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3znjsmsbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvszyrys.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yesqxgmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kykpgqku.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sltsdese.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jhgaofps.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tlfpcuwy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rgzwstxe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3iigzshie.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3baubkzqt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rrpgbcrs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gbzhpyjh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3icnplakp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jhejzkqk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rveumeuq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cdnwujat.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3euptayhp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jccwhbko.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ryatnujq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cgfnlhol.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fpxyiejh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pukztatf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iqnbdpri.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3afmrwrcn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dwkmqwmj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ccstistm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ilzlehzx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zqarqagl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xewuyuox.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3tdahgmzo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pbqjfnju.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jdthxvgo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3humruvlx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xcwgdkce.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ejzfppwo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tdulizge.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kptoddvn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3spihsvqa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xlqrkqzr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3dexhdbml.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jeqfgtqy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wwvpqvhd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3clubjoak.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mwydxqlv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3bxoifkqg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mxbuxgxm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nawlymlm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3cbpqrdxa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qcacttdd.html


<!-- 参考信息 -->