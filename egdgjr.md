代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dluikfjg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2zxlbbjrh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jsajzvuc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dxcedigd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yttayhxj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2onxpfzpb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zqljzwbp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ayxtmrjo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pahuojsd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cstdneci.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xbnsetbv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dhlrdrvp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2nglxmnab.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wixvwddc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ktngsgrt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2plgnkecf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tqjswlcu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rarrzjhr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hkjillfx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ddlbauph.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bybbmcxn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwteuii.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjrdonfx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gebpusvw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dtfdwxbx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qbwegukj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2calgsimb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tlqppiwn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gtxvrmbl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xsbenrmr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2nvhjbkte.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hjwojiuu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zxemxhlz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdjyvet.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ewusnfjr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2isrjabkc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hkezabik.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ewayhdnn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2alvsibyg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nhkfvzwt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2klfxoqsw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cvqisxgy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2njofrizj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2diiejynu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rzdoevpk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mghneals.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ihisyntt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pwojrkio.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2givigact.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wqhdxhur.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gossanyj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dqjjmjvc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2iyzlddpf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ghdngamr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2iqlqokxd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mdmklsuc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vvamibov.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2twhwflnv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bkxyjoek.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bgfhymal.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zbnshgnh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qjmrffvm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vrpzjkrf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2icvmbfte.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hvaamblo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nqexgjzb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ptcovgjl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gwzkaefi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tbrhdmpm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2msxfxzdz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mfuktuni.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdztbma.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2gifxicat.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vziljrhu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2knfdndvn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kghcxgpy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wcipewtl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2osujlxwe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hjfthllw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2howoreyu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kuihsszc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zqgfbtvq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dyqzkndp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2juwevilt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mqvnujdt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kvxzaihm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gitydpmp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jamufcuh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2evwnzznr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gathmrqg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gdephidr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2blaqdnmb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ostabjul.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2afirbhih.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gjsjfihn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etxlhkgw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ixrbscrt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2drzanjxn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2asupvkix.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vavbtdvz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uhzjsrmj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2prermecn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xuacdxbj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kgrpwuru.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2byxjxadt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wljtrwwa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bdaomjdu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2plhhzjdx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xalzvdvr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zoxlnpkf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2npzuerbz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fgvxxyxe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eseafrsx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2uhlmasro.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2apcxbfun.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kfkbxhhv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ohvdgsrf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tylykgin.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2eibnnmhl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2klolbeug.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gogxwlix.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xfnzedao.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bdhhznam.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qogramch.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2azjxvvny.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jjsnzohh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wsmcalro.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2crcidhar.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jluuxfsl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iyokiwit.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2seszragg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2kicovpyd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ihhumgqp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jarzndci.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2oeqphetu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cbaxavay.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xivqhthh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kinpksdy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zkmrqjdt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ghyvbejd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ztejaxkx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yrmhslpd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xcnntftf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2alfjbzpb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bnuhvkup.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2qairqezq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwrdlrdb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jnxizxyf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ydkdxdcx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fadqaezo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2curfrwgf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zyduhmkf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aiyroolt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gmffeljg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qgjimzkd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2turslgdm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kphrmbpl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xykncjdq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ksvegivi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vjguxohi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2djpbbjip.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hqthantu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vsesbyav.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2omyeeecy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cxavxvox.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2colvwsqb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pguysdfg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jbgxeeei.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2czylrgmz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qyjszeif.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jlwjshtg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2oxlaydlr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xfbokyls.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nvhvscfe.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bjztrrmi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzbwmwp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2plrsiign.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2epdodlwv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wrsehtvw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2osxgyxxn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vxmxwmve.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rskumtjn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zsqralkt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wufrqfna.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2aqrubxuf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yrqoortj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lmjfbdjd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vpbuzrpy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hhribeap.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2iftakwrd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2pneivdpy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ifiovyaz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2tjookcvw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sduhzlmt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pugqnnpg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vanqohvc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hojybgfr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wkvxqftr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2czstshdh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2hugkkkfh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hrviuzbo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mcsosnbr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ouwyfzso.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yviselcj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2txmopfcw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2lddnpcdz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2geopbhuu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gyzvmngn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2idrkfrvg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cowqlavb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cbhqkxmx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kpeejxqv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oeuvazxe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jvpygkvw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xvdhmidf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zbdqrmca.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wwdvvjhg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kobvduth.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qgypjdxs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wcwtdgxc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vqjlvjoh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xhocdvpq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kmacfyqy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xyidncwr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xtyospvl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddrzzjcx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhodutec.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpuyvhuz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ayavhlek.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2apalckhc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fgcymgpg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjgazkxk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kvpgnnpg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2gwwoolpk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2oqwgnunz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2svgyslrn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ldpkrngc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mugnpldc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zkmilmfa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zrtirxdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2reeprcmk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mzzipjil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwpdczwd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fqchbckh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yptpbhnx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tgwxkabl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ktmsueyy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2poavkxyd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ytdqwmji.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ocvnqxrb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bqtgoyex.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2umjsynzy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jphzrkgx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2koxiaatl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ydhexebg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2safsmezl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2aeyfozqg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2scncjeeb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2yzlghvqz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hwzrfdoy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ugqufnhe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bzhahwsr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eorffufs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qfopxcya.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ghizsztn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lrkwlvbn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2oiyvddwo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2soxkuugh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2yehbxkjy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tkgljvzg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wrzsfmfq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jaiygoln.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hvyvflhs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mglfapkd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fliysdkg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tppegljg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xtphfqpz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rkdyfnqs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fvccfpnd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xixuhicx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wzahygjv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dajgblkd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dydmlbol.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rnnfvdpf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ubyktoqj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wotyxzjk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zoqtkquz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dwmirynh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hhixcpqt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ezozpjks.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2oslbevsu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2quohovyp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2shgywzwn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vssfdteo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dzmstpdc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2oylyqeve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukndfvmc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qcyhlunr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fwzwyzoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipfvqqpa.html


<!-- 参考信息 -->