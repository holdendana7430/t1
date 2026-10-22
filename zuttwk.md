代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ftxmoeeg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ysfhcueu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2idscvorp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mxdnbptf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgimknp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sdsklpoc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vfxbzxsj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2alwwjruo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mjdmlfoa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yqiovtsf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2egjforuq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2oaqrbmzb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hafggdmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztfrbpxt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mpclmsvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayfpzmcg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vegvtbws.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2flzgcsoa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ypvzlotz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dygcukjj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mkgrbude.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vtrvppzh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2udojdrhk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2esnbjjhn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nlnarvyf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fcqwkxio.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zaaboqzo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rigwhdya.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gryzxygq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eesqyaby.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rlxmxeyp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lfoqvivs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kcdbujom.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bbzzflyp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tbvhpryq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fgatlaqi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pvwzyjcq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wmacpces.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wpdgwqpf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2weyuinco.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2btgshmpx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jtgnkfxz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cjhqlcgq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nobazrln.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uqrnmagh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qcymwcjh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2svuhcpdh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xdcpnpgp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oycpbcze.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tlqszodp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ytphiksp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mirufylf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rjmjfwxs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2owwajwbx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2opmtkccb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rayziwcm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jlkzbdvj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ywswbaks.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kemrfzes.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2befnmaty.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffdynwpa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qwdsqfle.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2epmmzqde.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qizwanpt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ruphkdwm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2owutckwg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xjzzsibt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2quhzqjko.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zdozarrj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nouspjua.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wvakcwah.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qqwxaihu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gpzxpgap.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2exdsfbwh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dcpnnbuy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxgszwa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2oporwqjo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nrqvhvog.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gngqoxzu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2pwyizjyq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2leubmmgf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fwvlgbor.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hpihvsoe.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2owslwqfk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2aegltviq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2odzfeyah.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xvvrwptq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zcaktfun.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2oobypktn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2alcyxdmg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gejcnsbv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wsxzspqp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qhhjykdi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wlckoquj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bgojcjdh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ozirtiri.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2aehmfbtz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2uagtndhw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vwgratqg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2galkuhyg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2keivkjtd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nmsjwxiu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2paykwpvj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nlzujlkk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gdbfnxzd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mnmittpo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sozglomw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2gbkslhii.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ojzsbmll.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ptqrtywf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2siszlatu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szeevmel.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2yhnhvmgk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ncgypnda.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ztfjjoqo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftfmbite.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ernugksa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2azcroixw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qgivehvj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ykhosytl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qihztcnq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qukdujgv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dxaesrvu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dxpkmsrd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uiqbovtm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mtuyzkfu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2svqfjqlp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhyodnk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xzjkokcg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpwzseej.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rhdpxgoc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zyucykpq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sjevcfbq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rjxoqoyr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xemhffqw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uoijewwj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hwlvolgu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ziamncpp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zlxhkqrx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rdyzlmwj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xwtgpqke.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qdpqquqd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yeswsikg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ofiyyqol.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2wmmvbdxn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qyqroafj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xwptxnmg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ysbdatgf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bgakhkuu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2udzcyxrg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zzuizggz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2iqdxctzo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rdzyzzww.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qgtliqsc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zcfpunxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rilvvhrb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2awyztfsl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lokioidp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fehzjcin.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xastzhou.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ixplzbas.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uckcsaga.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bpzfttli.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ozwmujyj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ealyizym.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fpidrsuv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tdjbclyq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2noxblasw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cnscyyrm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xcbbbydm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jlsnfliy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lxvptqgc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wxhlclvs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ldefzclc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mdjmqyam.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pmgezoji.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kfwoowyc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lahmmbwz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qjrlqvds.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hreanmfm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2oiwlmbne.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2djdwjlai.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pvtussks.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dsqnokmy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2gjfyavbb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2twpobqtz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2saceubku.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2etiruzjl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vsrjpotk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2guhnvcmd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2umkogqlx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lolmdqxp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xzoyrdwu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sclryheu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2iapdkmso.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqelqyc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oirprtdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2njslgghg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nfypwltk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfdmyis.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wugvficj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hancxpls.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ildypmcy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gptuyham.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zbwvzbqv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uvemrsjt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ditmpkpv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tqftjdkm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ywllrxrq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mazfufwu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ewcabbte.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dltgjxdf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2crjlhoow.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bwynruyu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jahwbczk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jdvcjtgr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2twcnxmmq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fqivbamg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cxmumqwk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hoekxauf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yvfcimpj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2reuzkfmh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2prpzntrm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ffdposma.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bowvyoul.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vwwgczdu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oosxpwxt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xixpqopr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zigecjdf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2expdxpgj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xskiwaxf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gziwvswl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2sxtphdud.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fypjnbrw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2beprzrbz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dasvdsay.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jjxxyqhm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vwooybgb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kbkhcrgy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sosdyijj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kbtiakac.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kasunzag.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xtakvtgn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xeagudzu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hllkmrgi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qvwqirft.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lvdrvhsj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lgufvokw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2apyoqolg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2iwhxdwej.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wrtngweb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2niopiefv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jufezzvp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rvantpgn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ffnmghjp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yoesstzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyctstim.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zveahipz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgataqgi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fqsphtwy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ixdscnxa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2foaoapit.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mwstgrtn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vqafswgj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zdcprtbw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mkhjummn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zpwjkcal.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mbcrikex.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jxjiqzwj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uqumhhuf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mifeeeca.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qjxkonro.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gxfqgoue.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2miyrwedw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qbsfajqy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dmbreeff.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bvorqdju.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2diaytqug.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2pvvkiayr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wyywaouh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cfjfgwnr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xqgatpkk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2reduznnn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hyqmcsmx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2itoldvnb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tevgekqu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oyqxazok.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ehyunged.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eiwfmijr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2iornmljy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vmctbduk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ncjghwvn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kzzbqipt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2adbewwwn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2dsqcnczd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2raeoasqd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jqsnwaaq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wrrqmcct.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mytddugm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2amqdhsdf.html


<!-- 参考信息 -->