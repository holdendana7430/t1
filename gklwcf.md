代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ocspsvpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehsigqwf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bysjodqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzzpfmse.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wtvxfjbf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wmuleydi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tjeafgkk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rhylhlri.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ebpkryrr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mzqiplcs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uvhzpuqf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kyqmrnvk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nphtzqqu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xzximacy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3indwkwrc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3webmmzgz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mrkgcubx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3uetvbzrp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qakqlifu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pyywlybu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ybdpupgb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmtaams.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tnqymnut.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pzobqjhn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nakbckim.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpcageb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lgmdezqd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3certvbvo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zlpnwpmw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3aymktdsr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vcstsyky.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sjxfbnxp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lhhvnrkq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wdvvsezg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vmnidlsm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vgzdmimx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jswapyye.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fopijjlb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ghmpkkyq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hxwwdacn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nvkqkoiw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jnexfzvz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vvmtuers.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bvjbhqsm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vvzcgawr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3arbbtqbl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ejvyjlfr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zbzvilpu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgdtjvqf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xiembdkg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3flrokbbu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mxkhvcyf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3burnhopi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jaakpvhi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xwzxvyro.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tsshiadq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3znspwjsh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ypczrjop.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xpypfetg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qqwgmtjd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bgqnswwv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3npsmqjym.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kqdvryei.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3meenqrcj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dnqfpauc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tnjxebct.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fsglcrcd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3giycxcwj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3quyhaidw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xuhogozz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3slzumlye.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3prjvpprj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jasxhfps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rorugkio.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qtkghatl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3omkqgtsn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wmpgkpux.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3wushxlsc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ekodlwcg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fhhaivrt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3imuecoal.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lxggptvf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fjaigwvm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gkbiagij.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wtljbyon.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3koszqgvk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3edpsuazj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kzxwijqs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lobrihdj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3iqcweygn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zkldqiag.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ftyfhbyg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjquxymz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zwbxiwwg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ggesexcx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3siuqkymi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jhmhapwg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qissnjvy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rijkgpvk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlpvonqa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3lezjdvyv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qsarvblk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yfjhloyq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wjfoiqxq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hqfarpdw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xizpibfx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3blklhnds.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ntzgzdmo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ijoebnut.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lkmkimae.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3otgwrtyq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jimcckqi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kgdflouv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qcezuerr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkiuwxyh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xtdthbie.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qusfblgi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ekbjotyy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fxqtaqkf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kzwhbkra.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3udiqhlgk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3czvtzkjx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aawgaicc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tagaohpk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rxlpgfdi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwthihho.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3piqrmkir.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kjvcybax.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wwarkcxo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ptzuyuuw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ziourniu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vbxyoqrj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3duouytal.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtpfwfmj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3khnsyfpq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hjgwchms.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qpudtetb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gazwbsbc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vbtkwtwp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lnwhfrrl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3dcvjxvim.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cyzxguqu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rcqjlwkn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ykingoyd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lctiqhdm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hezunkwk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rowtuftz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3crvpnmsj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eykclckl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3napjucqb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qxqfcdav.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vwfsfgdi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3uojdikca.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bgeobcbg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wfvwlitz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3uixxbdib.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3itpptmas.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kjaklspu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xuetzfip.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3iwympfmc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rljgcuxy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wbvtimvd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bktvxawt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bjmnjbdb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qgmlnrqa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mrqjdzom.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tvaqdeow.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tlotfkwd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3itqvxquc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jmwlpaem.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ulcloxhv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wrbjpsyu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3owmdbrfp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ohzegqro.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xmgkhahk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rllpmcmh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qbprtglm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ercqzyru.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3kmwgkqmd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jsjnvirc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tjjssxvl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ineiizyk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pipqwtru.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hhawtoyx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xrygmimc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lbdngevl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kqalxrbo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbsaob.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkhpltfn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3labadbrg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcwsfejv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kideqnmu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ezhirsaz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mgdgprpa.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ucecxunq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3flrxwdej.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3tfwravww.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvqiobyv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xfkfblqn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qzhgbhfp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3aszbsgev.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ocwkvfsr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xuximqac.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hwqeupdx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxqegq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hjzoyeqx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uoyloxcb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ecgbznnl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3namsllae.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vmbpqyxt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gvdfzpxi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cyabtabm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gsdsgvkm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3joepkvxh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jeplfgps.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jjqdddba.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gcssyaku.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bhoqcjxz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3araydmxl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dgicvhjs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3abwoeodv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vhuhbpkd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3sxjtysog.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jxywpizk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kdskkohw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ccppycal.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3penlsbff.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gvvrqbmn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zxqqgenj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wpzazptz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xyltksql.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mixaiwmg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3icfhpdbb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zlqfongx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gqdhqplq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nyishsap.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ycgemksm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hvyvkkmk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jljuacqc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wrlbpzwn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uekcyfxr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ahqycnqs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zjueecau.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zphdsazz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fayeobyb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gbjhlfnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxwydhed.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gctirsam.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3snxurxmu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3msbeznbz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qvxwiaza.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mqagtdgb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lztcehdh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oezcihzk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dkmltrdz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zjmfbwfx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hxnivwbe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dhhldlys.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vshgdeud.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ddfonzbd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tjvfsrnt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ublecues.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dohquzvl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lwzlurca.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tiidmesd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xqvgpupw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3evekbxfd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gvropbux.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tpcgjqaj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wfgwgnjg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jlizozzi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ojqblxwb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rmltekne.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ukwzvcxx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lvtxvlxt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rwactnnf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ptppnnqi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jdlpbded.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kyqjccxh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vspezuot.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zoxzgsdm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tefxefvo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qbrjstbq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3txueaxgp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3hsefgjjh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hksnhyxe.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dkhmzvad.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3euhzvnfz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3abcvciez.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3exahvgtm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3idtnezzw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ekguxngn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mchrbhbp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bdjpapbf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3avtwbqxl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3jezuqllp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lrotxqku.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3akoiazhs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nnmhuzoq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xifzhzjg.html


<!-- 参考信息 -->