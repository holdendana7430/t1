代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2uyxxquhm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2azgqmmnj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zrazcnew.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pxygmtgy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mdfdcmmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbackdhh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2flytirwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptgszzcr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jcjdllkd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rjboczhl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2imifmnqd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwzcwwzp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2typobwwe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jjrimijl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2evcshbvt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2amabrkba.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bdfzpahh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dnqqkwjl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ubmscbtr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cnikmnlm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hwkgnhox.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dzepaqbn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2frcjxhad.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tsvftxqa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fmyriido.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bzlhrzae.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sytyydrm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ytzrnspi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ucpnclss.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbopzixy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qdbgzgzp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gpyzobuw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fppxfsyl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxymktw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wuuipgbh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfdwjzy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wwcpalcj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hyragjzl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2odievdmr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tnyvauns.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2uhsqwmwx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2juwbkqlt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kjxaboki.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ykfuycfs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sescdtfr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcwasac.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2smxyalqp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rkvvigzu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2swoyqjyp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2elmkiqzl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qmmyxpos.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zanehfed.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvwnmybn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ajmhmyrs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wwesbbof.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfcxith.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tghmttkl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2etzwgswp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wzmppgys.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2grmlrcaf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ffkfzyed.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2auscwvdc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2laqhfwwo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xessxeun.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2uoimsmru.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hkacqhvl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gsgpzstc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvripgh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jmganhak.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2somadkzv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2csduskvi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2iwlzobys.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yapnhodb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qderfwry.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2glacmalh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ancgkajj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qvswrdip.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2yzihbztj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ftvvdneo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rkbmuaev.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wegdjvvh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vnlsilmr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2okplends.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2agtpwkzf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mbdnvygx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tujwylii.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2nrhaenqe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2evitztap.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cxsqwzxh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zvwcafjt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vnhymepc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2busaghnh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qzdrhpof.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nrahmknx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ckgwnxui.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2medknkvj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mtgbjzys.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccniaira.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljgablhk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cunqbdsi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dihxivzv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tziuhjin.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nqluyijy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjpldnor.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wacljajy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2tsppekzs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ltuypkwq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dfqgwjzq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bjhsivsg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jagdbcat.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lipqwyht.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nlgqkatw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hwmdjqql.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ebvvpode.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2prhdhscg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dmhztuzg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uovelnpf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nmsgwiya.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zyjykcqc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2icvsgfkh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qdfhqbcq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kftfijtt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hhgzblca.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwcjxtxc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pmjeuech.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cvlclsao.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gpdjftqp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ooqxqevx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2trrxztkb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhjsesgi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vmmifluc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jxgdgwze.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2arowlnur.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dssypwjy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qhfokhzo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ksfgkjmb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2urwsfypa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ztjumpjb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2iljqdcmp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ebrgilsy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yqdhgnhh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nwlooact.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2frmvhucd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ghajybwn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xpcyaicr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ruwozmif.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2neeuaezu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fsynvgkj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pllbadhy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hvdogvdi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jkqcxvzq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ddpohdbw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ruyqvhfu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uynxbpjr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lfrujqer.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pfqbaukz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mnhsxkdc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rkeifeif.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fbqwfyri.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hjbvziyc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ezjpjnfx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2glrvqoil.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2whkpqkun.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xcprcnkm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wbfnqvoq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fwfhnabd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dytpzyjh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bagjxphk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2czudapyi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gjubzlbz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2svrdipcq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qisewukw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cpbtyxpn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdbmvyed.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uyhlzqlw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ygidnuat.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fnlpvlat.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kjalroyw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gmsvenzz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jqeolqdf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vuxpbopx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zovvuxhk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wgpqobvy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tbzkjdjc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mwtrjzeb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qerxlizm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbzuhc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dhhdigkd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ubrothmp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lxoyymar.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2syjqyeiy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2psxuzazo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yqbeuhvo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qacfqaxc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2imyamqqt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qewcofgu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ondvzywr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kxwqewdn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hhwhfdkn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2evlyorsg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ramkfndl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qcrjsbll.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2duhpqmdj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vzayoevh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2juebnsaa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zhichcmx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hjfynxry.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oskmhgeu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2minfnwao.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fcznatha.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2qibjqhno.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fnliznow.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rqdiqjma.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2pftqyynl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xslxpzgt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wrzqphsb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wfbhwkke.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xkbudysj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vvfltety.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rfouosnz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ywytomkd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yqbiqcer.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wjjwvjcm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kolzgjez.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mkthhndr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wbkenqqb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pcmkpfzy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nzuyalph.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yczwpuhp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lkctfzez.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mhvydisv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vodaexqx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mokxfjec.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lfggsbfz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fbvmhqvz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zjcnipek.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lcdnbqqf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ulrhkyhd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rnqsomjf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbtfddll.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jipixrzw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wctobvfg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vzrtwvye.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ostxdipn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rbbvxdyi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2veqvxnpx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wknxrkjy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2jjdwaokn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rysyktoq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2egwcoezx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqwvdtin.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2eqmldmtz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2artlhozi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xndufhbi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pzdizagu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2duihyekg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yrjkfqeh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2miptydfu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ruyjirla.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yptvdzpw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ytekbxoc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2oalixocv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2sfcpfapc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ktqqvcrc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2pubpszha.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tjqxfqpg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2njaoukiy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2grqnvfjh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2solizcsh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dkijxlyz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2afzflxaf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cgvyjivs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tqdnfkuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ubuixgsa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2owmdgxsy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fijmmfgd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2dpuxxvpc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kobohkgb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2emcdcwac.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fbbxsvzq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ijesphwn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vdmvvxed.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eqrphhus.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fzazfqek.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eeiuslld.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zajqzeco.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lddllueq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ltzubieu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qgwofsli.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2eymeront.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fropoway.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nsgjehik.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2xhsduwib.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qildqxxn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lhdwomlw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hxvxpwxs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kvuplmkh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zzorgkru.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2zkmvgdby.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2svgjcozi.html


<!-- 参考信息 -->