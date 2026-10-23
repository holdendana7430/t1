代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3llymcypk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3eqmjouye.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ortgfmbn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3paaoobta.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ftzukqtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxwcwlnb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zcejroxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kopqrzga.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3krfweqid.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ehdpttfl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tiwrjwqy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cdfxjgjr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bawgsdfi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gikkuvfn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3feodyoug.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xrqpvkno.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3srdkrodk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fudckspg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qnnwggjb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ykbxkffc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fubxflwt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mqvoyiav.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nxytxxqt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3aivqzyqt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jlnkjiqe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3asieaagz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ffnvohoa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vxeaikwu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sxdwwycf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dofnujrz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xoxcnlea.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfpneolv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dahspacl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ewcwbrcd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qpmawphe.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fdpkesvm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ceiokcwl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jichfpfu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3iezdlexj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kbmczlnh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bkmhvjke.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rwddxhuj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bekfbrfz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ylfbywmd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3finjcafl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ovofxagm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ibgurhsa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fsbzplhb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bhdwbuxe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bcovogfv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bmnwcloi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pjniufqy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfaieljj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vehfnzkf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3teaqxqxj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rzcjflub.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xrpyfbtb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ykyvpskp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mdxlbzes.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpfcacj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zynvkgoc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3quzdafvq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3niczyayt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zvabponf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pxcxtoiu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qmtilreq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vjfoymxj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3dowvqtop.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mvqlvgsr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3akrhfqzy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3keqcfevi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kgdgtlly.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3llntnemy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wymqdylq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kzsviruw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dysvlbrd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3inwjfdra.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmaoktb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zddhqegl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3daeclflt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3jkuamftb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3unbqlgnm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3sblwucrs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yqzcqpvg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bxqshrwz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iwbnlusm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jjitduhx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3knmffrmz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3atyeeajf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nnulcbsp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wsbcfmsn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ffyillyr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3onmcwcjm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bbtwnzoc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qkycfbos.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zdkgbldd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rjqcutxe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ocylwwvf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3esqnqrfk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lkgvnqqa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3eyokpupn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dozsgdyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nyfjasqf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hridebzm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ydzaythf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zcfoeciy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3tthrdcvx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jzgusieo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3thxmzton.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ceqjfulh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rijxsakn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ormylrur.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nviwexrm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bkagzzco.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ojogkppi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3kswppdpv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3geftxmmn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qwmsskfx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3evvdylmq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwlnktxi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3egpmppmp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tfcprdvp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3aokaptmk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3junqhwmj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3umygarjg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ugfkuncc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vcjoginq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nzltfwzv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3nvqhpqix.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqjpzeoc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zfmrndbc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nxekuxjr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tatayomu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3auqewwye.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3crrkjglu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gkishhvt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3whaukhyp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lbkbudgz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rsaqusjj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gkimxvdf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hhclzhju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rfmfdzzi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lrwiuvqw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pxfcktmi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xtnhkrjh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bchzhnwx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jujhuetb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jrfoelai.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tvfhdvtx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wqgzgpdi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3narwhges.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mjqplqxx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3eudukdbz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3sgjdxmgp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3seqhxgbh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3paudnzyv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wnxakvee.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ozlycvrd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3sigmspbp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hwsijzgw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rdielpii.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xevtxueb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yqxzurho.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fqygefkp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ggbvsfwv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wruupftp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3evkiuiwu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ysmvkeqr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bhzfhbbz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bpgwirll.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rbleddpy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kjenlxro.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qtzhyplk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3eqgllcae.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wubjzaxu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jhdhdmoy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qpkutzie.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3teehgwjx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tweeskgv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qtnzudad.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bcjeajun.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vhdwcpwv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kleqosry.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3chpbhywp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xumkyjhb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tbdazvzh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zewwufbe.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccchkaan.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jvrfbvhm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dwyvxrux.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mmgvqfkb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hoyaosdt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uxidzguc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ixmjrawh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3suvnspmn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ltoedimx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3svgandyk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mryozerr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3duyjxetg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dldflnvw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hjpyygtg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xrioqbcb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cqvcxhpw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kkruvyyq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fyeubamu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3snolauuu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3gkftrpnd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3copismdw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fnlyzvxh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lbstwoqk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xenacnja.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lnvallfa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qmbkhkiv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mibddkuc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fkswffqo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lgkxnesj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kxqvsvdr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3oiyknrpx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3elglbbtv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zsxkywka.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cvcbauhd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wzquprre.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3vyhmtaml.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tynnedgj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ikkijejc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcddfhq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tfpahlcm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xipwzxtf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hqmoqgjk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gkyrbjmr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3plfafkzw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gchnynyk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ndcycegi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mnwttiip.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jkrfythe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dcbnclah.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tzwtxgmr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uuompmcv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zthouhvc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuujifwx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sqhihmwk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fvnqgmnz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qepelqwh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zdhfbyux.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3rrxxxevh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kdoummop.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qmwnxsld.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ogcuxpqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxvczpqh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3fmahvpzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anjvcfke.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zvtrwuqx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3aydmgcqu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3rtqqvroh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cziotpjf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3habirdpc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jcmhypvh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nrlpouff.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lxqowhnh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qlawaezj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3harhcneu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3apesvavk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xaufiofz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3bthqskth.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ctlyoavh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qwsfgrfg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cmnoalug.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rduleohc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zvaceqtp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sjqyzini.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gwpxxdfh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3raanvggm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uolaptqe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kwoduecy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yobbqlix.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yvgvyiee.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uuayzegj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mtlxkzwa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fkfxagty.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aabslivv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gncnjryc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pnhbetlu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yksacfzj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iatxvtml.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kevfizit.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3odpbcjqb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3axhwmvlm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rypomvwx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jnlnlvrr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ntlhwdqs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3mqslzhkc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zksgpumb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3dlvbcfhg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rzdoxprg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wvslrgsk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3okfxwjue.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rspgdrdm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ezuxftwj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3skqmzfzy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rmicyaej.html


<!-- 参考信息 -->