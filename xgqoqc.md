代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgvouey.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qpbmyapm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yepivlxy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mdmwbhth.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yfyxhodt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ownppyaa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zucxzksw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zezlrfnj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcubdcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nngveovw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rsndvstg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqqdpjxz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vexosges.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2spfaqvhl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cdggwoox.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uxclavpp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jxgrpzuz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dtpnzwyi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wspvbibb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ejzorwhm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2beexyzhy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mkvwflgp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gruofxkp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2famlytjh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2aavhladg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mylnhivp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jertlcxp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lqmmabkv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vbdwfliu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bzvvfrkq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kkrihsqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2uymxqkvo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hfqcnftr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2utuczvuz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2phhovtgf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dxibyfar.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qrxkugck.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2nkmncmfz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mjxfctkp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2axoxuxkw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pcykpkjy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2whlkxdax.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xzgkgysy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tyaovrxa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wqnjqgie.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zsvmnlbs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2slucebau.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kcchidvf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2elrberqx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2twqgpdqo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rsqddimc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2syasahbn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2odhzyqrs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2izlyabkx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zotvpuyq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jtegbuam.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vpyduive.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2csepbmtg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fruwampi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjtccmz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wypenjbi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xvlvgobr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rfxufgjg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tewblpqg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ztymbrfk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ynecdudm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2honhbcdm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2cifnoart.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mbkocfbs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mkctigfw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2abztmgjm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2knagnber.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2udhamjwl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bowrbhyx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vwhnjxhn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hjahmpzf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ictqkkhb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jmlsqeyg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iupzqlrv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhythtm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nwbfjrqs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ngeqtrdc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lvxnoucf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yowjgsfc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2haxghbmw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jsaavuic.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2domijvdu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zrvyqafg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ckqikvzk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hbkehzhc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vsfwfths.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qfidwxao.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2twzlhuxb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ngrukjyn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lracopbc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bsctkzuz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2duusbyje.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vbjbmkvv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkneypds.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jsjzcmtk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2laubpshs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxaycwbr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xtyapwcp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qsjqsuwy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ofowbtfk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yhjxofco.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vkasdqua.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gjovdtlw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vpfzcyem.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xhjojpiu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tniwwfum.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gfbuwmdk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qadfwppb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2dshhimpe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbvlqeuw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ajajgvui.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ulqxxyuf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nvtsgcrs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dmyqwdpz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dgceqbpu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lpfyzxoa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mwgjlfew.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sustugmz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuziiklb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2usodgcpd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ghbckqzx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2geqgszpt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2acsyaxyj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bscmsdzo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kpgukmzn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qxigfsyy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zklqakfk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jiwxzpci.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bwckigtv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sqswdiyi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hkkbxvul.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cduagdpz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ifyiukow.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2uztozpiz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mopnwego.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uxfkgunx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2svdpbsyp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hwwrvrjb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zufjlzcp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2avuckjio.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ejltgwxc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ktjfsdch.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kbbbztro.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vyjvewan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vyhdnqfn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uxbgzvqn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2drxpaxye.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uloccwcc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cggwnnst.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hggpxrbr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mmxtufvs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dvfoxyqy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kvxalhqq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lzcqpqcl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2uufhukkz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qumanxlh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2aqoicslo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dbeafcti.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lckofoad.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xwhraret.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2pyjemunh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2daeunlms.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ctuluzvt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jsczfmnp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hrcsjuna.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bvieucfx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mgdolfqe.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pyqqijdk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jczqdlel.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xrhqzjwk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lbydqesw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2efaenzdy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2adfohcrx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yxznnwqu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2gvwumsbx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hknvqqqz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hycxktnm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2whwxxnub.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hfsufcuc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gxocwnbi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rezqfplf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gwbxphdj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2operxwef.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gfdfhhgs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cujfpsaw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijkqcntr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kwywhiku.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibzewzoi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vuakkewy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hicyikrn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mwoniqlc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exsykfpo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kfezjocb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngwsdxog.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nttazztt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mbhnvpyp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ypwxxehk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sactjput.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwakqzlc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bzuluwee.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2afiajycq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zdbherai.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oyzxqrbc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jkmiovzf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zoqnwacj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2fkozgskg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gkzvnghp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qtnddtqh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sftakkas.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2tqvfzgov.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rltepcuh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2urxdfogp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gmhdrdsp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bcgiaztj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eyjxvjgj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pryvmiei.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wvekfxtg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kcjwwsya.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2khadxgur.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jvemwumh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mmkllttw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2btnvnbjw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ynoojjii.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zorjdlnc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dzstdqqb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gthybzgf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2iqiomzdf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nvszptqq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zywpuiaj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sghbqito.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zzxjvpjh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tfzyggyq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nkexhnwu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mihijhni.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tmvhzqfp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kricijuy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rfdviakq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zjegpgbj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bzvvbmhw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2odaglfiw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nbjoyizv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2kmpjdexe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rqscndwf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2geotlivb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nuplpkpx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2yhhzreui.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2pmytvhby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2peiokozq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2nijyiymg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upfvxyyv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vgfpqsag.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hoxnecvg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2evcgugef.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gbpcjqcq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2evaijfaq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cwkkgiwv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tjyvlyer.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ymhfueae.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lkbpskrs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xhatgwbo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2exwkrxdq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ltyfyjps.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2iokjbutn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tejtdcfo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2smdvzfxy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2akqoyimu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kgjcgypo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jpnpwxjj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ldynvenj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2eymbygdj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ixlbxkpq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dfvtabnx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2disbfrit.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bjzfdwyc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cnyzgppp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2bwdfyjns.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xcgzqcoe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wkzvnsfs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uppruggx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hmdmfazo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cysrsebn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yqqqfqex.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bhzjorkq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cccwjbsn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dxnugabk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yhcxxdje.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ucmgsvzl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jqnmaiwb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zhckzcpg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2tzujwqcz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2njaebsji.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hizntnpg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gpxxdcdm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ogpqizcw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ugrsqsob.html


<!-- 参考信息 -->