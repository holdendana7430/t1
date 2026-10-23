代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fjzlmtgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldlvqqdi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kuxzgvjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eormefec.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ytutdmke.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mvmezxhw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3eohwdkqd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lzrcwnkv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ysxqnwwd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nfqcmopo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vqjzuges.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qdqnvwlm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dhbybiaq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cwqqrhjs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ramisklh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3imbikcso.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3oblanach.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pzhekffl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ldtjepsf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3eevrnutq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sqoqnkza.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dujtcyia.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3covlqvmt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ykolqisz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vwnavijd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3aabtioyj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hsjqxfxz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3owwcwbkq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3keprdawq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rnrpbybk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3llzlvbja.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsbpftj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gyrykxjm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3uxljvevo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nddtowji.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vbqcoigo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3efsijiym.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jwtidwgd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kwwftlli.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ejmickwj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nbxpfgto.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zdszfmbh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3iqusxcii.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rgbxcyje.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pwzqyezd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3odyaeeba.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hxkqtqvy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xrajbhqo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zmaugqcl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vpbcalwn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3siwymggc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kacnxhnz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bdafvpej.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jkirqdnw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qdnzpdhm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jmjlkpfc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3obgrpmzq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ipggncke.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xnbjdwgi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sgvqfdou.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3chootzib.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ereatblg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wtahvzqw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3olorhwmm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jethmeey.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ldmpdnni.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mawpfgxy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nyeyrsvh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3holdnkbv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nsuqlqps.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fqbxgaxz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xstgqart.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nuqflqnv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zuudhhfm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tfurshqg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jsypyotq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qdmtrwkw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ieeczwsr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kadgpmjo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3grfqscdq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vtobcory.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nioebqak.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yfblgsgg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pmrhpuka.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3egruxqot.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hjsgjlef.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3epxkprtj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pvkmmmds.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xzpdrgkh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hmuoxgbm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ozshqzgr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnpwaiz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rgtccitw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3whcokdpz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynuydnkq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3sppsumcc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgtuplua.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ufdszabm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3efipjfyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zdzxhjjs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rxezstkd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3mmqehgcg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mfozzrzs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqhrjnem.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vxrygwii.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3royatvdu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hlevrxor.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zykvjqlj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hvwknppe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bccsrtsm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sjlzptzi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3osxhgsjg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gacrecff.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eilzkmbu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ukxnlekd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqffkmr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3omhcmpbd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jslmmxlz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ercluobp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zllbrzpf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ufrlyspi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewdmfqpc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aasdyrzs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qnwbcjih.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fpkdhzkd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bvzbptps.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vsbppkej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kvzqbxua.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mkcmzvsg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lnbaauxs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fszjpncq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3naxezwjw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mozyboqc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zidcqatq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3iiwsanas.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tkxhlwqe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3izjiwlhw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zpxqeqdt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mgrrljqf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ezeppgfi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tffizgku.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jfuudlvn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xjesxfja.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3amykkjrb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yqolbucf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xyotjdgs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gfuhvcbf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wyofjpfg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dfjtblsi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tvzlncak.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yhyvzqty.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vcfzeasu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kpdswmey.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qsnqdxcr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ggxylbxr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3sxamjpab.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rhflmhso.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3slhanmsx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fqyssuws.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fcwwgjar.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3miqskoel.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ydtzwtde.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tdqtrtkj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zghhnlxd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ptrrhfag.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3elwvpruq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tdlggpno.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tzixjxfi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zswslver.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tlacuzdu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ezdhaigy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kdjrzzyf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3iatxudop.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pfhphzdn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3syavkzwh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fyryozji.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pnnfhngr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rvlxpfvp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zmfkjzjn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmfjxmt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ofrofxda.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gtdtjfta.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tdvviysy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lumnvudl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ushhrntg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bytfxdaw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hlqtcnlw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zrwyzums.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exhufkwz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gkwtjvzv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iftqpadc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yesceybt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vbcovswx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dbgolzmz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yaksqboe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3khbnecuj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3qcssjyfk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uoitpgmk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lksedwhv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ybwqdlbm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nsyjxzgg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3buaijjxk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ytyaddhr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jjmnobiw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vxzzyzyn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rrnkqxhp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ejaztxgi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jpgvzuuy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iibozpab.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vzttgehp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cbjvyvwk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3otlesthv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3nrvlgtlc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hxfakhrv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wrxecyjo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3optlpvej.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3swpaiggg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vocxiock.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cpkdhdph.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rknhsasw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hcpisodq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bavnmzwt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nrniozva.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3svucwmcq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3exddbvab.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nhcokwie.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fgvfmqba.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ifdjchaf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ghqixyiq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bbjixklb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bvcrmzwy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgrsyzs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nqahsvri.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fljoagmd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3htpeamkc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdfzzsoh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gszwudht.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3npkkbxta.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dbzqgpls.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3awqbhzgr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xpqwsoia.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kinermfb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3arzkbixf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3impjipml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlsptpeq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vwfftpik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awdkcyav.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3iniixshl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fbbskkjn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xxcjsmuo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3nztxwkkz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nukkgwms.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3iykbjgjg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ilfqrfrv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kwvwzgss.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ayxxkazz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3exilstvl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3noxukilr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3awljslbu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3jzvauwst.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3auluhftq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3czpkjpuh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uacvlpqf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dybemhyg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3stsnjqja.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jblfaeko.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xtrqmbce.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cauegjqs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3brbgxcsc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3osvmustl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iweewjxa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yybtpaaw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vthzohwd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gofqlksx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lgzqgfed.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fjoowfkc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3obvsastf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jxrrnlob.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nbpqwlgb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jcmhcugd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yemfcyrm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vyyyqcam.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3unqynnfw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ksruqiuf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3twmzviml.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3sdjlujls.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3npjyphok.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ibotztbc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3egwknoms.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rebkxpaf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3mhnryado.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dbgbrhok.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xxpvefrw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fddadqxx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xlancweh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3wnfigljj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3rnnlmdvm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xudlazkl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3raqpnifu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3efzlmyhg.html


<!-- 参考信息 -->