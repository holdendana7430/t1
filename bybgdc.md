代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vrdyzler.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rbfnvllm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcdxhqcm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3txsugmhi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jgggdlhn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qxvelvbc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3prslhbiv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3relbmbak.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qcuohfbz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3eslrrhnm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lwuemdmh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dywqeove.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hjvyppiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydvfmpdv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yuqncagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dilizrrb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ebrpgixl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ejelgmpr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3comwoxpo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mvjtosjp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3umirppiq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vqdjaekw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oiegmzxu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ytxaihoi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3flzkzkvp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gkkxiiye.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3woaoatpz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3szxbpbwn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pemkccdp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rzojyvpd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qnucdrdj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ezbknzuu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xzixutoi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3sarmchnu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fxbqlykv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3lyvhwssi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dhhcqgvw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpnejibl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lolhnykl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tcpgkspy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3otnpamih.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pejgnklq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iwqrhfpi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ucabaogt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wzyjacys.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nubvkjrn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jtueofmm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nnmtbhzo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hsfdkpqc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3iepwginj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jwbtlnra.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3objaulzx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gbqnitke.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmqyznr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wzgyffcc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wfrzjnsh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3plpgaoyf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lbynejwn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hnzfyzur.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zvrdjoay.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qucwdbux.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fbiifchf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wfekgtlk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xknomxsk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3crxhsqau.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wfjbnlvi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3natxotnm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dxjhukxj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vthkxopq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iwkdmphp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3walsccyh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ogfqmljx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3opnfjshi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3nplnhumb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3clngfolr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fydtuafq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rwarzrdj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3udogcsey.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pghtvfdc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3onthjktu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hiwizvqw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qvzqxrqs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ilpdubqk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mojzjchy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kuvoafex.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3agvjlxve.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3twwxugke.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3klceovgt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wojseuqb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3loqkyqqk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xfnmhaic.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3awzgulgy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3sueeyhic.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dekxdulq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ygoiayzv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdvvgll.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tlfhibeb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zccelapa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3krrzleqk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pucjiwuk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hhtmlnxw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xaziwgwm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjlnomnz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rloffxfh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxhwluub.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uwuiqbcp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gytjcjnn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qvgxemrg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3umxzamqm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3glzumcuw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zslslzgq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ufjcqgwt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zqkttyvi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3skgtfmfk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qccvdsuh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3iguostxq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lsvufpec.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xjqjyxpl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbladcjv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kfvnnowd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mdtexptr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qftjmpcg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vdenqtsv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yyodhcor.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3uqochubt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tzdegrxd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ldgldpcy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3deyoydcj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hhpkuxah.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lhjiorjb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3anenrpsq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ubkgtttn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhcqhfcr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ovsyfxet.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gqqlldcg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tgbfsthh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3phxqomiq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vrsoeqkz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3alsjydpb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nobkpqly.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3shzenefh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3uiinetfm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zuxytjsl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3nrixfyub.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yeafrwwf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jeiwggkx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nxvwvxjp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ryzeyicn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gybiqloq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3thovnerk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ryvesumq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kdtqapjy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qbrrnrdu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvnfwlvo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rmiaganj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3swrwiyuy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dhfhvhvs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hccjfsef.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ouuyqklr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jesxvlfb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fjpfpkfa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hfquyzfe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzudjfbh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3sueonfym.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jrdvmzmy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dgvtuhsr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zeozyvwb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dyjjhmpq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3djgdikwy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3imynjaev.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dnyqxczo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vrcjntae.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ubmhswql.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ffcatsxp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3iutvwabj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3crbvudgi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3svkhdfyt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bxvkpgxg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jihndwfe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ofrenatt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qgqcjswn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3erukctwg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3snppmidn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3cgxejfcv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vutdcfpx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tdxhakrp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qvdowcfv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bnxfkqvc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3weufllrd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qzjumirt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ncjuyrer.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hsswcddj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rnbbftkg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qranawdj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3koodgmri.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqmetgqd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ikftioww.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vywyqjkv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3unqyuuof.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bljzbwra.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tleyiccf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3sgppgxvm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixxwxuuz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tjgwxqpp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nsgxzrnv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3asbcqgbb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hqjdwbho.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cadydfgp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xmgpskpp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hsmqptgh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lbzndpme.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xooacdaf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fpksdpbo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kskecsjk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3plkyxltv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bkqdsskd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fweanzxb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3byobhcrv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qdjlyzsb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ifykumak.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zetocgqj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rluadsjh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uyfzuthu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tfybcwxz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mpntdkyl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xmnhnvux.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ipdvnita.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kcxrilfd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bydpafnd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dhagxopk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ohkgtrsw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ehmzyfnk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vptzushh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3prlwmjxn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ywaespxk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bxhkvrrp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eqbsilvt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3snvhxjku.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ugwqcelt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nrcactgj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3iefcsdtb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iqlngxxn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rqydrdaw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3apzsdhag.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgotkg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nuvegkog.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xmlqjoio.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gxxpmrbp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ganbwiyh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rnhslrzz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zivzimhu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wiayisen.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wdjfzszj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3idvuzlwq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tgktofbu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3djnxijya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtqjmdrf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3irmtxyrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhjhwogy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zfvqszyq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jntukeue.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qjfzgwfc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gcanbmcy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qtuxzpee.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hrmctcud.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mytpmylu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wojcpbzj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xrsrvios.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ybyhviay.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mynsnehb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3yuwynynv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3itybzylc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3irwywxul.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ttstmvig.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jzioihiz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kjzsxvft.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xnyaubjt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ernslcgp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gchnugon.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3aysbcoaf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hccbzgkg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lyfmtkoi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ayapbmks.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fxgfxhca.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cbmztalt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nszvrglh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3odiuijje.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3chutzehp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pxhktaui.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jbxwbzny.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kcuhqhei.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3idklbwac.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xurfdgdt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zvimficv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qypwnofv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3omngzlfu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jxhluyld.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3clopmdrz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pzjznumc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wmxvbake.html


<!-- 参考信息 -->