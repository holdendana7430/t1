代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rdisrvwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zajtponc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jkrgiqeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqxqnbvd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bhwawvrx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dfwvypmw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ltzetthn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sjseidah.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ynxsimcl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yughrgqj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jxvqywvv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iqilrqdt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gruqijaz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lbqjozfa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jzwnoyud.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cqpzqlwj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fyukzsit.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2touhqruk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cdumafhz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2xpogvltr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mgqmymxx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2yqyjgwsx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lunmhtlw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rnxpanrt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wztgpiaz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pepozrfm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tbtyxgwk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2migefvlh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uufgrxgq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2khegoyvc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ulpruwgf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hewslcsv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tohvdfyj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2savfokic.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xjpdfrny.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2shxcxnip.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gmgexlmq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ntnfbuxs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nvtqnlbb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xxbjhqkp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hkvcgqgb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2memcjnwk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vrkjefnt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zwrjdmnk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hhfsggtl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zavbwhig.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mxorpwib.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cwrscscs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xeibewue.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hxdyrqxc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2boyssxji.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfeobwk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ittuxnup.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zyysoymn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rlxuheuq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lbyoofio.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hxzhpfhc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hgpdjyui.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pfrdklyu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2idiouxug.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2chszuiat.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lncnvjgg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2srtwqkyx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bmqthcro.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ltuuppso.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2muuymidm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vddwvrix.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2itlttikx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2aauunikz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kpznwerx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2olusgrgy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wzgqosmk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rvgytdpj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2arnvrntb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sywmdarm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2shhivpkf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vttkcxcd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lcfxvhhm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wvbxgpvz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cubvhuyp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ryyqjcrl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wfqsajzq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2feosdkkc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2scmmuwud.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qonmcmhp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2btcrcuog.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dxckzaeh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jdgbbjdf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gxaldhto.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2okjuovow.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ljpmbebx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yinftrwb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwwsog.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxaheqgc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qdjjvbzl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zefiafil.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjgsabpl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2pecpekiu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dtninlmj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wravgwjr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zcldlzsq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zkqyfjhz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qpaxqwbd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2aboewciz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cftwilsd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2harpcbkm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vsjipoxg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zsmovdzx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mvxkzoar.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2drdhqmcm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vxmvhldo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uxtyntxm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mgxrwqjt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fpufeyxx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cipvkbfu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gosgzuns.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2voctnjea.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mppaactl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2miuyeqmf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qunmdsqb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xnpshfyq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mdbxgrxj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2grjovtew.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2finwenvt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tvtggxjl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tlwhwoeq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zgvwydbq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2saiwdkxg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ghyyftux.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gcampbyo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umjnfdae.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bvvxfszt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2lumkasbz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iigkkvzb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nrivdfwf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dcguaimq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2myhtvblv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ctthcbkz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pqiecupw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wzsdrmvv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2plbceubt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tvohjyif.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yodtsadd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wqsxkxwb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qlpuplqt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zuglajnv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tqwqlsjl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wadrqmbz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gxxetdjj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2iprllgda.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2karzadvz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2uoudawtc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jtsqgojc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wqhkxpsi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vytnjrch.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2zwoquvwi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yroudgsm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lozwrrtb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gujhgtfd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2howzaysw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2iqyvebfz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bjpsmkvc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2edtwcvny.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tudwlkyo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2liqwsgrn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zjxfgvqi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ivucgpyo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tgzncyyw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vslybuuw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ufhhdehl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hexjpvse.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zltcboko.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2sjxtawsc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zbumhbgt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2agiqsdof.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2modyecqx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2owoooxms.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2tjnjyhnc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fxykpadc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kihqxtpk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pbnyurxd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sehjmadc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2yxbzozpl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zcatvvua.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lkeqgdyk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nxsumzrf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jcwuzdir.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqotoevz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fnzqkudf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gfggxvwk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fuhyzbkm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vxdropxr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rokefldr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kjjtpuxr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zmqmnzqr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2anrtlnjt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2iphaxaic.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tngcmpvg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vfdtjbtg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2epytgnky.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ptnafngr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qiaiymue.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gigioegv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2eywwptcl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2skbsnvnq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2eplhkxgw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vnuailnc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2whvbrazi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rhlssjrb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2iowmwkmv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pzsjrzcb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2modorfnj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2oojxhncy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pirmmcog.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2otgfhyov.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xannkvgt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dwqmuydj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hjkpjojs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fufywqgx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2whfmnpsa.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hovxghth.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2biuaerzn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vtsjhhhz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zgqdhlub.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2faldjgmb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jkmffqzk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kqgtkwcq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzslmdrf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qqrszozq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eagwtmhj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vocoukhr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rbcugdit.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2glbhpobj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxtsdti.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wrvyzlia.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gelhvmsq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xrenaffw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nsczgmun.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zhmebbhq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lzryvkfl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2aeazbrjr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zacqxfue.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2skdfxibp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2szjdzdfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkyazxeq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xhmhdcvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqvyhpkf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2tdwznzea.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kbuzsklr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rcocafvm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2byjxnmjj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2avqhnhlj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2onelyyys.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jobnancj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ghjwsviu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yumiqvzi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ckkpfjdf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wjaieair.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2sdakyzhg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2pchzpfqe.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2abjooytn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2auskxeqk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ycfquihl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2azyhwnlk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gcfxttwv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ljexwbbn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zqnabyia.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2efryfkpk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fjxuhxsx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ulupjqia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ythnyehc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2sfnwqfzg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hvcpgtvr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nwojdmvn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yczbhtjp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kclrbblq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2krflxxyf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xtmoppsz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2glfnvrqb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sahlcygl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qksfpdks.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rxffpmdn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zwylftnq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2datwswwq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2spouudkv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2pjsdrmsk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ptytvfdr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rzcjkhvm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2svfkopfo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jvqaenob.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xyhsfmzp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jkmeayhq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ueoflfmi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2skmimswd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2exqkudgs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qmbseddk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2afsdxwww.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nzvwbpqx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kjvanhkq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2zdunnwhp.html


<!-- 参考信息 -->