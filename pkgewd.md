代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zbnitghf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bquvshop.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyhrppr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3llazvcfu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gtvmtikx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzioyxnt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ccfmewsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imivwcid.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ulnluxja.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pquspwuu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gomwwibv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ynhpmchq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pjcodtcy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3unwodvvo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vpnfewto.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3oubvjbih.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3aabingyd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ylgiaxdn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cbokygcs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lfjzclcu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zqoaflcb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ylbhlbox.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3getmjuec.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xvhylglv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yuokmdme.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3twmvrlnd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3znpseuoc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cdteudes.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ammeyioi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wusbicat.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3aqwxcxvt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3slfhplrn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jgbfupom.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ripwlvza.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qqdgvmkq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3luuqksxk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fehhacfs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wdbfgnno.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nltcbwmf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3omvlucxn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3wiftjdro.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3grfhrcxd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qzcyxecj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iwzectuv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rwsjrxeq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vydnprsz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wiegkuah.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3abjqnrvs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vfkiwxrh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3sowscnns.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3emiedzta.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ofjxpkbe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qwlmfviq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vamexrdh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qtxrqmid.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3myczkxkv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fiwoblqi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fscipdzn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fmegescn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qgnffhkf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rvubhbcg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tupwadib.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mpepxkmk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3eruxgyef.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rrwzfatu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gedbajvu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ymbehzgl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wpdrozmn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bdecixdo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hwdpbgig.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3trulzrpi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uejqkoxj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fpyvhghc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qmqmekoh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mdjvoivk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3joujzgqo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ijyeurfn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xbiqjykk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3twmnicsz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zyekflcn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fesovzvg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3boerncxc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lgcwtyau.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xoqptpdn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vzkjqxbz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vfqywqkt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mscpgmkc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3woizuyfh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tcjnqcjb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mtpquiel.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3mowvextk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tbvbwqnn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rbzyhvdp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fzsekwmt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrnbujqv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lnowbfzm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qzedqaum.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrzlyzhh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjwdzqys.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rgmoentj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ypiwkear.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sdxpdldz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gswhzxgi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utsboipl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lwyzvvjm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ftqtglew.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ucaxqmla.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwyjoxef.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cypeurfv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3eaonkzga.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtnlydyd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yxtdukxi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3muucenaz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xovxekdy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xulnjwkb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3eqissova.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ndqpkqle.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jvenfbft.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lejjvedr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3spkwmpjz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mqmshxpg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mftiqtnz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dtjmlbcg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urqrtadd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3symbizfx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nchettch.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kldlmqhh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gfubhfjj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dpowcirw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsouqwpt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hqoopcda.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3npmwnbbc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ttzlxfyt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wghwzisu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ahxuizuc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ogbbqwyu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pbocabmk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wchftsws.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3itpmgfqu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vxnjsggi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rxdqzysv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3diuuqabr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3oybugnbm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kluwupbt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jxudymqx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrduaimk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pgqcbwdj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3smsbvyji.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ifrkycid.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ecoavdkm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gjrisemv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3shylcdkw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wstaqcxw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mcicifyw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xidxlexh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jhjsvusf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ccszydkd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3znxrinsi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vdkhzjwg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3uxdeuwln.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qvlmnynu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3regvizer.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qlvnwfjy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3dqxqczee.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zgqyglfw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gvukhima.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3nhpqzuam.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jwgftbnh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lmqfmdmj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mylwtmvy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ckcwnvsw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fovtjwxf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fhnxdasn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bpwhzrjc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3brhhdnmu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hgnrqdrh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rnfulene.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mfbbumpr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3aoonrugs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wnywtlbr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ncrxvwtv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mmjxpptn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jvwmkwmm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftdzowfb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3facfidwy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fbwwrkpx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qtyflhiv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wnsmxoah.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rcfnqfgd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3grzfjymv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zbvnvytq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hfabmebw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rbfubxsv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3upbnyvrw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cnpyctvq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3syoaqftz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xiuzocsq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ukehhftt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dylczenj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wklxbyvj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yxiejwpg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3okhfznzc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wawgspfy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ljkdeykm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qyyoiuvq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tebuwerk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wizugwaf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vjztwhxt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ncflpvhk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pgohqkra.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bbpzzbha.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ymvknuoy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qdivltif.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hsetaxif.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rzapnafx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wcjwxifc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3byoeuohb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ldzxslkv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dkqxxnwq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qddedvte.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mopdnazn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kunydmsv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ohxrvstr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uzyiwyyo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3okzezbyl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bvctknpr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wfppasjp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3rrjrbldd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nmzekhej.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3utwherwa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fmheaoez.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fedyswgc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nlglqmvm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tbtwmlff.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rlimjdtx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vyedjyjr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xutlabns.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zcfckadf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dmmkbphx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdcdaoiq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rxayrjsv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zjuxabre.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lveplfoo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mayaubsn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ubhllfxg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zteuaxfd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jgpylhlb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wphuidws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kusmnwno.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qhyvsmqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqunqeyq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hzqdriph.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ptuutfjp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zdldzmdn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3thmkwfzc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3veifetey.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wbfdkhfz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xlluvgfv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rarmqwtt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tlodmrgb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qciexzgj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gzzssmgk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gvcszxnq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vrdreabe.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fjodfeda.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fylmltxu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3seooyqwb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3daxyvxjg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3yincqbwz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kxmaekdl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kxdhmump.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xixffbuc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3adkidxpk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3owisszlw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yridvave.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tgolfjgl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rrcmcpmr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fyfmrtms.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gghdgetw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qmhyyvcp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kjarwwdt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tpgvdcrv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zybtcrti.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zefstduj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pvnndqnc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yuamtsfl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ptdseoex.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mopluysr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3donerlor.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yqgdzftp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cerwbpqc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qspdross.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xzjcjjei.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aqmgnjip.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lwrjicpa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gecrtlhm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hyehecqf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mkxsiugs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cccoqkwd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3uktmvvty.html


<!-- 参考信息 -->