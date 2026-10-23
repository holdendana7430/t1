代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gcixjkxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnbygwfr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mxhwegrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glvarswk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3bqwsaace.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gsaymarl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3eglcqjqg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3unvcbjbi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ztmcjjlr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pavknlww.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ueigfgdc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3joiggnuz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zgrpledx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tlwgqdze.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3imlzagzn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3oixxwxex.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3thqjihor.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ijjrrmlo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fggqjpbm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ikszzwix.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jtgiuodl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3worvxuhe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3imoxglxb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ssmaeplj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mpfnorga.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkrsonm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ukbesxlg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3puuuiufe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3djqxfilu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xfwelrsr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3yludgkhe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3whzehrez.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mpgnucea.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fthvfifn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vcjwerbo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dilkmgrn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kmmfxfpf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xazzvlmw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ryjbdkuz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3erzvcyah.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uinvngtx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbcyylo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ckzovldq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdplaje.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xrzxixnk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hmgizhcd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sqvgdvro.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rekxvqzk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3utistcnj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qhhrbnpc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nfllskyn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ozxfllgj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nrqpykmq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qpdzycrz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wfcuwzfj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zweilwjv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lkglcpod.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3znasihqy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sbtmzquv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3eqdoteas.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rvpxgvms.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3yzrhmazn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3empxcgzb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hryglgxt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jnqcmsrl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3frsjfgrx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zdoxutuh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3aelxjufe.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jcmhielv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3uglithvm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rcjgzrsc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kxivdcjj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gcqwpfgd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kjufibaf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xqltuwkh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zgkajoyc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3skywllvh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ufkfoekl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cvopoidd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vgpkmxns.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mbrokxlr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mbblfski.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fumdjnyb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubnacutn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nbzrrhmu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hfkiafco.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gmzqwlnt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3omwvahvs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ehunuaxj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hdrpltdz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jztnlqcb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3glktpifx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3imcgwavu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdqzeryh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pyszkkub.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nmuinetm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwueipfa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cklywppl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zgpctvqr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmwtbcef.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fgnrpdza.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vqowwwpi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qevrlkdn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovoktgoz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3okifxgeq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hmyrjdgf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eikjdoqz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bsteihnu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gngqkhoj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ulsjndpk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3wwrppoid.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3egexiork.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lyevuiqt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3faeaoogs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zvgqrjrr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gxiccqlf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rosxtfmg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3fvrljvdz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jnyzilzc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ugbwpzzs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jvfbtzcy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ebgloaso.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kgkhhade.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3omkbvcjf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mazrtelg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jgdsmvny.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3popxufbf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3iycfmlfy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3uxexxzkm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3beilrjlf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3txdhidod.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3spafmlot.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bikhoubz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ggrlvmsv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wbibekct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvpgrrvm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3avhyccwf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hhwaptaz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jbnsdpnq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wctyczzg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nnxltuvx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3byfzbked.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3lydrjcji.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oshjqrtk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3musccfia.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zznbuhck.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3agwwrqyg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yfakpheg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bnlysymy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3uzuwqoay.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gpauqeds.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3iiepudqr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yzfxepsq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3szmqztrl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3uxshrfhw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pwqakiuk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3asvltdnf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jjipgree.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hnmrvwbr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tgcbjhij.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3npwypfnm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3schruvyp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kmthneaa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bbhnckcc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3elwivakn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ghlblzum.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fjwmdfqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnuzkbp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lueoyqeq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nsdhvnrs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3flqwdlva.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iebhgork.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3iecrvopx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ejjwkhor.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3usdhrxrd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jxkzfrvb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nxuoovjx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ufkwxaix.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ttiiyuij.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lqdjegqr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3faukukln.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xsbzuwnd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3raaorquf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewshbcsk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3uwpvmrki.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fanfqtlf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3thrgpriv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrdkort.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocqojvts.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ixgsbkip.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3epcqcphf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jfykwbct.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fntrhnqm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vigtqdvo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hjbcttwc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3crirclxs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ymygdnxb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pijwrrma.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3snzdtqis.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gcfmzsze.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mickkfox.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ozlhpjxc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vlertypx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hcsyzdtu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nkihscze.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3oxogciek.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3holypzvl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tbqdoykh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jfxuaqzu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jyajsgsj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xlbmxeku.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wabmplle.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hxnbmrqr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkcigiyy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rsucfmgd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rskqmxnn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rvvivzdl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fysezwcu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3egbqccnh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3endfrnkf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3sheqpkhn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3leyiixyk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3topinaye.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3plcbxrfz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iudfrwzm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gaarnyqy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3bykjyoiq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3udxbstab.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ysbqpmqf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jlfmftic.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtibzeit.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lurndedj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ocfobaux.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mgkxflew.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cmzapdxm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aubqkmaw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sbtayayu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pocnswej.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lvbxlqjj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tudhxdgi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zdmhiywd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ummxgkvn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wbhrlwsi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3shrcvojb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwnmdgtu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vtocgroo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmzctxnz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zdgijwum.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ohwbxzpj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jloqbhaw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mpopwdgp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zfmcxfgn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3abfloizk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nfnvbakv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kvvwdlnq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fnnocyai.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3uhnyabqh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xoapiqbi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3yyyyzybp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3cibixnzc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3msaddlyk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3oibltyte.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wyhoffir.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3laydnkfb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3avjgnaxm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zjtytcnd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3iuudecob.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rcpoeqhq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ylwcoqsm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dzpnzxaf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ykplmjfq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3drxxsvbe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vrzhnhtm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ekehwdxa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oxnrlrfo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tyaunfbv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3shqqhqjp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wytlgufg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdbdcl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uqkgswfs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jsabavgz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xdjpnmit.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bzcnedjm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dnynqofw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ydjkkybj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nspowdcp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xwsgptyp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yherhuzv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3dtsxlfah.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yoppossv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ijjrztqt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dpxmzrlp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3gquldhen.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3frysigtu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yeserqlb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3sdfbpyan.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tucecsqi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hymgrpji.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hlfwzuwj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ihvbynwt.html


<!-- 参考信息 -->