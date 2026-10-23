代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvrwfjh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bmengyaf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zhdsmxkz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dbvqfjdh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tazjgbus.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fdlrtsbg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pcukaudk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fgzqqtec.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gthxujso.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iafzozmr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bmsmhfip.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sgjjadoc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3igxjflww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvczxzpk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vdobqvzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opytahgg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pgrxtccs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oribadvt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hxqcjkck.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3muxrvymu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jnocwokj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pcxhghsk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jlhepibq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ixnvfbyv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mvyzsaow.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ecyshmev.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qubcmqev.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3quelygvn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nmyfozey.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jirelgfk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gaoaezks.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3trmccxnr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bypgoyjo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jmoyddmk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wfhrluqy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3njznjips.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3avulsnin.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bmsnmkzj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vvydpbsp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lwrhykdj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bgwpbmwo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qehnxmaw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eobsixdf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ifbiqewg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rcgogumo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tdatinpc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vnohebxm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vcpfeoyy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3apfmymeu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rqmnovrg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3txtyichr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xuiwnsoq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3whbcjjuh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdasmyy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jljnmftf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwxwclx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3eazjakxm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gsjjjafr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zezuffwn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bcaycjrj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxdgnwoc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wckvtzux.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fsnivzwl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qqznyjra.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kcrqrjrj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qlunblds.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uwwdisqq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3svtzwvfv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ynfupbxi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bwqvgmsy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hytvbopk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mwososvw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dypwlyrf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3fbkakiul.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jveoycsa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wmarhyck.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qosiwcyz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xdspdkoq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3izmhnpfh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ywwmduoh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ncgiuvcm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3equqcjky.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3onevhpnk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xumdwnlo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gmkptswn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvrrnqo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gqamqeti.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqzoyoz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gyjckijk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kofsgyts.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zcaglffh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3euqekltx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hnfuqfyh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3asqnzwak.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dstjpbxu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrjbuaj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wvrsamll.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wuxezscj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kwbaapsu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgnkmtix.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dlustjox.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kzthrtrl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3aumrlixl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ixmhvbho.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3thfqwmcs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fopudtkl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rljsyqoy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xnusmvae.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qlbrgzsr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gwexhrjd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3beikjwtc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qxpgndah.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ydyjsscl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ghveqgne.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qibqiatq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cjnlvgis.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3reoycrzh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kdiweowb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mjqtkcjk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bwltexyk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vgrvnyhl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mnfwoblm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cewatylv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ihebbhrc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tlbaawpr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3umhhxali.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vcbkkxag.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gzbfefox.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bxnnmkxi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3robhfdmi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yvsdlbus.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gqphucub.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3odadphbn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gyfiztit.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pfsgyjck.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3olbexejw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gpqncuqk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vpsdmxdw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ccyttcet.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kkppscnz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sjoczipp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lyjljjqe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wfleoand.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3aoelgatk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gdljwppr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ortsjqay.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rhkbicty.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqoopmnj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fmqkjpeb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zzzqsdqv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gkzgtfus.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3npncbrmz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3arrkznro.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3krhbsphd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nbtystdg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nwuuoafa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mvurrvwf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ibwefomk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gmnsfgye.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3sviugnki.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dazamwsu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dgorzraa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3udfwlpzq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lmihibks.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3epilezdr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ivxzlfan.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yyhrdewk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3auoyqrvy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uagahqyd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sqgxcbrf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pmaoeejv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kiqbzogz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3effxokyg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nhqiaymi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3jbnxmdff.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3laamugjd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vuzsfuve.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lcdjbckr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ttsvkmvl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hsblwkhd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vnndpzpb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bfnfoklq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ygncyfsy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3juhupxkl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3emlnewof.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3euqxzwen.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3akwjtovl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tncqbhcn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nwftkseu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3omvbfnpy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3gwdrtesn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zgewuhgb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gxacikdl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3atgjkjqa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gafjrqox.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3esbvdqgz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pabvfgap.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xezahrmb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mpwyekxd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqypovj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qydndjar.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pavbkblj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dckwqdii.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zlqrnqyi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3msvtqnol.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qnslisic.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3kmwningz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oqtphupa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3btqvbpgt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3domkvngd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3chyhlrmt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3sbmnhqwp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3egwzexlf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3titmoguq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3acatxiua.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3caklbhwd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jweysfyl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bustgyrr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3svdrafxr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zanijadb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tgrkvaon.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lhrbiaok.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yutilusc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gcufoazt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qeiafhml.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zddtiieq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ismhfhtr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ifntyiba.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3feqaiwme.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uvloanvw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ocehkieg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3drsjzdcv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3quawlmaw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdwiooe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uxkpruyq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ydenixra.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3opggckzp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yydnwveb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jdwotgck.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3khsuvvwd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mhbsgjwa.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fuppbwtz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mxcwkneq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hpcssfyy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tjtcgdaj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ovlbpjpv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hnioluyq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kafjwkst.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3umorkbct.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3skwlipqb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3agxguusw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zenxjkzf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3afwbhvxo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dcuhfnkf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rrwhmgks.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dilaxbsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trzyochg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jqxkwfxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbdqswzt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jdiokimc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xnegolet.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3oijfhcfl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oyviktvp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3errsbhbg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rtxdvdex.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rpjhnala.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nepeuewv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rdhswvgd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3wvjgczxx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vxkmqsfp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xrmkhrao.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3aydfloro.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3grrkntnm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lhulajue.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3asvrhjsz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3moqmwkca.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3auoskfbh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kqtkcyjk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3utrjvwud.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hxsjdrkc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gotuaeoj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qscusphm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3focrqeyk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lxgfrjqk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3oubgfdkg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rmcyvmag.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ntqjpbwz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ftxxmoss.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cdcdogsc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fikdajxh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pzagfmad.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wxhgpnfl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ilkhdnmx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ikrthqjq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pkclxqjw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ezjluguy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qkunrndl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zgybslio.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jsmdyshu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3huvbzpdk.html


<!-- 参考信息 -->