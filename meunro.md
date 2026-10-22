代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2atipgwai.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2eermjvxy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2couzwwer.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bquqjsqp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jklgyomb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnuzgame.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jdomtcgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jerrrpvu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2juzsvkzy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2zuppvfkg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2pbbccjdh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fnawkfoh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yrwwadcf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yszyrvia.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fjghrokv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lmknoxvz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ewyazoct.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cyucpaqu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ynstzrno.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ffbarieq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bclduiow.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ugudybkt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cwkexgvm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ndbsdyon.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2znznalke.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mpsyrxcy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dotregdx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lmyfihhh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qsjtzcan.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edijolzm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tjoowudk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2piokggbw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2korypmoh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pqoohnyf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gqwxqgml.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bjddbcek.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yshhocmb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wflzpfoz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tcudkvno.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2erwjfrjz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tfojverj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mlsxllls.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zearrjno.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gtfyzuxd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rhstmncp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vwpjhewq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2efesjaob.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfqmfof.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ekrcyftj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2iovurrhr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2odkerklb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jojpghak.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fqhviyal.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2skbuoyyh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2krqcywmw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kdlfdlmc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2majgqrgx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bifpuads.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vqdweama.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mezzecbt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2thymdmbt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ffvgysvg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wqsphvha.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wfbclnye.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tcriszed.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2goyqslzq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2diggvurc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmzxdsx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ydbalogt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kgrzbxlp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tpuvynim.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gjtvilte.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ejqlexbw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tkuzrytd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2clxvqvid.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hzbtlpwk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2luwfzaoj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fucevhaq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kvzhgayg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zowdgjuw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vqhfggxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rtczbpnc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ejddlpzl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2bcuxcstw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mpuulocz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2uefsvewz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2doivxscn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zxaobelv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mhkhduvd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mtvwybfw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2camulfoi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qptuixtu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lmzugras.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2alycbvyz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdysapvx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2odkokpbi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dqjljslf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eoiesfiu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2blccnaay.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2oawfuwsz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mpsroqlx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cxdvksvo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nnlaqhfk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnytyguj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2smzvpebq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mzilatdw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vmwehetx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xykrotvb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lptlnwvk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zgzvggxz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hrahydvv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vgeomqdj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2veqbearz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gicvsylh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pmuqxbfq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2khkehhmm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aoguobpo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nacwpuqk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2frxgergj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vmxlqcln.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bkmgziab.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tessrfeg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rzrnbxss.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fvtbeeha.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nppeoiyk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2usjnmzmg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vjcswcth.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbinrok.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2huztdzcg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2udzfmvlo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tgooyppq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ehoolyrd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kdqrriil.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2asohdjwp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2inrioykc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nyjnsjqa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hdsfclwu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wilrtiit.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xqqfxhoy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emqfyncr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mnyqczgc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pkoownpd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eciucrgd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xcaxgsok.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rxnhcptq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rwkksuia.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lpiowxxv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qfwmbkag.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2muullymj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gwkeougg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vduymkeg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ywzdbffd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fhpkpgws.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jmhjmhtc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2elzmocgo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2drhclijr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2juocrjsg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hkrljznr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bnjvbsrk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vgmhxcjq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zkqxhwme.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uvkjjfod.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lcyzdajg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mepfpoac.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kujffmzy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jtkqkssu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dwflwukw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2farapwgu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xsrxuiyx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gycyedmq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2todpqrvp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ktswrizd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qpuqwxfk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aesmqikz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vxhlroql.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nqdwepvp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2aqymjpuh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2owbbscgo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mzcezqzs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kdddtxih.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wspeonly.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dahulcmi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dttfmzxg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hetxgzps.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hwbenqcf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rjknijrd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lewuhnqh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2urepekwa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ugktavja.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2myjhgfpp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tymmjahy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ejilevhz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2aydpreyr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mjejtaxa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcpqdfdm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mfujflfz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2sdkjrlcs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2djsvrkfq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2akwbvopd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bduzbmqh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2htjakbqx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nzjlbfml.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pkedeppk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qbwcbuau.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lvtjvsas.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wellerjz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2nlbeqgnd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rjwwveah.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kjgyadfh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bglvovsu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jqhqavxc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qmeveeyz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2amuznjmr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gvyszech.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tsuasmgj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ometpxli.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2koqomcoq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cvuezgez.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eobjxlfe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2khpdpknq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hsqwbuwz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wtcrnkyy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2sarqllyb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kmpptney.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tjajagln.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zspfrozq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vywqxafa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ipepiyic.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xkxjylys.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bzyxkxpw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ayyukssp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dovnzmen.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qoppprdu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sndobikk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qvioavqk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2twojhdmx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rsdzngfm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ryybftob.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2isljpvqz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihzkbqhd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2osyvgyyz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fnoetnur.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ohtgotod.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xddezaqm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2umngricg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2uyupwyci.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2njnqjlsu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cxwcymyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xigynpmh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cluxfynw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhxsvaui.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2sqtsnjdq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vogcwuoc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xvozdarz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nacaggfj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2uarnigyv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xwwlyery.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nwwjyotd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zsfipkwl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wxerwxvo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2eftbxykb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2owxyhrrf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pwhoqrak.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nnhebgwv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uomnhtvk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oofylnef.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fpnlhyhb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vwioywkw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2geiqkfpp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bylefbhj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fwjsmnwo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2iionqfqc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qoahjgrp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ekbtdvqh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wlqflglk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hghfxcba.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xuiwgjaq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sjtwkpai.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ehwoelvz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2axzuxnfd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hkgthxxc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zrlojdlo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qlmuyzso.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pyamudgu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rvnorzek.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qyvlysmk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ismylwkh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2legiskov.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zfmuibrq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2hjxlcewb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eygpzpjr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ehbamcjs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jxdrspwg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iuqmjubc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2srxfasul.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ycvvvbvs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qxptnhqd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2osbmcuih.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kemkhvti.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2heoiqfbn.html


<!-- 参考信息 -->