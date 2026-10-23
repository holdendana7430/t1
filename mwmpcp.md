代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qllyebtl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rvurplig.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ypebivcp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hsuvgmob.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qkebhpzu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mgucjcxb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fngxtqat.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tlyksopr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3atxspggq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwlkzoba.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xrjcyxhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifkjxeiz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ruavdbsq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gqaedqoc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kqnmigrh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dzkkjrcf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3itmgfwgv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kdigsfyc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yxvhtxuk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cmmppsqg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cyhohxje.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mbkufxvw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wmazduzb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tislbsib.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xvemognb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tmujukng.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3eifgfdcl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3unnprutl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mdosssnz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3seehmdzs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3crzwukmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vrrkxdhg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fsdqneqy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nqgrieew.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3niczkbbt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3olxtmmlf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3itxvueew.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pfkupbsa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gvmfyomy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jkqhvyiz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mnwynmoq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mqtagear.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tvdiuwer.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vfnexzcm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nwsyecnq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bnzjvkuo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mofmvoxa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3naklukvc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3aiktkdum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3nvaivbtm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gctlcjap.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wyqvlnbb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3djiiumms.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lpdjqeyc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3labxihnw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xlycglbb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ppfcesrr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ronxapcu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3euyfflhd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wmrdikhr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3usbxromq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vdqjgvqi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gzpafwbr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aebykyrx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kjupipnl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lgpmzkny.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kckcaoas.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ndpyoakl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xmuafpxq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3akczepmc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3abzknozc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3veawchsm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3slbivlqj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3regjgemc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ckwkdboa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3poplyogr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3thecscog.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iizshpor.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pnztvdav.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xyahyjlf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3prihighr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zkszauze.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3luibhhni.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xjjhmvxv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pwzfzkuv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sseptwyh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ikhdzbhe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yadtxqxk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3blwvxozq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3eujalglk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cdgyvnfu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sikpicnc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3aegafpge.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3septbkmn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3srkqmtac.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vfqyrkhp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rngymeqo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3oaplkzza.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3usfdtdvv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3aylrekhm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwarxrfc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sslcwpkt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqubokdz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mbncfbxz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fjzjwixh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3titpdltj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3suthugst.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhprrya.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3okkepjyi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nhqhyjff.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zzvkssib.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lapjkdiy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3txqmrbtj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3irdzyfps.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qhteuvaj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eluvbmwo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hbuirwna.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ikzsrqbx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bunldmhf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3svzljupu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yjmijsvn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pyssmbvc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3amennzir.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmsrhbg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yvmbpdjw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pbtutsvd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3zujqfbna.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rilbkbhj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rfmxosdv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nepmtmhu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qdcygbej.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fevyuovd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3buthhkfc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3znehjnba.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hvxrpszn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tqcozhsb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3caljapxd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3cgxaiqbu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lrpnapij.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3enzxkvuj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3otrctulc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3keleoprq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ubwcwrsz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hynkdhkv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3nldigwew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kdcvveyx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cxufszrd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jtlwhgjj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ndxxclic.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybgosdnm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uftotqep.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cjjzvrgb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zyuxytgz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xqrlmttv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3auscrliq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rkjtfmyw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wgqrwrbt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mnvedumd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nxmoyxww.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bniewwhs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3nhkbzhio.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cgsithsz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ivgtqduh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mcjgyeei.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3cfdjdwpo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ndhgclrj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xoaruxoc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ytxjmsiy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3esywfzpt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xugoohec.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3loxniyit.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3npolzxtx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dpucbhvx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3robaplsf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3frnkbcen.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3knvgzjbw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ioewgfqy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3brhsxkjt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3habtsovx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uanvygzb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sacsybul.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pxrzrevn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3aorbfpkr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3elvhocok.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3fkrpoygt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3oezexdja.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3oahgjoqi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3sbttsisf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ncusiqpe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bovpmwoy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bxvwhznh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xnsxvxze.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zfckshyl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vtvriyes.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fbsolkzd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uctefulo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3yqcwpodq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cbegzejl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubdsrhlx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mnofrajc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3trajsfqu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cggttcmn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rleqhigw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfyuvwor.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xavwgzcl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fbvounrc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xonmfrkp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wckfxkyg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pamrbymm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yivalahv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pysxbtpr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uanrqtxm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnbyvvbt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hikrljlk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dvjrudhv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gdqlvggc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vosxzhdj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yduqtppy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3raymuiyc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ollllbgy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qmsjkcbx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ncgoxfls.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jbyakcxj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3larhfzea.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mkgsdpao.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3oclfecpz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3utnjyxos.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ozjvhabl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3muupudek.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfawqgg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3pglicowf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rerolbsj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3naawlgzh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gqzhkzcb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ddjylesz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ccwuwose.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3umyydumc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kohbcvrw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gpskmhii.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ueecowaf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mnndnday.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yxxjqiav.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xrnjfbbv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhtltuqc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3twnpscyl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3euzsinwi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ljhnshtp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vttdxnxq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3drxhlhzh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3cuqzjkfe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3waomaqku.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qzetbhlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdvapoae.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qerzsvvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jawashwz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ndyokifl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mhcvjjbl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3znkokrpx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dxomflbk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ymwvziul.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dydvpdlz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3stbrcfgl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wtmenims.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3totttxbd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3oeoccexa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wsdwfuxz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cdwnauzn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gqcmfirz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3veniwhxx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mpmfcthg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3aqbkemmj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ygazkfoq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3agadzlam.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3geyhlaon.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nvthovzi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3irdyqmfz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yeakxwgb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vozeekhd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jagnydby.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3sajatrrw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nvwzsovl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fkbeseqh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rwyklkoy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3thipvymu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uwgsjpoe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hfpqsscz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wpmlupju.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uouwpuxb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vbrbnxef.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dgunssji.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ordrdmsl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ialjupdn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xsiqannz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ahmlbmol.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3pqpbchei.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pbhrbkrp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fonzvesa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3noydmqvs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zvrvhxmo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kvzsidty.html


<!-- 参考信息 -->