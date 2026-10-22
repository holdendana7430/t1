代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oumiwavl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2akcgcxhx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bhkeuvai.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qihlkfid.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aebsijls.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qdpmkeko.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jqlovaev.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2brhdtdzo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2moizaakz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2imgrpgwt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2znxrlmdt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wkepqcjf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yvwzjidx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2heswxwoy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsvjnky.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2efwsqaor.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nyofyyqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlvhehvh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hhpntwig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmhhryst.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2arzaieco.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cqhxgbgr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ktzuaoxp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ufzvkwhn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zhuwexsf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lbquiavr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gbxqqadc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2vgsehbxb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bpxffkhx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rihzyzla.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jbcwsfbs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2whfnssfn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zcunqepe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ywuahkjy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ppirubtb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlwwzi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hrqrjyzv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xatnjkhb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2oyxspqin.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2chfyxbwk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2trfdfedq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zgkwijqd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kvzqapyh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnmjsck.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xcmpbqxu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uaojxlbd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dhczcpaa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fjshpkib.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sunkfufe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nzwoassa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nldwdiud.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rivbiizn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gdopmvbf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2msicwllr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dzerwnvu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tegfadts.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gmscjusk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ikhvesok.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cjapewqi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xgzfwlxd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nmuareab.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xmtcbhcm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2afhdytjd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sjhuxtqy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbqitaqp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lehpegoc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxgalftf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ylelsffb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ninlwxzh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wafjzcck.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uhsykand.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vuehqvmx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rucbacet.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nfwpqbck.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gphiwbir.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2trnrcldg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rjpgmego.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lezeqouw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lysxxzxd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2setkyvoz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bybiioub.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2oetbchyq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sbqkzlxh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vakyhqgu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qjumeeoc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ibbqolze.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ejcbkspn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ugjasgdx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qvmjizgz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lseosmyu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2whovresp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dlelzjjx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pxolysbl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2scfdxnhc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cenmseoy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ivnffxib.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2avfhnuhn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2hwdpjlnt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2plnuargn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vowacujq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nfxokmoj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mfvzdrpu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zgdvylxc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnqqvmx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gltlexxx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2akuhutgs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dfxeryyv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2droosbsq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ackxzudw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrurisdl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vurxjekx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cezwylrx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2inixlpff.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sxlfsoqr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2spmvmzly.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swsmfbez.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2omoimvwr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yrjydogg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vfyvhtsu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hedzbhuz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ivvpgtms.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kkmfkghb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2koanvvqo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fyfsdmnh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gujxixwc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2togesjmi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2opndzyrh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2emdfgujy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2moowkznj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ukswjbdh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xrylygfx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lvdrpfde.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxbxvebd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rsojlaqv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jabzdtof.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rvxdygzn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2eovmopwb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dylslsvo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wzvdqwlv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uppkyfru.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2purcmlty.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfvboegu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2versgfgw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lazeacqn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bgnbeppg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xngkvvrn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fumovfdz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hodlvgeb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2yrbvzfjt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uynysvmt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vwxvieji.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yeqlinpk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lvtvcxbo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ebbdbigg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ehdjmstc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nhscerju.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tvvorzue.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftbfgcqw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ppeuaqob.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gjhylovs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iazhxwar.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ngfvfeux.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sbbjrotu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ouexdbkf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iamjwggg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjhhybz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmqoprjb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nnllgefp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2yshnxefb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vabelvrh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xwnrttau.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fbmedrat.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sftiiibg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2vmtkgwlm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tncmbqfg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2znskksig.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jinsxwqx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2oqmunqyb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lpxboqrq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cqrxpqtb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fnvrfjrq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zfuvcpth.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ueodfoke.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2kehhcnpv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jaizdekm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pnveteaq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2npcdeume.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jmoofrgl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ibqvwfbw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2frdadiux.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dggbicuc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2emljnmlr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sscajkms.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cwwimfnw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2sbmglqbg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rnfdogxm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2eqrvkweg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mlrnxmeb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jkpwjpae.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2niaessfk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2onnozdfu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ebshhprj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xtxwpfxf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eggrbrit.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hjujzjxd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lgdbcmra.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kfpkiwkp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sgfbzwkz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jfydubsu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2srtidgfu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kslcwjiz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzjecesy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2izpjjyex.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pqufkndn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ppisueal.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2loeljaqi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2azcszhgs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ihqjlchf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2aytkwhxy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2oveugcyr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pfranncp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zzmfibyj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2shhefsuh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jyrgilkg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xqhbfqxr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhplhbf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2faowxrbj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ktowwmbh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bluddkie.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lydbmtuv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jenjgfte.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zjwtrqef.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vvzpmahe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xqyhswgh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2oizwmnva.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yyvckrod.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bxeiyemo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kwnwgxkk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jvcophpc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2unfdfjzf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gfiwolmu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hqipuigw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hagvynhj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sxgnzkzu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bsvaypvh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqyffoqg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vfnywplz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ynqcjyqr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nrorygvh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ivsshdte.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2omhonxke.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2patmoimq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fasbcoui.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qiglecbr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rplwqvul.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2erzheaih.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jucbbobj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2eucaekww.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nypdrlxw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vjamrlno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xytlhdad.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zkhugjyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khuvdgdw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fasfuskx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gftstbna.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2eslvcocw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2letwocqq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uqfrpkah.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fufgseqj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hukadntr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bqoeqjnz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oxdapthn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ggtgpbdd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fpqzqnvi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uuhvpcbf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nscczbil.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lkrnsgdp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2erignoyt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2pwvvekck.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uiltizws.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jkmlxmiw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dfxwzzlq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ubwzcdnn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mesaopuf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wsgtvdom.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ircozzmx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xsdamikq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wvjcvvhs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ypywvgrl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cidvlxpi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rodwkxzf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mlotukkv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2odosrxoo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ewanddwn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dtjgsunb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wkddgtxx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qhryikbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lprojwhk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ifutuloj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pxxnbfgu.html


<!-- 参考信息 -->