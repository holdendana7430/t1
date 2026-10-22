代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kfnxsjet.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2lszpwdpf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wzcraoqu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mievfpme.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gnigjbdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkjctepk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2htuxjvrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdqjfb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mwbeivva.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2tspjmtna.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tmeoyixh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpixvdjz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kxpnjzay.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kaxqohft.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mrbcaeds.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ikxusygd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ejnencpf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ialwjcie.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gqhgjovd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mrcoahub.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mapijzpe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zthlzwve.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rtsmeexc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2icnrruut.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kgcerwix.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmqrdib.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ohmfufmj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iwdpczbq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2thdqwyln.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qpjpuonk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2sarmprix.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxiimer.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qwfqcrqn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2owtqepim.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nzfrblnl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lgmwirzn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xpttkpfr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2temwpkoh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gsjcxvns.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zypiapha.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2grgtshmp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fnwnwwmd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kkgjkhal.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ddlpneis.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2unfmpcxi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmlannp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xlbeqygh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ndiwvmeq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mxhadtru.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cucnyllu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bkxyiqzb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2capwaghe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2izlsbwxm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ezbhxbhw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rivkxliz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bapxjswh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pxqvmwfe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hhftemue.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jtfqjlmm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qqdjxkfm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2vlspbwlk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vvbhugmt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2eaoenxrs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bszxxlua.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ogwxhjkt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yjvmvhxf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2umfutclm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxsmcju.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pyhftwyc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pkkgdlej.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wmrningu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nxemoqyn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2htuubqfh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tewtjlqa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gjwuovje.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2geqdbtlp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hkuvqjix.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ikcbkegu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hpijqtxv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gjvnxqkf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qjjebptn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qvtiunop.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2abeebvlq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vssopcro.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uwuhcpst.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kympedxz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rqhxfnlo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rbtvrtec.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2murekylq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wvxbaecg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2eeemhaxu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gwldmptj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qtcxgbye.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hfhoxinp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2tkdhrefi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2doqfymuh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2niaqrwra.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olmdbqrt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tugrepah.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2iekhmqrj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ypxnsule.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vsuiltjx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vaqxlpkf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bpjfqlih.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2axwjwdpk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2heuusrzg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2cindgjib.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zveiajsf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vtuahiqz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bkqoynpi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cttjopeq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2imotwyxh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bsipwtji.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kbfaofvg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ybajjixv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2joncgrjz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jtqlhjfe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iyejgral.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cvagzrjs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhdhyii.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2extuezxx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xyreoktf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2voshflah.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2prlbtyvf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fwjxttbx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bitpoike.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vgiezqhl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cvjdnljw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qncxwjsn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2llifldaq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mvztmrgb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ngrqlnej.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hprvyhlb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bmwcbink.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mafdhwzl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fxilbqbc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zpryzpka.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2olspjglf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2izvrgcek.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mlhreeoh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vxoxcnpp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2igfrypkr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fafnbmoi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mreodqwl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rwlwgrdy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tzendibt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bvhlycsj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gehhnwrg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fucvraar.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2embanqnc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ubkpbsit.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nwenfgcn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xbythinf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2oujivyfq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ghqmdqiu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tzcoxagh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fhtvilbl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ntmzwwvl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ihtciqyz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fumktzmu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jcssngys.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tjmcdcpg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jelxpfly.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yyuachqz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sofzavwv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2brtowgsy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2acfxcqvp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fqkoaceh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wicsgynp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qkxpluzq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xhumeasu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qyngzsnw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pgcdyefm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uwtiawte.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qnzinmfv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nzrxuaow.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nowlpdbp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kmojwrwo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qubgqxcs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ewnuovpu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2irusxaun.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pavezymb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rqxhvnmo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ggndxphe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nmjstidt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ngbkzxwb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qkoeccrb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fiydrjcf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2nvyslwwo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vpcgycwb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xrpxript.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wopopnrc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xtxzkodu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2znwilsxv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ankofnjp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uudukpkg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nknldevl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yuloewoz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2gguvsfyk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqkqlfzn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yyjaifet.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rarlpzco.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ykahhonj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ogdodfva.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wmixmmyl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2otpyxxvl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2uibtfdyo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xnczoogh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vndfboxm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2eokiqtel.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zkhaltua.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ogjbuoyu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2itvuyvig.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hcgkqvmu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pttcrglg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zfqapcjn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kqznsjal.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vvnrowxe.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2myxdhggz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xutthtii.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ijrmysjn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlybhnu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2phfzoxol.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2blxofnzy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gweoorru.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oizkjvum.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kxktpmrm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dluzzcnq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fqcehius.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vaybeanf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vwhirmer.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ofepiova.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2nibrsbaj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gjweferl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fvtzausp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqdxjd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2utpmknwp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iudecmlk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tbawtgqm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nuyxahpo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vebhyhoz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qwmzahll.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fpcnfrhx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2isebcjeo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tfseebhk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jsyvdjwe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lsjvtexg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rjyrtkoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiclgfln.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2omgrkobk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpkgqbhp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2spqcotcp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2masnsemw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2bujcmjyi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oorfwhoo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mbxptrur.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xcsgedqh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aqdianjk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jfakzjvq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gwyncfwu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kvudrctd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qppijwrk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gnzfivxe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2oghbtzns.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ckerzdct.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vhqmffbl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ehljygrx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ivuxqarc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2iexwteyr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kofdddjo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ctmljncq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ilrjqmim.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2helgqgdt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bbmzwyem.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fwtilxou.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rjqhxiqm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lqoakpjg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2skbvhjfl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjhwkb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2chjpuhoy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wtecyglt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pfoqkylg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2huwxicfi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2krihetak.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qlzguvpp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mzjneltc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2oshbeyik.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rbgrtpnn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ynzejkwa.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mdagfndo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rgenjtnv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gbxjeaet.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rgsburiq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xeyycgcb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ghlikjws.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ermzivti.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tgkxldlx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hkfgdziq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2isdepohg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2aeakszpw.html


<!-- 参考信息 -->